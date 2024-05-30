# Comparing `tmp/UncountablePythonSDK-0.0.8.tar.gz` & `tmp/UncountablePythonSDK-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UncountablePythonSDK-0.0.8.tar", last modified: Mon Mar 18 17:03:10 2024, max compression
+gzip compressed data, was "UncountablePythonSDK-0.0.9.tar", last modified: Fri Apr  5 19:00:13 2024, max compression
```

## Comparing `UncountablePythonSDK-0.0.8.tar` & `UncountablePythonSDK-0.0.9.tar`

### file list

```diff
@@ -1,179 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.795829 UncountablePythonSDK-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.775829 UncountablePythonSDK-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-18 17:03:10.795829 UncountablePythonSDK-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.795829 UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-18 17:03:10.000000 UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-18 17:03:10.000000 UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:03:10.000000 UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-18 17:03:10.000000 UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-18 17:03:10.000000 UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/examples/create_entity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/examples/recipe-import/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/examples/recipe-import/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/pkgs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/pkgs/argument_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/argument_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/argument_parser/_is_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/argument_parser/_is_namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/argument_parser/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/argument_parser/case_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/pkgs/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/serialization/missing_sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/serialization/opaque_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/serialization/serial_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/pkgs/serialization_util/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/serialization_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/serialization_util/_get_type_for_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/serialization_util/serialization_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.779829 UncountablePythonSDK-0.0.8/pkgs/strenum_compat/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/strenum_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/strenum_compat/strenum_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.783829 UncountablePythonSDK-0.0.8/pkgs/type_spec/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38993 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_io_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_open_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_open_api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    35580 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_python.py
--rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_typescript.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_typescript_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/load_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/open_api_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.783829 UncountablePythonSDK-0.0.8/pkgs/type_spec/parts/
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/parts/base.py.prepart
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/parts/base.ts.prepart
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.783829 UncountablePythonSDK-0.0.8/pkgs/type_spec/type_info/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/type_info/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/type_info/emit_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.783829 UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/convert_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/emit_python.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 17:03:10.795829 UncountablePythonSDK-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.775829 UncountablePythonSDK-0.0.8/type_spec/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.775829 UncountablePythonSDK-0.0.8/type_spec/external/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.775829 UncountablePythonSDK-0.0.8/type_spec/external/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.783829 UncountablePythonSDK-0.0.8/type_spec/external/api/batch/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/batch/execute_batch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.783829 UncountablePythonSDK-0.0.8/type_spec/external/api/entity/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/entity/create_entities.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/entity/create_entity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/entity/get_entities_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/entity/list_entities.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/entity/resolve_entity_ids.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/entity/set_values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.783829 UncountablePythonSDK-0.0.8/type_spec/external/api/input_groups/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/input_groups/get_input_group_names.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.787829 UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/create_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/get_input_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/get_input_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/get_inputs_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/set_input_attribute_values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.787829 UncountablePythonSDK-0.0.8/type_spec/external/api/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/outputs/get_output_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/outputs/get_output_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/outputs/resolve_output_conditions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.787829 UncountablePythonSDK-0.0.8/type_spec/external/api/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/project/get_projects.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/project/get_projects_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.787829 UncountablePythonSDK-0.0.8/type_spec/external/api/recipe_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipe_metadata/get_recipe_metadata_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.787829 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/create_recipes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_curve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_calculations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_links.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_output_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipes_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/set_recipe_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/set_recipe_outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.787829 UncountablePythonSDK-0.0.8/uncountable/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.787829 UncountablePythonSDK-0.0.8/uncountable/core/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/batch/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/batch/execute_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/create_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/get_entities_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/list_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/resolve_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/entity/set_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/input_groups/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/input_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/input_groups/get_input_group_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/create_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/get_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/get_input_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/get_inputs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/set_input_attribute_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/get_output_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/get_output_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/resolve_output_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/project/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/project/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/project/get_projects_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.791829 UncountablePythonSDK-0.0.8/uncountable/types/api/recipe_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipe_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipe_metadata/get_recipe_metadata_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:03:10.795829 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/create_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_output_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipes_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/set_recipe_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/set_recipe_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21085 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/experiment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/field_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/input_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/recipe_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/recipe_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/recipe_output_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/recipe_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-18 17:03:04.000000 UncountablePythonSDK-0.0.8/uncountable/types/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.911732 UncountablePythonSDK-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.867732 UncountablePythonSDK-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.879732 UncountablePythonSDK-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-05 19:00:13.911732 UncountablePythonSDK-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.907732 UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-05 19:00:13.000000 UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-05 19:00:13.000000 UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:00:13.000000 UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 19:00:13.000000 UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 19:00:13.000000 UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.883732 UncountablePythonSDK-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/examples/create_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.883732 UncountablePythonSDK-0.0.9/examples/recipe-import/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/examples/recipe-import/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.883732 UncountablePythonSDK-0.0.9/pkgs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.883732 UncountablePythonSDK-0.0.9/pkgs/argument_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/argument_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/argument_parser/_is_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/argument_parser/_is_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/argument_parser/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/argument_parser/case_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.883732 UncountablePythonSDK-0.0.9/pkgs/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/serialization/missing_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/serialization/opaque_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/serialization/serial_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.887732 UncountablePythonSDK-0.0.9/pkgs/serialization_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/serialization_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/serialization_util/_get_type_for_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/serialization_util/serialization_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.887732 UncountablePythonSDK-0.0.9/pkgs/strenum_compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/strenum_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/strenum_compat/strenum_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.891732 UncountablePythonSDK-0.0.9/pkgs/type_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38993 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_io_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17461 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_open_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_open_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35580 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_typescript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_typescript_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/load_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/open_api_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.891732 UncountablePythonSDK-0.0.9/pkgs/type_spec/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/parts/base.py.prepart
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/parts/base.ts.prepart
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.891732 UncountablePythonSDK-0.0.9/pkgs/type_spec/type_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/type_info/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/type_info/emit_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.891732 UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/convert_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/emit_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:00:13.911732 UncountablePythonSDK-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.871732 UncountablePythonSDK-0.0.9/type_spec/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.871732 UncountablePythonSDK-0.0.9/type_spec/external/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.871732 UncountablePythonSDK-0.0.9/type_spec/external/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.891732 UncountablePythonSDK-0.0.9/type_spec/external/api/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/batch/execute_batch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.891732 UncountablePythonSDK-0.0.9/type_spec/external/api/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/entity/create_entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/entity/create_entity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/entity/get_entities_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/entity/list_entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/entity/resolve_entity_ids.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/entity/set_values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.891732 UncountablePythonSDK-0.0.9/type_spec/external/api/input_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/input_groups/get_input_group_names.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.895732 UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/create_inputs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/get_input_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/get_input_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/get_inputs_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/set_input_attribute_values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.895732 UncountablePythonSDK-0.0.9/type_spec/external/api/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/outputs/get_output_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/outputs/get_output_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/outputs/resolve_output_conditions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.895732 UncountablePythonSDK-0.0.9/type_spec/external/api/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/project/get_projects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/project/get_projects_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.895732 UncountablePythonSDK-0.0.9/type_spec/external/api/recipe_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipe_metadata/get_recipe_metadata_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.895732 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/create_recipes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_curve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_calculations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_links.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_output_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipes_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/set_recipe_inputs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/set_recipe_outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.895732 UncountablePythonSDK-0.0.9/uncountable/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.895732 UncountablePythonSDK-0.0.9/uncountable/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/core/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.899732 UncountablePythonSDK-0.0.9/uncountable/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/construct_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/cron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.899732 UncountablePythonSDK-0.0.9/uncountable/integration/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/db/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.899732 UncountablePythonSDK-0.0.9/uncountable/integration/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/executors/script_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/integration/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.903732 UncountablePythonSDK-0.0.9/uncountable/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.903732 UncountablePythonSDK-0.0.9/uncountable/types/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.903732 UncountablePythonSDK-0.0.9/uncountable/types/api/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/batch/execute_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.903732 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/create_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/get_entities_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/list_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/resolve_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/entity/set_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.903732 UncountablePythonSDK-0.0.9/uncountable/types/api/input_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/input_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/input_groups/get_input_group_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.903732 UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/create_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/get_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/get_input_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/get_inputs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/set_input_attribute_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.907732 UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/get_output_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/get_output_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/resolve_output_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.907732 UncountablePythonSDK-0.0.9/uncountable/types/api/project/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/project/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/project/get_projects_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.907732 UncountablePythonSDK-0.0.9/uncountable/types/api/recipe_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipe_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipe_metadata/get_recipe_metadata_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:00:13.907732 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/create_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_output_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipes_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/set_recipe_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/set_recipe_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21085 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/experiment_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/field_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/input_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/recipe_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/recipe_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/recipe_output_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/recipe_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 19:00:08.000000 UncountablePythonSDK-0.0.9/uncountable/types/workflows.py
```

### Comparing `UncountablePythonSDK-0.0.8/.github/workflows/publish.yml` & `UncountablePythonSDK-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/PKG-INFO` & `UncountablePythonSDK-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UncountablePythonSDK
-Version: 0.0.8
+Version: 0.0.9
 Summary: Uncountable SDK
 Project-URL: Homepage, https://github.com/uncountableinc/uncountable-python-sdk
 Project-URL: Repository, https://github.com/uncountableinc/uncountable-python-sdk.git
 Project-URL: Issues, https://github.com/uncountableinc/uncountable-python-sdk/issues
 Keywords: uncountable,sdk,api,uncountable-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -12,15 +12,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: requests>=2.31.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: SQLAlchemy==2.0.29
+Requires-Dist: APScheduler==3.10.4
 Provides-Extra: test
 Requires-Dist: mypy>=1.8.1; extra == "test"
 Requires-Dist: ruff>=0.2.1; extra == "test"
 Requires-Dist: pytest>=7.4.3; extra == "test"
 Requires-Dist: coverage[toml]>=6.5.0; extra == "test"
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
 Requires-Dist: pytest-xdist>=3.5.0; extra == "test"
```

### Comparing `UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/PKG-INFO` & `UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UncountablePythonSDK
-Version: 0.0.8
+Version: 0.0.9
 Summary: Uncountable SDK
 Project-URL: Homepage, https://github.com/uncountableinc/uncountable-python-sdk
 Project-URL: Repository, https://github.com/uncountableinc/uncountable-python-sdk.git
 Project-URL: Issues, https://github.com/uncountableinc/uncountable-python-sdk/issues
 Keywords: uncountable,sdk,api,uncountable-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -12,15 +12,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: requests>=2.31.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: SQLAlchemy==2.0.29
+Requires-Dist: APScheduler==3.10.4
 Provides-Extra: test
 Requires-Dist: mypy>=1.8.1; extra == "test"
 Requires-Dist: ruff>=0.2.1; extra == "test"
 Requires-Dist: pytest>=7.4.3; extra == "test"
 Requires-Dist: coverage[toml]>=6.5.0; extra == "test"
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
 Requires-Dist: pytest-xdist>=3.5.0; extra == "test"
```

### Comparing `UncountablePythonSDK-0.0.8/UncountablePythonSDK.egg-info/SOURCES.txt` & `UncountablePythonSDK-0.0.9/UncountablePythonSDK.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -75,14 +75,25 @@
 type_spec/external/api/recipes/get_recipes_data.yaml
 type_spec/external/api/recipes/set_recipe_inputs.yaml
 type_spec/external/api/recipes/set_recipe_outputs.yaml
 uncountable/__init__.py
 uncountable/py.typed
 uncountable/core/__init__.py
 uncountable/core/client.py
+uncountable/integration/__init__.py
+uncountable/integration/construct_client.py
+uncountable/integration/cron.py
+uncountable/integration/entrypoint.py
+uncountable/integration/job.py
+uncountable/integration/server.py
+uncountable/integration/types.py
+uncountable/integration/db/__init__.py
+uncountable/integration/db/connect.py
+uncountable/integration/executors/__init__.py
+uncountable/integration/executors/script_executor.py
 uncountable/types/__init__.py
 uncountable/types/base.py
 uncountable/types/calculations.py
 uncountable/types/client_base.py
 uncountable/types/curves.py
 uncountable/types/entity.py
 uncountable/types/experiment_groups.py
```

### Comparing `UncountablePythonSDK-0.0.8/examples/create_entity.py` & `UncountablePythonSDK-0.0.9/examples/create_entity.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/examples/recipe-import/importer.py` & `UncountablePythonSDK-0.0.9/examples/recipe-import/importer.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/argument_parser/argument_parser.py` & `UncountablePythonSDK-0.0.9/pkgs/argument_parser/argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,9 +403,9 @@
         return self.parser_storage(args)
 
     def parse_yaml_file(self, path: str) -> T:
         with open(path, encoding="utf-8") as data_in:
             return self.parse_storage(yaml.safe_load(data_in))
 
     def parse_yaml_resource(self, package: resources.Package, resource: str) -> T:
-        raw_data = resources.read_text(package, resource)
-        return self.parse_storage(yaml.safe_load(raw_data))
+        with resources.open_text(package, resource) as fp:
+            return self.parse_storage(yaml.safe_load(fp))
```

### Comparing `UncountablePythonSDK-0.0.8/pkgs/argument_parser/case_convert.py` & `UncountablePythonSDK-0.0.9/pkgs/argument_parser/case_convert.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/serialization/__init__.py` & `UncountablePythonSDK-0.0.9/pkgs/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/serialization/missing_sentry.py` & `UncountablePythonSDK-0.0.9/pkgs/serialization/missing_sentry.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/serialization/serial_class.py` & `UncountablePythonSDK-0.0.9/pkgs/serialization/serial_class.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/serialization_util/_get_type_for_serialization.py` & `UncountablePythonSDK-0.0.9/pkgs/serialization_util/_get_type_for_serialization.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/serialization_util/serialization_helpers.py` & `UncountablePythonSDK-0.0.9/pkgs/serialization_util/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/__main__.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/__main__.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/builder.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/builder.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/config.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/config.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_io_ts.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_io_ts.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_open_api.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_open_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,26 @@
         # assert path.path not in oa_paths
         oa_paths[path.path] = {"$ref": path.ref}
     oa_root["paths"] = oa_paths
 
     return yaml.dump(oa_root, sort_keys=False)
 
 
+def _emit_endpoint_parameters(typ: OpenAPIType | None) -> dict[str, list[dict[str, str]]]:
+    if not isinstance(typ, OpenAPIObjectType):
+        return {}
+
+    return {
+        "parameters": [
+            {"$ref": f"#/components/schema/Arguments/{prop_name}"}
+            for prop_name in typ.properties
+        ]
+    }
+
+
 def _emit_namespace(
     gctx: EmitOpenAPIGlobalContext,
     ctx: EmitOpenAPIContext,
     namespace: builder.SpecNamespace,
     *,
     config: OpenAPIConfig,
 ) -> None:
@@ -155,31 +167,36 @@
         _emit_endpoint(gctx, ctx, namespace, namespace.endpoint)
 
     oa_components: dict[str, object] = dict()
 
     if ctx.endpoint is not None:
         endpoint = ctx.endpoint
 
+        argument_type = ctx.types.get("Arguments")
         oa_endpoint = dict()
-        oa_endpoint[endpoint.method] = {
-            "tags": endpoint.tags,
-            "summary": endpoint.summary,
-            "description": endpoint.description,
-            "parameters": {"$ref": "#/components/schema/Arguments"},
-            "responses": {
-                "200": {
-                    "description": "OK",
-                    "content": {
-                        "application/json": {
-                            "schema": {"$ref": "#/components/schema/Data"}
-                        }
-                    },
-                }
-            },
-        }
+        oa_endpoint[endpoint.method] = (
+            {
+                "tags": endpoint.tags,
+                "summary": endpoint.summary,
+                "description": endpoint.description,
+            }
+            | _emit_endpoint_parameters(argument_type)
+            | {
+                "responses": {
+                    "200": {
+                        "description": "OK",
+                        "content": {
+                            "application/json": {
+                                "schema": {"$ref": "#/components/schema/Data"}
+                            }
+                        },
+                    }
+                },
+            }
+        )
         oa_components["endpoint"] = oa_endpoint
 
     types = ctx.types
     if ctx.endpoint is not None:
         # OpenAPI always expected Arguments and Data create
         # them here if they were not already created
         if "Arguments" not in types:
@@ -456,9 +473,9 @@
     if stype.namespace == ctx.namespace:
         # internal namespace resolution
         return OpenAPIRefType(source=f"#/components/schema/{stype.name}")
 
     ctx.namespaces.add(stype.namespace)
     # external namespace resolution
     return OpenAPIRefType(
-        source=f"{resolve_namespace_ref(ctx, stype.namespace, config=config)}/{stype.name}"
+        source=f"{resolve_namespace_ref(source_path=ctx.namespace.path, ref_path=stype.namespace.path, ref='/components/schema')}/{stype.name}"
     )
```

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_open_api_util.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_open_api_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import TypeAlias
 
 from . import builder
-from .config import OpenAPIConfig
 from .open_api_util import OpenAPIType
 
 MODIFY_NOTICE = "# DO NOT MODIFY -- This file is generated by type_spec"
 
 GlobalContextInfo: TypeAlias = dict[str, str | dict[str, str]]
 TagGroupToNamedTags: TypeAlias = dict[str, str | list[str]]
 TagPathsToRef: TypeAlias = dict[str, dict[str, str]]
@@ -71,16 +70,12 @@
     namespaces: set[builder.SpecNamespace] = field(default_factory=set)
 
     endpoint: EmitOpenAPIEndpoint | None = None
     types: dict[str, OpenAPIType] = field(default_factory=dict)
 
 
 def resolve_namespace_ref(
-    ctx: EmitOpenAPIContext,
-    namespace: builder.SpecNamespace,
-    *,
-    config: OpenAPIConfig,
+    *, source_path: list[str], ref_path: list[str], ref: str
 ) -> str:
-    # TODO: Handle namespaces not in root directory
-    if len(ctx.namespace.path) == 1:
-        return f"{namespace.name}.yaml#/components/schema"
-    return f"{config.static_url_path}/common/{namespace.name}.yaml#/components/schema"
+    to_root = "/".join(".." for _ in source_path)
+    location = "/".join(ref_path)
+    return f"{to_root}/common/{location}.yaml#{ref}"
```

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_python.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_python.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_typescript.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_typescript.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/emit_typescript_util.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/emit_typescript_util.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/load_types.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/load_types.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/open_api_util.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/open_api_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     nullable: bool = False
 
     def __init__(self, description: str | None = None, nullable: bool = False) -> None:
         self.description = description
         self.nullable = nullable
 
     @abstractmethod
-    def asdict(self) -> dict[str, object]: ...
+    def asdict(self) -> dict[str, object]:
+        pass
 
-    def asarguments(self) -> list[dict[str, object]]:
+    def asarguments(self) -> dict[str, dict[str, object]]:
         raise UnsupportedOperation
 
     def add_addl_info(self, emitted: dict[str, object]) -> dict[str, object]:
         if self.description is not None:
             emitted["description"] = self.description
         if self.nullable:
             emitted["nullable"] = self.nullable
@@ -143,16 +144,16 @@
 class OpenAPIFreeFormObjectType(OpenAPIType):
     def __init__(self, description: str | None = None, nullable: bool = False) -> None:
         super().__init__(description=description, nullable=nullable)
 
     def asdict(self) -> dict[str, object]:
         return self.add_addl_info({"type": "object"})
 
-    def asarguments(self) -> list[dict[str, object]]:
-        return []
+    def asarguments(self) -> dict[str, dict[str, object]]:
+        return {}
 
 
 class OpenAPIObjectType(OpenAPIType):
     """
     represents OpenAPIs type: "object"
     """
 
@@ -181,25 +182,25 @@
                     **property_type.asdict(),
                     "description": self.property_desc.get(property_name),
                 }
                 for property_name, property_type in self.properties.items()
             },
         })
 
-    def asarguments(self) -> list[dict[str, object]]:
-        argument_types: list[dict[str, object]] = []
+    def asarguments(self) -> dict[str, dict[str, object]]:
+        argument_types: dict[str, dict[str, object]] = {}
         for property_name, property_type in self.properties.items():
             desc = self.property_desc.get(property_name)
-            argument_types.append({
+            argument_types[property_name] = {
                 "name": property_name,
                 "in": "query",
                 "schema": property_type.asdict(),
                 "required": not property_type.nullable,
                 "description": desc or "",
-            })
+            }
         return argument_types
 
 
 class OpenAPIUnionType(OpenAPIType):
     """
     represents OpenAPIs type: "oneOf"
     """
@@ -215,19 +216,19 @@
         self.base_types = base_types
         super().__init__(description=description, nullable=nullable)
 
     def asdict(self) -> dict[str, object]:
         # TODO: use parents description and nullable
         return {"oneOf": [base_type.asdict() for base_type in self.base_types]}
 
-    def asarguments(self) -> list[dict[str, object]]:
+    def asarguments(self) -> dict[str, dict[str, object]]:
         # TODO handle inheritence (allOf and refs); need to inline here...
         # for now skip this endpoint
 
-        return []
+        return {}
 
 
 class OpenAPIIntersectionType(OpenAPIType):
     """
     represents OpenAPIs type: "allOf"
     """
 
@@ -242,12 +243,12 @@
         self.base_types = base_types
         super().__init__(description=description, nullable=nullable)
 
     def asdict(self) -> dict[str, object]:
         # TODO: use parents description and nullable
         return {"allOf": [base_type.asdict() for base_type in self.base_types]}
 
-    def asarguments(self) -> list[dict[str, object]]:
+    def asarguments(self) -> dict[str, dict[str, object]]:
         # TODO handle inheritence (allOf and refs); need to inline here...
         # for now skip this endpoint
 
-        return []
+        return {}
```

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/parts/base.py.prepart` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/parts/base.py.prepart`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/parts/base.ts.prepart` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/parts/base.ts.prepart`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/type_info/__main__.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/type_info/__main__.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/type_info/emit_type_info.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/type_info/emit_type_info.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/util.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/util.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/__main__.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/__main__.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/convert_type.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/convert_type.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pkgs/type_spec/value_spec/emit_python.py` & `UncountablePythonSDK-0.0.9/pkgs/type_spec/value_spec/emit_python.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/pyproject.toml` & `UncountablePythonSDK-0.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     "Typing :: Typed",
 ]
 keywords = [ "uncountable", "sdk", "api", "uncountable-sdk" ]
 # Untested with lower versions but likely works
 requires-python = ">=3.11"
 # May be compatible with older versions
 dependencies = [
-    "requests >= 2.31.0",
+    "requests == 2.31.0",
+    "SQLAlchemy == 2.0.29",
+    "APScheduler == 3.10.4",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 # May be compatible with older versions. Many of the versions below are the
 # latest ones that support Python 3.7.
 test = [
```

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/batch/execute_batch.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/batch/execute_batch.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/entity/create_entities.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/entity/create_entities.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/entity/create_entity.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/entity/create_entity.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/entity/get_entities_data.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/entity/get_entities_data.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/entity/list_entities.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/entity/list_entities.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/entity/resolve_entity_ids.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/entity/resolve_entity_ids.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/input_groups/get_input_group_names.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/input_groups/get_input_group_names.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/create_inputs.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/create_inputs.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/get_input_data.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/get_input_data.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         is_parameter:
             type: Boolean
             desc: "Whether the input is a process parameter (true) or an ingredient (false)"
         attributes:
             type: List<input_attributes.InputAttributeValue>
             desc: "Attributes associated with an input, such as CAS number, density, etc."
         global_category_id:
-            type: ObjectId
+            type: Optional<ObjectId>
             desc: "The global category ID associated with the input"
         subcategory_ids:
             type: List<ObjectId>
             desc: "The subcategory IDs associated with an input. Inputs can be placed into an unlimited number of subcategories"
 
 Data:
     type: Object
```

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/get_input_names.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/get_input_names.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/get_inputs_data.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/get_inputs_data.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/inputs/set_input_attribute_values.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/inputs/set_input_attribute_values.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/outputs/get_output_data.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/outputs/get_output_data.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,18 @@
         quantity_type:
             type: String
             desc: "The quantity type of the output, such as numeric, categorical, text, curve, or calculation"
         attributes:
             type: List<OutputAttrVal>
             desc: "Attributes associated with an output, such as a test documentation"
         global_category_id:
-            type: ObjectId
+            type: Optional<ObjectId>
             desc: "The global category ID associated with the output"
         unit_id:
-            type: ObjectId
+            type: Optional<ObjectId>
             desc: "The unit for the output, which all data is stored in. This may be different than the users default displayed information for the output"
 
 Data:
     type: Object
     properties:
         outputs:
             type: List<FullOutput>
```

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/outputs/get_output_names.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/outputs/get_output_names.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/outputs/resolve_output_conditions.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/outputs/resolve_output_conditions.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/project/get_projects.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/project/get_projects.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/project/get_projects_data.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/project/get_projects_data.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipe_metadata/get_recipe_metadata_data.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipe_metadata/get_recipe_metadata_data.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/create_recipes.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/create_recipes.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_curve.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_curve.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_calculations.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_calculations.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_links.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_links.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_names.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_names.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipe_output_metadata.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipe_output_metadata.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/get_recipes_data.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/get_recipes_data.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/set_recipe_inputs.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/set_recipe_inputs.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/type_spec/external/api/recipes/set_recipe_outputs.yaml` & `UncountablePythonSDK-0.0.9/type_spec/external/api/recipes/set_recipe_outputs.yaml`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/core/client.py` & `UncountablePythonSDK-0.0.9/uncountable/core/client.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/__init__.py` & `UncountablePythonSDK-0.0.9/uncountable/types/__init__.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/batch/execute_batch.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/batch/execute_batch.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/entity/create_entities.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/entity/create_entities.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/entity/create_entity.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/entity/create_entity.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/entity/get_entities_data.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/entity/get_entities_data.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/entity/list_entities.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/entity/list_entities.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/entity/resolve_entity_ids.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/entity/resolve_entity_ids.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/entity/set_values.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/entity/set_values.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/input_groups/get_input_group_names.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/input_groups/get_input_group_names.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/create_inputs.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/create_inputs.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/get_input_data.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/get_input_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 @dataclass(kw_only=True)
 class FullInput:
     input_id: base_t.ObjectId
     name: str
     quantity_type: str
     is_parameter: bool
     attributes: list[input_attributes_t.InputAttributeValue]
-    global_category_id: base_t.ObjectId
+    global_category_id: typing.Optional[base_t.ObjectId]
     subcategory_ids: list[base_t.ObjectId]
 
 
 # DO NOT MODIFY -- This file is generated by type_spec
 @dataclass(kw_only=True)
 class Data:
     inputs: list[FullInput]
```

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/get_input_names.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/get_input_names.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/get_inputs_data.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/get_inputs_data.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/inputs/set_input_attribute_values.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/inputs/set_input_attribute_values.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/get_output_data.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/get_output_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 # DO NOT MODIFY -- This file is generated by type_spec
 @dataclass(kw_only=True)
 class FullOutput:
     output_id: base_t.ObjectId
     name: str
     quantity_type: str
     attributes: list[OutputAttrVal]
-    global_category_id: base_t.ObjectId
-    unit_id: base_t.ObjectId
+    global_category_id: typing.Optional[base_t.ObjectId]
+    unit_id: typing.Optional[base_t.ObjectId]
 
 
 # DO NOT MODIFY -- This file is generated by type_spec
 @dataclass(kw_only=True)
 class Data:
     outputs: list[FullOutput]
     attrs: list[SimpleOutputAttr]
```

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/get_output_names.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/get_output_names.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/outputs/resolve_output_conditions.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/outputs/resolve_output_conditions.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/project/get_projects.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/project/get_projects.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/project/get_projects_data.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/project/get_projects_data.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipe_metadata/get_recipe_metadata_data.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipe_metadata/get_recipe_metadata_data.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/create_recipes.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/create_recipes.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_curve.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_curve.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_calculations.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_calculations.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_links.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_links.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_names.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_names.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipe_output_metadata.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipe_output_metadata.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/get_recipes_data.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/get_recipes_data.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/set_recipe_inputs.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/set_recipe_inputs.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/api/recipes/set_recipe_outputs.py` & `UncountablePythonSDK-0.0.9/uncountable/types/api/recipes/set_recipe_outputs.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/base.py` & `UncountablePythonSDK-0.0.9/uncountable/types/base.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/calculations.py` & `UncountablePythonSDK-0.0.9/uncountable/types/calculations.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/client_base.py` & `UncountablePythonSDK-0.0.9/uncountable/types/client_base.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/curves.py` & `UncountablePythonSDK-0.0.9/uncountable/types/curves.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/entity.py` & `UncountablePythonSDK-0.0.9/uncountable/types/entity.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/experiment_groups.py` & `UncountablePythonSDK-0.0.9/uncountable/types/experiment_groups.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/field_values.py` & `UncountablePythonSDK-0.0.9/uncountable/types/field_values.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/fields.py` & `UncountablePythonSDK-0.0.9/uncountable/types/fields.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/input_attributes.py` & `UncountablePythonSDK-0.0.9/uncountable/types/input_attributes.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/inputs.py` & `UncountablePythonSDK-0.0.9/uncountable/types/inputs.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/outputs.py` & `UncountablePythonSDK-0.0.9/uncountable/types/outputs.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/phases.py` & `UncountablePythonSDK-0.0.9/uncountable/types/phases.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/recipe_links.py` & `UncountablePythonSDK-0.0.9/uncountable/types/recipe_links.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/recipe_metadata.py` & `UncountablePythonSDK-0.0.9/uncountable/types/recipe_metadata.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/recipe_output_metadata.py` & `UncountablePythonSDK-0.0.9/uncountable/types/recipe_output_metadata.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/recipe_tags.py` & `UncountablePythonSDK-0.0.9/uncountable/types/recipe_tags.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/response.py` & `UncountablePythonSDK-0.0.9/uncountable/types/response.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/units.py` & `UncountablePythonSDK-0.0.9/uncountable/types/units.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/users.py` & `UncountablePythonSDK-0.0.9/uncountable/types/users.py`

 * *Files identical despite different names*

### Comparing `UncountablePythonSDK-0.0.8/uncountable/types/workflows.py` & `UncountablePythonSDK-0.0.9/uncountable/types/workflows.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 
 
 # DO NOT MODIFY -- This file is generated by type_spec
 @dataclass(kw_only=True)
 class SimpleWorkflowStep:
     workflow_step_id: base_t.ObjectId
-    name: str
+    name: typing.Optional[str]
 
 
 # DO NOT MODIFY -- This file is generated by type_spec
 @dataclass(kw_only=True)
 class SimpleWorkflow:
     workflow_id: base_t.ObjectId
     name: str
```

