# Comparing `tmp/spinedb_api-0.31.1.tar.gz` & `tmp/spinedb_api-0.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinedb_api-0.31.1.tar", last modified: Tue May 14 13:12:11 2024, max compression
+gzip compressed data, was "spinedb_api-0.31.2.tar", last modified: Thu May 30 13:45:41 2024, max compression
```

## Comparing `spinedb_api-0.31.1.tar` & `spinedb_api-0.31.2.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.519268 spinedb_api-0.31.1/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.487267 spinedb_api-0.31.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.487267 spinedb_api-0.31.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-14 13:12:11.519268 spinedb_api-0.31.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.487267 spinedb_api-0.31.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/datetime_from_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/map_from_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/mapped_item_getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/update_default_value_to_different_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/update_default_value_to_same_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/bin/build_doc.bat
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/bin/build_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/deploy-key.enc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/front_matter.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/img/spinetoolbox_on_wht.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/parameter_value_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/fig/eu-emblem-low-res.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:12:11.519268 spinedb_api-0.31.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.495267 spinedb_api-0.31.1/spinedb_api/
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.499267 spinedb_api-0.31.1/spinedb_api/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/README
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.499267 spinedb_api-0.31.1/spinedb_api/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/e010777927a5_change_active_by_default_server_default_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    45893 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    48172 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping_commit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    63433 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping_query_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/export_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52885 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/export_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/group_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22267 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/alternative_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/execution_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/renamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/scenario_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/value_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/graph_layout_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28826 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/import_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15737 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    39612 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    34426 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/mapped_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    60563 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/perfect_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/server_client_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_db_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28277 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_db_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/spine_io/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.507268 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/gdx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/sql_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/gdx_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.507268 spinedb_api-0.31.1/spinedb_api/spine_io/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/datapackage_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/gdx_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/sqlalchemy_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/temp_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/spinedb_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.511268 spinedb_api-0.31.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/custom_db_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.511268 spinedb_api-0.31.1/tests/export_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77130 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/test_export_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.511268 spinedb_api-0.31.1/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_alternative_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_execution_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_renamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27281 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_scenario_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_tool_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_value_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/import_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27529 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    87795 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/test_import_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/test_type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/spine_io/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/spine_io/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_gdx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_sql_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/spine_io/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_CSVConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_GdxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_datapackage_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_sqlalchemy_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/test_excel_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)   198916 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_DatabaseMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_check_integrity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_db_mapping_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_db_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_export_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    78082 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_import_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    48629 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_purge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.703070 spinedb_api-0.31.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.671070 spinedb_api-0.31.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.671070 spinedb_api-0.31.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-30 13:45:41.703070 spinedb_api-0.31.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.675070 spinedb_api-0.31.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/datetime_from_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/entity_class_mapping_import_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/map_from_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/mapped_item_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/update_default_value_to_different_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/update_default_value_to_same_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.675070 spinedb_api-0.31.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/bin/build_doc.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/bin/build_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/deploy-key.enc
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.675070 spinedb_api-0.31.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.675070 spinedb_api-0.31.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/source/front_matter.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.675070 spinedb_api-0.31.2/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/source/img/spinetoolbox_on_wht.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/source/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/source/parameter_value_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/docs/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.675070 spinedb_api-0.31.2/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/fig/eu-emblem-low-res.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:45:41.703070 spinedb_api-0.31.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.683070 spinedb_api-0.31.2/spinedb_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.683070 spinedb_api-0.31.2/spinedb_api/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.687070 spinedb_api-0.31.2/spinedb_api/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/e010777927a5_change_active_by_default_server_default_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46499 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/db_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50630 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/db_mapping_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/db_mapping_commit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63433 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/db_mapping_query_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/export_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.687070 spinedb_api-0.31.2/spinedb_api/export_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/export_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52885 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/export_mapping/export_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/export_mapping/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/export_mapping/group_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/export_mapping/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22267 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/export_mapping/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.691070 spinedb_api-0.31.2/spinedb_api/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/filters/alternative_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/filters/execution_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/filters/renamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/filters/scenario_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/filters/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/filters/value_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/graph_layout_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28826 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/import_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.691070 spinedb_api-0.31.2/spinedb_api/import_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/import_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15737 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/import_mapping/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39635 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/import_mapping/import_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/import_mapping/import_mapping_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/import_mapping/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36231 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/mapped_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60771 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/perfect_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/server_client_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28277 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_db_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.691070 spinedb_api-0.31.2/spinedb_api/spine_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.691070 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/gdx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/sql_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/exporters/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/gdx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.695070 spinedb_api-0.31.2/spinedb_api/spine_io/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/datapackage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/gdx_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/spine_io/importers/sqlalchemy_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/spinedb_api/temp_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 13:45:41.000000 spinedb_api-0.31.2/spinedb_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.703070 spinedb_api-0.31.2/spinedb_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-30 13:45:41.000000 spinedb_api-0.31.2/spinedb_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-30 13:45:41.000000 spinedb_api-0.31.2/spinedb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:45:41.000000 spinedb_api-0.31.2/spinedb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:45:41.000000 spinedb_api-0.31.2/spinedb_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 13:45:41.000000 spinedb_api-0.31.2/spinedb_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 13:45:41.000000 spinedb_api-0.31.2/spinedb_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.695070 spinedb_api-0.31.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/custom_db_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.695070 spinedb_api-0.31.2/tests/export_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/export_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77130 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/export_mapping/test_export_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/export_mapping/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/export_mapping/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.699070 spinedb_api-0.31.2/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/test_alternative_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/test_execution_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/test_renamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27281 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/test_scenario_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/test_tool_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/filters/test_value_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.699070 spinedb_api-0.31.2/tests/import_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/import_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29089 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/import_mapping/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87795 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/import_mapping/test_import_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/import_mapping/test_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/mock_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.699070 spinedb_api-0.31.2/tests/spine_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.699070 spinedb_api-0.31.2/tests/spine_io/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/exporters/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/exporters/test_excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/exporters/test_gdx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/exporters/test_sql_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/exporters/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:41.703070 spinedb_api-0.31.2/tests/spine_io/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/test_CSVConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/test_GdxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/test_datapackage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/test_excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/test_json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/importers/test_sqlalchemy_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/spine_io/test_excel_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211062 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_DatabaseMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_check_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_db_mapping_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_db_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_export_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78082 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_import_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48773 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-30 13:45:34.000000 spinedb_api-0.31.2/tests/test_purge.py
```

### Comparing `spinedb_api-0.31.1/.github/workflows/run_unit_tests.yml` & `spinedb_api-0.31.2/.github/workflows/run_unit_tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -27,35 +27,34 @@
       run: git describe --tags
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
         cache-dependency-path: |
-          requirements.txt
           pyproject.toml
+          dev-requirements.txt
     - name: Display Python version
       run:
          python -c "import sys; print(sys.version)"
     - name: Install unixodbc
       if: runner.os == 'Linux'
       run:
         sudo apt-get install -y unixodbc-dev  # Install to get sql.h headers
     - name: Install dependencies
       env:
         PYTHONUTF8: 1
       run: |
         python -m pip install --upgrade pip
-        python -m pip install .[dev]
+        python -m pip install -e .
+        python -m pip install -r dev-requirements.txt
     - name: List packages
       run:
         python -m pip list
     - name: Run tests
-      env: 
-        QT_QPA_PLATFORM: offscreen
       run:
         coverage run -m unittest discover --verbose
     - name: Upload coverage report to Codecov
       uses: codecov/codecov-action@v4
       env:
         CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
   toolbox-unit-tests:
@@ -73,34 +72,33 @@
         fetch-depth: 0
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
+        python -m pip install git+${{ github.server_url }}/${{ github.repository }}.git@${{ github.ref_name }}
     - name: List packages
       run:
         python -m pip list
-    - name: Install python3 kernelspecs
-      run: |
-        python -m pip install ipykernel
-        python -m ipykernel install --user
     - name: Run tests
       run: |
         if [ "$RUNNER_OS" != "Windows" ]; then
           export QT_QPA_PLATFORM=offscreen
         fi
         python -m unittest discover --verbose
       shell: bash
@@ -118,26 +116,29 @@
         repository: spine-tools/Spine-Toolbox
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
+        python -m pip install git+${{ github.server_url }}/${{ github.repository }}.git@${{ github.ref_name }}
     - name: List packages
       run:
         python -m pip list
     - name: Run tests
       run:
         python -m unittest discover --pattern execution_test.py --verbose
```

### Comparing `spinedb_api-0.31.1/.readthedocs.yml` & `spinedb_api-0.31.2/.readthedocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 formats:
   - htmlzip
   - pdf
 
 # Optionally set the version of Python and requirements required to build your docs
 python:
   install:
-    - requirements: requirements.txt
-    - requirements: docs/requirements.txt
+    - method: pip
+      path: .
+    - requirements: dev-requirements.txt
```

### Comparing `spinedb_api-0.31.1/COPYING` & `spinedb_api-0.31.2/COPYING`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/COPYING.LESSER` & `spinedb_api-0.31.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/PKG-INFO` & `spinedb_api-0.31.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: spinedb_api
-Version: 0.31.1
+Version: 0.31.2
 Summary: An API to talk to Spine databases.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/Spine-Database-API
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 Requires-Dist: sqlalchemy<1.4,>=1.3
 Requires-Dist: alembic>=1.7
-Requires-Dist: faker>=8.1.2
 Requires-Dist: datapackage>=1.15.2
 Requires-Dist: python-dateutil>=2.8.1
 Requires-Dist: numpy>=1.20.2
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: openpyxl!=3.1.1,>=3.0.7
 Requires-Dist: gdx2py>=2.1.1
 Requires-Dist: ijson>=3.1.4
 Requires-Dist: chardet>=4.0.0
 Requires-Dist: pymysql>=1.0.2
 Requires-Dist: psycopg2
-Provides-Extra: dev
-Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: pyperf; extra == "dev"
 
 # Spine Database API
 
 [![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
 [![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
 [![codecov](https://codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Database-API)
 [![PyPI version](https://badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api)
@@ -64,29 +60,27 @@
 
     $ pip install --upgrade git+https://github.com/spine-tools/Spine-Database-API.git
 
 
 ## Building the documentation
 
 Source files for the documentation can be found in `docs/source` directory. In order to 
-build the HTML docs, you need to install the additional documentation building requirements
+build the HTML docs, you need to install the developer dependencies
 by running:
 
-    $ pip install -r dev-requirements.txt 
+    $ pip install -r dev-requirements.txt
 
 This installs Sphinx (among other things), which is required in building the documentation.
 When Sphinx is installed, you can build the HTML pages from the source files by running:
 
-    > docs\make.bat html
+    > bin\build_doc.bat
     
 or
 
-    $ pushd docs
-    $ make html
-    $ popd
+    $ bin/build_doc.py
     
 depending on your operating system.        
  
 After running the build, the index page can be found in `docs/build/html/index.html`.
 
 &nbsp;
 <hr>
```

#### html2text {}

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.1 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.2 Summary: An API to talk
 to Spine databases. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/Spine-Database-API Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.8.1 Description-Content-Type: text/markdown License-File: COPYING
 License-File: COPYING.LESSER Requires-Dist: sqlalchemy<1.4,>=1.3 Requires-Dist:
-alembic>=1.7 Requires-Dist: faker>=8.1.2 Requires-Dist: datapackage>=1.15.2
-Requires-Dist: python-dateutil>=2.8.1 Requires-Dist: numpy>=1.20.2 Requires-
-Dist: scipy>=1.7.1 Requires-Dist: openpyxl!=3.1.1,>=3.0.7 Requires-Dist:
-gdx2py>=2.1.1 Requires-Dist: ijson>=3.1.4 Requires-Dist: chardet>=4.0.0
-Requires-Dist: pymysql>=1.0.2 Requires-Dist: psycopg2 Provides-Extra: dev
-Requires-Dist: coverage[toml]; extra == "dev" Requires-Dist: pyperf; extra ==
-"dev" # Spine Database API [![Documentation Status](https://readthedocs.org/
-projects/spine-database-api/badge/?version=latest)](https://spine-database-
-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests](https://github.com/
-spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://
-github.com/spine-tools/Spine-Database-API/
+alembic>=1.7 Requires-Dist: datapackage>=1.15.2 Requires-Dist: python-
+dateutil>=2.8.1 Requires-Dist: numpy>=1.20.2 Requires-Dist: scipy>=1.7.1
+Requires-Dist: openpyxl!=3.1.1,>=3.0.7 Requires-Dist: gdx2py>=2.1.1 Requires-
+Dist: ijson>=3.1.4 Requires-Dist: chardet>=4.0.0 Requires-Dist: pymysql>=1.0.2
+Requires-Dist: psycopg2 # Spine Database API [![Documentation Status](https://
+readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://
+spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests]
+(https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/
+badge.svg)](https://github.com/spine-tools/Spine-Database-API/
 actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
 tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/
 spine-tools/Spine-Database-API) [![PyPI version](https://badge.fury.io/py/
 spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A Python package to
 access and manipulate Spine databases in a customary, unified way. ## License
 Spine Database API is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
@@ -29,20 +27,20 @@
 install the package run: $ pip install spinedb_api To upgrade to the most
 recent version, run: $ pip install --upgrade spinedb_api You can also specify a
 branch, or a tag, for instance: $ pip install spinedb_api==0.12.1 To install
 the latest development version use the Git repository url: $ pip install --
 upgrade git+https://github.com/spine-tools/Spine-Database-API.git ## Building
 the documentation Source files for the documentation can be found in `docs/
 source` directory. In order to build the HTML docs, you need to install the
-additional documentation building requirements by running: $ pip install -
-r dev-requirements.txt This installs Sphinx (among other things), which is
-required in building the documentation. When Sphinx is installed, you can build
-the HTML pages from the source files by running: > docs\make.bat html or $
-pushd docs $ make html $ popd depending on your operating system. After running
-the build, the index page can be found in `docs/build/html/index.html`.  
+developer dependencies by running: $ pip install -r dev-requirements.txt This
+installs Sphinx (among other things), which is required in building the
+documentation. When Sphinx is installed, you can build the HTML pages from the
+source files by running: > bin\build_doc.bat or $ bin/build_doc.py depending on
+your operating system. After running the build, the index page can be found in
+`docs/build/html/index.html`.  
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spinedb_api-0.31.1/README.md` & `spinedb_api-0.31.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,29 +32,27 @@
 
     $ pip install --upgrade git+https://github.com/spine-tools/Spine-Database-API.git
 
 
 ## Building the documentation
 
 Source files for the documentation can be found in `docs/source` directory. In order to 
-build the HTML docs, you need to install the additional documentation building requirements
+build the HTML docs, you need to install the developer dependencies
 by running:
 
-    $ pip install -r dev-requirements.txt 
+    $ pip install -r dev-requirements.txt
 
 This installs Sphinx (among other things), which is required in building the documentation.
 When Sphinx is installed, you can build the HTML pages from the source files by running:
 
-    > docs\make.bat html
+    > bin\build_doc.bat
     
 or
 
-    $ pushd docs
-    $ make html
-    $ popd
+    $ bin/build_doc.py
     
 depending on your operating system.        
  
 After running the build, the index page can be found in `docs/build/html/index.html`.
 
 &nbsp;
 <hr>
```

#### html2text {}

```diff
@@ -14,20 +14,20 @@
 install the package run: $ pip install spinedb_api To upgrade to the most
 recent version, run: $ pip install --upgrade spinedb_api You can also specify a
 branch, or a tag, for instance: $ pip install spinedb_api==0.12.1 To install
 the latest development version use the Git repository url: $ pip install --
 upgrade git+https://github.com/spine-tools/Spine-Database-API.git ## Building
 the documentation Source files for the documentation can be found in `docs/
 source` directory. In order to build the HTML docs, you need to install the
-additional documentation building requirements by running: $ pip install -
-r dev-requirements.txt This installs Sphinx (among other things), which is
-required in building the documentation. When Sphinx is installed, you can build
-the HTML pages from the source files by running: > docs\make.bat html or $
-pushd docs $ make html $ popd depending on your operating system. After running
-the build, the index page can be found in `docs/build/html/index.html`.  
+developer dependencies by running: $ pip install -r dev-requirements.txt This
+installs Sphinx (among other things), which is required in building the
+documentation. When Sphinx is installed, you can build the HTML pages from the
+source files by running: > bin\build_doc.bat or $ bin/build_doc.py depending on
+your operating system. After running the build, the index page can be found in
+`docs/build/html/index.html`.  
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spinedb_api-0.31.1/benchmarks/README.md` & `spinedb_api-0.31.2/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/benchmarks/datetime_from_database.py` & `spinedb_api-0.31.2/benchmarks/datetime_from_database.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/benchmarks/map_from_database.py` & `spinedb_api-0.31.2/benchmarks/map_from_database.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/benchmarks/mapped_item_getitem.py` & `spinedb_api-0.31.2/benchmarks/mapped_item_getitem.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/benchmarks/update_default_value_to_different_value.py` & `spinedb_api-0.31.2/benchmarks/update_default_value_to_different_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/benchmarks/update_default_value_to_same_value.py` & `spinedb_api-0.31.2/benchmarks/update_default_value_to_same_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/benchmarks/utils.py` & `spinedb_api-0.31.2/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/deploy-key.enc` & `spinedb_api-0.31.2/deploy-key.enc`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/Makefile` & `spinedb_api-0.31.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/make.bat` & `spinedb_api-0.31.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/source/conf.py` & `spinedb_api-0.31.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 "     - value",
             ]
         )
         for f_name, f_dict in factory.fields.items():
             lines.extend([f"   * - {f_name}", f"     - {type_(f_dict)}", f"     - {f_dict['value']}"])
         lines.append("")
         lines.extend([".. list-table:: Unique keys", "   :header-rows: 0", ""])
-        for f_names in factory._unique_keys:
+        for f_names in factory.unique_keys:
             f_names = ", ".join(f_names)
             lines.append(f"   * - {f_names}")
         lines.append("")
     return lines
 
 
 def setup(sphinx):
@@ -277,15 +277,18 @@
 
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"https://docs.python.org/": None, "https://docs.sqlalchemy.org/en/13/": None}
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/", None),
+    "sqlalchemy": ("https://docs.sqlalchemy.org/en/13/", None)
+}
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
 autodoc_member_order = "bysource"
```

### Comparing `spinedb_api-0.31.1/docs/source/front_matter.rst` & `spinedb_api-0.31.2/docs/source/front_matter.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/source/img/spinetoolbox_on_wht.svg` & `spinedb_api-0.31.2/docs/source/img/spinetoolbox_on_wht.svg`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/source/index.rst` & `spinedb_api-0.31.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/source/metadata.rst` & `spinedb_api-0.31.2/docs/source/metadata.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/source/parameter_value_format.rst` & `spinedb_api-0.31.2/docs/source/parameter_value_format.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/docs/source/tutorial.rst` & `spinedb_api-0.31.2/docs/source/tutorial.rst`

 * *Files 11% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 Let's begin the party by adding a couple of entity classes::
 
     db_map.add_entity_class_item(name="fish", description="It swims.")
     db_map.add_entity_class_item(name="cat", description="Eats fish.")
 
 Now let's add a multi-dimensional entity class between the two above. For this we need to specify the class names
-as `dimension_name_list`::
+as ``dimension_name_list``::
 
     db_map.add_entity_class_item(
         name="fish__cat",
         dimension_name_list=("fish", "cat"),
         description="A fish getting eaten by a cat?",
     )
 
@@ -87,15 +87,15 @@
 
     db_map.add_entity_item(entity_class_name="fish", name="Nemo", description="Lost (for now).")
     db_map.add_entity_item(
         entity_class_name="cat", name="Felix", description="The wonderful wonderful cat."
     )
 
 Let's add a multi-dimensional entity to our multi-dimensional class. For this we need to specify the entity names
-as `element_name_list`::
+as ``element_name_list``::
 
     db_map.add_entity_item(entity_class_name="fish__cat", element_name_list=("Nemo", "Felix"))
 
 Let's add a parameter definition for one of our entity classes::
 
     db_map.add_parameter_definition_item(entity_class_name="fish", name="color")
 
@@ -112,15 +112,23 @@
         parameter_definition_name="color",
         alternative_name="Base",
         value=value,
         type=type_
     )
 
 Note that in the above, we refer to the entity by its *byname*.
-We also set the value to belong to an *alternative* called ``Base``
+Byname is a single-element tuple containing the name of the entity if it is 0-dimensional like ``("Nemo",)`` above.
+For multi-dimensional entities, byname consists of the entity's 0-dimensional elements
+such as ``("Nemo", "Felix")`` for the ``"fish__cat"`` entity.
+At a quick glance, ``entity_byname`` and ``element_name_list`` may look the same
+but this is true only for certain cases.
+``element_name_list`` contains the names of the n-1 dimensional elements of n-dimensional entities
+while ``entity_byname`` breaks the element names down to their 0-dimensional parts, or contains just the entity's name.
+
+We also set the value to belong to an *alternative* called ``"Base"``
 which is readily available in new databases.
 
 .. note::
 
   The data we've added so far is not yet in the DB, but only in an in-memory mapping within our ``db_map`` object.
   Don't worry, we will save it to the DB soon (see `Committing data`_ if you're impatient).
 
@@ -189,25 +197,42 @@
 
 Removing data
 -------------
 
 You know what, let's just remove the entity entirely.
 To do this we use the :meth:`~.PublicItem.remove` method of :class:`~.PublicItem`::
 
-    db_map.get_entity_item(entity_class_name="fish", name="NotNemo").remove()
+    not_nemo = db_map.get_entity_item(entity_class_name="fish", name="NotNemo")
+    not_nemo.remove()
 
 Note that the above call removes items in *cascade*,
 meaning that items that depend on ``"NotNemo"`` will get removed as well.
 We have one such item in the database, namely the ``"color"`` parameter value
 which also gets dropped when the above method is called.
 
 Restoring data
 --------------
 
-TODO
+Already regretting we lost Ne... I mean the fish that is not Nemo?
+It is possible to resurrect a removed item and bring back all its dependants with :meth:`~.PublicItem.restore`::
+
+    not_nemo.restore()
+
+The above will also bring back the ``"color"`` parameter value.
+
+Luckily, we stored ``"NotNemo"`` in a variable ``not_nemo`` before removing it
+so it was possible to call :meth:`~.PublicItem.restore` on it.
+What if you had removed ``"NotNemo"`` with the following::
+
+   db_map.get_entity_item(entity_class_name="fish", name="NotNemo").remove()
+
+It is still possible to access removed items by passing ``skip_removed=False`` to the ``get_*_item()`` methods::
+
+   not_nemo = db_map.get_entity_item(entity_class_name="fish", name="NotNemo", skip_removed=False)
+   not_nemo.restore()
 
 Committing data
 ---------------
 
 Enough messing around. To save the contents of the in-memory mapping into the DB,
 we use :meth:`~.DatabaseMapping.commit_session`::
```

### Comparing `spinedb_api-0.31.1/fig/eu-emblem-low-res.jpg` & `spinedb_api-0.31.2/fig/eu-emblem-low-res.jpg`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/pylintrc` & `spinedb_api-0.31.2/pylintrc`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/pyproject.toml` & `spinedb_api-0.31.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,34 +12,29 @@
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8.1"
 dependencies = [
     # v1.4 does not pass tests
     "sqlalchemy >=1.3, <1.4",
     "alembic >=1.7",
-    "faker >=8.1.2",
     "datapackage >=1.15.2",
     "python-dateutil >=2.8.1",
-    # v1.22 requires Python 3.8 or later
     "numpy >=1.20.2",
     "scipy >=1.7.1",
     "openpyxl >=3.0.7, !=3.1.1",
     "gdx2py >=2.1.1",
     "ijson >=3.1.4",
     "chardet >=4.0.0",
     "pymysql >=1.0.2",
     "psycopg2",
 ]
 
 [project.urls]
 Repository = "https://github.com/spine-tools/Spine-Database-API"
 
-[project.optional-dependencies]
-dev = ["coverage[toml]", "pyperf"]
-
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel", "build"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "spinedb_api/version.py"
 version_scheme = "release-branch-semver"
```

### Comparing `spinedb_api-0.31.1/spinedb_api/__init__.py` & `spinedb_api-0.31.2/spinedb_api/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/env.py` & `spinedb_api-0.31.2/spinedb_api/alembic/env.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/e010777927a5_change_active_by_default_server_default_.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/e010777927a5_change_active_by_default_server_default_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py` & `spinedb_api-0.31.2/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/alembic.ini` & `spinedb_api-0.31.2/spinedb_api/alembic.ini`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/compatibility.py` & `spinedb_api-0.31.2/spinedb_api/compatibility.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/db_mapping.py` & `spinedb_api-0.31.2/spinedb_api/db_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,14 +483,21 @@
         """
         item_type = self.real_item_type(item_type)
         mapped_table = self.mapped_table(item_type)
         self._convert_legacy(item_type, kwargs)
         if not check:
             return mapped_table.add_item(kwargs), None
         checked_item, error = mapped_table.checked_item_and_error(kwargs)
+        if not error:
+            existing_item = mapped_table.find_item_by_unique_key(checked_item, fetch=False, valid_only=False)
+            if existing_item:
+                if not existing_item.removed:
+                    raise RuntimeError("Logic error: item exists but no error was issued")
+                existing_item.invalidate_id()
+                mapped_table.remove_unique(existing_item)
         return (mapped_table.add_item(checked_item).public_item if checked_item else None, error)
 
     def add_items(self, item_type, *items, check=True, strict=False):
         """Adds many items to the in-memory mapping.
 
         Args:
             item_type (str): One of <spine_item_types>.
@@ -607,15 +614,16 @@
             tuple(:class:`PublicItem` or None, str): The removed item and any errors.
         """
         item_type = self.real_item_type(item_type)
         mapped_table = self.mapped_table(item_type)
         item, error = mapped_table.item_to_remove_and_error(id_)
         if check and error:
             return None, error
-        return mapped_table.remove_item(item).public_item, None
+        removed_item = mapped_table.remove_item(item)
+        return (removed_item.public_item, None) if removed_item else (None, "failed to remove")
 
     def remove_items(self, item_type, *ids, check=True, strict=False):
         """Removes many items from the in-memory mapping.
 
         Args:
             item_type (str): One of <spine_item_types>.
             *ids (Iterable(int)): Ids of items to be removed.
@@ -649,19 +657,20 @@
                 db_map.restore_item("entity", prince["id"])
 
         Args:
             item_type (str): One of <spine_item_types>.
             id_ (int): The id of the item to restore.
 
         Returns:
-            tuple(:class:`PublicItem` or None, str): The restored item if any.
+            tuple(:class:`PublicItem` or None, str): The restored item if any and possible error.
         """
         item_type = self.real_item_type(item_type)
         mapped_table = self.mapped_table(item_type)
-        return mapped_table.restore_item(id_).public_item
+        restored_item = mapped_table.restore_item(id_)
+        return (restored_item.public_item, "") if restored_item else (None, "failed to restore item")
 
     def restore_items(self, item_type, *ids):
         """Restores many previously removed items into the in-memory mapping.
 
         Args:
             item_type (str): One of <spine_item_types>.
             *ids (Iterable(int)): Ids of items to be removed.
@@ -885,15 +894,15 @@
 
     def _a(item_type):
         return "an" if any(item_type.lower().startswith(x) for x in "aeiou") else "a"
 
     def _uq_fields(factory):
         return {
             f_name: factory.fields[f_name]
-            for f_names in factory._unique_keys
+            for f_names in factory.unique_keys
             for f_name in set(f_names) & set(factory.fields.keys())
         }
 
     def _kwargs(fields):
         def type_(f_dict):
             return f_dict["type"].__name__ + (", optional" if f_dict.get("optional", False) else "")
```

### Comparing `spinedb_api-0.31.1/spinedb_api/db_mapping_base.py` & `spinedb_api-0.31.2/spinedb_api/db_mapping_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                     to_update.append(item)
             if item_type in purged_item_types:
                 to_remove.append(mapped_table.wildcard_item)
                 to_remove.extend(mapped_table.values())
             else:
                 for item in mapped_table.values():
                     item.validate()
-                    if item.status == Status.to_remove:
+                    if item.status == Status.to_remove and item.has_valid_id:
                         to_remove.append(item)
             if to_add or to_update or to_remove:
                 dirty_items.append((item_type, (to_add, to_update, to_remove)))
         return dirty_items
 
     def _rollback(self):
         """Discards uncommitted changes.
@@ -422,32 +422,34 @@
         """
         return self._db_map.make_item(self._item_type, **item)
 
     def find_item(self, item, skip_keys=(), fetch=True):
         """Returns a MappedItemBase that matches the given dictionary-item.
 
         Args:
-            item (dict)
+            item (dict): item's unique keys
+            skip_keys (tuple of str): unique keys to skip
+            fetch (bool): if True, fetch db if item is not found in-memory
 
         Returns:
             MappedItemBase or None
         """
         id_ = item.get("id")
         if id_ is not None:
             return self.find_item_by_id(id_, fetch=fetch)
-        return self._find_item_by_unique_key(item, skip_keys=skip_keys, fetch=fetch)
+        return self.find_item_by_unique_key(item, skip_keys=skip_keys, fetch=fetch)
 
     def find_item_by_id(self, id_, fetch=True):
         current_item = self.get(id_, {})
         if not current_item and fetch:
             self._db_map.do_fetch_all(self._item_type)
             current_item = self.get(id_, {})
         return current_item
 
-    def _find_item_by_unique_key(self, item, skip_keys=(), fetch=True, valid_only=True):
+    def find_item_by_unique_key(self, item, skip_keys=(), fetch=True, valid_only=True):
         for key, value in self._db_map.item_factory(self._item_type).unique_values_for_item(item, skip_keys=skip_keys):
             current_item = self._unique_key_value_to_item(key, value, fetch=fetch, valid_only=valid_only)
             if current_item:
                 return current_item
         # Maybe item is missing some key stuff, so try with a resolved and polished MappedItem too...
         mapped_item = self._make_item(item)
         error = mapped_item.resolve_internal_fields(skip_keys=item.keys())
@@ -470,21 +472,44 @@
             full_item, merge_error = current_item.merge(item)
             if full_item is None:
                 return None, merge_error
         else:
             current_item = None
             full_item, merge_error = item, None
         candidate_item = self._make_item(full_item)
+        if current_item is None:
+            error = self._check_unique_keys(candidate_item)
+            if error:
+                return None, error
         error = self._prepare_item(candidate_item, current_item, item)
         if error:
             return None, error
         valid_types = (type(None),) if for_update else ()
         self.check_fields(candidate_item._asdict(), valid_types=valid_types)
         return candidate_item, merge_error
 
+    def _check_unique_keys(self, item):
+        """Checks that unique keys are set in given item for addition.
+
+        Args:
+            item (MappedItemBase): item to check
+
+        Returns:
+            str: error or empty string if item is OK
+        """
+        missing = []
+        for key_set in item.unique_keys:
+            missing = [key for key in key_set if key not in item]
+            if not missing:
+                return ""
+            missing = [key for key in missing if item.corresponding_unique_id_keys.get(key) not in item]
+            if not missing:
+                return ""
+        return f"missing values for unique keys {missing}" if missing else ""
+
     def _prepare_item(self, candidate_item, current_item, original_item):
         """Prepares item for insertion or update, returns any errors.
 
         Args:
             candidate_item (MappedItem)
             current_item (MappedItem)
             original_item (dict)
@@ -547,22 +572,28 @@
         return item
 
     def add_item_from_db(self, item, is_db_clean):
         """Adds an item fetched from the DB.
 
         Args:
             item (dict): item from the DB.
-            is_db_clean (Bool)
+            is_db_clean (bool)
 
         Returns:
-            tuple(MappedItem,bool): A mapped item and whether it needs to be added to the unique key values dict.
+            tuple(MappedItem, bool): A mapped item and whether it needs to be added to the unique key values dict.
         """
-        mapped_item = self._find_item_by_unique_key(item, fetch=False, valid_only=False)
+        mapped_item = self.find_item_by_unique_key(item, fetch=False, valid_only=False)
         if mapped_item and (is_db_clean or self._same_item(mapped_item, item)):
             mapped_item.force_id(item["id"])
+            if mapped_item.status == Status.to_add:
+                # We could test if the non-unique fields of mapped_item and db item are equal
+                # and set status to Status.committed
+                # but that is potentially complex operation (for e.g. large parameter values)
+                # so we take a shortcut here and assume that mapped_item always contains modified data.
+                mapped_item.status = Status.to_update
             return mapped_item, False
         mapped_item = self.get(item["id"])
         if mapped_item and (is_db_clean or self._same_item(mapped_item.db_equivalent(), item)):
             return mapped_item, False
         conflicting_item = self.get(item["id"])
         if conflicting_item is not None:
             conflicting_item.handle_id_steal()
@@ -650,21 +681,25 @@
 class MappedItemBase(dict):
     """A dictionary that represents a db item."""
 
     fields = {}
     """A dictionary mapping fields to a another dict mapping "type" to a Python type,
     "value" to a description of the value for the key, and "optional" to a bool."""
     _defaults = {}
-    """A dictionary mapping fields to their default values"""
-    _unique_keys = ()
-    """A tuple where each element is itself a tuple of fields corresponding to a unique key"""
+    """A dictionary mapping fields to their default values."""
+    unique_keys = ()
+    """A tuple where each element is itself a tuple of fields corresponding to a unique key."""
+    corresponding_unique_id_keys = {}
+    """A dictionary mapping unique keys to corresponding id keys."""
     _references = {}
     """A dictionary mapping source fields, to a tuple of reference item type and reference field.
     Used to access external fields.
     """
+    _soft_references = set()
+    """A set of reference source fields that are OK to have no external field value."""
     _external_fields = {}
     """A dictionary mapping fields that are not in the original dictionary, to a tuple of source field
     and target field.
     When accessing fields in _external_fields, we first find the reference pointed at by the source field,
     and then return the target field of that reference.
     """
     _alt_references = {}
@@ -778,15 +813,14 @@
             str
         """
         return self._item_type
 
     @property
     def key(self):
         """Returns a tuple (item_type, id) for convenience, or None if this item doesn't yet have an id.
-        TODO: When does the latter happen?
 
         Returns:
             tuple(str,int) or None
         """
         id_ = dict.get(self, "id")
         if id_ is None:
             return None
@@ -796,14 +830,18 @@
     def has_valid_id(self):
         return self._has_valid_id
 
     def invalidate_id(self):
         """Sets id as invalid."""
         self._has_valid_id = False
 
+    def validate_id(self):
+        """Sets id as valid"""
+        self._has_valid_id = True
+
     def _extended(self):
         """Returns a dict from this item's original fields plus all the references resolved statically.
 
         Returns:
             dict
         """
         d = self._asdict()
@@ -879,14 +917,16 @@
         If successful, replace source fields referring to db-ids with the reference's TempId.
 
         Yields:
             tuple(str,MappedItem or None): the source field and resolved ref.
         """
         for src_key, (ref_type, ref_key) in self._references.items():
             ref = self._get_full_ref(src_key, ref_type, ref_key)
+            if not ref and src_key in self._soft_references:
+                continue
             if isinstance(ref, tuple):
                 for r in ref:
                     yield src_key, r
             else:
                 yield src_key, ref
 
     def _get_full_ref(self, src_key, ref_type, ref_key, strong=True):
@@ -902,15 +942,15 @@
         ref = self._get_ref(ref_type, {ref_key: src_val}, strong=strong)
         if ref and ref_key == "id":
             self[src_key] = ref["id"]
         return ref
 
     @classmethod
     def unique_values_for_item(cls, item, skip_keys=()):
-        for key in cls._unique_keys:
+        for key in cls.unique_keys:
             if key not in skip_keys:
                 value = tuple(item.get(k) for k in key)
                 if None not in value:
                     yield key, value
 
     def unique_key_values(self, skip_keys=()):
         """Yields tuples of unique keys and their values.
@@ -1217,14 +1257,16 @@
         if self._status == Status.committed:
             self._status = Status.to_update
             self._backup = self._asdict()
         elif self._status in (Status.to_remove, Status.added_and_removed):
             raise RuntimeError("invalid status of item being updated")
         for src_key, (ref_type, ref_key) in self._references.items():
             src_val = self[src_key]
+            if src_val is None and src_key in self._soft_references:
+                continue
             if src_key in other and other[src_key] != src_val:
                 # Invalidate references
                 if isinstance(src_val, tuple):
                     for x in src_val:
                         self._invalidate_ref(ref_type, {ref_key: x})
                 else:
                     self._invalidate_ref(ref_type, {ref_key: src_val})
@@ -1240,18 +1282,15 @@
 
         Args:
             id_ (int): The most recent id_ of the item as fetched from the DB.
         """
         mapped_id = self["id"]
         if mapped_id == id_:
             return
-        # Resolve the TempId to the new db id (and commit the item if pending)
         mapped_id.resolve(id_)
-        if self.status == Status.to_add:
-            self.status = Status.committed
 
     def handle_id_steal(self):
         """Called when a new item is fetched from the DB with this item's id."""
         self["id"].unresolve()
         # TODO: Test if the below works...
         if self.is_committed():
             self._status = self._status_when_committed
@@ -1270,14 +1309,17 @@
     @property
     def item_type(self):
         return self._mapped_item.item_type
 
     def __getitem__(self, key):
         return self._mapped_item[key]
 
+    def __contains__(self, item):
+        return self._mapped_item._extended().__contains__(item)
+
     def __eq__(self, other):
         if isinstance(other, dict):
             return self._mapped_item == other
         return super().__eq__(other)
 
     def __repr__(self):
         return repr(self._mapped_item)
@@ -1306,14 +1348,24 @@
     def update(self, **kwargs):
         self._db_map.update_item(self.item_type, id=self["id"], **kwargs)
 
     def remove(self):
         return self._db_map.remove_item(self.item_type, self["id"])
 
     def restore(self):
+        if not self._mapped_item.has_valid_id:
+            mapped_table = self._db_map.mapped_table(self.item_type)
+            existing_item = mapped_table.find_item_by_unique_key(self, fetch=False, valid_only=False)
+            if existing_item:
+                if not existing_item.removed:
+                    return None, "restoring would create a conflict with another item with same unique values"
+                existing_item.invalidate_id()
+                mapped_table.remove_unique(existing_item)
+                self._mapped_item.validate_id()
+                mapped_table.add_unique(self._mapped_item)
         return self._db_map.restore_item(self.item_type, self["id"])
 
     def add_update_callback(self, callback):
         self._mapped_item.update_callbacks.add(callback)
 
     def add_remove_callback(self, callback):
         self._mapped_item.remove_callbacks.add(callback)
```

### Comparing `spinedb_api-0.31.1/spinedb_api/db_mapping_commit_mixin.py` & `spinedb_api-0.31.2/spinedb_api/db_mapping_commit_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/db_mapping_query_mixin.py` & `spinedb_api-0.31.2/spinedb_api/db_mapping_query_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/exception.py` & `spinedb_api-0.31.2/spinedb_api/exception.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/export_functions.py` & `spinedb_api-0.31.2/spinedb_api/export_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/export_mapping/__init__.py` & `spinedb_api-0.31.2/spinedb_api/export_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/export_mapping/export_mapping.py` & `spinedb_api-0.31.2/spinedb_api/export_mapping/export_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/export_mapping/generator.py` & `spinedb_api-0.31.2/spinedb_api/export_mapping/generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/export_mapping/group_functions.py` & `spinedb_api-0.31.2/spinedb_api/export_mapping/group_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/export_mapping/pivot.py` & `spinedb_api-0.31.2/spinedb_api/export_mapping/pivot.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/export_mapping/settings.py` & `spinedb_api-0.31.2/spinedb_api/export_mapping/settings.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/filters/__init__.py` & `spinedb_api-0.31.2/spinedb_api/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/filters/alternative_filter.py` & `spinedb_api-0.31.2/spinedb_api/filters/alternative_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/filters/execution_filter.py` & `spinedb_api-0.31.2/spinedb_api/filters/execution_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/filters/renamer.py` & `spinedb_api-0.31.2/spinedb_api/filters/renamer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/filters/scenario_filter.py` & `spinedb_api-0.31.2/spinedb_api/filters/scenario_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/filters/tools.py` & `spinedb_api-0.31.2/spinedb_api/filters/tools.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/filters/value_transformer.py` & `spinedb_api-0.31.2/spinedb_api/filters/value_transformer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/graph_layout_generator.py` & `spinedb_api-0.31.2/spinedb_api/graph_layout_generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/helpers.py` & `spinedb_api-0.31.2/spinedb_api/helpers.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/import_functions.py` & `spinedb_api-0.31.2/spinedb_api/import_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/import_mapping/__init__.py` & `spinedb_api-0.31.2/spinedb_api/import_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/import_mapping/generator.py` & `spinedb_api-0.31.2/spinedb_api/import_mapping/generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping.py` & `spinedb_api-0.31.2/spinedb_api/import_mapping/import_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
             return
         if errors is None:
             errors = []
         if not (self.position == Position.hidden and self.value is None):
             source_data = self._data(source_row)
             if source_data is None:
                 self._skip_row(state)
+                return
             else:
                 try:
                     self._import_row(source_data, state, mapped_data)
                 except KeyError as err:
                     for key in err.args:
                         msg = f"Required key '{key}' is invalid"
                         error = InvalidMappingComponent(msg, self.rank, key)
```

### Comparing `spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping_compat.py` & `spinedb_api-0.31.2/spinedb_api/import_mapping/import_mapping_compat.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/import_mapping/type_conversion.py` & `spinedb_api-0.31.2/spinedb_api/import_mapping/type_conversion.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/mapped_items.py` & `spinedb_api-0.31.2/spinedb_api/mapped_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 from operator import itemgetter
 import time
-from .helpers import name_from_elements
+from .helpers import name_from_dimensions, name_from_elements
 from .parameter_value import to_database, from_database, ParameterValueFormatError
 from .db_mapping_base import MappedItemBase
 
 
 def item_factory(item_type):
     return {
         "commit": CommitItem,
@@ -34,24 +34,27 @@
         "scenario_alternative": ScenarioAlternativeItem,
         "metadata": MetadataItem,
         "entity_metadata": EntityMetadataItem,
         "parameter_value_metadata": ParameterValueMetadataItem,
     }.get(item_type, MappedItemBase)
 
 
-_ENTITY_BYNAME_VALUE = "A tuple with the entity name as single element if the entity is zero-dimensional, or the element names if the entity is multi-dimensional."
+_ENTITY_BYNAME_VALUE = (
+    "A tuple with the entity name as single element if the entity is 0-dimensional, "
+    "or the 0-dimensional element names if the entity is multi-dimensional."
+)
 
 
 class CommitItem(MappedItemBase):
     fields = {
         "comment": {"type": str, "value": "A comment describing the commit."},
         "date": {"type": str, "value": "Date and time of the commit in ISO 8601 format."},
         "user": {"type": str, "value": "Username of the committer."},
     }
-    _unique_keys = (("date",),)
+    unique_keys = (("date",),)
     is_protected = True
 
     def commit(self, commit_id):
         raise RuntimeError("Commits are created automatically when session is committed.")
 
 
 class EntityClassItem(MappedItemBase):
@@ -72,43 +75,44 @@
         "hidden": {"type": int, "value": "Not in use at the moment.", "optional": True},
         "active_by_default": {
             "type": bool,
             "value": "Default activity for the entity alternatives of the class.",
             "optional": True,
         },
     }
-    _defaults = {"description": None, "display_icon": None, "display_order": 99, "hidden": False}
-    _unique_keys = (("name",),)
+    _defaults = {
+        "description": None,
+        "display_icon": None,
+        "display_order": 99,
+        "hidden": False,
+        "active_by_default": True,
+    }
+    unique_keys = (("name",),)
     _references = {"dimension_id_list": ("entity_class", "id")}
     _external_fields = {"dimension_name_list": ("dimension_id_list", "name")}
     _alt_references = {("dimension_name_list",): ("entity_class", ("name",))}
     _internal_fields = {"dimension_id_list": (("dimension_name_list",), "id")}
     _private_fields = {"dimension_count"}
 
     def __init__(self, *args, **kwargs):
         dimension_id_list = kwargs.get("dimension_id_list")
         if dimension_id_list is None:
             dimension_id_list = ()
+            if "name" not in kwargs and "dimension_name_list" in kwargs:
+                kwargs["name"] = name_from_dimensions(kwargs["dimension_name_list"])
         if isinstance(dimension_id_list, str):
             dimension_id_list = (int(id_) for id_ in dimension_id_list.split(","))
         kwargs["dimension_id_list"] = tuple(dimension_id_list)
         super().__init__(*args, **kwargs)
 
     def __getitem__(self, key):
         if key in ("superclass_id", "superclass_name"):
             return self._get_ref("superclass_subclass", {"subclass_id": self["id"]}, strong=False).get(key)
         return super().__getitem__(key)
 
-    def polish(self):
-        error = super().polish()
-        if error:
-            return error
-        if "active_by_default" not in self:
-            self["active_by_default"] = True
-
     def merge(self, other):
         dimension_id_list = other.pop("dimension_id_list", None)
         error = (
             "can't modify dimensions of an entity class"
             if dimension_id_list is not None and dimension_id_list != self["dimension_id_list"]
             else ""
         )
@@ -122,22 +126,22 @@
 class EntityItem(MappedItemBase):
     fields = {
         "entity_class_name": {"type": str, "value": "The entity class name."},
         "name": {"type": str, "value": "The entity name."},
         "element_name_list": {"type": tuple, "value": "The element names if the entity is multi-dimensional."},
         "entity_byname": {
             "type": tuple,
-            "value": "A tuple with the entity name as single element if the entity is zero-dimensional,"
-            "or the element names if it is multi-dimensional.",
+            "value": _ENTITY_BYNAME_VALUE,
         },
         "description": {"type": str, "value": "The entity description.", "optional": True},
     }
 
     _defaults = {"description": None}
-    _unique_keys = (("entity_class_name", "name"), ("entity_class_name", "entity_byname"))
+    unique_keys = (("entity_class_name", "name"), ("entity_class_name", "entity_byname"))
+    corresponding_unique_id_keys = {"entity_class_name": "class_id"}
     _references = {"class_id": ("entity_class", "id"), "element_id_list": ("entity", "id")}
     _external_fields = {
         "entity_class_name": ("class_id", "name"),
         "dimension_id_list": ("class_id", "dimension_id_list"),
         "dimension_name_list": ("class_id", "dimension_name_list"),
         "superclass_id": ("class_id", "superclass_id"),
         "superclass_name": ("class_id", "superclass_name"),
@@ -153,14 +157,16 @@
         "element_id_list": (("dimension_name_list", "element_name_list"), "id"),
     }
 
     def __init__(self, *args, **kwargs):
         element_id_list = kwargs.get("element_id_list")
         if element_id_list is None:
             element_id_list = ()
+            if "name" not in kwargs and "element_name_list" in kwargs:
+                kwargs["name"] = name_from_elements(kwargs["element_name_list"])
         if isinstance(element_id_list, str):
             element_id_list = (int(id_) for id_ in element_id_list.split(","))
         kwargs["element_id_list"] = tuple(element_id_list)
         super().__init__(*args, **kwargs)
 
     @classmethod
     def unique_values_for_item(cls, item, skip_keys=()):
@@ -263,15 +269,20 @@
 
 class EntityGroupItem(MappedItemBase):
     fields = {
         "entity_class_name": {"type": str, "value": "The entity class name."},
         "group_name": {"type": str, "value": "The group entity name."},
         "member_name": {"type": str, "value": "The member entity name."},
     }
-    _unique_keys = (("entity_class_name", "group_name", "member_name"),)
+    unique_keys = (("entity_class_name", "group_name", "member_name"),)
+    corresponding_unique_id_keys = {
+        "entity_class_name": "entity_class_id",
+        "group_name": "entity_id",
+        "member_name": "member_id",
+    }
     _references = {
         "entity_class_id": ("entity_class", "id"),
         "entity_id": ("entity", "id"),
         "member_id": ("entity", "id"),
     }
     _external_fields = {
         "entity_class_name": ("entity_class_id", "name"),
@@ -312,15 +323,16 @@
         "active": {
             "type": bool,
             "value": "Whether the entity is active in the alternative - defaults to True.",
             "optional": True,
         },
     }
     _defaults = {"active": True}
-    _unique_keys = (("entity_class_name", "entity_byname", "alternative_name"),)
+    unique_keys = (("entity_class_name", "entity_byname", "alternative_name"),)
+    corresponding_unique_id_keys = {"entity_class_name": "entity_class_id", "alternative_name": "alternative_id"}
     _references = {
         "entity_id": ("entity", "id"),
         "entity_class_id": ("entity_class", "id"),
         "alternative_id": ("alternative", "id"),
     }
     _external_fields = {
         "entity_class_id": ("entity_id", "class_id"),
@@ -434,15 +446,18 @@
         if list_name is None:
             self["list_value_id"] = None
             return
         try:
             type_ = super().__getitem__(self._type_key)
         except KeyError:
             if isinstance(self, ParameterValueItem):
-                return f"parameter value {self['parameter_definition_name']} for class {self['entity_class_name']}, entity {self['entity_byname']}, alternative {self['alternative_name']} has no list value"
+                return (
+                    f"parameter value {self['parameter_definition_name']} for class {self['entity_class_name']}, "
+                    f"entity {self['entity_byname']}, alternative {self['alternative_name']} has no list value"
+                )
             return f"parameter {self['name']} for class {self['entity_class_name']} has no list value"
         if type_ == "list_value_ref":
             return
         value = super().__getitem__(self._value_key)
         parsed_value = from_database(value, type_)
         if parsed_value is None:
             return
@@ -465,20 +480,23 @@
             "type": str,
             "value": "The parameter value list name if any.",
             "optional": True,
         },
         "description": {"type": str, "value": "The parameter description.", "optional": True},
     }
     _defaults = {"description": None, "default_value": None, "default_type": None, "parameter_value_list_id": None}
-    _unique_keys = (("entity_class_name", "name"),)
-    _references = {"entity_class_id": ("entity_class", "id")}
+    unique_keys = (("entity_class_name", "name"),)
+    corresponding_unique_id_keys = {"entity_class_name": "entity_class_id"}
+    _references = {"entity_class_id": ("entity_class", "id"), "parameter_value_list_id": ("parameter_value_list", "id")}
+    _soft_references = {"parameter_value_list_id"}
     _external_fields = {
         "entity_class_name": ("entity_class_id", "name"),
         "dimension_id_list": ("entity_class_id", "dimension_id_list"),
         "dimension_name_list": ("entity_class_id", "dimension_name_list"),
+        "parameter_value_list_name": ("parameter_value_list_id", "name"),
     }
     _alt_references = {
         ("entity_class_name",): ("entity_class", ("name",)),
         ("parameter_value_list_name",): ("parameter_value_list", ("name",)),
     }
     _internal_fields = {
         "entity_class_id": (("entity_class_name",), "id"),
@@ -537,15 +555,21 @@
             "type": tuple,
             "value": _ENTITY_BYNAME_VALUE,
         },
         "value": {"type": bytes, "value": "The value."},
         "type": {"type": str, "value": "The value type.", "optional": True},
         "alternative_name": {"type": str, "value": "The alternative name - defaults to 'Base'.", "optional": True},
     }
-    _unique_keys = (("entity_class_name", "parameter_definition_name", "entity_byname", "alternative_name"),)
+    unique_keys = (("entity_class_name", "parameter_definition_name", "entity_byname", "alternative_name"),)
+    corresponding_unique_id_keys = {
+        "entity_class_name": "entity_id",
+        "parameter_definition_name": "parameter_definition_id",
+        "entity_byname": "entity_id",
+        "alternative_name": "alternative_id",
+    }
     _references = {
         "entity_class_id": ("entity_class", "id"),
         "parameter_definition_id": ("parameter_definition", "id"),
         "entity_id": ("entity", "id"),
         "alternative_id": ("alternative", "id"),
     }
     _external_fields = {
@@ -598,25 +622,26 @@
             f"value {parsed_value} of {self['parameter_definition_name']} for {self['entity_byname']} "
             f"is not in {list_name}"
         )
 
 
 class ParameterValueListItem(MappedItemBase):
     fields = {"name": {"type": str, "value": "The parameter value list name."}}
-    _unique_keys = (("name",),)
+    unique_keys = (("name",),)
 
 
 class ListValueItem(ParsedValueBase):
     fields = {
         "parameter_value_list_name": {"type": str, "value": "The parameter value list name."},
         "value": {"type": bytes, "value": "The value."},
         "type": {"type": str, "value": "The value type.", "optional": True},
         "index": {"type": int, "value": "The value index.", "optional": True},
     }
-    _unique_keys = (("parameter_value_list_name", "value_and_type"), ("parameter_value_list_name", "index"))
+    unique_keys = (("parameter_value_list_name", "value_and_type"), ("parameter_value_list_name", "index"))
+    corresponding_unique_id_keys = {"parameter_value_list_name": "parameter_value_list_id"}
     _references = {"parameter_value_list_id": ("parameter_value_list", "id")}
     _external_fields = {"parameter_value_list_name": ("parameter_value_list_id", "name")}
     _alt_references = {("parameter_value_list_name",): ("parameter_value_list", ("name",))}
     _internal_fields = {"parameter_value_list_id": (("parameter_value_list_name",), "id")}
 
     @property
     def _value_key(self):
@@ -634,25 +659,25 @@
 
 class AlternativeItem(MappedItemBase):
     fields = {
         "name": {"type": str, "value": "The alternative name."},
         "description": {"type": str, "value": "The alternative description.", "optional": True},
     }
     _defaults = {"description": None}
-    _unique_keys = (("name",),)
+    unique_keys = (("name",),)
 
 
 class ScenarioItem(MappedItemBase):
     fields = {
         "name": {"type": str, "value": "The scenario name."},
         "description": {"type": str, "value": "The scenario description.", "optional": True},
         "active": {"type": bool, "value": "Not in use at the moment.", "optional": True},
     }
     _defaults = {"active": False, "description": None}
-    _unique_keys = (("name",),)
+    unique_keys = (("name",),)
 
     def __getitem__(self, key):
         if key == "alternative_id_list":
             return [x["alternative_id"] for x in self.sorted_scenario_alternatives]
         if key == "alternative_name_list":
             return [x["alternative_name"] for x in self.sorted_scenario_alternatives]
         if key == "sorted_scenario_alternatives":
@@ -670,15 +695,16 @@
 
 class ScenarioAlternativeItem(MappedItemBase):
     fields = {
         "scenario_name": {"type": str, "value": "The scenario name."},
         "alternative_name": {"type": str, "value": "The alternative name."},
         "rank": {"type": int, "value": "The rank - higher has precedence."},
     }
-    _unique_keys = (("scenario_name", "alternative_name"), ("scenario_name", "rank"))
+    unique_keys = (("scenario_name", "alternative_name"), ("scenario_name", "rank"))
+    corresponding_unique_id_keys = {"scenario_name": "scenario_id", "alternative_name": "alternative_id"}
     _references = {"scenario_id": ("scenario", "id"), "alternative_id": ("alternative", "id")}
     _external_fields = {"scenario_name": ("scenario_id", "name"), "alternative_name": ("alternative_id", "name")}
     _alt_references = {("scenario_name",): ("scenario", ("name",)), ("alternative_name",): ("alternative", ("name",))}
     _internal_fields = {"scenario_id": (("scenario_name",), "id"), "alternative_id": (("alternative_name",), "id")}
 
     def __getitem__(self, key):
         # The 'before' is to be interpreted as, this scenario alternative goes *before* the before_alternative.
@@ -697,25 +723,31 @@
 
 
 class MetadataItem(MappedItemBase):
     fields = {
         "name": {"type": str, "value": "The metadata entry name."},
         "value": {"type": str, "value": "The metadata entry value."},
     }
-    _unique_keys = (("name", "value"),)
+    unique_keys = (("name", "value"),)
 
 
 class EntityMetadataItem(MappedItemBase):
     fields = {
         "entity_class_name": {"type": str, "value": "The entity class name."},
         "entity_byname": {"type": tuple, "value": _ENTITY_BYNAME_VALUE},
         "metadata_name": {"type": str, "value": "The metadata entry name."},
         "metadata_value": {"type": str, "value": "The metadata entry value."},
     }
-    _unique_keys = (("entity_class_name", "entity_byname", "metadata_name", "metadata_value"),)
+    unique_keys = (("entity_class_name", "entity_byname", "metadata_name", "metadata_value"),)
+    corresponding_unique_id_keys = {
+        "entity_class_name": "entity_id",
+        "entity_byname": "entity_id",
+        "metadata_name": "metadata_id",
+        "metadata_value": "metadata_id",
+    }
     _references = {
         "entity_id": ("entity", "id"),
         "metadata_id": ("metadata", "id"),
     }
     _external_fields = {
         "entity_class_name": ("entity_id", "entity_class_name"),
         "entity_byname": ("entity_id", "entity_byname"),
@@ -743,24 +775,32 @@
             "type": tuple,
             "value": _ENTITY_BYNAME_VALUE,
         },
         "alternative_name": {"type": str, "value": "The alternative name."},
         "metadata_name": {"type": str, "value": "The metadata entry name."},
         "metadata_value": {"type": str, "value": "The metadata entry value."},
     }
-    _unique_keys = (
+    unique_keys = (
         (
             "entity_class_name",
             "parameter_definition_name",
             "entity_byname",
             "alternative_name",
             "metadata_name",
             "metadata_value",
         ),
     )
+    corresponding_unique_id_keys = {
+        "entity_class_name": "parameter_value_id",
+        "parameter_definition_name": "parameter_value_id",
+        "entity_byname": "parameter_value_id",
+        "alternative_name": "parameter_value_id",
+        "metadata_name": "metadata_id",
+        "metadata_value": "metadata_id",
+    }
     _references = {"parameter_value_id": ("parameter_value", "id"), "metadata_id": ("metadata", "id")}
     _external_fields = {
         "entity_class_name": ("parameter_value_id", "entity_class_name"),
         "parameter_definition_name": ("parameter_value_id", "parameter_definition_name"),
         "entity_byname": ("parameter_value_id", "entity_byname"),
         "alternative_name": ("parameter_value_id", "alternative_name"),
         "metadata_name": ("metadata_id", "name"),
@@ -783,15 +823,16 @@
 
 
 class SuperclassSubclassItem(MappedItemBase):
     fields = {
         "superclass_name": {"type": str, "value": "The superclass name."},
         "subclass_name": {"type": str, "value": "The subclass name."},
     }
-    _unique_keys = (("subclass_name",),)
+    unique_keys = (("subclass_name",),)
+    corresponding_unique_id_keys = {"subclass_name": "subclass_id"}
     _references = {"superclass_id": ("entity_class", "id"), "subclass_id": ("entity_class", "id")}
     _external_fields = {
         "superclass_name": ("superclass_id", "name"),
         "subclass_name": ("subclass_id", "name"),
     }
     _alt_references = {
         ("superclass_name",): ("entity_class", ("name",)),
```

### Comparing `spinedb_api-0.31.1/spinedb_api/mapping.py` & `spinedb_api-0.31.2/spinedb_api/mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/parameter_value.py` & `spinedb_api-0.31.2/spinedb_api/parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -894,15 +894,15 @@
 
     def __setitem__(self, position, index):
         old_index = self.__getitem__(position)
         self.position_lookup[index] = self.position_lookup.pop(old_index, "")
         super().__setitem__(position, index)
 
     def __eq__(self, other):
-        return len(self) == len(other) and np.all(super().__eq__(other))
+        return np.array_equal(self, other)
 
     def __bool__(self):
         return np.size(self) != 0
 
 
 class IndexedValue(ParameterValue):
     """
@@ -1620,14 +1620,20 @@
                 new_values.append(x)
         return Map(list(value.indexes), new_values, index_name=value.index_name)
     if isinstance(value, IndexedValue):
         if not value:
             if isinstance(value, TimeSeries):
                 return Map([], [], DateTime, index_name=TimeSeries.DEFAULT_INDEX_NAME)
             return Map([], [], str)
+        if isinstance(value, TimeSeries):
+            return Map(
+                [DateTime(t) for t in np.datetime_as_string(value.indexes)],
+                list(value.values),
+                index_name=value.index_name,
+            )
         return Map(list(value.indexes), list(value.values), index_name=value.index_name)
     return value
 
 
 def convert_map_to_table(map_, make_square=True, row_this_far=None, empty=None):
     """
     Converts :class:`Map` into list of rows recursively.
```

### Comparing `spinedb_api-0.31.1/spinedb_api/perfect_split.py` & `spinedb_api-0.31.2/spinedb_api/perfect_split.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/purge.py` & `spinedb_api-0.31.2/spinedb_api/purge.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/query.py` & `spinedb_api-0.31.2/spinedb_api/query.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/server_client_helpers.py` & `spinedb_api-0.31.2/spinedb_api/server_client_helpers.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_db_client.py` & `spinedb_api-0.31.2/spinedb_api/spine_db_client.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_db_server.py` & `spinedb_api-0.31.2/spinedb_api/spine_db_server.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/__init__.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/__init__.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/csv_writer.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/exporters/csv_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/exporters/excel.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel_writer.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/exporters/excel_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/gdx_writer.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/exporters/gdx_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 # Spine Database API is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-"""
-Module contains a .gdx writer implementation.
-
-"""
+""" Module contains a .gdx writer implementation. """
 import math
 from gdx2py import GAMSSet, GAMSScalar, GAMSParameter, GdxFile
 from gdx2py.gdxfile import EPS_VALUE
 import gdxcc
 from .writer import Writer, WriterException
 
 
-SPECIAL_CONVERSIONS = {EPS_VALUE: gdxcc.GMS_SV_EPS, math.inf: gdxcc.GMS_SV_PINF, -math.inf: gdxcc.GMS_SV_MINF}
+SPECIAL_CONVERSIONS = {
+    EPS_VALUE: gdxcc.GMS_SV_EPS,
+    1e-10: gdxcc.GMS_SV_EPS,
+    math.inf: gdxcc.GMS_SV_PINF,
+    -math.inf: gdxcc.GMS_SV_MINF,
+}
 
 
 class GdxWriter(Writer):
     def __init__(self, file_path, gams_directory):
         """
         Args:
             file_path (str): path ot output file
@@ -123,17 +125,19 @@
         raise e
 
 
 def _convert_to_gams(x):
     """Converts special float values to corresponding GAMS constants, otherwise returns x as is.
 
     Args:
-        x (float): value to convert
+        x (float or Any): value to convert
 
     Returns:
-        float: converted value
+        float or Any: converted value
     """
     if not isinstance(x, float):
+        if x == "EPS":
+            return gdxcc.GMS_SV_EPS
         return x
     if math.isnan(x):
         return gdxcc.GMS_SV_UNDEF
     return SPECIAL_CONVERSIONS.get(x, x)
```

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/sql_writer.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/exporters/sql_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/writer.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/exporters/writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/gdx_utils.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/gdx_utils.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/__init__.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/csv_reader.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/datapackage_reader.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/datapackage_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/excel_reader.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/excel_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/gdx_connector.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/gdx_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/json_reader.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/json_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/reader.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/spine_io/importers/sqlalchemy_connector.py` & `spinedb_api-0.31.2/spinedb_api/spine_io/importers/sqlalchemy_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api/temp_id.py` & `spinedb_api-0.31.2/spinedb_api/temp_id.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/spinedb_api.egg-info/PKG-INFO` & `spinedb_api-0.31.2/spinedb_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: spinedb_api
-Version: 0.31.1
+Version: 0.31.2
 Summary: An API to talk to Spine databases.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/Spine-Database-API
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 Requires-Dist: sqlalchemy<1.4,>=1.3
 Requires-Dist: alembic>=1.7
-Requires-Dist: faker>=8.1.2
 Requires-Dist: datapackage>=1.15.2
 Requires-Dist: python-dateutil>=2.8.1
 Requires-Dist: numpy>=1.20.2
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: openpyxl!=3.1.1,>=3.0.7
 Requires-Dist: gdx2py>=2.1.1
 Requires-Dist: ijson>=3.1.4
 Requires-Dist: chardet>=4.0.0
 Requires-Dist: pymysql>=1.0.2
 Requires-Dist: psycopg2
-Provides-Extra: dev
-Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: pyperf; extra == "dev"
 
 # Spine Database API
 
 [![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
 [![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
 [![codecov](https://codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Database-API)
 [![PyPI version](https://badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api)
@@ -64,29 +60,27 @@
 
     $ pip install --upgrade git+https://github.com/spine-tools/Spine-Database-API.git
 
 
 ## Building the documentation
 
 Source files for the documentation can be found in `docs/source` directory. In order to 
-build the HTML docs, you need to install the additional documentation building requirements
+build the HTML docs, you need to install the developer dependencies
 by running:
 
-    $ pip install -r dev-requirements.txt 
+    $ pip install -r dev-requirements.txt
 
 This installs Sphinx (among other things), which is required in building the documentation.
 When Sphinx is installed, you can build the HTML pages from the source files by running:
 
-    > docs\make.bat html
+    > bin\build_doc.bat
     
 or
 
-    $ pushd docs
-    $ make html
-    $ popd
+    $ bin/build_doc.py
     
 depending on your operating system.        
  
 After running the build, the index page can be found in `docs/build/html/index.html`.
 
 &nbsp;
 <hr>
```

#### html2text {}

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.1 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.2 Summary: An API to talk
 to Spine databases. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/Spine-Database-API Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.8.1 Description-Content-Type: text/markdown License-File: COPYING
 License-File: COPYING.LESSER Requires-Dist: sqlalchemy<1.4,>=1.3 Requires-Dist:
-alembic>=1.7 Requires-Dist: faker>=8.1.2 Requires-Dist: datapackage>=1.15.2
-Requires-Dist: python-dateutil>=2.8.1 Requires-Dist: numpy>=1.20.2 Requires-
-Dist: scipy>=1.7.1 Requires-Dist: openpyxl!=3.1.1,>=3.0.7 Requires-Dist:
-gdx2py>=2.1.1 Requires-Dist: ijson>=3.1.4 Requires-Dist: chardet>=4.0.0
-Requires-Dist: pymysql>=1.0.2 Requires-Dist: psycopg2 Provides-Extra: dev
-Requires-Dist: coverage[toml]; extra == "dev" Requires-Dist: pyperf; extra ==
-"dev" # Spine Database API [![Documentation Status](https://readthedocs.org/
-projects/spine-database-api/badge/?version=latest)](https://spine-database-
-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests](https://github.com/
-spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://
-github.com/spine-tools/Spine-Database-API/
+alembic>=1.7 Requires-Dist: datapackage>=1.15.2 Requires-Dist: python-
+dateutil>=2.8.1 Requires-Dist: numpy>=1.20.2 Requires-Dist: scipy>=1.7.1
+Requires-Dist: openpyxl!=3.1.1,>=3.0.7 Requires-Dist: gdx2py>=2.1.1 Requires-
+Dist: ijson>=3.1.4 Requires-Dist: chardet>=4.0.0 Requires-Dist: pymysql>=1.0.2
+Requires-Dist: psycopg2 # Spine Database API [![Documentation Status](https://
+readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://
+spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests]
+(https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/
+badge.svg)](https://github.com/spine-tools/Spine-Database-API/
 actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
 tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/
 spine-tools/Spine-Database-API) [![PyPI version](https://badge.fury.io/py/
 spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A Python package to
 access and manipulate Spine databases in a customary, unified way. ## License
 Spine Database API is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
@@ -29,20 +27,20 @@
 install the package run: $ pip install spinedb_api To upgrade to the most
 recent version, run: $ pip install --upgrade spinedb_api You can also specify a
 branch, or a tag, for instance: $ pip install spinedb_api==0.12.1 To install
 the latest development version use the Git repository url: $ pip install --
 upgrade git+https://github.com/spine-tools/Spine-Database-API.git ## Building
 the documentation Source files for the documentation can be found in `docs/
 source` directory. In order to build the HTML docs, you need to install the
-additional documentation building requirements by running: $ pip install -
-r dev-requirements.txt This installs Sphinx (among other things), which is
-required in building the documentation. When Sphinx is installed, you can build
-the HTML pages from the source files by running: > docs\make.bat html or $
-pushd docs $ make html $ popd depending on your operating system. After running
-the build, the index page can be found in `docs/build/html/index.html`.  
+developer dependencies by running: $ pip install -r dev-requirements.txt This
+installs Sphinx (among other things), which is required in building the
+documentation. When Sphinx is installed, you can build the HTML pages from the
+source files by running: > bin\build_doc.bat or $ bin/build_doc.py depending on
+your operating system. After running the build, the index page can be found in
+`docs/build/html/index.html`.  
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spinedb_api-0.31.1/spinedb_api.egg-info/SOURCES.txt` & `spinedb_api-0.31.2/spinedb_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 .readthedocs.yml
 CHANGELOG.md
 COPYING
 COPYING.LESSER
 MANIFEST.in
 README.md
 deploy-key.enc
+dev-requirements.txt
 pylintrc
 pyproject.toml
-requirements.txt
 .github/pull_request_template.md
 .github/workflows/run_unit_tests.yml
 benchmarks/README.md
 benchmarks/__init__.py
 benchmarks/datetime_from_database.py
+benchmarks/entity_class_mapping_import_row.py
 benchmarks/map_from_database.py
 benchmarks/mapped_item_getitem.py
 benchmarks/update_default_value_to_different_value.py
 benchmarks/update_default_value_to_same_value.py
 benchmarks/utils.py
 bin/build_doc.bat
 bin/build_doc.py
 docs/Makefile
 docs/make.bat
-docs/requirements.txt
 docs/source/conf.py
 docs/source/front_matter.rst
 docs/source/index.rst
 docs/source/metadata.rst
 docs/source/parameter_value_format.rst
 docs/source/tutorial.rst
 docs/source/img/spinetoolbox_on_wht.svg
@@ -119,14 +119,15 @@
 spinedb_api/spine_io/importers/excel_reader.py
 spinedb_api/spine_io/importers/gdx_connector.py
 spinedb_api/spine_io/importers/json_reader.py
 spinedb_api/spine_io/importers/reader.py
 spinedb_api/spine_io/importers/sqlalchemy_connector.py
 tests/__init__.py
 tests/custom_db_mapping.py
+tests/mock_helpers.py
 tests/test_DatabaseMapping.py
 tests/test_check_integrity.py
 tests/test_db_mapping_base.py
 tests/test_db_server.py
 tests/test_export_functions.py
 tests/test_helpers.py
 tests/test_import_functions.py
```

### Comparing `spinedb_api-0.31.1/tests/__init__.py` & `spinedb_api-0.31.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/custom_db_mapping.py` & `spinedb_api-0.31.2/tests/custom_db_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Unit tests for DatabaseMapping class.
-
-"""
-from spinedb_api import DatabaseMapping, SpineIntegrityError
+""" Unit tests for DatabaseMapping class. """
+from spinedb_api import DatabaseMapping
 
 
 class CustomDatabaseMapping(DatabaseMapping):
     def add_object_classes(self, *items, **kwargs):
         return self.add_items("object_class", *items, **kwargs)
 
     def add_objects(self, *items, **kwargs):
```

### Comparing `spinedb_api-0.31.1/tests/export_mapping/__init__.py` & `spinedb_api-0.31.2/tests/export_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/export_mapping/test_export_mapping.py` & `spinedb_api-0.31.2/tests/export_mapping/test_export_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/export_mapping/test_pivot.py` & `spinedb_api-0.31.2/tests/export_mapping/test_pivot.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/export_mapping/test_settings.py` & `spinedb_api-0.31.2/tests/export_mapping/test_settings.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/__init__.py` & `spinedb_api-0.31.2/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/test_alternative_filter.py` & `spinedb_api-0.31.2/tests/filters/test_alternative_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/test_execution_filter.py` & `spinedb_api-0.31.2/tests/filters/test_execution_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/test_renamer.py` & `spinedb_api-0.31.2/tests/filters/test_renamer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/test_scenario_filter.py` & `spinedb_api-0.31.2/tests/filters/test_scenario_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/test_tool_filter.py` & `spinedb_api-0.31.2/tests/filters/test_tool_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/test_tools.py` & `spinedb_api-0.31.2/tests/filters/test_tools.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/filters/test_value_transformer.py` & `spinedb_api-0.31.2/tests/filters/test_value_transformer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/import_mapping/__init__.py` & `spinedb_api-0.31.2/tests/import_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/import_mapping/test_generator.py` & `spinedb_api-0.31.2/tests/import_mapping/test_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Contains unit tests for the generator module.
-
-"""
+""" Contains unit tests for the generator module. """
 import unittest
 
 from spinedb_api import Array, Map
 from spinedb_api.import_mapping.generator import get_mapped_data
 from spinedb_api.import_mapping.type_conversion import value_to_convert_spec
 
 
@@ -509,10 +506,40 @@
                 "parameter_definitions": [("unit__node__node", "flow")],
                 "parameter_values": [
                     ["unit__node__node", ("Dyson sphere", "Gamma Ceti", "Ring world"), "flow", 23.3, "Base"]
                 ],
             },
         )
 
+    def test_importing_empty_rows_does_unnecessarily_not_repeat_mapped_data(self):
+        header = ["Generator", "HydroGenerator"]
+        data_source = iter(
+            [["MyHydroGenerator", "MyHydroGenerator"], ["NonHydroGenerator", None], ["OtherGenerator", None]]
+        )
+        mappings = [
+            [
+                {"map_type": "EntityClass", "position": "header", "value": 0},
+                {"map_type": "Entity", "position": 1},
+                {"map_type": "EntityMetadata", "position": "hidden"},
+                {"map_type": "ParameterDefinition", "position": "hidden", "value": "Type"},
+                {"map_type": "Alternative", "position": "hidden"},
+                {"map_type": "ParameterValueMetadata", "position": "hidden"},
+                {"map_type": "ParameterValue", "position": "hidden", "value": "Hydro"},
+            ]
+        ]
+        convert_function_specs = {0: "string", 1: "string"}
+        convert_functions = {column: value_to_convert_spec(spec) for column, spec in convert_function_specs.items()}
+        mapped_data, errors = get_mapped_data(data_source, mappings, header, column_convert_fns=convert_functions)
+        self.assertEqual(errors, [])
+        self.assertEqual(
+            mapped_data,
+            {
+                "entities": [("Generator", "MyHydroGenerator")],
+                "entity_classes": [("Generator",)],
+                "parameter_definitions": [("Generator", "Type")],
+                "parameter_values": [["Generator", "MyHydroGenerator", "Type", "Hydro"]],
+            },
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `spinedb_api-0.31.1/tests/import_mapping/test_import_mapping.py` & `spinedb_api-0.31.2/tests/import_mapping/test_import_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/import_mapping/test_type_conversion.py` & `spinedb_api-0.31.2/tests/import_mapping/test_type_conversion.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/__init__.py` & `spinedb_api-0.31.2/tests/spine_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/exporters/__init__.py` & `spinedb_api-0.31.2/tests/spine_io/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/exporters/test_csv_writer.py` & `spinedb_api-0.31.2/tests/spine_io/exporters/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/exporters/test_excel_writer.py` & `spinedb_api-0.31.2/tests/spine_io/exporters/test_excel_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/exporters/test_gdx_writer.py` & `spinedb_api-0.31.2/tests/spine_io/exporters/test_gdx_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -272,21 +272,33 @@
         db_map.close()
 
     @unittest.skipIf(_gams_dir is None, "No working GAMS installation found.")
     def test_special_value_conversions(self):
         db_map = DatabaseMapping("sqlite://", create=True)
         import_object_classes(db_map, ("oc",))
         import_object_parameters(
-            db_map, (("oc", "epsilon"), ("oc", "infinity"), ("oc", "negative_infinity"), ("oc", "nan"))
+            db_map,
+            (
+                ("oc", "epsilon1"),
+                ("oc", "epsilon2"),
+                ("oc", "epsilon3"),
+                ("oc", "epsilon4"),
+                ("oc", "infinity"),
+                ("oc", "negative_infinity"),
+                ("oc", "nan"),
+            ),
         )
         import_objects(db_map, (("oc", "o1"),))
         import_object_parameter_values(
             db_map,
             (
-                ("oc", "o1", "epsilon", sys.float_info.min),
+                ("oc", "o1", "epsilon1", sys.float_info.min),
+                ("oc", "o1", "epsilon2", 2.2250738585072014e-308),
+                ("oc", "o1", "epsilon3", 1e-10),
+                ("oc", "o1", "epsilon4", "EPS"),
                 ("oc", "o1", "infinity", math.inf),
                 ("oc", "o1", "negative_infinity", -math.inf),
                 ("oc", "o1", "nan", math.nan),
             ),
         )
         db_map.commit_session("Add test data.")
         root_mapping = entity_parameter_value_export(
@@ -297,16 +309,19 @@
         with TemporaryDirectory() as temp_dir:
             file_path = Path(temp_dir, "test_special_value_conversions.gdx")
             writer = GdxWriter(str(file_path), self._gams_dir)
             write(db_map, writer, root_mapping)
             with GdxFile(str(file_path), "r", self._gams_dir) as gdx_file:
                 self.assertEqual(len(gdx_file), 1)
                 gams_parameter = gdx_file["oc"]
-                self.assertEqual(len(gams_parameter), 4)
-                self.assertEqual(gams_parameter[("o1", "epsilon")], sys.float_info.min)
+                self.assertEqual(len(gams_parameter), 7)
+                self.assertEqual(gams_parameter[("o1", "epsilon1")], sys.float_info.min)
+                self.assertEqual(gams_parameter[("o1", "epsilon2")], sys.float_info.min)
+                self.assertEqual(gams_parameter[("o1", "epsilon3")], sys.float_info.min)
+                self.assertEqual(gams_parameter[("o1", "epsilon4")], sys.float_info.min)
                 self.assertEqual(gams_parameter[("o1", "infinity")], math.inf)
                 self.assertEqual(gams_parameter[("o1", "negative_infinity")], -math.inf)
                 self.assertTrue(math.isnan(gams_parameter[("o1", "nan")]))
         db_map.close()
 
 
 if __name__ == "__main__":
```

### Comparing `spinedb_api-0.31.1/tests/spine_io/exporters/test_sql_writer.py` & `spinedb_api-0.31.2/tests/spine_io/exporters/test_sql_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/exporters/test_writer.py` & `spinedb_api-0.31.2/tests/spine_io/exporters/test_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/__init__.py` & `spinedb_api-0.31.2/tests/spine_io/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/test_CSVConnector.py` & `spinedb_api-0.31.2/tests/spine_io/importers/test_CSVConnector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/test_GdxConnector.py` & `spinedb_api-0.31.2/tests/spine_io/importers/test_GdxConnector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/test_datapackage_reader.py` & `spinedb_api-0.31.2/tests/spine_io/importers/test_datapackage_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/test_excel_reader.py` & `spinedb_api-0.31.2/tests/spine_io/importers/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/test_json_reader.py` & `spinedb_api-0.31.2/tests/spine_io/importers/test_json_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/test_reader.py` & `spinedb_api-0.31.2/tests/spine_io/importers/test_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/importers/test_sqlalchemy_connector.py` & `spinedb_api-0.31.2/tests/spine_io/importers/test_sqlalchemy_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/spine_io/test_excel_integration.py` & `spinedb_api-0.31.2/tests/spine_io/test_excel_integration.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_DatabaseMapping.py` & `spinedb_api-0.31.2/tests/test_DatabaseMapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,18 @@
     DatabaseMapping,
     import_functions,
     from_database,
     to_database,
     SpineDBAPIError,
     SpineIntegrityError,
 )
+from spinedb_api.db_mapping_base import PublicItem, Status
 from spinedb_api.helpers import Asterisk, name_from_elements
 from tests.custom_db_mapping import CustomDatabaseMapping
+from tests.mock_helpers import AssertSuccessTestCase
 
 
 def create_query_wrapper(db_map):
     def query_wrapper(*args, orig_query=db_map.query, **kwargs):
         arg = args[0]
         if isinstance(arg, mock.Mock):
             return arg.value
@@ -81,21 +83,14 @@
                 db_map = CustomDatabaseMapping(url)
             except:
                 self.fail("CustomDatabaseMapping.__init__() should not raise.")
             else:
                 db_map.close()
 
 
-class AssertSuccessTestCase(unittest.TestCase):
-    def _assert_success(self, result):
-        item, error = result
-        self.assertIsNone(error)
-        return item
-
-
 class TestDatabaseMapping(AssertSuccessTestCase):
     def test_active_by_default_is_initially_true_for_zero_dimensional_entity_class(self):
         with DatabaseMapping("sqlite://", create=True) as db_map:
             item = self._assert_success(db_map.add_entity_class_item(name="Entity"))
             self.assertTrue(item["active_by_default"])
 
     def test_active_by_default_is_initially_false_for_multi_dimensional_entity_class(self):
@@ -854,14 +849,215 @@
                     entity_class_name="Object",
                     entity_byname=("knife",),
                     parameter_definition_name="x",
                     alternative_name="extra alternative",
                 )
                 self.assertEqual(value, {})
 
+    def test_add_entity_class_by_dimension_names(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            self._assert_success(db_map.add_entity_class_item(name="Fish"))
+            self._assert_success(db_map.add_entity_class_item(name="Cat"))
+            entity_class = self._assert_success(db_map.add_entity_class_item(dimension_name_list=("Fish", "Cat")))
+            self.assertEqual(entity_class["name"], "Fish__Cat")
+
+    def test_add_entity_by_element_names(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            self._assert_success(db_map.add_entity_class_item(name="Fish"))
+            self._assert_success(db_map.add_entity_item(name="Nemo", entity_class_name="Fish"))
+            self._assert_success(db_map.add_entity_class_item(name="Cat"))
+            self._assert_success(db_map.add_entity_item(name="Jerry", entity_class_name="Cat"))
+            relation = self._assert_success(db_map.add_entity_class_item(dimension_name_list=("Fish", "Cat")))
+            entity = self._assert_success(
+                db_map.add_entity_item(entity_class_name=relation["name"], element_name_list=("Nemo", "Jerry"))
+            )
+            self.assertEqual(entity["name"], "Nemo__Jerry")
+
+    def test_add_alternative_without_name_gives_error(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            item, error = db_map.add_alternative_item()
+            self.assertEqual(error, "missing values for unique keys ['name']")
+            self.assertIsNone(item)
+
+    def test_byname_versus_element_name_list(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            self._assert_success(db_map.add_entity_class_item(name="unit"))
+            self._assert_success(db_map.add_entity_class_item(name="node"))
+            unit_node = self._assert_success(db_map.add_entity_class_item(dimension_name_list=("unit", "node")))
+            unit_node_unit_node = self._assert_success(
+                db_map.add_entity_class_item(dimension_name_list=(unit_node["name"], unit_node["name"]))
+            )
+            self._assert_success(db_map.add_entity_item(name="U", entity_class_name="unit"))
+            self._assert_success(db_map.add_entity_item(name="N", entity_class_name="node"))
+            u_n = self._assert_success(
+                db_map.add_entity_item(element_name_list=("U", "N"), entity_class_name=unit_node["name"])
+            )
+            u_n_u_n = self._assert_success(
+                db_map.add_entity_item(
+                    element_name_list=(u_n["name"], u_n["name"]), entity_class_name=unit_node_unit_node["name"]
+                )
+            )
+            self.assertEqual(u_n_u_n["element_name_list"], ("U__N", "U__N"))
+            self.assertEqual(u_n_u_n["entity_byname"], ("U", "N", "U", "N"))
+
+    def test_get_parameter_definition_item_has_value_list_name(self):
+        with TemporaryDirectory() as temp_dir:
+            url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
+            with DatabaseMapping(url, create=True) as db_map:
+                self._assert_success(db_map.add_parameter_value_list_item(name="Values"))
+                self._assert_success(db_map.add_entity_class_item(name="Object"))
+                definition_item = self._assert_success(
+                    db_map.add_parameter_definition_item(
+                        name="x", entity_class_name="Object", parameter_value_list_name="Values"
+                    )
+                )
+                self.assertIn("parameter_value_list_name", definition_item)
+                self.assertEqual(definition_item["parameter_value_list_name"], "Values")
+                db_map.commit_session("Add test data.")
+            with DatabaseMapping(url) as db_map:
+                definition_item = db_map.get_parameter_definition_item(name="x", entity_class_name="Object")
+                self.assertIn("parameter_value_list_name", definition_item)
+                self.assertEqual(definition_item["parameter_value_list_name"], "Values")
+
+    def test_get_parameter_definition_item_without_value_list_(self):
+        with TemporaryDirectory() as temp_dir:
+            url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
+            with DatabaseMapping(url, create=True) as db_map:
+                self._assert_success(db_map.add_entity_class_item(name="Object"))
+                definition_item = self._assert_success(
+                    db_map.add_parameter_definition_item(name="x", entity_class_name="Object")
+                )
+                self.assertIsNone(definition_item["parameter_value_list_name"])
+                db_map.commit_session("Add test data.")
+            with DatabaseMapping(url) as db_map:
+                definition_item = db_map.get_parameter_definition_item(name="x", entity_class_name="Object")
+                self.assertIsNone(definition_item["parameter_value_list_name"])
+
+    def test_get_non_existent_parameter_definition_item_without_value_list_returns_empty_dict(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            definition_item = db_map.get_parameter_definition_item(
+                name="x", entity_class_name="Object", parameter_value_list_name=None
+            )
+            self.assertEqual(definition_item, {})
+
+    def test_remove_parameter_value_list_removes_parameter_definition(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            list_item = self._assert_success(db_map.add_parameter_value_list_item(name="Values"))
+            self._assert_success(db_map.add_entity_class_item(name="Object"))
+            definition_item = self._assert_success(
+                db_map.add_parameter_definition_item(
+                    name="x", entity_class_name="Object", parameter_value_list_name="Values"
+                )
+            )
+            list_item.remove()
+            self.assertFalse(definition_item.is_valid())
+
+    def test_adding_scenario_with_same_name_as_previously_removed_one(self):
+        with TemporaryDirectory() as temp_dir:
+            url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
+            with DatabaseMapping(url, create=True) as db_map:
+                scenario = self._assert_success(db_map.add_scenario_item(name="high lows"))
+                db_map.commit_session("Add 'high lows' scenario")
+                self._assert_success(scenario.remove())
+                self._assert_success(db_map.add_scenario_item(name="high lows", description="Readded scenario"))
+                db_map.commit_session("Readd 'high lows' scenario")
+            with DatabaseMapping(url) as db_map:
+                scenario = db_map.get_scenario_item(name="high lows")
+                self.assertNotEqual(scenario, {})
+                self.assertEqual(scenario["name"], "high lows")
+                self.assertEqual(scenario["description"], "Readded scenario")
+
+    def test_restoring_original_item_fails_after_it_has_been_removed_and_replaced(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            scenario = self._assert_success(db_map.add_scenario_item(name="high lows"))
+            scenario.remove()
+            self._assert_success(db_map.add_scenario_item(name="high lows"))
+            self.assertEqual(
+                scenario.restore(),
+                (None, "restoring would create a conflict with another item with same unique values"),
+            )
+
+    def test_restoring_original_item_succeeds_after_readded_item_has_been_removed(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            original_scenario = self._assert_success(db_map.add_scenario_item(name="high lows"))
+            original_scenario.remove()
+            readded_scenario = self._assert_success(db_map.add_scenario_item(name="high lows"))
+            readded_scenario.remove()
+            self.assertIsNotNone(original_scenario.restore())
+
+    def test_restoring_original_item_restores_referrers_after_readded_item_has_been_removed(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            original_scenario = self._assert_success(db_map.add_scenario_item(name="high lows"))
+            scenario_alternative = self._assert_success(
+                db_map.add_scenario_alternative_item(scenario_name="high lows", alternative_name="Base")
+            )
+            original_scenario.remove()
+            self.assertFalse(scenario_alternative.is_valid())
+            readded_scenario = self._assert_success(db_map.add_scenario_item(name="high lows"))
+            readded_scenario.remove()
+            self.assertIsNotNone(original_scenario.restore())
+            self.assertTrue(scenario_alternative.is_valid)
+
+    def test_shuffle_scenario_alternatives(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            scenario = self._assert_success(db_map.add_scenario_item(name="scenario"))
+            base = db_map.get_alternative_item(name="Base")
+            next_level = self._assert_success(db_map.add_alternative_item(name="Next level"))
+            scenario_alternative_1 = self._assert_success(
+                db_map.add_scenario_alternative_item(scenario_id=scenario["id"], alternative_id=base["id"], rank=1)
+            )
+            scenario_alternative_2 = self._assert_success(
+                db_map.add_scenario_alternative_item(
+                    scenario_id=scenario["id"], alternative_id=next_level["id"], rank=2
+                )
+            )
+            removed, error = db_map.remove_item("scenario_alternative", scenario_alternative_2["id"])
+            self.assertIsNone(error)
+            self.assertIsInstance(removed, PublicItem)
+            removed, error = db_map.remove_item("scenario_alternative", scenario_alternative_1["id"])
+            self.assertIsNone(error)
+            self.assertIsInstance(removed, PublicItem)
+            scenario_alternative_3 = self._assert_success(
+                db_map.add_scenario_alternative_item(
+                    scenario_id=scenario["id"], alternative_id=next_level["id"], rank=1
+                )
+            )
+            scenario_alternative_4 = self._assert_success(
+                db_map.add_scenario_alternative_item(scenario_id=scenario["id"], alternative_id=base["id"], rank=2)
+            )
+            removed, error = db_map.remove_item("scenario_alternative", scenario_alternative_4["id"])
+            self.assertIsNone(
+                error,
+            )
+            self.assertIsInstance(removed, PublicItem)
+            removed, error = db_map.remove_item("scenario_alternative", scenario_alternative_3["id"])
+            self.assertIsNone(error)
+            self.assertIsInstance(removed, PublicItem)
+
+    def test_get_items_with_skip_removed(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            alternative = db_map.get_alternative_item(name="Base")
+            self._assert_success(alternative.remove())
+            alternatives = db_map.get_items("alternative", skip_removed=False)
+            self.assertEqual(len(alternatives), 1)
+            self.assertEqual(alternatives[0]["name"], "Base")
+            self.assertFalse(alternatives[0].is_valid())
+
+    def test_get_items_with_skip_removed_after_readding_item(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            alternative = db_map.get_alternative_item(name="Base")
+            self._assert_success(alternative.remove())
+            self._assert_success(db_map.add_alternative_item(name="Base"))
+            alternatives = db_map.get_items("alternative", skip_removed=False)
+            self.assertEqual(len(alternatives), 2)
+            self.assertEqual(alternatives[0]["name"], "Base")
+            self.assertFalse(alternatives[0].is_valid())
+            self.assertEqual(alternatives[1]["name"], "Base")
+            self.assertTrue(alternatives[1].is_valid())
+
 
 class TestDatabaseMappingLegacy(unittest.TestCase):
     """'Backward compatibility' tests, i.e. pre-entity tests converted to work with the entity structure."""
 
     _db_map = None
 
     @classmethod
@@ -3153,71 +3349,71 @@
 
     def _do_test_concurrent_commit(self, make_concurrent):
         def _commit_on_thread(db_map, msg):
             db_map.commit_session(msg)
 
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "database.sqlite")
-            with CustomDatabaseMapping(url, create=True) as db_map1:
-                with CustomDatabaseMapping(url) as db_map2:
-                    db_map1.add_entity_class_item(name="dog")
-                    db_map1.add_entity_class_item(name="cat")
-                    db_map2.add_entity_class_item(name="cat")
+            with DatabaseMapping(url, create=True) as db_map1:
+                with DatabaseMapping(url) as db_map2:
+                    self._assert_success(db_map1.add_entity_class_item(name="dog"))
+                    self._assert_success(db_map1.add_entity_class_item(name="cat"))
+                    self._assert_success(db_map2.add_entity_class_item(name="cat"))
                     c1 = make_concurrent(target=_commit_on_thread, args=(db_map1, "one"))
                     c2 = make_concurrent(target=_commit_on_thread, args=(db_map2, "two"))
                     c2.start()
                     c1.start()
                     c1.join()
                     c2.join()
-            with CustomDatabaseMapping(url) as db_map:
+            with DatabaseMapping(url) as db_map:
                 commit_msgs = {x["comment"] for x in db_map.query(db_map.commit_sq)}
                 entity_class_names = [x["name"] for x in db_map.query(db_map.entity_class_sq)]
                 self.assertEqual(commit_msgs, {"Create the database", "one", "two"})
                 self.assertEqual(len(entity_class_names), 2)
                 self.assertEqual(set(entity_class_names), {"cat", "dog"})
 
     def test_uncommitted_mapped_items_take_id_from_externally_committed_items(self):
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "database.sqlite")
-            with CustomDatabaseMapping(url, create=True) as db_map1:
-                db_map1.add_entity_class_item(name="widget")
-                db_map1.add_entity_class_item(name="gadget")
-                with CustomDatabaseMapping(url) as db_map2:
+            with DatabaseMapping(url, create=True) as db_map1:
+                self._assert_success(db_map1.add_entity_class_item(name="widget"))
+                self._assert_success(db_map1.add_entity_class_item(name="gadget"))
+                with DatabaseMapping(url) as db_map2:
                     # Add the same classes in different order
-                    db_map2.add_entity_class_item(name="gadget")
-                    db_map2.add_entity_class_item(name="widget")
+                    self._assert_success(db_map2.add_entity_class_item(name="gadget"))
+                    self._assert_success(db_map2.add_entity_class_item(name="widget"))
                     db_map2.commit_session("No comment")
                     committed_resolved_entity_classes = [x.resolve() for x in db_map2.get_items("entity_class")]
                     committed_resolved_id_by_name = {x["name"]: x["id"] for x in committed_resolved_entity_classes}
                 # Verify that the uncommitted classes are now seen as 'committed'
                 uncommitted_entity_classes = db_map1.get_items("entity_class")
                 uncommitted_resolved_entity_classes = [x.resolve() for x in uncommitted_entity_classes]
                 uncommitted_resolved_id_by_name = {x["name"]: x["id"] for x in uncommitted_resolved_entity_classes}
                 self.assertEqual(committed_resolved_id_by_name, uncommitted_resolved_id_by_name)
                 for mapped_item in uncommitted_entity_classes:
-                    self.assertTrue(mapped_item.is_committed())
-                with self.assertRaises(SpineDBAPIError):
-                    db_map1.commit_session("No comment")
+                    self.assertFalse(mapped_item.is_committed())
+                    self.assertEqual(mapped_item._mapped_item.status, Status.to_update)
+                db_map1.commit_session("Update classes already in database.")
 
     def test_committed_mapped_items_take_id_from_externally_committed_items(self):
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "database.sqlite")
-            with CustomDatabaseMapping(url, create=True) as db_map0:
+            with DatabaseMapping(url, create=True) as db_map0:
                 # Add widget before gadget
-                db_map0.add_entity_class_item(name="widget")
-                db_map0.add_entity_class_item(name="gadget")
+                self._assert_success(db_map0.add_entity_class_item(name="widget"))
+                self._assert_success(db_map0.add_entity_class_item(name="gadget"))
                 db_map0.commit_session("No comment")
-            with CustomDatabaseMapping(url) as db_map1:
-                with CustomDatabaseMapping(url) as db_map2:
+            with DatabaseMapping(url) as db_map1:
+                with DatabaseMapping(url) as db_map2:
                     # Purge, then add *gadget* before *widget* (swap the order)
                     # Also add an entity
                     db_map2.purge_items("entity_class")
-                    db_map2.add_entity_class_item(name="gadget")
-                    db_map2.add_entity_class_item(name="widget")
-                    db_map2.add_entity_item(entity_class_name="gadget", name="phone")
+                    self._assert_success(db_map2.add_entity_class_item(name="gadget"))
+                    self._assert_success(db_map2.add_entity_class_item(name="widget"))
+                    self._assert_success(db_map2.add_entity_item(entity_class_name="gadget", name="phone"))
                     db_map2.commit_session("No comment")
                 # Check that we see the entity added by the other mapping
                 phone = db_map1.get_entity_item(entity_class_name="gadget", name="phone")
                 self.assertIsNotNone(phone)
 
     def test_fetching_entities_after_external_change_has_renamed_their_classes(self):
         with TemporaryDirectory() as temp_dir:
@@ -3286,15 +3482,16 @@
                     shadow_db_map.commit_session("Add entity with different name, probably reusing previous id.")
                 # db_map.refresh_session()
                 items = db_map.fetch_more("entity")
                 self.assertEqual(len(items), 1)
                 self.assertEqual(items[0]["name"], "other_entity")
                 all_items = db_map.get_entity_items()
                 self.assertEqual(len(all_items), 1)
-                restored_item = db_map.restore_item("entity", original_id)
+                restored_item, error = db_map.restore_item("entity", original_id)
+                self.assertEqual(error, "")
                 self.assertEqual(restored_item["name"], "my_entity")
                 all_items = db_map.get_entity_items()
                 self.assertEqual(len(all_items), 2)
 
     def test_cunning_ways_to_make_external_changes(self):
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
@@ -3619,15 +3816,15 @@
 
     def test_db_items_prevail_if_mapped_items_are_committed(self):
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
             with DatabaseMapping(url, create=True) as db_map:
                 self._assert_success(db_map.add_entity_class_item(name="my_class"))
                 db_map.commit_session("Add some data")
-            with DatabaseMapping(url, create=True) as db_map:
+            with DatabaseMapping(url) as db_map:
                 db_map.purge_items("entity_class")
                 db_map.commit_session("Purge all")
                 with DatabaseMapping(url) as shadow_db_map:
                     self._assert_success(shadow_db_map.add_entity_class_item(name="my_class"))
                     shadow_db_map.commit_session("Add same class")
                 entity_class_item = db_map.get_entity_class_item(name="my_class")
                 self.assertTrue(entity_class_item)
@@ -3636,15 +3833,15 @@
     def test_remove_items_then_refresh_then_readd(self):
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
             with DatabaseMapping(url, create=True) as db_map:
                 self._assert_success(db_map.add_entity_class_item(name="my_class"))
                 self._assert_success(db_map.add_entity_class_item(name="new_class"))
                 db_map.commit_session("Add some data")
-            with DatabaseMapping(url, create=True) as db_map:
+            with DatabaseMapping(url) as db_map:
                 db_map.fetch_all("entity_class")
                 with DatabaseMapping(url) as shadow_db_map:
                     shadow_db_map.purge_items("entity_class")
                     self._assert_success(shadow_db_map.add_entity_class_item(name="new_class"))
                     shadow_db_map.commit_session("Purge then add new class back")
                 db_map.refresh_session()
                 entity_class_names = [x["name"] for x in db_map.get_entity_class_items()]
@@ -3655,15 +3852,15 @@
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
             with DatabaseMapping(url, create=True) as db_map:
                 self._assert_success(db_map.add_entity_class_item(name="xxx"))
                 self._assert_success(db_map.add_entity_class_item(name="yyy"))
                 self._assert_success(db_map.add_entity_class_item(name="zzz"))
                 db_map.commit_session("Add some data")
-            with DatabaseMapping(url, create=True) as db_map:
+            with DatabaseMapping(url) as db_map:
                 db_map.fetch_all("entity_class")
                 with DatabaseMapping(url) as shadow_db_map:
                     shadow_db_map.purge_items("entity_class")
                     self._assert_success(shadow_db_map.add_entity_class_item(name="zzz"))
                     self._assert_success(shadow_db_map.add_entity_class_item(name="www"))
                     shadow_db_map.commit_session("Purge then add one old class and one new class")
                 db_map.refresh_session()
```

### Comparing `spinedb_api-0.31.1/tests/test_check_integrity.py` & `spinedb_api-0.31.2/tests/test_check_integrity.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_db_mapping_base.py` & `spinedb_api-0.31.2/tests/test_db_mapping_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 import unittest
 
-from spinedb_api.db_mapping_base import MappedItemBase, DatabaseMappingBase
+from spinedb_api.db_mapping_base import MappedItemBase, DatabaseMappingBase, PublicItem
+from spinedb_api import DatabaseMapping
+from tests.mock_helpers import AssertSuccessTestCase
 
 
 class TestDBMapping(DatabaseMappingBase):
     @staticmethod
     def item_types():
         return ["cutlery"]
 
@@ -78,9 +80,16 @@
         item = MappedItemBase(db_map, "cutlery")
         item.invalidate_id()
         self.assertFalse(item.has_valid_id)
         item["id"] = 23
         self.assertTrue(item.has_valid_id)
 
 
+class TestPublicItem(AssertSuccessTestCase):
+    def test_contains_operator(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            item = self._assert_success(db_map.add_scenario_item(name="my scenario"))
+            self.assertIn("name", item)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `spinedb_api-0.31.1/tests/test_db_server.py` & `spinedb_api-0.31.2/tests/test_db_server.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_export_functions.py` & `spinedb_api-0.31.2/tests/test_export_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_helpers.py` & `spinedb_api-0.31.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_import_functions.py` & `spinedb_api-0.31.2/tests/test_import_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_mapping.py` & `spinedb_api-0.31.2/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_migration.py` & `spinedb_api-0.31.2/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.1/tests/test_parameter_value.py` & `spinedb_api-0.31.2/tests/test_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -864,14 +864,17 @@
         nested_map = Map(["a"], [-2.3])
         map_value = Map(["A"], [nested_map])
         self.assertEqual(map_value, Map(["A"], [Map(["a"], [-2.3])]))
 
     def test_Map_inequality(self):
         map_value = Map(["1", "2", "3", "4", "5"], [-2.3, 2.3, 2.3, 2.3, 2.3])
         self.assertNotEqual(map_value, Map(["a", "b"], [2.3, -2.3]))
+        self.assertNotEqual(
+            Map([DateTime("2024-05-30T00:00:00")], [2.3]), Map([DateTime("2024-05-30T10:00:00")], [2.3])
+        )
 
     def test_TimePattern_equality(self):
         pattern = TimePattern(["D1-2", "D3-7"], np.array([-2.3, -5.0]))
         self.assertEqual(pattern, pattern)
         equal_pattern = TimePattern(["D1-2", "D3-7"], np.array([-2.3, -5.0]))
         self.assertEqual(pattern, equal_pattern)
         inequal_pattern = TimePattern(["M1-3", "M4-12"], np.array([-5.0, 23.0]))
```

### Comparing `spinedb_api-0.31.1/tests/test_purge.py` & `spinedb_api-0.31.2/tests/test_purge.py`

 * *Files identical despite different names*

