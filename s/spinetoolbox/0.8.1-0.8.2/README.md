# Comparing `tmp/spinetoolbox-0.8.1.tar.gz` & `tmp/spinetoolbox-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinetoolbox-0.8.1.tar", last modified: Tue May 14 13:12:37 2024, max compression
+gzip compressed data, was "spinetoolbox-0.8.2.tar", last modified: Thu May 30 13:45:42 2024, max compression
```

## Comparing `spinetoolbox-0.8.1.tar` & `spinetoolbox-0.8.2.tar`

### file list

```diff
@@ -1,874 +1,875 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.762010 spinetoolbox-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.610009 spinetoolbox-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.610009 spinetoolbox-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/.github/workflows/bundle.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/.github/workflows/test_runner.yml
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    39026 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28878 2024-05-14 13:12:37.762010 spinetoolbox-0.8.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.614009 spinetoolbox-0.8.1/PyInstaller hooks/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/PyInstaller hooks/hook-datapackage.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/PyInstaller hooks/hook-jill.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/PyInstaller hooks/hook-spine_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/PyInstaller hooks/hook-spinedb_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/PyInstaller hooks/hook-tableschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/PyInstaller hooks/hook-tabulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27660 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.614009 spinetoolbox-0.8.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/benchmarks/compound_model_filter_accepts_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/benchmarks/db_mngr_get_icon_mngr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/benchmarks/db_mngr_get_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/benchmarks/db_mngr_get_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.614009 spinetoolbox-0.8.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/append_license.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/build_doc.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/build_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/build_ui.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)     4594 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/build_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/builddocs.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/configure_julia.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/upgrade_spine_reqs.bat
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/bin/upgrade_spine_reqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/cx_Freeze_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.618009 spinetoolbox-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/cleandocs.json
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.622009 spinetoolbox-0.8.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/contribution_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.626009 spinetoolbox-0.8.1/docs/source/data/
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/A5_importer_specification.json
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/Fallet_node.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/Spranget_node.txt
--rw-r--r--   0 runner    (1001) docker     (127)    47789 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/a5.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/contracted_load.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__from_node-relationship-parameter-values.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__from_node.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__node__node-relationship-parameter-values.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__to_node.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-model-parameter-values.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-node-parameter-values.txt
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-node__commodity.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-temporal_block-parameter-values.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__from_node-relationship-parameter-values.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__from_node.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__node__node-relationship-parameter-values.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__to_node.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/el_prices.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data/value_stored_water_vom.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27308 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/data_import_export.rst
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/developer_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/executing_projects.rst
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/execution_tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15441 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/how_to_run_spineopt.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.642009 spinetoolbox-0.8.1/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (127)    47972 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/DB_Tool_link_properties.png
--rw-r--r--   0 runner    (1001) docker     (127)    41203 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/Tool_DB_link_properties.png
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/dag_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/edit_tool_specification_blank.png
--rw-r--r--   0 runner    (1001) docker     (127)    25719 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/example_dags.png
--rw-r--r--   0 runner    (1001) docker     (127)    17515 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/executable_tool_spec_dir_runner.png
--rw-r--r--   0 runner    (1001) docker     (127)   107965 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/execution_data_connection_selected.png
--rw-r--r--   0 runner    (1001) docker     (127)   120568 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/execution_julia_tool_selected.png
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/exporter_mapping_options_dock.png
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/exporter_mapping_specification_dock.png
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/exporter_mappings_dock.png
--rw-r--r--   0 runner    (1001) docker     (127)    19996 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/exporter_preview_docks.png
--rw-r--r--   0 runner    (1001) docker     (127)    39469 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/exporter_properties.png
--rw-r--r--   0 runner    (1001) docker     (127)    63652 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/exporter_specification_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)    39515 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_added_input_file.png
--rw-r--r--   0 runner    (1001) docker     (127)   124750 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_after_first_execution.png
--rw-r--r--   0 runner    (1001) docker     (127)    17345 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_dc_properties.png
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_dc_to_tool_connected.png
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_dc_with_an_input_file.png
--rw-r--r--   0 runner    (1001) docker     (127)   125132 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_final_execution_successful.png
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_first_tool_created.png
--rw-r--r--   0 runner    (1001) docker     (127)    84038 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_first_tool_spec_created.png
--rw-r--r--   0 runner    (1001) docker     (127)   115014 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_say_hello_world_failed.png
--rw-r--r--   0 runner    (1001) docker     (127)    28102 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_tool_properties.png
--rw-r--r--   0 runner    (1001) docker     (127)    36347 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/getting_started_tool_spec_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/import_editor_column_data_type_menu.png
--rw-r--r--   0 runner    (1001) docker     (127)    19562 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/import_editor_preview_table_mapping_menu.png
--rw-r--r--   0 runner    (1001) docker     (127)    66722 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/import_editor_window.png
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/importer_connector_type.png
--rw-r--r--   0 runner    (1001) docker     (127)    15867 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/importer_properties.png
--rw-r--r--   0 runner    (1001) docker     (127)    81698 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/importer_spec_editor_anonymous_mode.png
--rw-r--r--   0 runner    (1001) docker     (127)    37796 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/julia_jupyter_console_selected.png
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/julia_kernel_specification_creator.png
--rw-r--r--   0 runner    (1001) docker     (127)    40319 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/main_window_no_project.png
--rw-r--r--   0 runner    (1001) docker     (127)    29983 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/minimal_tool_specification.png
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/open_tool_specification_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/plot_data.png
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/plotting_popup_menu.png
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/plotting_popup_menu_plot_in_window.png
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/plotting_use_as_x_popup.png
--rw-r--r--   0 runner    (1001) docker     (127)    38098 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/plotting_window_added_plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    24352 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/plotting_window_single_column.png
--rw-r--r--   0 runner    (1001) docker     (127)    35913 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/python_jupyter_console_selected.png
--rw-r--r--   0 runner    (1001) docker     (127)    15902 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/python_kernel_specification_creator.png
--rw-r--r--   0 runner    (1001) docker     (127)    41169 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/right_click_options.png
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/select_url_for_remote_db_export.png
--rw-r--r--   0 runner    (1001) docker     (127)    57174 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/settings_db_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/settings_engine.png
--rw-r--r--   0 runner    (1001) docker     (127)    49149 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/settings_general.png
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/settings_specification_editors.png
--rw-r--r--   0 runner    (1001) docker     (127)    35968 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/settings_tools_default.png
--rw-r--r--   0 runner    (1001) docker     (127)    17351 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/spineopt_install_wizard_successful.png
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/spinetoolbox_on_wht.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/start_jupyter_console_menu_listing.png
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/toolbar_with_one_tool_specification.png
--rw-r--r--   0 runner    (1001) docker     (127)    44865 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/using_input_output_files_in_tool_scripts.png
--rw-r--r--   0 runner    (1001) docker     (127)    46428 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_array.png
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_datetime.png
--rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_duration.png
--rw-r--r--   0 runner    (1001) docker     (127)    31828 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_map.png
--rw-r--r--   0 runner    (1001) docker     (127)    16590 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_map_after_conversion.png
--rw-r--r--   0 runner    (1001) docker     (127)    25102 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_map_before_conversion.png
--rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_parameter_type.png
--rw-r--r--   0 runner    (1001) docker     (127)    14114 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_plain.png
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_time_pattern.png
--rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_time_series_fixed.png
--rw-r--r--   0 runner    (1001) docker     (127)    34633 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/img/value_editor_time_series_variable.png
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/links.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/main_window.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/metadata_description.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/parameter_value_editor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/project_item_development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/project_items.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/publishing_to_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/setting_up.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/settings.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.642009 spinetoolbox-0.8.1/docs/source/spine_db_editor/
--rw-r--r--   0 runner    (1001) docker     (127)    15996 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/adding_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/committing_and_history.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entities_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entities_dialog_2D.png
--rw-r--r--   0 runner    (1001) docker     (127)    16696 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entity_classes_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    20829 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entity_classes_dialog_2D.png
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entity_group_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/alternative_tree.png
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/commit_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/commit_viewer.png
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/dirty_db.png
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/edit_entity_classes_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_alternative_table.png
--rw-r--r--   0 runner    (1001) docker     (127)    52808 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   105932 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_icon_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_name_filter_menu.png
--rw-r--r--   0 runner    (1001) docker     (127)    39149 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_parameter_value_table.png
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_tree.png
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_tree_context_menu.png
--rw-r--r--   0 runner    (1001) docker     (127)    35459 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/excel_entity_sheet.png
--rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/excel_entity_sheet_timeseries.png
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/export_bar.png
--rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/generate_scenarios_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/item_metadata.png
--rw-r--r--   0 runner    (1001) docker     (127)   101708 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/manage_entities_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/manage_members_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    27082 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/mass_export_items_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/metadata.png
--rw-r--r--   0 runner    (1001) docker     (127)    20869 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/parameter_value_list.png
--rw-r--r--   0 runner    (1001) docker     (127)    43379 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/pivot_table.png
--rw-r--r--   0 runner    (1001) docker     (127)    37996 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/plain_db_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/purge_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/remove_entities_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/scenario_tree.png
--rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/img/uncommitted_changes_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/importing_and_exporting_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/managing_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/removing_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/spine_data_structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/updating_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/vacuum.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_db_editor/viewing_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/spine_engine_server.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/terminology.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/tool_specification_editor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/ui_guidelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/unit_testing_guidelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/docs/source/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/execution_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/execution_tests/active_by_default/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/active_by_default/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/execution_tests/active_by_default/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/active_by_default/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.594009 spinetoolbox-0.8.1/execution_tests/active_by_default/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/execution_tests/active_by_default/.spinetoolbox/specifications/Exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/active_by_default/.spinetoolbox/specifications/Exporter/export_entities.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/active_by_default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/active_by_default/execution_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/execution_tests/alternative_filters/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/alternative_filters/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/execution_tests/alternative_filters/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/alternative_filters/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.594009 spinetoolbox-0.8.1/execution_tests/alternative_filters/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.650009 spinetoolbox-0.8.1/execution_tests/alternative_filters/.spinetoolbox/specifications/Exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/alternative_filters/.spinetoolbox/specifications/Exporter/export_values.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/alternative_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/alternative_filters/execution_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.598009 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/Exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/Exporter/entities.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/execution_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.598009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/.spinetoolbox/specifications/Tool/simple_tool_spec.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.598009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/client_secfolder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/client_secfolder/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/client_secfolder/private_keys/client.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/client_secfolder/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/client_secfolder/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/client_secfolder/public_keys/server.key
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/input_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.598009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/secfolder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/secfolder/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/secfolder/private_keys/client.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/secfolder/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/secfolder/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/secfolder/public_keys/server.key
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/allowEndpoints.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/certificates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/certificates/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.654009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/private_keys/server.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secfolder/public_keys/server.key
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/server_secure.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/hello_world_on_server/simple_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/import_file_packs/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/import_file_packs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.598009 spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/specifications/Importer/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/specifications/Importer/import_dat_files.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/specifications/Tool/create_file_pack.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/import_file_packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/import_file_packs/create_data_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/import_file_packs/execution_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.598009 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/items/initial_counter_data/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/items/initial_counter_data/counter_init.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.598009 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/counter_data_importer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/import_data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Tool/data_writer.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/merger_write_order/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/merger_write_order/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.658009 spinetoolbox-0.8.1/execution_tests/merger_write_order/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/merger_write_order/.spinetoolbox/project.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/merger_write_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/merger_write_order/execution_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.602009 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/Exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/Exporter/exporter.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.602009 spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/specifications/Importer/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/specifications/Importer/import_tool_output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/specifications/Tool/test_tool.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.602009 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Importer/
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Importer/import_tool_output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.662009 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Tool/test_tool.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/execution_tests/scenario_filters/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.602009 spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/specifications/Importer/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/specifications/Importer/input_data_mapping.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/specifications/Tool/write_values.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/input_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/scenario_filters/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.spinetoolbox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.602009 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.spinetoolbox/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.spinetoolbox/items/raw_data/
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.spinetoolbox/items/raw_data/units.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.spinetoolbox/project.json
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/Importer 1 - units.xlsx.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/server.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.666010 spinetoolbox-0.8.1/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/fig/eu-emblem-low-res.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/fig/spinetoolbox_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/fig/spinetoolbox_on_wht.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/setup-debug.iss
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:12:37.762010 spinetoolbox-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/setup.iss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.678010 spinetoolbox-0.8.1/spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 13:12:37.000000 spinetoolbox-0.8.1/spinetoolbox/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/execution_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/fetch_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)    28374 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/headless.py
--rw-r--r--   0 runner    (1001) docker     (127)    61992 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/kernel_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    25909 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/load_project_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/log_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/logger_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/metaobject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.682010 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/compound_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/empty_row_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/file_list_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/filter_checkbox_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/filter_execution_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/indexed_value_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/map_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/minimal_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/minimal_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/project_item_specification_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/resource_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/time_pattern_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    67706 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    26513 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.682010 spinetoolbox-0.8.1/spinetoolbox/project_item/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18789 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_item/logging_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17442 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_item/project_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_item/project_item_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_item/specification_editor_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    30182 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_item_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    37062 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/project_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/qthread_pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)  1451299 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/resources_icons_rc.py
--rw-r--r--   0 runner    (1001) docker     (127)   434871 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/resources_logos_rc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.682010 spinetoolbox-0.8.1/spinetoolbox/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/server/engine_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.686010 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40872 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/graphics_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.690010 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/alternative_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/alternative_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/compound_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/empty_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    19889 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    78046 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/scenario_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11606 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/single_and_empty_model_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/single_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/scenario_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.690010 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/db_commit_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/db_commit_viewer.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/scenario_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/scenario_generator.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/select_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/select_databases.ui
--rw-r--r--   0 runner    (1001) docker     (127)    37266 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    35685 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.698010 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43112 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/commit_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_delegates.py
--rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_editors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_menus.py
--rw-r--r--   0 runner    (1001) docker     (127)    41223 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py
--rw-r--r--   0 runner    (1001) docker     (127)    51193 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py
--rw-r--r--   0 runner    (1001) docker     (127)    34088 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/element_name_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    39339 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/metadata_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/scenario_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/select_graph_parameters_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    51055 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/stacked_view_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/url_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_icon_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    68176 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_db_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15503 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_engine_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/spine_engine_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.706010 spinetoolbox-0.8.1/spinetoolbox/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/about.py
--rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/about.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/add_project_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/add_project_item.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/array_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/array_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/datetime_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/datetime_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/duration_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/duration_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/import_source_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/import_source_selector.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/jump_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/jump_properties.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/link_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/link_properties.ui
--rw-r--r--   0 runner    (1001) docker     (127)    38780 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    29944 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/mainwindow.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/map_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/map_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/mini_kernel_editor_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/mini_kernel_editor_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/open_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/open_project_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/parameter_value_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/parameter_value_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/plain_parameter_value_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/plain_parameter_value_editor.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.718010 spinetoolbox-0.8.1/spinetoolbox/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    17862 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/Energy_Reform_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/KTH_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/KU_Leuven_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/Spine_symbol.png
--rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/UCD_Dublin_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    83366 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/VTT_Multicolour_Logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (127)   105515 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/app.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/black_plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/book.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25777 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/check-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/database-edit.svg
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/database.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/datapkg.svg
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/desktop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/double-at.svg
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/downward_triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/eye.svg
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/file-download.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/file-link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/file-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/folder-plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/fontawesome5-codepoints.json
--rw-r--r--   0 runner    (1001) docker     (127)    84681 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/fontawesome5-searchterms.json
--rw-r--r--   0 runner    (1001) docker     (127)   204528 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/fontawesome5-solid-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/home.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.726010 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/angle-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/angle-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/bolt-lightning.svg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/broom.svg
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/check.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cog.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cog_minus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/copy.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cube_minus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cube_pen.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cube_plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cubes_minus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cubes_pen.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cubes_plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/database-export.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/database-import.svg
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/door-closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/edit.svg
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/ellipsis-h.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/exchange-alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/eye.svg
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/file-alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/file-export.svg
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/file-import.svg
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/folder-open-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/folder-open-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/hands-helping.svg
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/history.svg
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/info-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/level-up-alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/map-signs-minus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/map-signs-plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/paste.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/pivot-table.svg
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/play-circle-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/play-circle-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/question-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/save_regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/save_solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/server.svg
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/stop-circle-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/sync.svg
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/table.svg
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/times.svg
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/trash-alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/tree.svg
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/user.svg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/window-close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/minus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project-diagram.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.726010 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/binoculars.svg
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/blender.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/data_connection.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/database-export.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/database-import.svg
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/database.svg
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/exclamation-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/file-alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/hammer.svg
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/paint-brush-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/qt_extended_48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/resources_icons.qrc
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/resources_logos.qrc
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/share.svg
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/slash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/sliders-h.svg
--rw-r--r--   0 runner    (1001) docker     (127)   164289 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/spinetoolbox_on_wht.png
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/tools.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/tractor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/wrench.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/wrench_minus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/resources/wrench_plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)    82269 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    77415 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/settings.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/time_pattern_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/time_pattern_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/time_series_fixed_resolution_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/time_series_fixed_resolution_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/time_series_variable_resolution_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/time_series_variable_resolution_editor.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/tool_configuration_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui/tool_configuration_assistant.ui
--rw-r--r--   0 runner    (1001) docker     (127)   111473 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/ui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.738010 spinetoolbox-0.8.1/spinetoolbox/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/about_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/add_project_item_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/add_up_spine_opt_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/array_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/array_value_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/code_text_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/commit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_combobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_delegates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_menus.py
--rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qgraphicsscene.py
--rw-r--r--   0 runner    (1001) docker     (127)    23451 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qgraphicsviews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qlineedits.py
--rw-r--r--   0 runner    (1001) docker     (127)    38512 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qtableview.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qtextbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qtreeview.py
--rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/datetime_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/duration_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/indexed_value_table_context_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/install_julia_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/jump_properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/jupyter_console_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    29868 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/kernel_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/link_properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/map_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/map_value_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/multi_tab_spec_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/multi_tab_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/open_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/options_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/parameter_value_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/parameter_value_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    40349 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/persistent_console_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/plain_parameter_value_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/plot_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/plugin_manager_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/project_item_drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/report_plotting_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/select_database_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/set_description_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    62760 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/settings_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/statusbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/time_pattern_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/time_series_fixed_resolution_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/time_series_variable_resolution_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox/widgets/toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.762010 spinetoolbox-0.8.1/spinetoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28878 2024-05-14 13:12:37.000000 spinetoolbox-0.8.1/spinetoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-05-14 13:12:37.000000 spinetoolbox-0.8.1/spinetoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:12:37.000000 spinetoolbox-0.8.1/spinetoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 13:12:37.000000 spinetoolbox-0.8.1/spinetoolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:12:36.000000 spinetoolbox-0.8.1/spinetoolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 13:12:37.000000 spinetoolbox-0.8.1/spinetoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 13:12:37.000000 spinetoolbox-0.8.1/spinetoolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/spinetoolbox.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.742010 spinetoolbox-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mock_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.742010 spinetoolbox-0.8.1/tests/mvcmodels/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_ArrayModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_FileListModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_FilterCheckboxList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_IndexedValueTableModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    29044 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_MapModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_MinimalTableModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_TimePatternModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/mvcmodels/test_resource_filter_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.742010 spinetoolbox-0.8.1/tests/project_item/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/project_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/project_item/test_ProjectItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/project_item/test_logging_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/project_item/test_specification_editor_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.742010 spinetoolbox-0.8.1/tests/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.606009 spinetoolbox-0.8.1/tests/server/client_secfolder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.742010 spinetoolbox-0.8.1/tests/server/client_secfolder/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/client_secfolder/private_keys/client.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/server/client_secfolder/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/client_secfolder/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/client_secfolder/public_keys/server.key
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/helloworld.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.606009 spinetoolbox-0.8.1/tests/server/secfolder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/server/secfolder/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/secfolder/private_keys/client.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/server/secfolder/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/secfolder/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/secfolder/public_keys/server.key
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/server/server_secfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/server_secfolder/allowEndpoints.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/server/server_secfolder/certificates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/server_secfolder/certificates/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/server/server_secfolder/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/server_secfolder/private_keys/server.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/server/server_secfolder/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/server_secfolder/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/server_secfolder/public_keys/server.key
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/test_EngineClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/server/test_RemoteSpineEngineManager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.746010 spinetoolbox-0.8.1/tests/spine_db_editor/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.750010 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_PivotModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_alternative_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_compound_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_frozen_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_item_metadata_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_metadata_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_single_parameter_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_tree_item_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/test_graphics_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.754010 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/spine_db_editor_test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_add_items_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_commit_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_delegates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_editors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_menus.py
--rw-r--r--   0 runner    (1001) docker     (127)    23479 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_qtableview.py
--rw-r--r--   0 runner    (1001) docker     (127)    42097 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_qtreeview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_edit_or_remove_items_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_mass_select_items_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_multi_spine_db_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_scenario_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_tabular_view_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_url_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_ProjectUpgrader.py
--rw-r--r--   0 runner    (1001) docker     (127)    24899 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_SpineDBManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    41387 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_SpineToolboxProject.py
--rw-r--r--   0 runner    (1001) docker     (127)    47778 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_ToolboxUI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_execution_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21340 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_load_project_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    48004 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_project_item_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.754010 spinetoolbox-0.8.1/tests/test_resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.606009 spinetoolbox-0.8.1/tests/test_resources/Project Directory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.754010 spinetoolbox-0.8.1/tests/test_resources/Project Directory/.spinetoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/Project Directory/.spinetoolbox/project.json
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/basic_model_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.754010 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v1.json
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v10.json
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v11.json
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v3.json
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v4.json
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v5.json
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v9.json
--rw-r--r--   0 runner    (1001) docker     (127)    68068 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/spineopt_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_resources/test_tool_spec.json
--rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_spine_db_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/test_spine_engine_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:37.758010 spinetoolbox-0.8.1/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_AboutWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_AddProjectItemWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_AddUpSpineOptWizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_ArrayTableView.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_CopyPasteTableView.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_DatetimeEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_DurationEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_IndexedValueTableView.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_InstallJuliaWizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    16195 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_JupyterConsoleWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_KernelFetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_MapEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_MapTableView.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_ParameterValueEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_PlainParameterValueEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_TimePatternEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_TimeSeriesFixedResolutionEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_TimeSeriesFixedResolutionTableView.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_TimeSeriesVariableResolutionEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_custom_combobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_custom_qgraphicsscene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_custom_qlineedits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_custom_qtextbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_custom_qwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_indexed_value_table_context_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_jump_properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_kernel_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_open_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_plugin_manager_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_select_database_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-14 13:12:30.000000 spinetoolbox-0.8.1/tests/widgets/test_settings_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.485160 spinetoolbox-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.345157 spinetoolbox-0.8.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.349157 spinetoolbox-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.github/workflows/bundle.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.github/workflows/make_bundle.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.github/workflows/manual_bundling.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.github/workflows/test_runner.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    39365 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28671 2024-05-30 13:45:42.481160 spinetoolbox-0.8.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.349157 spinetoolbox-0.8.2/PyInstaller hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/PyInstaller hooks/hook-datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/PyInstaller hooks/hook-jill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/PyInstaller hooks/hook-spine_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/PyInstaller hooks/hook-spinedb_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/PyInstaller hooks/hook-tableschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/PyInstaller hooks/hook-tabulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27482 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.349157 spinetoolbox-0.8.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/benchmarks/compound_model_filter_accepts_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/benchmarks/db_mngr_get_icon_mngr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/benchmarks/db_mngr_get_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/benchmarks/db_mngr_get_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.353157 spinetoolbox-0.8.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/append_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/build_doc.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/build_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/build_ui.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4594 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/build_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/builddocs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/configure_julia.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/upgrade_spine_reqs.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/bin/upgrade_spine_reqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/cx_Freeze_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.353157 spinetoolbox-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/cleandocs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.357158 spinetoolbox-0.8.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/contribution_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.361158 spinetoolbox-0.8.2/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/A5_importer_specification.json
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/Fallet_node.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/Spranget_node.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    47789 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/a5.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/contracted_load.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__from_node-relationship-parameter-values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__from_node.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__node__node-relationship-parameter-values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__to_node.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-model-parameter-values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-node-parameter-values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-node__commodity.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-temporal_block-parameter-values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__from_node-relationship-parameter-values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__from_node.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__node__node-relationship-parameter-values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__to_node.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/el_prices.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data/value_stored_water_vom.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27782 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/data_import_export.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/developer_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/executing_projects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/execution_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15441 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/how_to_run_spineopt.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.377158 spinetoolbox-0.8.2/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    47972 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/DB_Tool_link_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41203 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/Tool_DB_link_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/dag_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/edit_tool_specification_blank.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25719 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/example_dags.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17515 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/executable_tool_spec_dir_runner.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107965 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/execution_data_connection_selected.png
+-rw-r--r--   0 runner    (1001) docker     (127)   120568 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/execution_julia_tool_selected.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/exporter_mapping_options_dock.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/exporter_mapping_specification_dock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/exporter_mappings_dock.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19996 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/exporter_preview_docks.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39469 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/exporter_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63652 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/exporter_specification_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39515 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_added_input_file.png
+-rw-r--r--   0 runner    (1001) docker     (127)   124750 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_after_first_execution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17345 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_dc_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_dc_to_tool_connected.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_dc_with_an_input_file.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125132 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_final_execution_successful.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_first_tool_created.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84038 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_first_tool_spec_created.png
+-rw-r--r--   0 runner    (1001) docker     (127)   115014 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_say_hello_world_failed.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28102 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_tool_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36347 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/getting_started_tool_spec_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/import_editor_column_data_type_menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19562 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/import_editor_preview_table_mapping_menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66722 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/import_editor_window.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/importer_connector_type.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15867 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/importer_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81698 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/importer_spec_editor_anonymous_mode.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37796 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/julia_jupyter_console_selected.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/julia_kernel_specification_creator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40319 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/main_window_no_project.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29983 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/minimal_tool_specification.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/open_tool_specification_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/plot_data.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/plotting_popup_menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/plotting_popup_menu_plot_in_window.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/plotting_use_as_x_popup.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38098 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/plotting_window_added_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24352 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/plotting_window_single_column.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35913 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/python_jupyter_console_selected.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15902 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/python_kernel_specification_creator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41169 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/right_click_options.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/select_url_for_remote_db_export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57174 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/settings_db_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/settings_engine.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49149 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/settings_general.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/settings_specification_editors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35968 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/settings_tools_default.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17351 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/spineopt_install_wizard_successful.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/spinetoolbox_on_wht.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/start_jupyter_console_menu_listing.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/toolbar_with_one_tool_specification.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44865 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/using_input_output_files_in_tool_scripts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46428 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_array.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_datetime.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_duration.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31828 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16590 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_map_after_conversion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25102 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_map_before_conversion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_parameter_type.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14114 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_plain.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_time_pattern.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_time_series_fixed.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34633 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/img/value_editor_time_series_variable.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/links.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/main_window.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/metadata_description.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/parameter_value_editor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/project_item_development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/project_items.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/publishing_to_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/setting_up.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/settings.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.377158 spinetoolbox-0.8.2/docs/source/spine_db_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/adding_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/committing_and_history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entities_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entities_dialog_2D.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16696 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entity_classes_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20829 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entity_classes_dialog_2D.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entity_group_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/alternative_tree.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/commit_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/commit_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/dirty_db.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/edit_entity_classes_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_alternative_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52808 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76799 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_icon_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_name_filter_menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39149 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_parameter_value_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22697 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_tree.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_tree_context_menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35459 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/excel_entity_sheet.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/excel_entity_sheet_timeseries.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/export_bar.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/generate_scenarios_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/item_metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)   101708 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/manage_entities_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/manage_members_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27082 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/mass_export_items_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20869 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/parameter_value_list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43379 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/pivot_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37996 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/plain_db_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/purge_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/remove_entities_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/scenario_tree.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/img/uncommitted_changes_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/importing_and_exporting_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/managing_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/removing_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/spine_data_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/updating_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/vacuum.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_db_editor/viewing_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/spine_engine_server.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/terminology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/tool_specification_editor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/ui_guidelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/unit_testing_guidelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/docs/source/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/active_by_default/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/active_by_default/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/active_by_default/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/active_by_default/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.329157 spinetoolbox-0.8.2/execution_tests/active_by_default/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/active_by_default/.spinetoolbox/specifications/Exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/active_by_default/.spinetoolbox/specifications/Exporter/export_entities.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/active_by_default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/active_by_default/execution_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/alternative_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/alternative_filters/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/alternative_filters/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/alternative_filters/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.329157 spinetoolbox-0.8.2/execution_tests/alternative_filters/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/alternative_filters/.spinetoolbox/specifications/Exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/alternative_filters/.spinetoolbox/specifications/Exporter/export_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/alternative_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/alternative_filters/execution_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.329157 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.385158 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/Exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/Exporter/entities.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/execution_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.333157 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/.spinetoolbox/specifications/Tool/simple_tool_spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.333157 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/client_secfolder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/client_secfolder/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/client_secfolder/private_keys/client.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/client_secfolder/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/client_secfolder/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/client_secfolder/public_keys/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/input_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.333157 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/secfolder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/secfolder/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/secfolder/private_keys/client.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/secfolder/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/secfolder/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/secfolder/public_keys/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/allowEndpoints.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/certificates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/certificates/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/private_keys/server.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secfolder/public_keys/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/server_secure.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/hello_world_on_server/simple_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/import_file_packs/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/import_file_packs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.333157 spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.389158 spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/specifications/Importer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/specifications/Importer/import_dat_files.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/specifications/Tool/create_file_pack.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/import_file_packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/import_file_packs/create_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/import_file_packs/execution_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.333157 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/items/initial_counter_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/items/initial_counter_data/counter_init.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.333157 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/counter_data_importer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/import_data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Tool/data_writer.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/merger_write_order/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/merger_write_order/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/merger_write_order/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/merger_write_order/.spinetoolbox/project.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/merger_write_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/merger_write_order/execution_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.333157 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/Exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/Exporter/exporter.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/parallel_importer/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.337157 spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.393158 spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/specifications/Importer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/specifications/Importer/import_tool_output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/specifications/Tool/test_tool.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.337157 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Importer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Importer/import_tool_output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Tool/test_tool.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/scenario_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.337157 spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/specifications/Importer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/specifications/Importer/input_data_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/specifications/Tool/write_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/input_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/scenario_filters/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.spinetoolbox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.337157 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.spinetoolbox/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.397158 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.spinetoolbox/items/raw_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.spinetoolbox/items/raw_data/units.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.spinetoolbox/project.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/Importer 1 - units.xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/server.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.401158 spinetoolbox-0.8.2/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/fig/eu-emblem-low-res.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/fig/spinetoolbox_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/fig/spinetoolbox_on_wht.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/setup-debug.iss
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:45:42.485160 spinetoolbox-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/setup.iss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.409158 spinetoolbox-0.8.2/spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 13:45:42.000000 spinetoolbox-0.8.2/spinetoolbox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/execution_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/fetch_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28374 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/headless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62046 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/kernel_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25909 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/load_project_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/log_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/logger_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/metaobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.413159 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15400 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/compound_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/empty_row_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/file_list_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/filter_checkbox_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/filter_execution_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/indexed_value_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/map_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/minimal_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/minimal_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/project_item_specification_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/resource_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/time_pattern_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67706 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26513 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.413159 spinetoolbox-0.8.2/spinetoolbox/project_item/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18789 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_item/logging_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17442 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_item/project_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_item/project_item_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_item/specification_editor_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30182 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_item_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37062 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/project_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/qthread_pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1451299 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/resources_icons_rc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   434871 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/resources_logos_rc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.413159 spinetoolbox-0.8.2/spinetoolbox/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/server/engine_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.413159 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40906 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/graphics_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.417158 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/alternative_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/alternative_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/compound_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/empty_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19889 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78046 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/scenario_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11606 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/single_and_empty_model_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/single_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/scenario_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.421159 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/db_commit_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/db_commit_viewer.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/scenario_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/scenario_generator.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/select_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/select_databases.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    37266 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35685 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.425159 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45636 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/commit_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36015 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_delegates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_editors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41374 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34351 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/element_name_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39339 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/metadata_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/scenario_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/select_graph_parameters_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51634 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/stacked_view_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/url_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_icon_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68176 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_db_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15503 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_engine_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/spine_engine_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.433159 spinetoolbox-0.8.2/spinetoolbox/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/about.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/add_project_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/add_project_item.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/array_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/array_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/datetime_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/datetime_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/duration_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/duration_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/import_source_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/import_source_selector.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/jump_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/jump_properties.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/link_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/link_properties.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    38780 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29944 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/mainwindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/map_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/map_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/mini_kernel_editor_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/mini_kernel_editor_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/open_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/open_project_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/parameter_value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/parameter_value_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/plain_parameter_value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/plain_parameter_value_editor.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.441159 spinetoolbox-0.8.2/spinetoolbox/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    17862 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/Energy_Reform_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/KTH_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/KU_Leuven_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/Spine_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/UCD_Dublin_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83366 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/VTT_Multicolour_Logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   105515 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/app.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/black_plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/book.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25777 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/check-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/database-edit.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/database.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/datapkg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/double-at.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/downward_triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/eye.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/file-download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/file-link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/file-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/folder-plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/fontawesome5-codepoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84681 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/fontawesome5-searchterms.json
+-rw-r--r--   0 runner    (1001) docker     (127)   204528 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/fontawesome5-solid-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/home.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.449159 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/angle-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/angle-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/bolt-lightning.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/broom.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/check.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cog.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cog_minus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cube_minus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cube_pen.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cube_plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cubes_minus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cubes_pen.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cubes_plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/database-export.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/database-import.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/door-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/ellipsis-h.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/exchange-alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/eye.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/file-alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/file-export.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/file-import.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/folder-open-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/folder-open-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/hands-helping.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/history.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/info-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/level-up-alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/map-signs-minus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/map-signs-plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/pivot-table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/play-circle-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/play-circle-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/question-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/save_regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/save_solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/server.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/stop-circle-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/sync.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/times.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/trash-alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/tree.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/user.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/window-close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/minus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project-diagram.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.449159 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/binoculars.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/blender.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/data_connection.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/database-export.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/database-import.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/database.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/exclamation-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/file-alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/hammer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/paint-brush-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/qt_extended_48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/resources_icons.qrc
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/resources_logos.qrc
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/share.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/slash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/sliders-h.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   164289 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/spinetoolbox_on_wht.png
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/tools.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/tractor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/wrench.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/wrench_minus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/resources/wrench_plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77415 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/settings.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/time_pattern_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/time_pattern_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/time_series_fixed_resolution_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/time_series_fixed_resolution_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/time_series_variable_resolution_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/time_series_variable_resolution_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/tool_configuration_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui/tool_configuration_assistant.ui
+-rw-r--r--   0 runner    (1001) docker     (127)   111538 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/ui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.457159 spinetoolbox-0.8.2/spinetoolbox/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/about_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/add_project_item_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/add_up_spine_opt_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/array_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/array_value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/code_text_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/commit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_combobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_delegates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qgraphicsscene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23498 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qgraphicsviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qlineedits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38512 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qtableview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qtextbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qtreeview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/datetime_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/duration_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/indexed_value_table_context_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/install_julia_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/jump_properties_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/jupyter_console_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29868 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/kernel_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/link_properties_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/map_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/map_value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/multi_tab_spec_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/multi_tab_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/open_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/options_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/parameter_value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/parameter_value_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40349 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/persistent_console_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/plain_parameter_value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/plot_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/plugin_manager_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/project_item_drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/properties_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/report_plotting_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/select_database_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/set_description_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62760 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/settings_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/statusbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/time_pattern_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/time_series_fixed_resolution_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/time_series_variable_resolution_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox/widgets/toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.481160 spinetoolbox-0.8.2/spinetoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28671 2024-05-30 13:45:42.000000 spinetoolbox-0.8.2/spinetoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36013 2024-05-30 13:45:42.000000 spinetoolbox-0.8.2/spinetoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:45:42.000000 spinetoolbox-0.8.2/spinetoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 13:45:42.000000 spinetoolbox-0.8.2/spinetoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:45:41.000000 spinetoolbox-0.8.2/spinetoolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-30 13:45:42.000000 spinetoolbox-0.8.2/spinetoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 13:45:42.000000 spinetoolbox-0.8.2/spinetoolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/spinetoolbox.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.461159 spinetoolbox-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mock_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.461159 spinetoolbox-0.8.2/tests/mvcmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_ArrayModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_FileListModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_FilterCheckboxList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_IndexedValueTableModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29044 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_MapModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_MinimalTableModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_TimePatternModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/mvcmodels/test_resource_filter_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.461159 spinetoolbox-0.8.2/tests/project_item/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/project_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/project_item/test_ProjectItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/project_item/test_logging_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/project_item/test_specification_editor_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.461159 spinetoolbox-0.8.2/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.341157 spinetoolbox-0.8.2/tests/server/client_secfolder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.461159 spinetoolbox-0.8.2/tests/server/client_secfolder/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/client_secfolder/private_keys/client.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/server/client_secfolder/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/client_secfolder/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/client_secfolder/public_keys/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/helloworld.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.341157 spinetoolbox-0.8.2/tests/server/secfolder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/server/secfolder/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/secfolder/private_keys/client.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/server/secfolder/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/secfolder/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/secfolder/public_keys/server.key
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/server/server_secfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/server_secfolder/allowEndpoints.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/server/server_secfolder/certificates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/server_secfolder/certificates/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/server/server_secfolder/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/server_secfolder/private_keys/server.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/server/server_secfolder/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/server_secfolder/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/server_secfolder/public_keys/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/test_EngineClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/server/test_RemoteSpineEngineManager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.465159 spinetoolbox-0.8.2/tests/spine_db_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.469159 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_PivotModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_alternative_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_compound_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_frozen_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_item_metadata_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_metadata_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_single_parameter_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_tree_item_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/test_graphics_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.473159 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/spine_db_editor_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_add_items_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_commit_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_delegates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_editors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_qtableview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44229 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_qtreeview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_edit_or_remove_items_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_mass_select_items_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_multi_spine_db_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_scenario_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_tabular_view_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_url_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_ProjectUpgrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24899 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_SpineDBManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41387 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_SpineToolboxProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47778 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_ToolboxUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_execution_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21340 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_load_project_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48008 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_project_item_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.473159 spinetoolbox-0.8.2/tests/test_resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.341157 spinetoolbox-0.8.2/tests/test_resources/Project Directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.473159 spinetoolbox-0.8.2/tests/test_resources/Project Directory/.spinetoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/Project Directory/.spinetoolbox/project.json
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/basic_model_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.477160 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v11.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v9.json
+-rw-r--r--   0 runner    (1001) docker     (127)    68068 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/spineopt_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_resources/test_tool_spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_spine_db_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/test_spine_engine_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:42.481160 spinetoolbox-0.8.2/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_AboutWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_AddProjectItemWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_AddUpSpineOptWizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_ArrayTableView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_CopyPasteTableView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_DatetimeEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_DurationEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_IndexedValueTableView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_InstallJuliaWizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16195 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_JupyterConsoleWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_KernelFetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_MapEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_MapTableView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_ParameterValueEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_PlainParameterValueEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_TimePatternEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_TimeSeriesFixedResolutionEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_TimeSeriesFixedResolutionTableView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_TimeSeriesVariableResolutionEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_custom_combobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_custom_qgraphicsscene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_custom_qlineedits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_custom_qtextbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_custom_qwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_indexed_value_table_context_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_jump_properties_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_kernel_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_open_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_plugin_manager_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_select_database_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 13:45:32.000000 spinetoolbox-0.8.2/tests/widgets/test_settings_widget.py
```

### Comparing `spinetoolbox-0.8.1/.github/workflows/test_runner.yml` & `spinetoolbox-0.8.2/.github/workflows/test_runner.yml`

 * *Files 13% similar despite different names*

```diff
@@ -14,54 +14,49 @@
 jobs:
   unit-tests:
     name: Unit tests
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: true
       matrix:
-        python-version: [3.8, 3.9, "3.10", 3.11]
+        python-version: [3.8, 3.9, "3.10", 3.11, 3.12]
         os: [windows-latest, ubuntu-22.04]
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Version from Git tags
       run: git describe --tags
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
         cache-dependency-path: |
-          requirements.txt
           pyproject.toml
+          requirements.txt
+          dev-requirements.txt
     - name: Display Python version
       run:
          python -c "import sys; print(sys.version)"
     - name: Install additional packages for Linux
       if: runner.os == 'Linux'
       run: |
         sudo apt-get update -y
         sudo apt-get install -y libegl1
     - name: Install dependencies
       env:
         PYTHONUTF8: 1
       run: |
         python -m pip install --upgrade pip
         python -m pip install -r requirements.txt
+        python -m pip install -r dev-requirements.txt
     - name: List packages
       run:
         python -m pip list
-    - name: Install python3 kernelspecs
-      run: |
-        python -m pip install ipykernel
-        python -m ipykernel install --user
-    - name: Install coverage
-      run:
-        python -m pip install coverage[toml]
     - name: Run tests
       run: |
         if [ "$RUNNER_OS" != "Windows" ]; then
           export QT_QPA_PLATFORM=offscreen
         fi
         coverage run -m unittest discover --verbose
       shell: bash
@@ -71,37 +66,39 @@
         CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
   execution-tests:
     name: Execution tests
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.8, 3.9, "3.10", 3.11]
+        python-version: [3.8, 3.9, "3.10", 3.11, 3.12]
         os: [windows-latest, ubuntu-22.04]
 #    needs: unit-tests
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
         cache-dependency-path: |
-          requirements.txt
           pyproject.toml
+          requirements.txt
+          dev-requirements.txt
     - name: Install additional packages for Linux
       if: runner.os == 'Linux'
       run: |
         sudo apt-get update -y
         sudo apt-get install -y libegl1
     - name: Install dependencies
       env:
         PYTHONUTF8: 1
       run: |
         python -m pip install --upgrade pip
         python -m pip install -r requirements.txt
+        python -m pip install -r dev-requirements.txt
     - name: List packages
       run: 
         python -m pip list
     - name: Run tests
       run:
         python -m unittest discover --pattern execution_test.py --verbose
```

### Comparing `spinetoolbox-0.8.1/.readthedocs.yml` & `spinetoolbox-0.8.2/.readthedocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
   - htmlzip
   - pdf
 
 # Optionally set the version of Python and requirements required to build your docs
 python:
   install:
     - requirements: requirements.txt
-    - requirements: docs/requirements.txt
+    - requirements: dev-requirements.txt
```

### Comparing `spinetoolbox-0.8.1/CHANGELOG.md` & `spinetoolbox-0.8.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # Changelog
 All **notable** changes to this project are documented here.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 
-## [Unreleased]
+## [0.8.2]
 
 ### Added
 
-### Changed
-
-### Deprecated
-
-### Removed
+- A button next to each entity class in **Entity Tree** that opens the *Add entities* -dialog.
+- Alternative -column in *Add entities* -dialog. If filled, the created entity will be set active in that alternative.
 
-### Fixed
+### Changed
 
-### Security
+- Python 3.12 and later is now supported.
+- When exporting GAMS `.gdx` files with Exporter, special values 10<sup>-10</sup> and `EPS`
+  now get converted to GAMS Eps (epsilon).
 
-## 0.8.1
+## [0.8.1]
 
 ### Added
+
 - Importer: it is now possible to reorder source tables by dragging and dropping.
 - Importer: it is now possible to reorder mappings by dragging and dropping.
 - Importer: it is now possible to copy mappings between source tables by dragging selected
   mappings from Mappings list onto destination source table item.
 
 ### Removed
 
 - Scenario active flag mappings have been removed from Importer and Exporter.
   The flag is not used anywhere and has not been accessible in Database editor
   for a long time.
 
-## 0.8.0
+## [0.8.0]
 
 ### Added
 
 - New context menu action (Select superclass) for entity class items in the entity tree.
 - Added Tool Specification type (Python, Gams, etc.) icons on Design View.
 - There is now a new filter type, Alternative filter available in Link properties.
   Unlike scenario filters, the execution is not parallelized.
```

### Comparing `spinetoolbox-0.8.1/COPYING` & `spinetoolbox-0.8.2/COPYING`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/COPYING.LESSER` & `spinetoolbox-0.8.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/PKG-INFO` & `spinetoolbox-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: spinetoolbox
-Version: 0.8.1
+Version: 0.8.2
 Summary: An application to define, manage, and execute various energy system simulation models
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://spine-toolbox.readthedocs.io/
 Project-URL: Repository, https://github.com/spine-tools/Spine-Toolbox
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.8.1
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: pyside6!=6.5.3,!=6.6.3,>=6.5.0
+Requires-Dist: pyside6!=6.5.3,!=6.6.3,!=6.7.0,>=6.5.0
 Requires-Dist: jupyter-client>=6.0
 Requires-Dist: qtconsole>=5.1
-Requires-Dist: sqlalchemy>=1.3
-Requires-Dist: spinedb_api>=0.31.1
-Requires-Dist: spine_engine>=0.24.0
+Requires-Dist: spinedb_api>=0.31.2
+Requires-Dist: spine_engine>=0.24.1
 Requires-Dist: numpy>=1.20.2
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: pandas>=1.3.2
 Requires-Dist: pygments>=2.8
 Requires-Dist: jill>=0.9.2
 Requires-Dist: pyzmq>=21.0
-Requires-Dist: spine-items>=0.22.1
+Requires-Dist: spine-items>=0.22.2
 
 # Spine Toolbox
 Link to the documentation: [https://spine-toolbox.readthedocs.io/en/latest/?badge=latest](https://spine-toolbox.readthedocs.io/en/latest/?badge=latest)
 
-[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
+[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Documentation Status](https://readthedocs.org/projects/spine-toolbox/badge/?version=latest)](https://spine-toolbox.readthedocs.io/en/latest/?badge=latest)
 [![Test suite](https://github.com/spine-tools/Spine-Toolbox/actions/workflows/test_runner.yml/badge.svg)](https://github.com/spine-tools/Spine-Toolbox/actions/workflows/test_runner.yml)
 [![codecov](https://codecov.io/gh/spine-tools/Spine-Toolbox/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Toolbox)
 [![PyPI version](https://badge.fury.io/py/spinetoolbox.svg)](https://badge.fury.io/py/spinetoolbox)
 [![Join the chat at https://gitter.im/spine-tools/Spine-Toolbox](https://badges.gitter.im/spine-tools/Spine-Toolbox.svg)](https://gitter.im/spine-tools/Spine-Toolbox?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 Spine Toolbox is an open source Python package to manage data, scenarios and workflows for modelling and simulation. 
@@ -46,23 +45,14 @@
 <p align="center" width="100%">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="./fig/spinetoolbox_logo.svg" width="50%">
     <img alt="Spine Toolbox" src="./fig/spinetoolbox_on_wht.svg" width="50%">
   </picture>
 </p>
 
-## Programming language
-
-- Python 3.8*
-- Python 3.9
-- Python 3.10
-- Python 3.11
-
-*Python 3.8.0 is not supported (use Python 3.8.1 or later).<br>
-
 ## License
 
 Spine Toolbox is released under the GNU Lesser General Public License (LGPL) license. 
 All accompanying documentation, original graphics and other material are released under the 
 [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
 Licenses of all packages used by Spine Toolbox are listed in the Spine Toolbox User 
 Guide.
@@ -86,16 +76,16 @@
 - [Windows installation package](#windows-64-bit-installer-package) (these are quite old - not recommended)
 
 ### Pre-installation
 
 These steps apply to both [Python/pipx](#installation-with-python-and-pipx) option and to 
 [From source files](#installation-from-sources-using-git) option.
 
-1. If you don't have Python installed, please install e.g. **Python 3.11** from 
-[Python.org](https://www.python.org/downloads/release/python-3117/).
+1. If you don't have Python installed, please install it e.g. from 
+[Python.org](https://www.python.org/downloads/).
 
 2. Test that python is now in your PATH. Open a new terminal (e.g. Command Prompt) window and type 
 
        python --version
 
     The output should be the Python version. If it did not work (e.g. the output is *'python' command not found* or 
 similar or the [Microsoft Store opens](https://learn.microsoft.com/en-us/windows/python/faqs#why-does-running-python-exe-open-the-microsoft-store-)),
@@ -277,48 +267,48 @@
 a quick look at how Spine Toolbox looks and feels (although even that has changed).
 Download the installer package from 
 [here](https://github.com/spine-tools/Spine-Toolbox/releases),
 run it, and follow the instructions to install Spine Toolbox.
 
 ### About requirements
 
-Python 3.8.1-3.11 is required. Python 3.8.0 is not supported due to problems in DLL loading on Windows.
+Python 3.8.1 or later is required. Python 3.8.0 is not supported due to problems in DLL loading on Windows.
 
 See the files `pyproject.toml` and `requirements.txt` for packages required to run Spine Toolbox.
 (Additional packages needed for development are listed in `dev-requirements.txt`.)
 
 The requirements include three packages ([`spinedb_api`](https://github.com/spine-tools/Spine-Database-API),
 [`spine_engine`](https://github.com/spine-tools/spine-engine), and 
 [`spine_items`](https://github.com/spine-tools/spine-items)), developed by the Spine project consortium.
 
 ### Building the User Guide
 
 You can find the latest documentation on [readthedocs](https://spine-toolbox.readthedocs.io/en/latest/index.html).
 If you want to build the documentation yourself,
 source files for the User Guide can be found in `docs/source` directory. In order to 
-build the HTML docs, you need to install the *optional requirements* (see section 
-'Installing requirements' above). This installs Sphinx (among other things), which 
+build the HTML docs, you need to install the *development requirements* (see section 
+'About requirements' above). This installs Sphinx (among other things), which 
 is required in building the documentation. When Sphinx is installed, you can build the 
 HTML pages from the user guide source files by using the `bin/build_doc.bat` script on 
-Windows or the `bin/build_doc.sh` script on Linux and Mac. After running the script, the 
+Windows or the `bin/build_doc.py` script on Linux and Mac. After running the script, the 
 index page can be found in `docs/build/html/index.html`. The User Guide can also 
-be opened from Spine Toolbox menu Help->User Guide (F2).
+be opened from Spine Toolbox menu Help->User Guide (F1).
 
 ### Troubleshooting
 
 #### Obscure crashes that may produce a traceback related to PySide6's model classes
 
 The first thing is to make sure that you are not using Anaconda. Only Miniconda is supported. Anaconda's base 
 environment includes Qt related packages and we suspect that they leak some shared Qt libraries into environments,
 even when specifically requesting that base environment packages should not be linked to environment packages. See
 also [Problems in starting the application](#problems-in-starting-the-application) below.
 
 #### Installation fails
 
-Please make sure you are using Python 3.8, 3.9, 3.10, or 3.11 to install the requirements.
+Please make sure you are using Python 3.8.1 or later to install the requirements.
 
 #### 'No Python' error when installing with pipx
 
 If you see the following error when running the command `python -m pipx install spinetoolbox`
 
 ```
 No Python at 'c:\python38\python.exe'
```

### Comparing `spinetoolbox-0.8.1/README.md` & `spinetoolbox-0.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Spine Toolbox
 Link to the documentation: [https://spine-toolbox.readthedocs.io/en/latest/?badge=latest](https://spine-toolbox.readthedocs.io/en/latest/?badge=latest)
 
-[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
+[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Documentation Status](https://readthedocs.org/projects/spine-toolbox/badge/?version=latest)](https://spine-toolbox.readthedocs.io/en/latest/?badge=latest)
 [![Test suite](https://github.com/spine-tools/Spine-Toolbox/actions/workflows/test_runner.yml/badge.svg)](https://github.com/spine-tools/Spine-Toolbox/actions/workflows/test_runner.yml)
 [![codecov](https://codecov.io/gh/spine-tools/Spine-Toolbox/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Toolbox)
 [![PyPI version](https://badge.fury.io/py/spinetoolbox.svg)](https://badge.fury.io/py/spinetoolbox)
 [![Join the chat at https://gitter.im/spine-tools/Spine-Toolbox](https://badges.gitter.im/spine-tools/Spine-Toolbox.svg)](https://gitter.im/spine-tools/Spine-Toolbox?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 Spine Toolbox is an open source Python package to manage data, scenarios and workflows for modelling and simulation. 
@@ -14,23 +14,14 @@
 <p align="center" width="100%">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="./fig/spinetoolbox_logo.svg" width="50%">
     <img alt="Spine Toolbox" src="./fig/spinetoolbox_on_wht.svg" width="50%">
   </picture>
 </p>
 
-## Programming language
-
-- Python 3.8*
-- Python 3.9
-- Python 3.10
-- Python 3.11
-
-*Python 3.8.0 is not supported (use Python 3.8.1 or later).<br>
-
 ## License
 
 Spine Toolbox is released under the GNU Lesser General Public License (LGPL) license. 
 All accompanying documentation, original graphics and other material are released under the 
 [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
 Licenses of all packages used by Spine Toolbox are listed in the Spine Toolbox User 
 Guide.
@@ -54,16 +45,16 @@
 - [Windows installation package](#windows-64-bit-installer-package) (these are quite old - not recommended)
 
 ### Pre-installation
 
 These steps apply to both [Python/pipx](#installation-with-python-and-pipx) option and to 
 [From source files](#installation-from-sources-using-git) option.
 
-1. If you don't have Python installed, please install e.g. **Python 3.11** from 
-[Python.org](https://www.python.org/downloads/release/python-3117/).
+1. If you don't have Python installed, please install it e.g. from 
+[Python.org](https://www.python.org/downloads/).
 
 2. Test that python is now in your PATH. Open a new terminal (e.g. Command Prompt) window and type 
 
        python --version
 
     The output should be the Python version. If it did not work (e.g. the output is *'python' command not found* or 
 similar or the [Microsoft Store opens](https://learn.microsoft.com/en-us/windows/python/faqs#why-does-running-python-exe-open-the-microsoft-store-)),
@@ -245,48 +236,48 @@
 a quick look at how Spine Toolbox looks and feels (although even that has changed).
 Download the installer package from 
 [here](https://github.com/spine-tools/Spine-Toolbox/releases),
 run it, and follow the instructions to install Spine Toolbox.
 
 ### About requirements
 
-Python 3.8.1-3.11 is required. Python 3.8.0 is not supported due to problems in DLL loading on Windows.
+Python 3.8.1 or later is required. Python 3.8.0 is not supported due to problems in DLL loading on Windows.
 
 See the files `pyproject.toml` and `requirements.txt` for packages required to run Spine Toolbox.
 (Additional packages needed for development are listed in `dev-requirements.txt`.)
 
 The requirements include three packages ([`spinedb_api`](https://github.com/spine-tools/Spine-Database-API),
 [`spine_engine`](https://github.com/spine-tools/spine-engine), and 
 [`spine_items`](https://github.com/spine-tools/spine-items)), developed by the Spine project consortium.
 
 ### Building the User Guide
 
 You can find the latest documentation on [readthedocs](https://spine-toolbox.readthedocs.io/en/latest/index.html).
 If you want to build the documentation yourself,
 source files for the User Guide can be found in `docs/source` directory. In order to 
-build the HTML docs, you need to install the *optional requirements* (see section 
-'Installing requirements' above). This installs Sphinx (among other things), which 
+build the HTML docs, you need to install the *development requirements* (see section 
+'About requirements' above). This installs Sphinx (among other things), which 
 is required in building the documentation. When Sphinx is installed, you can build the 
 HTML pages from the user guide source files by using the `bin/build_doc.bat` script on 
-Windows or the `bin/build_doc.sh` script on Linux and Mac. After running the script, the 
+Windows or the `bin/build_doc.py` script on Linux and Mac. After running the script, the 
 index page can be found in `docs/build/html/index.html`. The User Guide can also 
-be opened from Spine Toolbox menu Help->User Guide (F2).
+be opened from Spine Toolbox menu Help->User Guide (F1).
 
 ### Troubleshooting
 
 #### Obscure crashes that may produce a traceback related to PySide6's model classes
 
 The first thing is to make sure that you are not using Anaconda. Only Miniconda is supported. Anaconda's base 
 environment includes Qt related packages and we suspect that they leak some shared Qt libraries into environments,
 even when specifically requesting that base environment packages should not be linked to environment packages. See
 also [Problems in starting the application](#problems-in-starting-the-application) below.
 
 #### Installation fails
 
-Please make sure you are using Python 3.8, 3.9, 3.10, or 3.11 to install the requirements.
+Please make sure you are using Python 3.8.1 or later to install the requirements.
 
 #### 'No Python' error when installing with pipx
 
 If you see the following error when running the command `python -m pipx install spinetoolbox`
 
 ```
 No Python at 'c:\python38\python.exe'
```

### Comparing `spinetoolbox-0.8.1/benchmarks/compound_model_filter_accepts_model.py` & `spinetoolbox-0.8.2/benchmarks/compound_model_filter_accepts_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/benchmarks/db_mngr_get_icon_mngr.py` & `spinetoolbox-0.8.2/benchmarks/db_mngr_get_icon_mngr.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/benchmarks/db_mngr_get_item.py` & `spinetoolbox-0.8.2/benchmarks/db_mngr_get_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/benchmarks/db_mngr_get_value.py` & `spinetoolbox-0.8.2/benchmarks/db_mngr_get_value.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/bin/append_license.py` & `spinetoolbox-0.8.2/bin/append_license.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/bin/build_ui.py` & `spinetoolbox-0.8.2/bin/build_ui.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/bin/configure_julia.py` & `spinetoolbox-0.8.2/bin/configure_julia.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/bin/upgrade_spine_reqs.py` & `spinetoolbox-0.8.2/bin/upgrade_spine_reqs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/cx_Freeze_setup.py` & `spinetoolbox-0.8.2/cx_Freeze_setup.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/Makefile` & `spinetoolbox-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/make.bat` & `spinetoolbox-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/conf.py` & `spinetoolbox-0.8.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/contribution_guide.rst` & `spinetoolbox-0.8.2/docs/source/contribution_guide.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/A5_importer_specification.json` & `spinetoolbox-0.8.2/docs/source/data/A5_importer_specification.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/a5.xlsx` & `spinetoolbox-0.8.2/docs/source/data/a5.xlsx`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/contracted_load.txt` & `spinetoolbox-0.8.2/docs/source/data/contracted_load.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__from_node-relationship-parameter-values.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__from_node-relationship-parameter-values.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__from_node.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__from_node.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__node__node-relationship-parameter-values.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__node__node-relationship-parameter-values.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-connection__to_node.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-connection__to_node.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-node-parameter-values.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-node-parameter-values.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-node__commodity.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-node__commodity.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__from_node-relationship-parameter-values.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__from_node-relationship-parameter-values.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__from_node.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__from_node.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__node__node-relationship-parameter-values.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__node__node-relationship-parameter-values.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/cs-a5-unit__to_node.txt` & `spinetoolbox-0.8.2/docs/source/data/cs-a5-unit__to_node.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/el_prices.txt` & `spinetoolbox-0.8.2/docs/source/data/el_prices.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data/value_stored_water_vom.txt` & `spinetoolbox-0.8.2/docs/source/data/value_stored_water_vom.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/data_import_export.rst` & `spinetoolbox-0.8.2/docs/source/data_import_export.rst`

 * *Files 3% similar despite different names*

```diff
@@ -439,14 +439,24 @@
 
 **Scalars:**
 
 * A table that contains a numerical value in the top left cell is considered a GAMS scalar.
   Everything else (except the table name) is ignored.
 * The data in the top left cell is the scalar's value.
 
+The following conversions are done for GAMS special values:
+
+==================  ====================================================
+GAMS special value  Original value
+==================  ====================================================
++Inf                IEEE 754 infinity
+-Inf                Negative IEEE 754 infinity
+Eps                 2.2250738585072014e-308, 1e-10 or the string ``EPS``
+==================  ====================================================
+
 .. _Basic regular expressions for filtering:
 
 Basic regular expressions for filtering
 ***************************************
 
 See regular expressions on `wikipedia <https://en.wikipedia.org/wiki/Regular_expression>`_ and on
 Python's `documentation <https://docs.python.org/3/library/re.html#regular-expression-syntax>`_.
```

### Comparing `spinetoolbox-0.8.1/docs/source/executing_projects.rst` & `spinetoolbox-0.8.2/docs/source/executing_projects.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/execution_tests.rst` & `spinetoolbox-0.8.2/docs/source/execution_tests.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/getting_started.rst` & `spinetoolbox-0.8.2/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/how_to_run_spineopt.rst` & `spinetoolbox-0.8.2/docs/source/how_to_run_spineopt.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/DB_Tool_link_properties.png` & `spinetoolbox-0.8.2/docs/source/img/DB_Tool_link_properties.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/Tool_DB_link_properties.png` & `spinetoolbox-0.8.2/docs/source/img/Tool_DB_link_properties.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/dag_broken.png` & `spinetoolbox-0.8.2/docs/source/img/dag_broken.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/edit_tool_specification_blank.png` & `spinetoolbox-0.8.2/docs/source/img/edit_tool_specification_blank.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/example_dags.png` & `spinetoolbox-0.8.2/docs/source/img/example_dags.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/executable_tool_spec_dir_runner.png` & `spinetoolbox-0.8.2/docs/source/img/executable_tool_spec_dir_runner.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/execution_data_connection_selected.png` & `spinetoolbox-0.8.2/docs/source/img/execution_data_connection_selected.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/execution_julia_tool_selected.png` & `spinetoolbox-0.8.2/docs/source/img/execution_julia_tool_selected.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/exporter_mapping_options_dock.png` & `spinetoolbox-0.8.2/docs/source/img/exporter_mapping_options_dock.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/exporter_mapping_specification_dock.png` & `spinetoolbox-0.8.2/docs/source/img/exporter_mapping_specification_dock.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/exporter_mappings_dock.png` & `spinetoolbox-0.8.2/docs/source/img/exporter_mappings_dock.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/exporter_preview_docks.png` & `spinetoolbox-0.8.2/docs/source/img/exporter_preview_docks.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/exporter_properties.png` & `spinetoolbox-0.8.2/docs/source/img/exporter_properties.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/exporter_specification_editor.png` & `spinetoolbox-0.8.2/docs/source/img/exporter_specification_editor.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_added_input_file.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_added_input_file.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_after_first_execution.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_after_first_execution.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_dc_properties.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_dc_properties.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_dc_to_tool_connected.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_dc_to_tool_connected.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_dc_with_an_input_file.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_dc_with_an_input_file.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_final_execution_successful.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_final_execution_successful.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_first_tool_created.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_first_tool_created.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_first_tool_spec_created.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_first_tool_spec_created.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_say_hello_world_failed.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_say_hello_world_failed.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_tool_properties.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_tool_properties.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/getting_started_tool_spec_editor.png` & `spinetoolbox-0.8.2/docs/source/img/getting_started_tool_spec_editor.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/import_editor_column_data_type_menu.png` & `spinetoolbox-0.8.2/docs/source/img/import_editor_column_data_type_menu.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/import_editor_preview_table_mapping_menu.png` & `spinetoolbox-0.8.2/docs/source/img/import_editor_preview_table_mapping_menu.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/import_editor_window.png` & `spinetoolbox-0.8.2/docs/source/img/import_editor_window.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/importer_connector_type.png` & `spinetoolbox-0.8.2/docs/source/img/importer_connector_type.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/importer_properties.png` & `spinetoolbox-0.8.2/docs/source/img/importer_properties.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/importer_spec_editor_anonymous_mode.png` & `spinetoolbox-0.8.2/docs/source/img/importer_spec_editor_anonymous_mode.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/julia_jupyter_console_selected.png` & `spinetoolbox-0.8.2/docs/source/img/julia_jupyter_console_selected.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/julia_kernel_specification_creator.png` & `spinetoolbox-0.8.2/docs/source/img/julia_kernel_specification_creator.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/main_window_no_project.png` & `spinetoolbox-0.8.2/docs/source/img/main_window_no_project.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/minimal_tool_specification.png` & `spinetoolbox-0.8.2/docs/source/img/minimal_tool_specification.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/open_tool_specification_editor.png` & `spinetoolbox-0.8.2/docs/source/img/open_tool_specification_editor.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/plot_data.png` & `spinetoolbox-0.8.2/docs/source/img/plot_data.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/plotting_popup_menu.png` & `spinetoolbox-0.8.2/docs/source/img/plotting_popup_menu.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/plotting_popup_menu_plot_in_window.png` & `spinetoolbox-0.8.2/docs/source/img/plotting_popup_menu_plot_in_window.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/plotting_use_as_x_popup.png` & `spinetoolbox-0.8.2/docs/source/img/plotting_use_as_x_popup.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/plotting_window_added_plot.png` & `spinetoolbox-0.8.2/docs/source/img/plotting_window_added_plot.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/plotting_window_single_column.png` & `spinetoolbox-0.8.2/docs/source/img/plotting_window_single_column.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/python_jupyter_console_selected.png` & `spinetoolbox-0.8.2/docs/source/img/python_jupyter_console_selected.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/python_kernel_specification_creator.png` & `spinetoolbox-0.8.2/docs/source/img/python_kernel_specification_creator.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/right_click_options.png` & `spinetoolbox-0.8.2/docs/source/img/right_click_options.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/select_url_for_remote_db_export.png` & `spinetoolbox-0.8.2/docs/source/img/select_url_for_remote_db_export.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/settings_db_editor.png` & `spinetoolbox-0.8.2/docs/source/img/settings_db_editor.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/settings_engine.png` & `spinetoolbox-0.8.2/docs/source/img/settings_engine.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/settings_general.png` & `spinetoolbox-0.8.2/docs/source/img/settings_general.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/settings_specification_editors.png` & `spinetoolbox-0.8.2/docs/source/img/settings_specification_editors.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/settings_tools_default.png` & `spinetoolbox-0.8.2/docs/source/img/settings_tools_default.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/spineopt_install_wizard_successful.png` & `spinetoolbox-0.8.2/docs/source/img/spineopt_install_wizard_successful.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/spinetoolbox_on_wht.svg` & `spinetoolbox-0.8.2/docs/source/img/spinetoolbox_on_wht.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/start_jupyter_console_menu_listing.png` & `spinetoolbox-0.8.2/docs/source/img/start_jupyter_console_menu_listing.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/toolbar_with_one_tool_specification.png` & `spinetoolbox-0.8.2/docs/source/img/toolbar_with_one_tool_specification.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/using_input_output_files_in_tool_scripts.png` & `spinetoolbox-0.8.2/docs/source/img/using_input_output_files_in_tool_scripts.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_array.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_array.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_datetime.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_datetime.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_duration.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_duration.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_map.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_map.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_map_after_conversion.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_map_after_conversion.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_map_before_conversion.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_map_before_conversion.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_parameter_type.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_parameter_type.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_plain.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_plain.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_time_pattern.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_time_pattern.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_time_series_fixed.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_time_series_fixed.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/img/value_editor_time_series_variable.png` & `spinetoolbox-0.8.2/docs/source/img/value_editor_time_series_variable.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/index.rst` & `spinetoolbox-0.8.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/links.rst` & `spinetoolbox-0.8.2/docs/source/links.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/main_window.rst` & `spinetoolbox-0.8.2/docs/source/main_window.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/metadata_description.rst` & `spinetoolbox-0.8.2/docs/source/metadata_description.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/parameter_value_editor.rst` & `spinetoolbox-0.8.2/docs/source/parameter_value_editor.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/plotting.rst` & `spinetoolbox-0.8.2/docs/source/plotting.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/project_item_development.rst` & `spinetoolbox-0.8.2/docs/source/project_item_development.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/project_items.rst` & `spinetoolbox-0.8.2/docs/source/project_items.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/publishing_to_pypi.rst` & `spinetoolbox-0.8.2/docs/source/publishing_to_pypi.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/setting_up.rst` & `spinetoolbox-0.8.2/docs/source/setting_up.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/settings.rst` & `spinetoolbox-0.8.2/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/adding_data.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/adding_data.rst`

 * *Files 1% similar despite different names*

```diff
@@ -66,30 +66,33 @@
 
 Adding entities
 ===============
 
 From **Entity Tree** or **Graph View**
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Right-click on the root item in **Entity Tree** and select **Add entities**, or click on an empty space
+There are several different ways to add entities to an existing entity class. The easiest way is to click on the
+(|add|) -button next to an entity class. The other ways are to
+right-click on the class or root item in **Entity Tree** and select **Add entities**, or click on an empty space
 in the **Graph View** and select **Add entities...** from the context menu.
 
-This will open up the **Add entities** dialog:
+All of these methods will open up the **Add entities** dialog:
 
 .. image:: img/add_entities_dialog.png
    :align: center
 
 Select the class where you want to add the entities from **Entity class**. It will list all of the entity classes.
 To narrow down the list, instead of opening the dialog from the root item, open it from a specific entity class item
 in the **Entity Tree**. This way the class will be preselected from the list and the list will overall only contain
 other classes that are relevant to the selected class.
 
-Enter the names of the entities under **entity name**. Finally, select the databases where you want to add the
-entities under **databases**. When you're ready, press **Ok**. Rows can once again be deleted with the
-**Remove selected rows** -button.
+Enter the names of the entities under **entity name**. The column **alternative** is optional. Filling it in
+will automatically set the entity active in the selected alternative. Finally, select the databases where you
+want to add the entities under **databases**. When you're ready, press **Ok**. Rows can once again be deleted
+with the **Remove selected rows** -button.
 
 With N-D entity classes, the elements need to be specified. After defining the elements the entity's name can be
 modified:
 
 .. image:: img/add_entities_dialog_2D.png
    :align: center
```

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/committing_and_history.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/committing_and_history.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/getting_started.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/getting_started.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entity_classes_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entity_classes_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entity_classes_dialog_2D.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entity_classes_dialog_2D.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/add_entity_group_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/add_entity_group_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/alternative_tree.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/alternative_tree.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/commit_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/commit_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/commit_viewer.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/commit_viewer.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/dirty_db.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/dirty_db.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/edit_entity_classes_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/edit_entity_classes_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_alternative_table.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_alternative_table.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_graph.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_graph.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_name_filter_menu.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_name_filter_menu.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_parameter_value_table.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_parameter_value_table.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/entity_tree_context_menu.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/entity_tree_context_menu.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/excel_entity_sheet.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/excel_entity_sheet.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/excel_entity_sheet_timeseries.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/excel_entity_sheet_timeseries.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/export_bar.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/export_bar.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/generate_scenarios_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/generate_scenarios_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/item_metadata.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/item_metadata.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/manage_entities_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/manage_entities_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/manage_members_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/manage_members_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/mass_export_items_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/mass_export_items_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/metadata.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/metadata.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/parameter_value_list.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/parameter_value_list.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/pivot_table.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/pivot_table.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/plain_db_editor.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/plain_db_editor.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/purge_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/purge_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/remove_entities_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/remove_entities_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/scenario_tree.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/scenario_tree.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/img/uncommitted_changes_dialog.png` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/img/uncommitted_changes_dialog.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/importing_and_exporting_data.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/importing_and_exporting_data.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/managing_data.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/managing_data.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/removing_data.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/removing_data.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/updating_data.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/updating_data.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/vacuum.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/vacuum.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_db_editor/viewing_data.rst` & `spinetoolbox-0.8.2/docs/source/spine_db_editor/viewing_data.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/spine_engine_server.rst` & `spinetoolbox-0.8.2/docs/source/spine_engine_server.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/terminology.rst` & `spinetoolbox-0.8.2/docs/source/terminology.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/tool_specification_editor.rst` & `spinetoolbox-0.8.2/docs/source/tool_specification_editor.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/ui_guidelines.rst` & `spinetoolbox-0.8.2/docs/source/ui_guidelines.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/docs/source/unit_testing_guidelines.rst` & `spinetoolbox-0.8.2/docs/source/unit_testing_guidelines.rst`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/active_by_default/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/active_by_default/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/active_by_default/.spinetoolbox/specifications/Exporter/export_entities.json` & `spinetoolbox-0.8.2/execution_tests/active_by_default/.spinetoolbox/specifications/Exporter/export_entities.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/active_by_default/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/active_by_default/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/alternative_filters/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/alternative_filters/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/alternative_filters/.spinetoolbox/specifications/Exporter/export_values.json` & `spinetoolbox-0.8.2/execution_tests/alternative_filters/.spinetoolbox/specifications/Exporter/export_values.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/alternative_filters/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/alternative_filters/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/Exporter/entities.json` & `spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/.spinetoolbox/specifications/Exporter/entities.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/export_entities_with_entity_alternatives/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/export_entities_with_entity_alternatives/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/hello_world_on_server/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/hello_world_on_server/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/hello_world_on_server/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/hello_world_on_server/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/import_file_packs/.spinetoolbox/specifications/Importer/import_dat_files.json` & `spinetoolbox-0.8.2/execution_tests/import_file_packs/.spinetoolbox/specifications/Importer/import_dat_files.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/import_file_packs/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/import_file_packs/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/counter_data_importer.json` & `spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/counter_data_importer.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/import_data.json` & `spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/.spinetoolbox/specifications/Importer/import_data.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/loop_condition_with_cmd_line_args/tool.py` & `spinetoolbox-0.8.2/execution_tests/loop_condition_with_cmd_line_args/tool.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/merger_write_order/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/merger_write_order/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/merger_write_order/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/merger_write_order/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/Exporter/exporter.json` & `spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/.spinetoolbox/specifications/Exporter/exporter.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/modify_connection_filter_by_script/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/modify_connection_filter_by_script/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/parallel_importer/.spinetoolbox/specifications/Importer/import_tool_output.json` & `spinetoolbox-0.8.2/execution_tests/parallel_importer/.spinetoolbox/specifications/Importer/import_tool_output.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/parallel_importer/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/parallel_importer/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Importer/import_tool_output.json` & `spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/.spinetoolbox/specifications/Importer/import_tool_output.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/parallel_importer_with_datapackage/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/parallel_importer_with_datapackage/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/scenario_filters/.spinetoolbox/specifications/Importer/input_data_mapping.json` & `spinetoolbox-0.8.2/execution_tests/scenario_filters/.spinetoolbox/specifications/Importer/input_data_mapping.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/scenario_filters/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/scenario_filters/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.spinetoolbox/items/raw_data/units.xlsx` & `spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.spinetoolbox/items/raw_data/units.xlsx`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/Importer 1 - units.xlsx.json` & `spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/Importer 1 - units.xlsx.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/execution_tests/simple_importer_on_server/execution_test.py` & `spinetoolbox-0.8.2/execution_tests/simple_importer_on_server/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/fig/eu-emblem-low-res.jpg` & `spinetoolbox-0.8.2/fig/eu-emblem-low-res.jpg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/fig/spinetoolbox_logo.svg` & `spinetoolbox-0.8.2/fig/spinetoolbox_logo.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/fig/spinetoolbox_on_wht.svg` & `spinetoolbox-0.8.2/fig/spinetoolbox_on_wht.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/pylintrc` & `spinetoolbox-0.8.2/pylintrc`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/pyproject.toml` & `spinetoolbox-0.8.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 keywords = ["energy system modelling", "workflow", "optimisation", "database"]
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.8.1, <3.12"
+requires-python = ">=3.8.1"
 dependencies = [
-    "pyside6 >= 6.5.0, != 6.5.3, != 6.6.3",
+    "pyside6 >= 6.5.0, != 6.5.3, != 6.6.3, != 6.7.0",
     "jupyter-client >=6.0",
     "qtconsole >=5.1",
-    "sqlalchemy >=1.3",
-    "spinedb_api>=0.31.1",
-    "spine_engine>=0.24.0",
+    "spinedb_api>=0.31.2",
+    "spine_engine>=0.24.1",
     "numpy >=1.20.2",
     "matplotlib >= 3.5",
     "scipy >=1.7.1",
     "networkx >=2.6",
     "pandas >=1.3.2",
     "pygments >=2.8",
     "jill >=0.9.2",
     "pyzmq >=21.0",
-    "spine-items>=0.22.1",
+    "spine-items>=0.22.2",
 ]
 
 [project.urls]
 Documentation = "https://spine-toolbox.readthedocs.io/"
 Repository = "https://github.com/spine-tools/Spine-Toolbox"
 
 [project.scripts]
```

### Comparing `spinetoolbox-0.8.1/setup-debug.iss` & `spinetoolbox-0.8.2/setup-debug.iss`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/setup.iss` & `spinetoolbox-0.8.2/setup.iss`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/__main__.py` & `spinetoolbox-0.8.2/spinetoolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/config.py` & `spinetoolbox-0.8.2/spinetoolbox/config.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/execution_managers.py` & `spinetoolbox-0.8.2/spinetoolbox/execution_managers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/fetch_parent.py` & `spinetoolbox-0.8.2/spinetoolbox/fetch_parent.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/headless.py` & `spinetoolbox-0.8.2/spinetoolbox/headless.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/helpers.py` & `spinetoolbox-0.8.2/spinetoolbox/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1203,15 +1203,18 @@
     Returns:
         ProjectItemSpecification: item specification or None if reading the file failed
     """
     spec_dict = parse_specification_file(spec_path, logger)
     if spec_dict is None:
         return None
     spec_dict["definition_file_path"] = spec_path
-    spec = specification_from_dict(spec_dict, local_data_dict, spec_factories, app_settings, logger)
+    try:
+        spec = specification_from_dict(spec_dict, local_data_dict, spec_factories, app_settings, logger)
+    except KeyError:
+        spec = None
     if spec is not None:
         spec.definition_file_path = spec_path
     return spec
 
 
 def specification_from_dict(spec_dict, local_data_dict, spec_factories, app_settings, logger):
     """Returns item specification from a dictionary.
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/kernel_fetcher.py` & `spinetoolbox-0.8.2/spinetoolbox/kernel_fetcher.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/link.py` & `spinetoolbox-0.8.2/spinetoolbox/link.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/load_project_items.py` & `spinetoolbox-0.8.2/spinetoolbox/load_project_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/log_mixin.py` & `spinetoolbox-0.8.2/spinetoolbox/log_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/logger_interface.py` & `spinetoolbox-0.8.2/spinetoolbox/logger_interface.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/main.py` & `spinetoolbox-0.8.2/spinetoolbox/main.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/metaobject.py` & `spinetoolbox-0.8.2/spinetoolbox/metaobject.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/array_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/array_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/compound_table_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/compound_table_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 from PySide6.QtCore import Qt, Signal, Slot, QModelIndex, QTimer
 from ..mvcmodels.minimal_table_model import MinimalTableModel
 
 
 class CompoundTableModel(MinimalTableModel):
     """A model that concatenates several sub table models vertically."""
 
-    refreshed = Signal()
-
     def __init__(self, parent=None, header=None):
         """Initializes model.
 
         Args:
             parent (QObject, optional): the parent object
             header (list of str, optional): header labels
         """
@@ -115,15 +113,14 @@
     def _do_refresh(self):
         """Recomputes the row and inverse row maps."""
         self._row_map.clear()
         self._inv_row_map.clear()
         for model in self.sub_models:
             row_map = self._row_map_for_model(model)
             self._append_row_map(row_map)
-        self.refreshed.emit()
 
     def _append_row_map(self, row_map):
         """Appends given row map to the tail of the model.
 
         Args:
             row_map (list): tuples (model, row number)
         """
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/empty_row_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/empty_row_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/file_list_models.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/file_list_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/filter_checkbox_list_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/filter_checkbox_list_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/filter_execution_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/filter_execution_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/indexed_value_table_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/indexed_value_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/map_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/map_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/minimal_table_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/minimal_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/minimal_tree_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/minimal_tree_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/project_item_specification_models.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/project_item_specification_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/resource_filter_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/resource_filter_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/shared.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/shared.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/time_pattern_model.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/time_pattern_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py` & `spinetoolbox-0.8.2/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/plotting.py` & `spinetoolbox-0.8.2/spinetoolbox/plotting.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/plugin_manager.py` & `spinetoolbox-0.8.2/spinetoolbox/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project.py` & `spinetoolbox-0.8.2/spinetoolbox/project.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_commands.py` & `spinetoolbox-0.8.2/spinetoolbox/project_commands.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_item/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/project_item/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_item/logging_connection.py` & `spinetoolbox-0.8.2/spinetoolbox/project_item/logging_connection.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_item/project_item.py` & `spinetoolbox-0.8.2/spinetoolbox/project_item/project_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_item/project_item_factory.py` & `spinetoolbox-0.8.2/spinetoolbox/project_item/project_item_factory.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_item/specification_editor_window.py` & `spinetoolbox-0.8.2/spinetoolbox/project_item/specification_editor_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_item_icon.py` & `spinetoolbox-0.8.2/spinetoolbox/project_item_icon.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_settings.py` & `spinetoolbox-0.8.2/spinetoolbox/project_settings.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/project_upgrader.py` & `spinetoolbox-0.8.2/spinetoolbox/project_upgrader.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/qthread_pool_executor.py` & `spinetoolbox-0.8.2/spinetoolbox/qthread_pool_executor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/resources_icons_rc.py` & `spinetoolbox-0.8.2/spinetoolbox/resources_icons_rc.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/resources_logos_rc.py` & `spinetoolbox-0.8.2/spinetoolbox/resources_logos_rc.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/server/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/server/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/server/engine_client.py` & `spinetoolbox-0.8.2/spinetoolbox/server/engine_client.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_commands.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_commands.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/graphics_items.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/graphics_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -892,15 +892,17 @@
 
     def refresh_icon(self):
         """Refreshes the icon."""
         el_items = [arc_item.el_item for arc_item in self.arc_items]
         dimension_name_list = tuple(
             el_item.entity_class_name for el_item in el_items if not isinstance(el_item, CrossHairsItem)
         )
-        self._renderer = self.db_mngr.get_icon_mngr(self.first_db_map).multi_class_renderer(dimension_name_list)
+        self._renderer = self.db_mngr.get_icon_mngr(self.first_db_map).multi_class_renderer(
+            None, dimension_name_list, None
+        )
         self._install_renderer()
 
     def contextMenuEvent(self, e):
         e.accept()
 
 
 class CrossHairsArcItem(ArcItem):
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/helpers.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/main.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/main.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/alternative_item.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/alternative_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/alternative_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/alternative_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/colors.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/colors.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/compound_models.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/compound_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/empty_models.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/empty_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/mime_types.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/mime_types.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/scenario_item.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/scenario_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/scenario_model.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/scenario_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/single_and_empty_model_mixins.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/single_and_empty_model_mixins.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/single_models.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/single_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/mvcmodels/utils.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/mvcmodels/utils.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/scenario_generation.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/scenario_generation.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.ui` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/commit_viewer_affected_item_info.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/db_commit_viewer.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/db_commit_viewer.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/db_commit_viewer.ui` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/db_commit_viewer.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/scenario_generator.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/scenario_generator.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/scenario_generator.ui` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/scenario_generator.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/select_databases.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/select_databases.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/select_databases.ui` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/select_databases.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.ui` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -480,19 +480,29 @@
         # Base class is zero-dimensional, check if given ent_cls containts it
         return self.entity_class["name"] in set(ent_cls["dimension_name_list"]) | {ent_cls["name"]}
 
     def make_model(self):
         return EmptyRowModel(self)
 
     def _do_reset_model(self):
-        header = self.dimension_name_list + ("entity name", "databases")
+        header = self.dimension_name_list + ("entity name", "alternative", "databases")
         self.model.set_horizontal_header_labels(header)
         default_db_maps = [db_map for db_map, keys in self.db_map_ent_cls_lookup.items() if self.class_key in keys]
         db_names = ",".join([db_name for db_name, db_map in self.keyed_db_maps.items() if db_map in default_db_maps])
-        defaults = {"databases": db_names}
+        alt_selection_model = self.parent().ui.alternative_tree_view.selectionModel()
+        alt_selection = alt_selection_model.selection()
+        alternative = None
+        if alt_selection:
+            selected_alternative_index = alt_selection_model.currentIndex()
+            alternative = selected_alternative_index.model().item_from_index(selected_alternative_index)
+        all_databases = [db_map for db_name, db_map in self.keyed_db_maps.items() if db_map in default_db_maps]
+        alt_name_list = [x["name"] for db_map in all_databases for x in self.db_mngr.get_items(db_map, "alternative")]
+        alt_name_list.append("")
+        alternative_name = alternative.name if alternative else alt_name_list[0]
+        defaults = {"databases": db_names, "alternative": alternative_name}
         defaults.update(self.entity_names_by_class_name)
         self.model.set_default_row(**defaults)
         self.model.clear()
 
     def get_db_map_data(self):
         db_map_data = {}
         name_column = self.model.horizontal_header_labels().index("entity name")
@@ -541,16 +551,51 @@
         db_map_data = self.get_db_map_data()
         if db_map_data is None:
             return
         if not db_map_data:
             self.parent().msg_error.emit("Nothing to add")
             return
         self.db_mngr.add_entities(db_map_data)
+        created_entities = {}
+        for db_map, data in db_map_data.items():
+            for item in data:
+                created_entities.update(
+                    {item["name"]: db_map.get_entity_item(class_id=item["class_id"], name=item["name"])}
+                )
+        entity_alternatives = self.make_entity_alternatives(created_entities)
+        if entity_alternatives:  # If alternatives have been defined
+            self.db_mngr.add_entity_alternatives(entity_alternatives)
         super().accept()
 
+    def make_entity_alternatives(self, entities):
+        """Creates a mapping from db_map to entity alternatives that are to be created"""
+        entity_alternatives = {}
+        name_column = self.model.horizontal_header_labels().index("entity name")
+        alternative_column = self.model.horizontal_header_labels().index("alternative")
+        db_column = self.model.horizontal_header_labels().index("databases")
+        for i in range(self.model.rowCount() - 1):
+            row_data = self.model.row_data(i)
+            alternative = row_data[alternative_column]
+            if not alternative:
+                continue
+            entity_name = row_data[name_column]
+            entity = entities[entity_name]
+            db_names = row_data[db_column]
+            for db_name in db_names.split(","):
+                db_map = self.keyed_db_maps[db_name]
+                entity_alternatives.setdefault(db_map, []).append(
+                    {
+                        "entity_class_name": entity["entity_class_name"],
+                        "alternative_name": alternative,
+                        "entity_byname": entity["entity_byname"],
+                        "active": True,
+                    }
+                )
+        return entity_alternatives
+
 
 class ManageElementsDialog(AddEntitiesOrManageElementsDialog):
     """A dialog to query user's preferences for managing entity dimensions."""
 
     def __init__(self, parent, item, db_mngr, *db_maps):
         """
         Args:
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/commit_viewer.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/commit_viewer.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_delegates.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_delegates.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Custom item delegates."""
 from numbers import Number
-from PySide6.QtCore import QModelIndex, Qt, Signal
+from PySide6.QtCore import QModelIndex, Qt, Signal, QRect, QEvent
+from PySide6.QtGui import QIcon, QFontMetrics
 from PySide6.QtWidgets import QStyledItemDelegate
 from spinedb_api import to_database
 from spinedb_api.parameter_value import join_value_and_type
 from spinetoolbox.spine_db_editor.widgets.custom_editors import (
     BooleanSearchBarEditor,
     CustomLineEditor,
     CustomComboBoxEditor,
@@ -705,14 +706,32 @@
         Args:
             editor (QWidget): editor widget
             index (QModelIndex): index being edited
         """
         if isinstance(editor, SearchBarEditor):
             editor.data_committed.connect(lambda *_: self.close_editor(editor, index))
 
+    def _create_alternative_editor(self, parent, index):
+        """Creates an editor.
+
+        Args:
+            parent (QWidget): parent widget
+            index (QModelIndex): index being edited
+
+        Returns:
+            QWidget: editor
+        """
+        editor = SearchBarEditor(self.parent(), parent)
+        all_databases = self.parent().keyed_db_maps.values()
+        name_list = [
+            x["name"] for db_map in all_databases for x in self.parent().db_mngr.get_items(db_map, "alternative")
+        ]
+        editor.set_data(index.data(Qt.ItemDataRole.EditRole), name_list)
+        return editor
+
     def _create_database_editor(self, parent, index):
         """Creates an editor.
 
         Args:
             parent (QWidget): parent widget
             index (QModelIndex): index being edited
 
@@ -781,14 +800,16 @@
         header = index.model().horizontal_header_labels()
         if header[index.column()] == "entity name":
             editor = CustomLineEditor(parent)
             data = index.data(Qt.ItemDataRole.EditRole)
             editor.set_data(data)
         elif header[index.column()] == "databases":
             editor = self._create_database_editor(parent, index)
+        elif header[index.column()] == "alternative":
+            editor = self._create_alternative_editor(parent, index)
         else:
             editor = SearchBarEditor(parent)
             entity_name_list = self.parent().entity_name_list(index.row(), index.column())
             editor.set_data(index.data(Qt.ItemDataRole.EditRole), entity_name_list)
         self.connect_editor_signals(editor, index)
         return editor
 
@@ -842,7 +863,59 @@
                 if self._metadata_model.index(i, MetadataColumn.DB_MAP).data() == database_codename:
                     items.add(self._metadata_model.index(i, self._column).data())
         else:
             for i in range(self._metadata_model.rowCount() - 1):
                 items.add(self._metadata_model.index(i, self._column).data())
         editor.addItems(sorted(items))
         return editor
+
+
+class AddEntityButtonDelegate(QStyledItemDelegate):
+    """A delegate for adding entities from a button in Entity Tree View."""
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.plus_icon = QIcon(":/icons/menu_icons/cube_plus.svg")
+
+    def paint(self, painter, option, index):
+        super().paint(painter, option, index)
+        if not self.is_entity_class(index):  # Add the button only for entity classes
+            return
+        text = index.data(Qt.DisplayRole)
+        font_metrics = QFontMetrics(option.font)
+        text_width = font_metrics.width(text)
+        icon_size = option.decorationSize
+        button_rect = self.get_button_rect(option, icon_size.width(), text_width)
+        self.plus_icon.paint(painter, button_rect)
+
+    @staticmethod
+    def is_entity_class(index):
+        """Check if index refers to entity class"""
+        parent_index = index.parent()
+        grand_parent = parent_index.parent()
+        return index.column() == 0 and (parent_index.isValid() and not grand_parent.isValid())
+
+    @staticmethod
+    def get_button_rect(option, icon_width, text_width):
+        size = 16
+        margin = 20
+        x = option.rect.left() + icon_width + text_width + margin
+        y = option.rect.center().y() - size // 2
+        return QRect(x, y, size, size)
+
+    def editorEvent(self, event, model, option, index):
+        if event.type() == QEvent.MouseButtonPress and event.buttons() & Qt.LeftButton:
+            text = index.data(Qt.DisplayRole)
+            font_metrics = QFontMetrics(option.font)
+            text_width = font_metrics.width(text)
+            icon_size = option.decorationSize
+            button_rect = self.get_button_rect(option, icon_size.width(), text_width)
+            if button_rect.contains(event.pos()) and self.is_entity_class(index):
+                self.handle_button_click(index)
+                return True
+        return super().editorEvent(event, model, option, index)
+
+    def handle_button_click(self, index):
+        """Opens the Add Entities -dialog for the selected entity class item"""
+        entity_tree_view = self.parent()
+        entity_tree_view._context_item = entity_tree_view.model().item_from_index(index)
+        entity_tree_view.add_entities()
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_editors.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_editors.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_menus.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
     def prune_selected_items(self, checked=False):
         """Prunes selected items."""
         key = self._get_selected_entity_names()
         self._spine_db_editor.prune_graph(key, {db_map_id for x in self.selected_items for db_map_id in x.db_map_ids})
 
     @Slot(QAction)
     def _prune_class(self, action):
-        """Prunnes some class."""
+        """Prunes some class."""
         key = action.text()
         self._spine_db_editor.prune_graph(
             key,
             {
                 (db_map, x["id"])
                 for item in self._items_per_class[key]
                 for db_map in item.db_maps
@@ -874,14 +874,19 @@
     def keyPressEvent(self, event):
         """Aborts relationship creation if user presses ESC."""
         super().keyPressEvent(event)
         if event.key() == Qt.Key_Escape and self.cross_hairs_items:
             self._spine_db_editor.msg.emit("Relationship creation aborted.")
             self.clear_cross_hairs_items()
 
+    def focusOutEvent(self, event):
+        if self.cross_hairs_items:
+            self.clear_cross_hairs_items()
+        super().focusOutEvent(event)
+
     def contextMenuEvent(self, e):
         """Shows context menu.
 
         Args:
             e (QContextMenuEvent): Context menu event
         """
         super().contextMenuEvent(e)
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,18 @@
     def _set_column_resize_modes(self, old_column_count, new_column_count):
         if new_column_count != self._EXPECTED_COLUMN_COUNT:
             return
         for column in range(new_column_count):
             width = self._initial_column_size(column)
             self.horizontalHeader().resizeSection(column, width)
 
+    def set_db_column_visibility(self, visible):
+        """Sets the visibility of the db column"""
+        self.setColumnHidden(self._EXPECTED_COLUMN_COUNT - 1, not visible)
+
 
 class ParameterTableView(StackedTableView):
     value_column_header: str = NotImplemented
     """Either "default_value" or "value". Used to identify the value column for advanced editing and plotting."""
 
     def __init__(self, parent):
         """
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Classes for custom QTreeViews and QTreeWidgets."""
-from PySide6.QtWidgets import QApplication, QHeaderView, QMenu, QAbstractItemView, QTreeWidget, QTreeWidgetItem
+from PySide6.QtWidgets import QApplication, QHeaderView, QMenu, QAbstractItemView
 from PySide6.QtCore import Signal, Slot, Qt, QEvent, QTimer, QModelIndex, QItemSelection, QSignalBlocker
 from PySide6.QtGui import QMouseEvent, QIcon, QGuiApplication
 from spinetoolbox.widgets.custom_qtreeview import CopyPasteTreeView
-from spinetoolbox.helpers import busy_effect, CharIconEngine, DB_ITEM_SEPARATOR
-from .custom_delegates import ScenarioDelegate, AlternativeDelegate, ParameterValueListDelegate
+from spinetoolbox.helpers import busy_effect, CharIconEngine
+from .custom_delegates import ScenarioDelegate, AlternativeDelegate, ParameterValueListDelegate, AddEntityButtonDelegate
 from .scenario_generator import ScenarioGenerator
 from ..mvcmodels import mime_types
 from ..mvcmodels.alternative_item import AlternativeItem
 from ..mvcmodels.scenario_item import ScenarioDBItem, ScenarioAlternativeItem, ScenarioItem
 
 
 class EntityTreeView(CopyPasteTreeView):
@@ -30,14 +30,15 @@
 
     def __init__(self, parent):
         """
         Args:
             parent (QWidget): parent widget
         """
         super().__init__(parent=parent)
+        self.setItemDelegate(AddEntityButtonDelegate(self))
         self._context_item = None
         self._selected_indexes = {}
         self._menu = QMenu(self)
         self._spine_db_editor = None
         self._fully_expand_action = None
         self._fully_collapse_action = None
         self._add_entity_classes_action = None
@@ -57,16 +58,16 @@
         self._fetch_more_timer = QTimer(self)
         self._fetch_more_timer.setSingleShot(True)
         self._fetch_more_timer.setInterval(100)
         self._fetch_more_timer.timeout.connect(self._fetch_more_visible)
         self._find_next_action = None
         self._hide_empty_classes_action = None
         self._entity_index = None
-        header = self.header()
-        header.setSectionResizeMode(QHeaderView.ResizeMode.ResizeToContents)
+        self._header = self.header()
+        self._header.setSectionResizeMode(QHeaderView.ResizeMode.ResizeToContents)
 
     def reset(self):
         super().reset()
         self._selected_indexes = {}
 
     def connect_spine_db_editor(self, spine_db_editor):
         """Connects a Spine db editor to work with this view.
@@ -74,14 +75,21 @@
         Args:
              spine_db_editor (SpineDBEditor)
         """
         self._spine_db_editor = spine_db_editor
         self._create_context_menu()
         self.connect_signals()
 
+    def set_db_column_visibility(self, visible):
+        """Sets the visibility of the db column"""
+        if visible:
+            self._header.showSection(1)
+        else:
+            self._header.hideSection(1)
+
     def _add_middle_actions(self):
         self._add_entity_classes_action = self._menu.addAction(
             self._cube_plus_icon, "Add entity classes", self.add_entity_classes
         )
         self._add_entities_action = self._menu.addAction(self._cube_plus_icon, "Add entities", self.add_entities)
         self._add_entity_group_action = self._menu.addAction(
             self._cube_plus_icon, "Add entity group", self.add_entity_group
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/element_name_list_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/element_name_list_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/metadata_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/metadata_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/scenario_generator.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/scenario_generator.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/select_graph_parameters_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/select_graph_parameters_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,16 @@
         self.init_add_undo_redo_actions()
         self.setWindowTitle(f"{self.db_names}")  # This sets the tab name, just in case
         if update_history:
             self.url_toolbar.add_urls_to_history(self.db_urls)
         self.update_last_view()
         self.restore_ui(self.last_view, fresh=True)
         self.update_commit_enabled()
+        db_column_visible = True if len(self.db_maps) > 1 else False
+        self.set_db_column_visibility(db_column_visible)
         return True
 
     def init_add_undo_redo_actions(self):
         new_undo_action = self.db_mngr.undo_action[self.first_db_map]
         new_redo_action = self.db_mngr.redo_action[self.first_db_map]
         self._replace_undo_redo_actions(new_undo_action, new_redo_action)
 
@@ -979,17 +981,28 @@
         self._dock_views = {d: d.findChild(QAbstractScrollArea) for d in self.findChildren(QDockWidget)}
         self._timer_refresh_tab_order = QTimer(self)  # Used to limit refresh
         self._timer_refresh_tab_order.setSingleShot(True)
         self.add_main_menu()
         self.connect_signals()
         self.last_view = None
         self.apply_stacked_style()
+        self.set_db_column_visibility(False)
         if db_url_codenames is not None:
             self.load_db_urls(db_url_codenames)
 
+    def set_db_column_visibility(self, visible):
+        """Set the visibility of the database -column in all the views it is present"""
+        for view in [
+            self.ui.tableView_entity_alternative,
+            self.ui.tableView_parameter_value,
+            self.ui.tableView_parameter_definition,
+            self.ui.treeView_entity,
+        ]:
+            view.set_db_column_visibility(visible)
+
     def emit_pinned_values_updated(self):
         self.pinned_values_updated.emit(self.ui.tableView_parameter_value.pinned_values)
 
     def connect_signals(self):
         super().connect_signals()
         self._metadata_editor.connect_signals(self.ui)
         self._item_metadata_editor.connect_signals(self.ui)
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/stacked_view_mixin.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/stacked_view_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Contains the StackedViewMixin class."""
-from PySide6.QtCore import Qt, Slot, QModelIndex, QSignalBlocker
+from PySide6.QtCore import QItemSelection, Qt, Slot, QModelIndex, QSignalBlocker
 from PySide6.QtWidgets import QHeaderView
 from PySide6.QtGui import QGuiApplication
 from .element_name_list_editor import ElementNameListEditor
 from ..mvcmodels.compound_models import (
     CompoundParameterValueModel,
     CompoundParameterDefinitionModel,
     CompoundEntityAlternativeModel,
@@ -55,14 +55,15 @@
         self.ui.alternative_tree_view.alternative_selection_changed.connect(self._handle_alternative_selection_changed)
         self.ui.scenario_tree_view.scenario_selection_changed.connect(
             self._handle_scenario_alternative_selection_changed
         )
         self.ui.treeView_entity.tree_selection_changed.connect(
             self._handle_entity_tree_selection_changed_in_parameter_tables
         )
+        self.ui.treeView_entity.model().dataChanged.connect(self._update_empty_rows)
         self.ui.graphicsView.graph_selection_changed.connect(self._handle_graph_selection_changed)
 
     def init_models(self):
         """Initializes models."""
         super().init_models()
         for model in self._all_stacked_models:
             model.reset_db_maps(self.db_maps)
@@ -121,14 +122,31 @@
 
     def set_default_parameter_data(self, default_data, default_db_map):
         for model in self._all_stacked_models:
             model.empty_model.db_map = default_db_map
             model.empty_model.set_default_row(**default_data)
             model.empty_model.set_rows_to_default(model.empty_model.rowCount() - 1)
 
+    @Slot(QModelIndex, QModelIndex, list)
+    def _update_empty_rows(self, top_left, bottom_right, roles):
+        """Updates empty default data on empty rows if relevant entity (class) name has changed.
+
+        Args:
+            top_left (QModelIndex): top left corner of changed data in Entity tree
+            bottom_right (QModelIndex): bottom right corner of changed data in Entity tree
+            roles (list of Qt.ItemDataRole): affected item data roles
+        """
+        entity_selection_model = self.ui.treeView_entity.selectionModel()
+        current_entity_index = entity_selection_model.currentIndex()
+        if not current_entity_index.isValid() or (roles and Qt.ItemDataRole.DisplayRole not in roles):
+            return
+        selection = QItemSelection(top_left, bottom_right)
+        if selection.contains(current_entity_index):
+            self._set_default_parameter_data(current_entity_index)
+
     def clear_all_filters(self):
         for model in self._all_stacked_models:
             model.clear_auto_filter()
         self._filter_class_ids = {}
         self._filter_entity_ids = {}
         self._filter_alternative_ids = {}
         self._reset_filters()
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_editor/widgets/url_toolbar.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_editor/widgets/url_toolbar.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_icon_manager.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_icon_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,23 @@
 
     def _create_class_renderer(self, class_name):
         display_icon = self.display_icons.get(class_name, -1)
         icon_code, color_code = interpret_icon_id(display_icon)
         self._class_renderers[class_name] = self.icon_renderer(chr(icon_code), color_code)
 
     def _create_multi_class_renderer(self, name, dimension_name_list, id_):
+        if not any(dimension_name_list):
+            self._multi_class_renderers[
+                (
+                    name,
+                    dimension_name_list,
+                    id_,
+                )
+            ] = self.icon_renderer("\uf1b3", 0)
+            return
         font = QFont("Font Awesome 5 Free Solid")
         scene = QGraphicsScene()
         display_icon = self.display_icons.get(name, None)
         if display_icon and display_icon != default_icon_id():  # If the entity class has an icon set, use that one.
             icon_code, color_code = interpret_icon_id(display_icon)
             self._multi_class_renderers[
                 (
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_manager.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_manager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_parcel.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_parcel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_db_worker.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_db_worker.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_engine_manager.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_engine_manager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/spine_engine_worker.py` & `spinetoolbox-0.8.2/spinetoolbox/spine_engine_worker.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/about.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/about.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/about.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/about.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/add_project_item.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/add_project_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/add_project_item.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/add_project_item.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/array_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/array_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/array_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/array_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/datetime_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/datetime_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/datetime_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/datetime_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/duration_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/duration_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/duration_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/duration_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/import_source_selector.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/import_source_selector.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/import_source_selector.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/import_source_selector.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/jump_properties.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/jump_properties.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/jump_properties.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/jump_properties.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/link_properties.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/link_properties.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/link_properties.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/link_properties.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/mainwindow.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/mainwindow.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/map_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/map_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/map_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/map_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/mini_kernel_editor_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/mini_kernel_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/mini_kernel_editor_dialog.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/mini_kernel_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/open_project_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/open_project_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/open_project_dialog.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/open_project_dialog.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/parameter_value_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/parameter_value_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/parameter_value_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/plain_parameter_value_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/plain_parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/plain_parameter_value_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/plain_parameter_value_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/Energy_Reform_logo.png` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/Energy_Reform_logo.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/KTH_logo.png` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/KTH_logo.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/KU_Leuven_logo.png` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/KU_Leuven_logo.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/Spine_symbol.png` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/Spine_symbol.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/UCD_Dublin_logo.png` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/UCD_Dublin_logo.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/VTT_Multicolour_Logo.jpg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/VTT_Multicolour_Logo.jpg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/ajax-loader.gif` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/app.ico` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/app.ico`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/black_plus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/black_plus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/book.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/book.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/cat.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/cat.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/check-circle.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/check-circle.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/database-edit.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/database-edit.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/datapkg.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/datapkg.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/double-at.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/double-at.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/file-link.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/file-link.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/fontawesome5-codepoints.json` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/fontawesome5-codepoints.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/fontawesome5-searchterms.json` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/fontawesome5-searchterms.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/fontawesome5-solid-webfont.ttf` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/fontawesome5-solid-webfont.ttf`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/home.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/home.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/bolt-lightning.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/bolt-lightning.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/broom.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/broom.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cog.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cog.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cog_minus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cog_minus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cube_minus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cube_minus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cube_pen.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cube_pen.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cube_plus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cube_plus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cubes_minus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cubes_minus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cubes_pen.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cubes_pen.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/cubes_plus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/cubes_plus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/database-export.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/database-export.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/database-import.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/database-import.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/edit.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/edit.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/file-alt.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/file-alt.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/hands-helping.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/hands-helping.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/history.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/history.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/map-signs-minus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/map-signs-minus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/map-signs-plus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/map-signs-plus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/paste.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/paste.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/pivot-table.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/pivot-table.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/question-circle.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/question-circle.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/save_regular.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/save_regular.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/save_solid.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/save_solid.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/server.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/server.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/sync.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/sync.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/trash-alt.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/trash-alt.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/tree.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/tree.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/undo.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/undo.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/menu_icons/window-close.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/menu_icons/window-close.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/minus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/minus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/plus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/plus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/binoculars.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/binoculars.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/blender.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/blender.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/data_connection.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/data_connection.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/database-export.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/database-export.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/database-import.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/database-import.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/file-alt.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/file-alt.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/hammer.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/hammer.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/project_item_icons/paint-brush-solid.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/project_item_icons/paint-brush-solid.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/qt_extended_48x48.png` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/qt_extended_48x48.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/resources_icons.qrc` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/resources_icons.qrc`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/sliders-h.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/sliders-h.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/spinetoolbox_on_wht.png` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/spinetoolbox_on_wht.png`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/tools.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/tools.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/tractor.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/tractor.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/wrench.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/wrench.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/wrench_minus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/wrench_minus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/resources/wrench_plus.svg` & `spinetoolbox-0.8.2/spinetoolbox/ui/resources/wrench_plus.svg`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/select_database_items_dialog.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/select_database_items_dialog.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/settings.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 ################################################################################
 ## Form generated from reading UI file 'settings.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.7.0
+## Created by: Qt User Interface Compiler version 6.6.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -402,16 +402,16 @@
         self.verticalLayout.addWidget(self.radioButton_use_julia_jupyter_console)
 
 
         self.horizontalLayout_14.addLayout(self.verticalLayout)
 
         self.line_3 = QFrame(self.groupBox_julia)
         self.line_3.setObjectName(u"line_3")
-        self.line_3.setFrameShape(QFrame.Shape.VLine)
-        self.line_3.setFrameShadow(QFrame.Shadow.Sunken)
+        self.line_3.setFrameShape(QFrame.VLine)
+        self.line_3.setFrameShadow(QFrame.Sunken)
 
         self.horizontalLayout_14.addWidget(self.line_3)
 
         self.verticalLayout_15 = QVBoxLayout()
         self.verticalLayout_15.setObjectName(u"verticalLayout_15")
         self.horizontalLayout_8 = QHBoxLayout()
         self.horizontalLayout_8.setObjectName(u"horizontalLayout_8")
@@ -485,16 +485,16 @@
         self.horizontalLayout_14.addLayout(self.verticalLayout_15)
 
 
         self.verticalLayout_10.addLayout(self.horizontalLayout_14)
 
         self.line = QFrame(self.groupBox_julia)
         self.line.setObjectName(u"line")
-        self.line.setFrameShape(QFrame.Shape.HLine)
-        self.line.setFrameShadow(QFrame.Shadow.Sunken)
+        self.line.setFrameShape(QFrame.HLine)
+        self.line.setFrameShadow(QFrame.Sunken)
 
         self.verticalLayout_10.addWidget(self.line)
 
         self.horizontalLayout_12 = QHBoxLayout()
         self.horizontalLayout_12.setObjectName(u"horizontalLayout_12")
         self.pushButton_install_julia = QPushButton(self.groupBox_julia)
         self.pushButton_install_julia.setObjectName(u"pushButton_install_julia")
@@ -539,16 +539,16 @@
         self.verticalLayout_14.addWidget(self.radioButton_use_python_jupyter_console)
 
 
         self.horizontalLayout_5.addLayout(self.verticalLayout_14)
 
         self.line_2 = QFrame(self.groupBox_python)
         self.line_2.setObjectName(u"line_2")
-        self.line_2.setFrameShape(QFrame.Shape.VLine)
-        self.line_2.setFrameShadow(QFrame.Shadow.Sunken)
+        self.line_2.setFrameShape(QFrame.VLine)
+        self.line_2.setFrameShadow(QFrame.Sunken)
 
         self.horizontalLayout_5.addWidget(self.line_2)
 
         self.verticalLayout_5 = QVBoxLayout()
         self.verticalLayout_5.setObjectName(u"verticalLayout_5")
         self.horizontalLayout_10 = QHBoxLayout()
         self.horizontalLayout_10.setObjectName(u"horizontalLayout_10")
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/settings.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/settings.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/time_pattern_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/time_pattern_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/time_pattern_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/time_pattern_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/time_series_fixed_resolution_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/time_series_fixed_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/time_series_fixed_resolution_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/time_series_fixed_resolution_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/time_series_variable_resolution_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/time_series_variable_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/time_series_variable_resolution_editor.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/time_series_variable_resolution_editor.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/tool_configuration_assistant.py` & `spinetoolbox-0.8.2/spinetoolbox/ui/tool_configuration_assistant.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui/tool_configuration_assistant.ui` & `spinetoolbox-0.8.2/spinetoolbox/ui/tool_configuration_assistant.ui`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/ui_main.py` & `spinetoolbox-0.8.2/spinetoolbox/ui_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1059,14 +1059,15 @@
         def_file = os.path.abspath(answer[0])
         # Load specification
         local_data = load_specification_local_data(self._project.config_dir)
         specification = load_specification_from_file(
             def_file, local_data, self._item_specification_factories, self._qsettings, self
         )
         if not specification:
+            self.msg_error.emit("Failed to load specification.")
             return
         self.undo_stack.push(AddSpecificationCommand(self._project, specification, save_to_disk=False))
 
     def replace_specification(self, name, specification):
         """Pushes an ReplaceSpecificationCommand to undo stack."""
         if name == specification.name:
             # If the spec name didn't change, we don't need to make a command.
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/version.py` & `spinetoolbox-0.8.2/spinetoolbox/version.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/__init__.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/about_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/about_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/add_project_item_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/add_project_item_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
         self.ui.setupUi(self)
         # Add status bar to form
         self.statusbar = QStatusBar(self)
         self.statusbar.setFixedHeight(20)
         self.statusbar.setSizeGripEnabled(False)
         self.statusbar.setStyleSheet(STATUSBAR_SS)
         self.ui.horizontalLayout_statusbar_placeholder.addWidget(self.statusbar)
-        # Init
         if toolbox.supports_specifications(class_.item_type()):
             self.ui.comboBox_specification.setModel(toolbox.filtered_spec_factory_models[class_.item_type()])
             if spec:
-                self.ui.comboBox_specification.hide()
+                self.ui.comboBox_specification.setCurrentText(spec)
+                self.ui.comboBox_specification.setDisabled(True)
                 prefix = spec
             else:
                 prefix = class_.item_type()
                 self.ui.comboBox_specification.setCurrentIndex(-1)
         else:
             prefix = class_.item_type()
             self.ui.comboBox_specification.hide()
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/add_up_spine_opt_wizard.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/add_up_spine_opt_wizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/array_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/array_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/array_value_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/array_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/code_text_edit.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/code_text_edit.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/commit_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/commit_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_combobox.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_combobox.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_delegates.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_delegates.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_menus.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qgraphicsscene.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qgraphicsscene.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qgraphicsviews.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qgraphicsviews.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         item = self.itemAt(event.position().toPoint())
         if not item or not item.acceptedMouseButtons() & event.buttons():
             button = event.button()
             if button == Qt.MouseButton.LeftButton:
                 self.viewport().setCursor(Qt.CrossCursor)
             elif button == Qt.MouseButton.MiddleButton:
                 self.reset_zoom()
-            if button == Qt.MouseButton.RightButton:
+            elif button == Qt.MouseButton.RightButton:
                 self.setDragMode(QGraphicsView.DragMode.ScrollHandDrag)
                 self._last_right_mouse_press = event.timestamp()
                 event = _fake_left_button_event(event)
         super().mousePressEvent(event)
 
     def mouseMoveEvent(self, event):
         if (
@@ -108,15 +108,15 @@
     def mouseReleaseEvent(self, event):
         """Reestablish scroll hand drag mode."""
         context_menu_disabled = False
         if self.dragMode() == QGraphicsView.DragMode.ScrollHandDrag:
             if self._drag_duration_passed(event):
                 context_menu_disabled = True
                 self.disable_context_menu()
-            else:
+            elif event.button() == Qt.MouseButton.RightButton:
                 self.contextMenuEvent(
                     QContextMenuEvent(QContextMenuEvent.Reason.Mouse, event.pos(), event.globalPos(), event.modifiers())
                 )
             event = _fake_left_button_event(event)
         super().mouseReleaseEvent(event)
         self.setDragMode(QGraphicsView.DragMode.RubberBandDrag)
         self._previous_mouse_pos = None
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qlineedits.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qlineedits.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qtableview.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qtableview.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qtextbrowser.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qtextbrowser.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qtreeview.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qtreeview.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/custom_qwidgets.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/custom_qwidgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/datetime_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/datetime_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/duration_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/duration_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/indexed_value_table_context_menu.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/indexed_value_table_context_menu.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/install_julia_wizard.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/install_julia_wizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/jump_properties_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/jump_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/jupyter_console_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/jupyter_console_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/kernel_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/kernel_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/link_properties_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/link_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/map_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/map_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/map_value_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/map_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/multi_tab_spec_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/multi_tab_spec_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/multi_tab_window.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/multi_tab_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/notification.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/notification.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/open_project_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/open_project_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/options_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/options_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/parameter_value_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/parameter_value_editor_base.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/parameter_value_editor_base.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/persistent_console_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/persistent_console_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/plain_parameter_value_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/plain_parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/plot_canvas.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/plot_canvas.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/plot_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/plot_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/plugin_manager_widgets.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/plugin_manager_widgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/project_item_drag.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/project_item_drag.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/properties_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/properties_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/report_plotting_failure.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/report_plotting_failure.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/select_database_items.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/select_database_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/set_description_dialog.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/set_description_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/settings_widget.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/settings_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/statusbars.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/statusbars.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/time_pattern_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/time_pattern_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/time_series_fixed_resolution_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/time_series_fixed_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/time_series_variable_resolution_editor.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/time_series_variable_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox/widgets/toolbars.py` & `spinetoolbox-0.8.2/spinetoolbox/widgets/toolbars.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox.egg-info/PKG-INFO` & `spinetoolbox-0.8.2/spinetoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: spinetoolbox
-Version: 0.8.1
+Version: 0.8.2
 Summary: An application to define, manage, and execute various energy system simulation models
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://spine-toolbox.readthedocs.io/
 Project-URL: Repository, https://github.com/spine-tools/Spine-Toolbox
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.8.1
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: pyside6!=6.5.3,!=6.6.3,>=6.5.0
+Requires-Dist: pyside6!=6.5.3,!=6.6.3,!=6.7.0,>=6.5.0
 Requires-Dist: jupyter-client>=6.0
 Requires-Dist: qtconsole>=5.1
-Requires-Dist: sqlalchemy>=1.3
-Requires-Dist: spinedb_api>=0.31.1
-Requires-Dist: spine_engine>=0.24.0
+Requires-Dist: spinedb_api>=0.31.2
+Requires-Dist: spine_engine>=0.24.1
 Requires-Dist: numpy>=1.20.2
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: pandas>=1.3.2
 Requires-Dist: pygments>=2.8
 Requires-Dist: jill>=0.9.2
 Requires-Dist: pyzmq>=21.0
-Requires-Dist: spine-items>=0.22.1
+Requires-Dist: spine-items>=0.22.2
 
 # Spine Toolbox
 Link to the documentation: [https://spine-toolbox.readthedocs.io/en/latest/?badge=latest](https://spine-toolbox.readthedocs.io/en/latest/?badge=latest)
 
-[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
+[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Documentation Status](https://readthedocs.org/projects/spine-toolbox/badge/?version=latest)](https://spine-toolbox.readthedocs.io/en/latest/?badge=latest)
 [![Test suite](https://github.com/spine-tools/Spine-Toolbox/actions/workflows/test_runner.yml/badge.svg)](https://github.com/spine-tools/Spine-Toolbox/actions/workflows/test_runner.yml)
 [![codecov](https://codecov.io/gh/spine-tools/Spine-Toolbox/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Toolbox)
 [![PyPI version](https://badge.fury.io/py/spinetoolbox.svg)](https://badge.fury.io/py/spinetoolbox)
 [![Join the chat at https://gitter.im/spine-tools/Spine-Toolbox](https://badges.gitter.im/spine-tools/Spine-Toolbox.svg)](https://gitter.im/spine-tools/Spine-Toolbox?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 Spine Toolbox is an open source Python package to manage data, scenarios and workflows for modelling and simulation. 
@@ -46,23 +45,14 @@
 <p align="center" width="100%">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="./fig/spinetoolbox_logo.svg" width="50%">
     <img alt="Spine Toolbox" src="./fig/spinetoolbox_on_wht.svg" width="50%">
   </picture>
 </p>
 
-## Programming language
-
-- Python 3.8*
-- Python 3.9
-- Python 3.10
-- Python 3.11
-
-*Python 3.8.0 is not supported (use Python 3.8.1 or later).<br>
-
 ## License
 
 Spine Toolbox is released under the GNU Lesser General Public License (LGPL) license. 
 All accompanying documentation, original graphics and other material are released under the 
 [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
 Licenses of all packages used by Spine Toolbox are listed in the Spine Toolbox User 
 Guide.
@@ -86,16 +76,16 @@
 - [Windows installation package](#windows-64-bit-installer-package) (these are quite old - not recommended)
 
 ### Pre-installation
 
 These steps apply to both [Python/pipx](#installation-with-python-and-pipx) option and to 
 [From source files](#installation-from-sources-using-git) option.
 
-1. If you don't have Python installed, please install e.g. **Python 3.11** from 
-[Python.org](https://www.python.org/downloads/release/python-3117/).
+1. If you don't have Python installed, please install it e.g. from 
+[Python.org](https://www.python.org/downloads/).
 
 2. Test that python is now in your PATH. Open a new terminal (e.g. Command Prompt) window and type 
 
        python --version
 
     The output should be the Python version. If it did not work (e.g. the output is *'python' command not found* or 
 similar or the [Microsoft Store opens](https://learn.microsoft.com/en-us/windows/python/faqs#why-does-running-python-exe-open-the-microsoft-store-)),
@@ -277,48 +267,48 @@
 a quick look at how Spine Toolbox looks and feels (although even that has changed).
 Download the installer package from 
 [here](https://github.com/spine-tools/Spine-Toolbox/releases),
 run it, and follow the instructions to install Spine Toolbox.
 
 ### About requirements
 
-Python 3.8.1-3.11 is required. Python 3.8.0 is not supported due to problems in DLL loading on Windows.
+Python 3.8.1 or later is required. Python 3.8.0 is not supported due to problems in DLL loading on Windows.
 
 See the files `pyproject.toml` and `requirements.txt` for packages required to run Spine Toolbox.
 (Additional packages needed for development are listed in `dev-requirements.txt`.)
 
 The requirements include three packages ([`spinedb_api`](https://github.com/spine-tools/Spine-Database-API),
 [`spine_engine`](https://github.com/spine-tools/spine-engine), and 
 [`spine_items`](https://github.com/spine-tools/spine-items)), developed by the Spine project consortium.
 
 ### Building the User Guide
 
 You can find the latest documentation on [readthedocs](https://spine-toolbox.readthedocs.io/en/latest/index.html).
 If you want to build the documentation yourself,
 source files for the User Guide can be found in `docs/source` directory. In order to 
-build the HTML docs, you need to install the *optional requirements* (see section 
-'Installing requirements' above). This installs Sphinx (among other things), which 
+build the HTML docs, you need to install the *development requirements* (see section 
+'About requirements' above). This installs Sphinx (among other things), which 
 is required in building the documentation. When Sphinx is installed, you can build the 
 HTML pages from the user guide source files by using the `bin/build_doc.bat` script on 
-Windows or the `bin/build_doc.sh` script on Linux and Mac. After running the script, the 
+Windows or the `bin/build_doc.py` script on Linux and Mac. After running the script, the 
 index page can be found in `docs/build/html/index.html`. The User Guide can also 
-be opened from Spine Toolbox menu Help->User Guide (F2).
+be opened from Spine Toolbox menu Help->User Guide (F1).
 
 ### Troubleshooting
 
 #### Obscure crashes that may produce a traceback related to PySide6's model classes
 
 The first thing is to make sure that you are not using Anaconda. Only Miniconda is supported. Anaconda's base 
 environment includes Qt related packages and we suspect that they leak some shared Qt libraries into environments,
 even when specifically requesting that base environment packages should not be linked to environment packages. See
 also [Problems in starting the application](#problems-in-starting-the-application) below.
 
 #### Installation fails
 
-Please make sure you are using Python 3.8, 3.9, 3.10, or 3.11 to install the requirements.
+Please make sure you are using Python 3.8.1 or later to install the requirements.
 
 #### 'No Python' error when installing with pipx
 
 If you see the following error when running the command `python -m pipx install spinetoolbox`
 
 ```
 No Python at 'c:\python38\python.exe'
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox.egg-info/SOURCES.txt` & `spinetoolbox-0.8.2/spinetoolbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 requirements.txt
 setup-debug.iss
 setup.iss
 spinetoolbox.py
 spinetoolbox.spec
 .github/pull_request_template.md
 .github/workflows/bundle.yml
+.github/workflows/make_bundle.yml
+.github/workflows/manual_bundling.yml
 .github/workflows/test_runner.yml
 PyInstaller hooks/hook-datapackage.py
 PyInstaller hooks/hook-jill.py
 PyInstaller hooks/hook-spine_engine.py
 PyInstaller hooks/hook-spinedb_api.py
 PyInstaller hooks/hook-tableschema.py
 PyInstaller hooks/hook-tabulator.py
@@ -39,15 +41,14 @@
 bin/builddocs.json
 bin/configure_julia.py
 bin/upgrade_spine_reqs.bat
 bin/upgrade_spine_reqs.py
 docs/Makefile
 docs/cleandocs.json
 docs/make.bat
-docs/requirements.txt
 docs/source/conf.py
 docs/source/contribution_guide.rst
 docs/source/data_import_export.rst
 docs/source/developer_documentation.rst
 docs/source/executing_projects.rst
 docs/source/execution_tests.rst
 docs/source/getting_started.rst
```

### Comparing `spinetoolbox-0.8.1/spinetoolbox.py` & `spinetoolbox-0.8.2/spinetoolbox.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/spinetoolbox.spec` & `spinetoolbox-0.8.2/spinetoolbox.spec`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/__init__.py` & `spinetoolbox-0.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mock_helpers.py` & `spinetoolbox-0.8.2/tests/mock_helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/__init__.py` & `spinetoolbox-0.8.2/tests/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_ArrayModel.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_ArrayModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_FileListModel.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_FileListModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_FilterCheckboxList.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_FilterCheckboxList.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_IndexedValueTableModel.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_IndexedValueTableModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_MapModel.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_MapModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_MinimalTableModel.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_MinimalTableModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_TimePatternModel.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_TimePatternModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/mvcmodels/test_resource_filter_model.py` & `spinetoolbox-0.8.2/tests/mvcmodels/test_resource_filter_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/project_item/__init__.py` & `spinetoolbox-0.8.2/tests/project_item/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/project_item/test_ProjectItem.py` & `spinetoolbox-0.8.2/tests/project_item/test_ProjectItem.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/project_item/test_logging_connection.py` & `spinetoolbox-0.8.2/tests/project_item/test_logging_connection.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/project_item/test_specification_editor_window.py` & `spinetoolbox-0.8.2/tests/project_item/test_specification_editor_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/server/__init__.py` & `spinetoolbox-0.8.2/tests/server/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/server/helloworld.zip` & `spinetoolbox-0.8.2/tests/server/helloworld.zip`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/server/test_EngineClient.py` & `spinetoolbox-0.8.2/tests/server/test_EngineClient.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/server/test_RemoteSpineEngineManager.py` & `spinetoolbox-0.8.2/tests/server/test_RemoteSpineEngineManager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/__init__.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/helpers.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/__init__.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_PivotModel.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_PivotModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_alternative_model.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_alternative_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_compound_models.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_compound_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_frozen_table_model.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_frozen_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_item_metadata_table_model.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_item_metadata_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_metadata_table_model.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_metadata_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_scenario_model.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_scenario_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_single_parameter_models.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_single_parameter_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_tree_item_utility.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_tree_item_utility.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/mvcmodels/test_utils.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/mvcmodels/test_utils.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/test_graphics_items.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/test_graphics_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/test_helpers.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/test_helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/__init__.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/helpers.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,7 +111,15 @@
 
 def add_entity(view, name, entity_class_index=0):
     model = view.model()
     root_index = model.index(0, 0)
     class_index = model.index(entity_class_index, 0, root_index)
     view._context_item = model.item_from_index(class_index)
     add_entity_tree_item({0: name}, view, "Add entities", AddEntitiesDialog)
+
+
+def add_entity_with_alternative(view, name, alternative, entity_class_index=0):
+    model = view.model()
+    root_index = model.index(0, 0)
+    class_index = model.index(entity_class_index, 0, root_index)
+    view._context_item = model.item_from_index(class_index)
+    add_entity_tree_item({0: name, 1: alternative}, view, "Add entities", AddEntitiesDialog)
```

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/spine_db_editor_test_base.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/spine_db_editor_test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,25 +121,27 @@
             cls.pluto_nemo_rel["id"],
             cls.combined_mojo_parameter["id"],
             1,
             b"100",
             None,
         )
 
+    db_codename = "database"
+
     def setUp(self):
         """Makes instances of SpineDBEditor classes."""
         with mock.patch("spinetoolbox.spine_db_editor.widgets.spine_db_editor.SpineDBEditor.restore_ui"), mock.patch(
             "spinetoolbox.spine_db_editor.widgets.spine_db_editor.SpineDBEditor.show"
         ):
             mock_settings = mock.Mock()
             mock_settings.value.side_effect = lambda *args, **kwargs: 0
             self.db_mngr = TestSpineDBManager(mock_settings, None)
             logger = mock.MagicMock()
-            self.mock_db_map = self.db_mngr.get_db_map("sqlite://", logger, codename="database", create=True)
-            self.spine_db_editor = SpineDBEditor(self.db_mngr, {"sqlite://": "database"})
+            self.mock_db_map = self.db_mngr.get_db_map("sqlite://", logger, codename=self.db_codename, create=True)
+            self.spine_db_editor = SpineDBEditor(self.db_mngr, {"sqlite://": self.db_codename})
             self.spine_db_editor.pivot_table_model = mock.MagicMock()
             self.spine_db_editor.entity_tree_model.hide_empty_classes = False
 
     def tearDown(self):
         with mock.patch(
             "spinetoolbox.spine_db_editor.widgets.spine_db_editor.SpineDBEditor.save_window_state"
         ) as mock_save_w_s, mock.patch("spinetoolbox.spine_db_manager.QMessageBox"):
```

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_add_items_dialog.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_add_items_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_commit_viewer.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_commit_viewer.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_delegates.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_delegates.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_editors.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_editors.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_menus.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_menus.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_qtableview.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_qtableview.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,20 @@
             lines = plot_widget.canvas.axes.get_lines()
             self.assertEqual(len(lines), 1)
             self.assertEqual(list(lines[0].get_xdata(orig=True)), [0, 1])
             self.assertEqual(list(lines[0].get_ydata(orig=True)), [2.3, 23.0])
         finally:
             plot_widget.deleteLater()
 
+    def test_set_db_column_visible(self):
+        table_view = self._db_editor.ui.tableView_parameter_definition
+        self.assertTrue(table_view.isColumnHidden(table_view._EXPECTED_COLUMN_COUNT - 1))
+        self._db_editor.ui.tableView_parameter_definition.set_db_column_visibility(True)
+        self.assertFalse(table_view.isColumnHidden(table_view._EXPECTED_COLUMN_COUNT - 1))
+
 
 class TestParameterValueTableView(TestBase):
     def test_paste_empty_string_to_entity_byname_column(self):
         table_view = self._db_editor.ui.tableView_parameter_value
         model = table_view.model()
         byname_column = model.header.index("entity_byname")
         table_view.selectionModel().setCurrentIndex(
@@ -278,14 +284,20 @@
             lines = plot_widget.canvas.axes.get_lines()
             self.assertEqual(len(lines), 1)
             self.assertEqual(list(lines[0].get_xdata(orig=True)), [0, 1])
             self.assertEqual(list(lines[0].get_ydata(orig=True)), [2.3, 23.0])
         finally:
             plot_widget.deleteLater()
 
+    def test_set_db_column_visible(self):
+        table_view = self._db_editor.ui.tableView_parameter_definition
+        self.assertTrue(table_view.isColumnHidden(table_view._EXPECTED_COLUMN_COUNT - 1))
+        self._db_editor.ui.tableView_parameter_definition.set_db_column_visibility(True)
+        self.assertFalse(table_view.isColumnHidden(table_view._EXPECTED_COLUMN_COUNT - 1))
+
 
 class TestParameterValueTableWithExistingData(TestBase):
     _CHUNK_SIZE = 100  # This has to be large enough, so the chunk won't 'fit' into the table view.
 
     @mock.patch("spinetoolbox.spine_db_worker._CHUNK_SIZE", new=_CHUNK_SIZE)
     def setUp(self):
         self._temp_dir = TemporaryDirectory()
@@ -419,14 +431,20 @@
             [None, None, None, None, "TestEntityAlternativeTableView_db"],
         ]
         for row in range(model.rowCount()):
             for column in range(model.columnCount()):
                 with self.subTest(row=row, column=column):
                     self.assertEqual(model.index(row, column).data(), expected[row][column])
 
+    def test_set_db_column_visible(self):
+        table_view = self._db_editor.ui.tableView_parameter_definition
+        self.assertTrue(table_view.isColumnHidden(table_view._EXPECTED_COLUMN_COUNT - 1))
+        self._db_editor.ui.tableView_parameter_definition.set_db_column_visibility(True)
+        self.assertFalse(table_view.isColumnHidden(table_view._EXPECTED_COLUMN_COUNT - 1))
+
 
 def _set_row_data(view, model, row, data, delegate_mock):
     for column, cell_data in enumerate(data):
         delegate_mock.reset()
         delegate_mock.write_to_index(view, model.index(row, column), cell_data)
```

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_custom_qtreeview.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_custom_qtreeview.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 )
 from tests.spine_db_editor.helpers import TestBase
 from tests.spine_db_editor.widgets.helpers import (
     EditorDelegateMocking,
     add_entity_tree_item,
     add_zero_dimension_entity_class,
     add_entity,
+    add_entity_with_alternative,
 )
 
 
 class _ParameterValueListEdits:
     def __init__(self, view):
         self._view = view
         self.view_editor = EditorDelegateMocking()
@@ -190,14 +191,52 @@
         data = self._db_map.query(self._db_map.entity_class_sq).all()
         self.assertEqual(len(data), 1)
         self.assertEqual(data[0].name, "an_entity_class")
         data = self._db_map.query(self._db_map.entity_sq).all()
         self.assertEqual(len(data), 1)
         self.assertEqual(data[0].name, "an_entity")
 
+    def test_add_entity_with_alternative(self):
+        view = self._db_editor.ui.treeView_entity
+        add_zero_dimension_entity_class(view, "an_entity_class")
+        with mock.patch.object(self._db_mngr, "add_entity_alternatives") as mock_add_entity_alternatives:
+            add_entity_with_alternative(view, "an_entity", "Alt1")
+            mock_add_entity_alternatives.assert_called_once_with(
+                {
+                    self._db_map: [
+                        {
+                            "active": True,
+                            "alternative_name": "Alt1",
+                            "entity_byname": ("an_entity",),
+                            "entity_class_name": "an_entity_class",
+                        }
+                    ]
+                }
+            )
+        model = view.model()
+        root_index = model.index(0, 0)
+        class_index = model.index(0, 0, root_index)
+        model.fetchMore(class_index)
+        while model.rowCount(class_index) != 1:
+            QApplication.processEvents()
+        self.assertEqual(model.rowCount(class_index), 1)
+        self.assertEqual(class_index.data(), "an_entity_class")
+        entity_index = model.index(0, 0, class_index)
+        self.assertEqual(model.rowCount(entity_index), 0)
+        self.assertEqual(entity_index.data(), "an_entity")
+        entity_database_index = model.index(0, 1, class_index)
+        self.assertEqual(entity_database_index.data(), self.db_codename)
+        self._commit_changes_to_database("Add entity.")
+        data = self._db_map.query(self._db_map.entity_class_sq).all()
+        self.assertEqual(len(data), 1)
+        self.assertEqual(data[0].name, "an_entity_class")
+        data = self._db_map.query(self._db_map.entity_sq).all()
+        self.assertEqual(len(data), 1)
+        self.assertEqual(data[0].name, "an_entity")
+
     def test_add_entity_with_single_dimension(self):
         view = self._db_editor.ui.treeView_entity
         add_zero_dimension_entity_class(view, "an_entity_class")
         add_entity(view, "an_entity")
         model = view.model()
         root_index = model.index(0, 0)
         class_index = model.index(0, 0, root_index)
@@ -394,14 +433,20 @@
         entity_index = model.index(0, 0, class_index)
         self.assertEqual(entity_index.data(), "entity_2")
         self._commit_changes_to_database("Remove entity.")
         data = self._db_map.query(self._db_map.entity_sq).all()
         self.assertEqual(len(data), 1)
         self.assertEqual(data[0].name, "entity_2")
 
+    def test_set_db_column_visibility(self):
+        view = self._db_editor.ui.treeView_entity
+        self.assertTrue(view._header.isSectionHidden(1))
+        view.set_db_column_visibility(True)
+        self.assertFalse(view._header.isSectionHidden(1))
+
     def _rename_entity_class(self, class_name):
         view = self._db_editor.ui.treeView_entity
         _edit_entity_tree_item({0: class_name}, view, "Edit...", EditEntityClassesDialog)
 
     def _rename_entity(self, entity_name):
         view = self._db_editor.ui.treeView_entity
         _edit_entity_tree_item({0: entity_name}, view, "Edit...", EditEntitiesDialog)
```

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_edit_or_remove_items_dialogs.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_edit_or_remove_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_mass_select_items_dialogs.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_mass_select_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_multi_spine_db_editor.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_multi_spine_db_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_scenario_generator.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_scenario_generator.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_tabular_view_mixin.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_tabular_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/spine_db_editor/widgets/test_url_toolbar.py` & `spinetoolbox-0.8.2/tests/spine_db_editor/widgets/test_url_toolbar.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_ProjectUpgrader.py` & `spinetoolbox-0.8.2/tests/test_ProjectUpgrader.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_SpineDBManager.py` & `spinetoolbox-0.8.2/tests/test_SpineDBManager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_SpineToolboxProject.py` & `spinetoolbox-0.8.2/tests/test_SpineToolboxProject.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_ToolboxUI.py` & `spinetoolbox-0.8.2/tests/test_ToolboxUI.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_execution_managers.py` & `spinetoolbox-0.8.2/tests/test_execution_managers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_helpers.py` & `spinetoolbox-0.8.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_load_project_items.py` & `spinetoolbox-0.8.2/tests/test_load_project_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_plotting.py` & `spinetoolbox-0.8.2/tests/test_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         object_tree_model = self._db_editor.ui.treeView_entity.model()
         root_index = object_tree_model.index(0, 0)
         if object_tree_model.canFetchMore(root_index):
             object_tree_model.fetchMore(root_index)
         self.assertEqual(object_tree_model.rowCount(root_index), 1)
         class_index = object_tree_model.index(0, 0, root_index)
         refreshing_models = [self._db_editor.parameter_value_model, self._db_editor.parameter_definition_model]
-        with multi_signal_waiter([model.refreshed for model in refreshing_models]) as at_filter_refresh:
+        with multi_signal_waiter([model.layoutChanged for model in refreshing_models]) as at_filter_refresh:
             self._db_editor.ui.treeView_entity.selectionModel().setCurrentIndex(
                 class_index, QItemSelectionModel.ClearAndSelect
             )
             at_filter_refresh.wait()
 
     def _fill_pivot(self, values):
         self._add_object_parameter_values(values)
```

### Comparing `spinetoolbox-0.8.1/tests/test_project_item_icon.py` & `spinetoolbox-0.8.2/tests/test_project_item_icon.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/Project Directory/.spinetoolbox/project.json` & `spinetoolbox-0.8.2/tests/test_resources/Project Directory/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/basic_model_template.json` & `spinetoolbox-0.8.2/tests/test_resources/basic_model_template.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v1.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v1.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v10.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v10.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v11.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v11.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v2.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v2.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v3.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v3.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v4.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v4.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v5.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v5.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/project_json_versions/proj_v9.json` & `spinetoolbox-0.8.2/tests/test_resources/project_json_versions/proj_v9.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_resources/spineopt_template.json` & `spinetoolbox-0.8.2/tests/test_resources/spineopt_template.json`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_spine_db_fetcher.py` & `spinetoolbox-0.8.2/tests/test_spine_db_fetcher.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/test_spine_engine_worker.py` & `spinetoolbox-0.8.2/tests/test_spine_engine_worker.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/__init__.py` & `spinetoolbox-0.8.2/tests/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_AboutWidget.py` & `spinetoolbox-0.8.2/tests/widgets/test_AboutWidget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_AddProjectItemWidget.py` & `spinetoolbox-0.8.2/tests/widgets/test_AddProjectItemWidget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_AddUpSpineOptWizard.py` & `spinetoolbox-0.8.2/tests/widgets/test_AddUpSpineOptWizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_ArrayTableView.py` & `spinetoolbox-0.8.2/tests/widgets/test_ArrayTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_CopyPasteTableView.py` & `spinetoolbox-0.8.2/tests/widgets/test_CopyPasteTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_DatetimeEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_DatetimeEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_DurationEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_DurationEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_IndexedValueTableView.py` & `spinetoolbox-0.8.2/tests/widgets/test_IndexedValueTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_InstallJuliaWizard.py` & `spinetoolbox-0.8.2/tests/widgets/test_InstallJuliaWizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_JupyterConsoleWidget.py` & `spinetoolbox-0.8.2/tests/widgets/test_JupyterConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_KernelFetcher.py` & `spinetoolbox-0.8.2/tests/widgets/test_KernelFetcher.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_MapEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_MapEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_MapTableView.py` & `spinetoolbox-0.8.2/tests/widgets/test_MapTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_ParameterValueEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_ParameterValueEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_PlainParameterValueEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_PlainParameterValueEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_TimePatternEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_TimePatternEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_TimeSeriesFixedResolutionEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_TimeSeriesFixedResolutionEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_TimeSeriesFixedResolutionTableView.py` & `spinetoolbox-0.8.2/tests/widgets/test_TimeSeriesFixedResolutionTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_TimeSeriesVariableResolutionEditor.py` & `spinetoolbox-0.8.2/tests/widgets/test_TimeSeriesVariableResolutionEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_custom_combobox.py` & `spinetoolbox-0.8.2/tests/widgets/test_custom_combobox.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_custom_qgraphicsscene.py` & `spinetoolbox-0.8.2/tests/widgets/test_custom_qgraphicsscene.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_custom_qlineedits.py` & `spinetoolbox-0.8.2/tests/widgets/test_custom_qlineedits.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_custom_qtextbrowser.py` & `spinetoolbox-0.8.2/tests/widgets/test_custom_qtextbrowser.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_custom_qwidgets.py` & `spinetoolbox-0.8.2/tests/widgets/test_custom_qwidgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_indexed_value_table_context_menu.py` & `spinetoolbox-0.8.2/tests/widgets/test_indexed_value_table_context_menu.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_jump_properties_widget.py` & `spinetoolbox-0.8.2/tests/widgets/test_jump_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_kernel_editor.py` & `spinetoolbox-0.8.2/tests/widgets/test_kernel_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_notification.py` & `spinetoolbox-0.8.2/tests/widgets/test_notification.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_open_project_dialog.py` & `spinetoolbox-0.8.2/tests/widgets/test_open_project_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_plot_widget.py` & `spinetoolbox-0.8.2/tests/widgets/test_plot_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_plugin_manager_widgets.py` & `spinetoolbox-0.8.2/tests/widgets/test_plugin_manager_widgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_select_database_items.py` & `spinetoolbox-0.8.2/tests/widgets/test_select_database_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.8.1/tests/widgets/test_settings_widget.py` & `spinetoolbox-0.8.2/tests/widgets/test_settings_widget.py`

 * *Files identical despite different names*

