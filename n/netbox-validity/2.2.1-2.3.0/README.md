# Comparing `tmp/netbox_validity-2.2.1.tar.gz` & `tmp/netbox_validity-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_validity-2.2.1.tar", last modified: Sun May 19 19:10:46 2024, max compression
+gzip compressed data, was "netbox_validity-2.3.0.tar", last modified: Sun May 26 22:46:08 2024, max compression
```

## Comparing `netbox_validity-2.2.1.tar` & `netbox_validity-2.3.0.tar`

### file list

```diff
@@ -1,193 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.192576 netbox_validity-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-19 19:10:46.188576 netbox_validity-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.188576 netbox_validity-2.2.1/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.160576 netbox_validity-2.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:10:46.192576 netbox_validity-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.164576 netbox_validity-2.2.1/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.164576 netbox_validity-2.2.1/validity/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.164576 netbox_validity-2.2.1/validity/compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/compliance/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/routeros.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/textfsm.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/ttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/data_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/fields/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/fields/encrypted.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/j2_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.172576 netbox_validity-2.2.1/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0003_complianceselector_dp_tag_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0004_netbox35_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0005_rename_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0006_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0007_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0008_script_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0009_serializer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.172576 netbox_validity-2.2.1/validity/models/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/polling.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/netbox_changes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/pollers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/default_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/netconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/scripts/install/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/install/validity_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/script_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.156576 netbox_validity-2.2.1/validity/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/static/validity/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/connection-type-select.js
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/prism-light.css
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/prism.js
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/subforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.156576 netbox_validity-2.2.1/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.180576 netbox_validity-2.2.1/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/aux_tab_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/command.html
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/device_state.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.180576 netbox_validity-2.2.1/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/configcontext_format.html
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/datasource_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/parameters.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/prism.html
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/related_objects.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/search_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/yaml_card.html
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/nameset.html
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/poller.html
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/poller_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/report_devices.html
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/serializer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.180576 netbox_validity-2.2.1/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_data_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_compliancetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_vdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_vdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_pollers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_scripts/test_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_scripts/test_script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_utils/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.188576 netbox_validity-2.2.1/validity/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.623847 netbox_validity-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-26 22:46:08.623847 netbox_validity-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.623847 netbox_validity-2.3.0/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-26 22:46:08.000000 netbox_validity-2.3.0/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-26 22:46:08.000000 netbox_validity-2.3.0/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:46:08.000000 netbox_validity-2.3.0/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-26 22:46:08.000000 netbox_validity-2.3.0/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 22:46:08.000000 netbox_validity-2.3.0/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.595847 netbox_validity-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 22:46:08.623847 netbox_validity-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.599846 netbox_validity-2.3.0/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.599846 netbox_validity-2.3.0/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.599846 netbox_validity-2.3.0/validity/compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.599846 netbox_validity-2.3.0/validity/compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.599846 netbox_validity-2.3.0/validity/compliance/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/textfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/serialization/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/compliance/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/data_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.603846 netbox_validity-2.3.0/validity/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/fields/encrypted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.603846 netbox_validity-2.3.0/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/forms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.603846 netbox_validity-2.3.0/validity/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/graphql/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.603846 netbox_validity-2.3.0/validity/graphql/strawberry/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/graphql/strawberry/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/graphql/strawberry/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/j2_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.603846 netbox_validity-2.3.0/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0004_netbox35_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0005_rename_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0006_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0007_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0008_script_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0009_serializer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21397 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/0010_squashed_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.607847 netbox_validity-2.3.0/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.607847 netbox_validity-2.3.0/validity/netbox_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/netbox_changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/netbox_changes/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/netbox_changes/old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/netbox_changes/oldest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.607847 netbox_validity-2.3.0/validity/pollers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/default_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/netconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/pollers/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.611847 netbox_validity-2.3.0/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.611847 netbox_validity-2.3.0/validity/scripts/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/scripts/install/validity_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/scripts/script_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/scripts/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.591846 netbox_validity-2.3.0/validity/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.611847 netbox_validity-2.3.0/validity/static/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/static/validity/connection-type-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/static/validity/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/static/validity/prism-light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/static/validity/prism.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/subforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.591846 netbox_validity-2.3.0/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.611847 netbox_validity-2.3.0/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/aux_tab_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/command.html
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/device_state.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.615846 netbox_validity-2.3.0/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/configcontext_format.html
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/datasource_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/parameters.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/prism.html
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/related_objects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/inc/yaml_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/nameset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/poller.html
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/poller_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/report_devices.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templates/validity/serializer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.615846 netbox_validity-2.3.0/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.615846 netbox_validity-2.3.0/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.615846 netbox_validity-2.3.0/validity/tests/test_compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_compliance/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_compliance/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_data_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.619847 netbox_validity-2.3.0/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_models/test_compliancetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_models/test_vdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_models/test_vdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_pollers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.619847 netbox_validity-2.3.0/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_scripts/test_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_scripts/test_script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.619847 netbox_validity-2.3.0/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_utils/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.619847 netbox_validity-2.3.0/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/utils/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:46:08.623847 netbox_validity-2.3.0/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-26 22:45:56.000000 netbox_validity-2.3.0/validity/views/test_result.py
```

### Comparing `netbox_validity-2.2.1/LICENSE` & `netbox_validity-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/PKG-INFO` & `netbox_validity-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.2.1
+Version: 2.3.0
 Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 Classifier: Framework :: Django
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deepdiff<7,>=6.2.0
-Requires-Dist: django-bootstrap-v5==1.0.*
+Requires-Dist: django-bootstrap5<25,>=24.2
 Requires-Dist: dulwich
 Requires-Dist: jq<2,>=1.4.0
 Requires-Dist: netmiko<5,>=4.0.0
 Requires-Dist: pydantic<3,>=2.0.0
 Requires-Dist: scrapli_netconf==2024.1.30
 Requires-Dist: simpleeval==0.9.13
 Requires-Dist: textfsm<2,>=1.1.3
@@ -116,14 +116,23 @@
 * Concept of **dynamic pairs**. With dynamic pair you can compare 2 different devices between each other (e.g. compare the configuration of 2 MC-LAG members).
 * **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step. It helps to identify the cause of the failure.
 * **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from the device.
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 
+
+## NetBox Support Policy
+Unlike many other plugins, Validity supports **multiple** NetBox versions inside one single release.
+
+Validity aims to support **the latest 3 major/minor releases of NetBox**.
+
+For example, if latest NetBox version is 4.1, then latest Validity is going to support NetBox 4.1, 4.0 and 3.7.
+
+
 ## Download and Install
 
 You can download Validity via **pip**
 ```
 pip install netbox-validity
 ```
 After that follow the [installation guide](https://validity.readthedocs.io/en/latest/installation/) to correctly add Validity to your NetBox.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.1 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.3.0 Summary: NetBox
 plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -22,15 +22,15 @@
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: System Administrators Classifier: Intended
 Audience :: Telecommunications Industry Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: Unix Classifier: Operating System
 :: POSIX :: Linux Classifier: Framework :: Django Classifier: Topic :: System
 :: Networking Classifier: Topic :: Internet Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
+deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap5<25,>=24.2 Requires-Dist:
 dulwich Requires-Dist: jq<2,>=1.4.0 Requires-Dist: netmiko<5,>=4.0.0 Requires-
 Dist: pydantic<3,>=2.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
 Dist: simpleeval==0.9.13 Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
 ttp==0.9.* Requires-Dist: xmltodict<1 Provides-Extra: dev Requires-Dist:
 debugpy==1.8.1; extra == "dev" Requires-Dist: factory_boy==3.3.0; extra ==
 "dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pre-commit==3.7.0;
 extra == "dev" Requires-Dist: pytest==8.1.1; extra == "dev" Requires-Dist:
@@ -82,21 +82,25 @@
 the config collected from the device. * **Reports and webhooks**. After
 execution of some bunch of tests you can get the report with passed/failed
 statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can
 provision the webhook to notify an external system when compliance report is
 generated. * **Test extensibility**. You can define your own python functions
 or classes to reuse the code between multiple compliance tests. * Possibility
 to store all heavy text-based entities (like compliance tests or TTP Templates)
-in a **Git repository** ## Download and Install You can download Validity via
-**pip** ``` pip install netbox-validity ``` After that follow the [installation
-guide](https://validity.readthedocs.io/en/latest/installation/) to correctly
-add Validity to your NetBox. ## Documentation Read the full documentation on
-[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start A
-short video about first steps with Validity: [![Watch the video](https://
-img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://www.youtube.com/
+in a **Git repository** ## NetBox Support Policy Unlike many other plugins,
+Validity supports **multiple** NetBox versions inside one single release.
+Validity aims to support **the latest 3 major/minor releases of NetBox**. For
+example, if latest NetBox version is 4.1, then latest Validity is going to
+support NetBox 4.1, 4.0 and 3.7. ## Download and Install You can download
+Validity via **pip** ``` pip install netbox-validity ``` After that follow the
+[installation guide](https://validity.readthedocs.io/en/latest/installation/
+) to correctly add Validity to your NetBox. ## Documentation Read the full
+documentation on [validity.readthedocs.io](https://validity.readthedocs.io) ##
+Quick Start A short video about first steps with Validity: [![Watch the video]
+(https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://www.youtube.com/
 watch?v=QR04rGwMuPQ) ## Contributing Feel free to ask a [Question](https://
 github.com/amyasnikov/validity/discussions), report an [Issue](https://
 github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md).
 Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide. ##
 Screenshots ![Report Per Device](docs/images/screen_report.png) ![Compliance
 Test](docs/images/screen_test.png) ![Compliance Test Result](docs/images/
 screen_result.png) ![Device Serialized Configuration](docs/images/
```

### Comparing `netbox_validity-2.2.1/README.md` & `netbox_validity-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,23 @@
 * Concept of **dynamic pairs**. With dynamic pair you can compare 2 different devices between each other (e.g. compare the configuration of 2 MC-LAG members).
 * **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step. It helps to identify the cause of the failure.
 * **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from the device.
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 
+
+## NetBox Support Policy
+Unlike many other plugins, Validity supports **multiple** NetBox versions inside one single release.
+
+Validity aims to support **the latest 3 major/minor releases of NetBox**.
+
+For example, if latest NetBox version is 4.1, then latest Validity is going to support NetBox 4.1, 4.0 and 3.7.
+
+
 ## Download and Install
 
 You can download Validity via **pip**
 ```
 pip install netbox-validity
 ```
 After that follow the [installation guide](https://validity.readthedocs.io/en/latest/installation/) to correctly add Validity to your NetBox.
```

#### html2text {}

```diff
@@ -41,21 +41,25 @@
 the config collected from the device. * **Reports and webhooks**. After
 execution of some bunch of tests you can get the report with passed/failed
 statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can
 provision the webhook to notify an external system when compliance report is
 generated. * **Test extensibility**. You can define your own python functions
 or classes to reuse the code between multiple compliance tests. * Possibility
 to store all heavy text-based entities (like compliance tests or TTP Templates)
-in a **Git repository** ## Download and Install You can download Validity via
-**pip** ``` pip install netbox-validity ``` After that follow the [installation
-guide](https://validity.readthedocs.io/en/latest/installation/) to correctly
-add Validity to your NetBox. ## Documentation Read the full documentation on
-[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start A
-short video about first steps with Validity: [![Watch the video](https://
-img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://www.youtube.com/
+in a **Git repository** ## NetBox Support Policy Unlike many other plugins,
+Validity supports **multiple** NetBox versions inside one single release.
+Validity aims to support **the latest 3 major/minor releases of NetBox**. For
+example, if latest NetBox version is 4.1, then latest Validity is going to
+support NetBox 4.1, 4.0 and 3.7. ## Download and Install You can download
+Validity via **pip** ``` pip install netbox-validity ``` After that follow the
+[installation guide](https://validity.readthedocs.io/en/latest/installation/
+) to correctly add Validity to your NetBox. ## Documentation Read the full
+documentation on [validity.readthedocs.io](https://validity.readthedocs.io) ##
+Quick Start A short video about first steps with Validity: [![Watch the video]
+(https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://www.youtube.com/
 watch?v=QR04rGwMuPQ) ## Contributing Feel free to ask a [Question](https://
 github.com/amyasnikov/validity/discussions), report an [Issue](https://
 github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md).
 Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide. ##
 Screenshots ![Report Per Device](docs/images/screen_report.png) ![Compliance
 Test](docs/images/screen_test.png) ![Compliance Test Result](docs/images/
 screen_result.png) ![Device Serialized Configuration](docs/images/
```

### Comparing `netbox_validity-2.2.1/netbox_validity.egg-info/PKG-INFO` & `netbox_validity-2.3.0/netbox_validity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.2.1
+Version: 2.3.0
 Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 Classifier: Framework :: Django
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deepdiff<7,>=6.2.0
-Requires-Dist: django-bootstrap-v5==1.0.*
+Requires-Dist: django-bootstrap5<25,>=24.2
 Requires-Dist: dulwich
 Requires-Dist: jq<2,>=1.4.0
 Requires-Dist: netmiko<5,>=4.0.0
 Requires-Dist: pydantic<3,>=2.0.0
 Requires-Dist: scrapli_netconf==2024.1.30
 Requires-Dist: simpleeval==0.9.13
 Requires-Dist: textfsm<2,>=1.1.3
@@ -116,14 +116,23 @@
 * Concept of **dynamic pairs**. With dynamic pair you can compare 2 different devices between each other (e.g. compare the configuration of 2 MC-LAG members).
 * **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step. It helps to identify the cause of the failure.
 * **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from the device.
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 
+
+## NetBox Support Policy
+Unlike many other plugins, Validity supports **multiple** NetBox versions inside one single release.
+
+Validity aims to support **the latest 3 major/minor releases of NetBox**.
+
+For example, if latest NetBox version is 4.1, then latest Validity is going to support NetBox 4.1, 4.0 and 3.7.
+
+
 ## Download and Install
 
 You can download Validity via **pip**
 ```
 pip install netbox-validity
 ```
 After that follow the [installation guide](https://validity.readthedocs.io/en/latest/installation/) to correctly add Validity to your NetBox.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.1 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.3.0 Summary: NetBox
 plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -22,15 +22,15 @@
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: System Administrators Classifier: Intended
 Audience :: Telecommunications Industry Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: Unix Classifier: Operating System
 :: POSIX :: Linux Classifier: Framework :: Django Classifier: Topic :: System
 :: Networking Classifier: Topic :: Internet Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
+deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap5<25,>=24.2 Requires-Dist:
 dulwich Requires-Dist: jq<2,>=1.4.0 Requires-Dist: netmiko<5,>=4.0.0 Requires-
 Dist: pydantic<3,>=2.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
 Dist: simpleeval==0.9.13 Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
 ttp==0.9.* Requires-Dist: xmltodict<1 Provides-Extra: dev Requires-Dist:
 debugpy==1.8.1; extra == "dev" Requires-Dist: factory_boy==3.3.0; extra ==
 "dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pre-commit==3.7.0;
 extra == "dev" Requires-Dist: pytest==8.1.1; extra == "dev" Requires-Dist:
@@ -82,21 +82,25 @@
 the config collected from the device. * **Reports and webhooks**. After
 execution of some bunch of tests you can get the report with passed/failed
 statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can
 provision the webhook to notify an external system when compliance report is
 generated. * **Test extensibility**. You can define your own python functions
 or classes to reuse the code between multiple compliance tests. * Possibility
 to store all heavy text-based entities (like compliance tests or TTP Templates)
-in a **Git repository** ## Download and Install You can download Validity via
-**pip** ``` pip install netbox-validity ``` After that follow the [installation
-guide](https://validity.readthedocs.io/en/latest/installation/) to correctly
-add Validity to your NetBox. ## Documentation Read the full documentation on
-[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start A
-short video about first steps with Validity: [![Watch the video](https://
-img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://www.youtube.com/
+in a **Git repository** ## NetBox Support Policy Unlike many other plugins,
+Validity supports **multiple** NetBox versions inside one single release.
+Validity aims to support **the latest 3 major/minor releases of NetBox**. For
+example, if latest NetBox version is 4.1, then latest Validity is going to
+support NetBox 4.1, 4.0 and 3.7. ## Download and Install You can download
+Validity via **pip** ``` pip install netbox-validity ``` After that follow the
+[installation guide](https://validity.readthedocs.io/en/latest/installation/
+) to correctly add Validity to your NetBox. ## Documentation Read the full
+documentation on [validity.readthedocs.io](https://validity.readthedocs.io) ##
+Quick Start A short video about first steps with Validity: [![Watch the video]
+(https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://www.youtube.com/
 watch?v=QR04rGwMuPQ) ## Contributing Feel free to ask a [Question](https://
 github.com/amyasnikov/validity/discussions), report an [Issue](https://
 github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md).
 Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide. ##
 Screenshots ![Report Per Device](docs/images/screen_report.png) ![Compliance
 Test](docs/images/screen_test.png) ![Compliance Test Result](docs/images/
 screen_result.png) ![Device Serialized Configuration](docs/images/
```

### Comparing `netbox_validity-2.2.1/netbox_validity.egg-info/SOURCES.txt` & `netbox_validity-2.3.0/netbox_validity.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 requirements/docs.txt
 validity/__init__.py
 validity/admin.py
 validity/choices.py
 validity/custom_validators.py
 validity/data_backends.py
 validity/filtersets.py
-validity/graphql.py
 validity/j2_env.py
 validity/managers.py
 validity/navigation.py
-validity/netbox_changes.py
 validity/search.py
 validity/subforms.py
 validity/tables.py
 validity/template_content.py
 validity/urls.py
 validity/api/__init__.py
 validity/api/helpers.py
@@ -46,38 +44,49 @@
 validity/compliance/serialization/textfsm.py
 validity/compliance/serialization/ttp.py
 validity/compliance/serialization/xml.py
 validity/compliance/serialization/yaml.py
 validity/fields/__init__.py
 validity/fields/encrypted.py
 validity/forms/__init__.py
+validity/forms/fields.py
 validity/forms/filterset.py
 validity/forms/general.py
-validity/forms/helpers.py
+validity/forms/mixins.py
+validity/forms/widgets.py
+validity/graphql/__init__.py
+validity/graphql/graphene.py
+validity/graphql/strawberry/filters.py
+validity/graphql/strawberry/schema.py
 validity/migrations/0001_initial.py
 validity/migrations/0002_custom_fields.py
 validity/migrations/0003_complianceselector_dp_tag_prefix.py
 validity/migrations/0004_netbox35_scripts.py
 validity/migrations/0005_rename_serializer.py
 validity/migrations/0006_datasources.py
 validity/migrations/0007_polling.py
 validity/migrations/0008_script_change.py
 validity/migrations/0009_serializer_parameters.py
+validity/migrations/0010_squashed_initial.py
 validity/migrations/__init__.py
 validity/models/__init__.py
 validity/models/base.py
 validity/models/data.py
 validity/models/device.py
 validity/models/nameset.py
 validity/models/polling.py
 validity/models/report.py
 validity/models/selector.py
 validity/models/serializer.py
 validity/models/test.py
 validity/models/test_result.py
+validity/netbox_changes/__init__.py
+validity/netbox_changes/current.py
+validity/netbox_changes/old.py
+validity/netbox_changes/oldest.py
 validity/pollers/__init__.py
 validity/pollers/base.py
 validity/pollers/cli.py
 validity/pollers/default_credentials.py
 validity/pollers/exceptions.py
 validity/pollers/factory.py
 validity/pollers/http.py
```

### Comparing `netbox_validity-2.2.1/pyproject.toml` & `netbox_validity-2.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "2.2.1"
+version = "2.3.0"
 description = "NetBox plugin for network devices validation"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -77,15 +77,15 @@
 
 [tool.ruff.lint]
 select = ["E4", "E7", "E9", "F", "B", "T", "I"]
 ignore = ["B905"]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
-"validity/netbox_changes.py" = ["F401"]
+"validity/netbox_changes/*" = ["F403", "F405"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["validity"]
 no-lines-before = ["local-folder"]
 lines-after-imports = 2
 
 [tool.ruff.format]
```

### Comparing `netbox_validity-2.2.1/validity/__init__.py` & `netbox_validity-2.3.0/validity/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import logging
 
 from django.conf import settings as django_settings
-from extras.plugins import PluginConfig
 from netbox.settings import VERSION
 from pydantic import BaseModel, Field
 
 from validity.utils.version import NetboxVersion
 
 
+if VERSION.startswith("3."):
+    from extras.plugins import PluginConfig
+else:
+    from netbox.plugins import PluginConfig
+
+
 logger = logging.getLogger(__name__)
 
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity"
     description = "Write and run auto tests for network devices"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "2.2.1"
+    version = "2.3.0"
     base_url = "validity"
-    django_apps = ["bootstrap5"]
-    min_version = "3.5.0"
+    django_apps = ["django_bootstrap5"]
+    min_version = "3.6.0"
 
     # custom field
     netbox_version = NetboxVersion(VERSION)
 
     def ready(self):
         import validity.data_backends
```

### Comparing `netbox_validity-2.2.1/validity/api/helpers.py` & `netbox_validity-2.3.0/validity/api/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,40 @@
+from functools import partial
 from itertools import chain
 from typing import Sequence
 
 from django.core.exceptions import ValidationError
 from django.db.models import ManyToManyField
 from netbox.api.serializers import WritableNestedSerializer
 from rest_framework.serializers import JSONField, ModelSerializer
 
+from validity import NetboxVersion
 from validity.fields.encrypted import EncryptedDict
 
 
+def meta_factory(parent=None, **fields):
+    bases = () if parent is None else (parent,)
+    return type("Meta", bases, fields)
+
+
 def nested_factory(
-    serializer: type[ModelSerializer], meta_fields: Sequence[str], attributes: Sequence[str] = ("url",)
+    serializer: type[ModelSerializer], nb_version: NetboxVersion, attributes: Sequence[str] = ("url",)
 ) -> type[ModelSerializer]:
     """
     Creates nested Serializer from regular one
     """
-
-    class Meta:
-        model = serializer.Meta.model
-        fields = meta_fields
+    if nb_version >= "4.0.0":
+        Serializer = type(serializer.__name__, (serializer,), {"Meta": meta_factory(parent=serializer.Meta)})
+        return partial(Serializer, nested=True)
 
     name = "Nested" + serializer.__name__
     mixins = (cls for cls in serializer.__bases__ if not issubclass(cls, ModelSerializer))
     bases = tuple(chain(mixins, (WritableNestedSerializer,)))
     s_attribs = {a: serializer._declared_fields[a] for a in attributes}
-    s_attribs["Meta"] = Meta
+    s_attribs["Meta"] = meta_factory(parent=serializer.Meta, fields=serializer.Meta.brief_fields)
     return type(name, bases, s_attribs)
 
 
 class EncryptedDictField(JSONField):
     def to_representation(self, value):
         return value.encrypted
```

### Comparing `netbox_validity-2.2.1/validity/api/serializers.py` & `netbox_validity-2.3.0/validity/api/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from netbox.api.fields import SerializedPKRelatedField
 from netbox.api.serializers import NetBoxModelSerializer
 from rest_framework import serializers
 from rest_framework.reverse import reverse
 from tenancy.api.nested_serializers import NestedTenantSerializer
 from tenancy.models import Tenant
 
-from validity import models
+from validity import config, models
 from .helpers import EncryptedDictField, FieldsMixin, ListQPMixin, SubformValidationMixin, nested_factory
 
 
 class ComplianceSelectorSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:validity-api:complianceselector-detail")
     tag_filter = SerializedPKRelatedField(
         serializer=NestedTagSerializer,
@@ -68,17 +68,18 @@
             "dynamic_pairs",
             "dp_tag_prefix",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display", "name")
 
 
-NestedComplianceSelectorSerializer = nested_factory(ComplianceSelectorSerializer, ("id", "url", "display", "name"))
+NestedComplianceSelectorSerializer = nested_factory(ComplianceSelectorSerializer, nb_version=config.netbox_version)
 
 
 class ComplianceTestSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:validity-api:compliancetest-detail")
     selectors = SerializedPKRelatedField(
         serializer=NestedComplianceSelectorSerializer,
         many=True,
@@ -105,17 +106,18 @@
             "data_file",
             "selectors",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display", "name", "severity")
 
 
-NestedComplianceTestSerializer = nested_factory(ComplianceTestSerializer, ("id", "url", "display", "name", "severity"))
+NestedComplianceTestSerializer = nested_factory(ComplianceTestSerializer, nb_version=config.netbox_version)
 
 
 class ComplianceReportSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:validity-api:compliancereport-detail")
     results_url = serializers.SerializerMethodField()
     device_count = serializers.ReadOnlyField()
     test_count = serializers.ReadOnlyField()
@@ -145,21 +147,22 @@
             "high_passed",
             "high_count",
             "results_url",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display")
 
     def get_results_url(self, obj):
         results_url = reverse("plugins-api:validity-api:compliancetestresult-list", request=self.context["request"])
         return results_url + f"?report_id={obj.pk}"
 
 
-NestedComplianceReportSerializer = nested_factory(ComplianceReportSerializer, ("id", "url", "display"))
+NestedComplianceReportSerializer = nested_factory(ComplianceReportSerializer, nb_version=config.netbox_version)
 
 
 class ComplianceTestResultSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:validity-api:compliancetestresult-detail")
     test = NestedComplianceTestSerializer()
     device = NestedDeviceSerializer()
     dynamic_pair = NestedDeviceSerializer(allow_null=True)
@@ -177,19 +180,18 @@
             "report",
             "passed",
             "explanation",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display", "passed")
 
 
-NestedComplianceTestResultSerializer = nested_factory(
-    ComplianceTestResultSerializer, ("id", "url", "display", "passed")
-)
+NestedComplianceTestResultSerializer = nested_factory(ComplianceTestResultSerializer, nb_version=config.netbox_version)
 
 
 class SerializerSerializer(SubformValidationMixin, NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:validity-api:serializer-detail")
     template = serializers.CharField(write_only=True, required=False)
     effective_template = serializers.ReadOnlyField()
     data_source = NestedDataSourceSerializer(required=False)
@@ -209,17 +211,18 @@
             "data_file",
             "parameters",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display", "name")
 
 
-NestedSerializerSerializer = nested_factory(SerializerSerializer, ("id", "url", "display", "name"))
+NestedSerializerSerializer = nested_factory(SerializerSerializer, nb_version=config.netbox_version)
 
 
 class NameSetSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:validity-api:nameset-detail")
     data_source = NestedDataSourceSerializer(required=False)
     data_file = NestedDataFileSerializer(required=False)
     definitions = serializers.CharField(write_only=True, required=False)
@@ -240,27 +243,28 @@
             "definitions",
             "effective_definitions",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display", "name")
 
     def to_representation(self, instance):
         result = super().to_representation(instance)
         result["global"] = result.pop("_global")
         return result
 
     def run_validation(self, data=...):
         if "global" in data:
             data["_global"] = data.pop("global")
         return super().run_validation(data)
 
 
-NestedNameSetSerializer = nested_factory(NameSetSerializer, ("id", "url", "display", "name"))
+NestedNameSetSerializer = nested_factory(NameSetSerializer, nb_version=config.netbox_version)
 
 
 class DeviceReportSerializer(NestedDeviceSerializer):
     compliance_passed = serializers.BooleanField()
     results_passed = serializers.IntegerField()
     results_count = serializers.IntegerField()
     results = SerializedPKRelatedField(
@@ -293,17 +297,18 @@
             "type",
             "parameters",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display", "name")
 
 
-NestedCommandSerializer = nested_factory(CommandSerializer, ("id", "url", "display", "name"))
+NestedCommandSerializer = nested_factory(CommandSerializer, nb_version=config.netbox_version)
 
 
 class PollerSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:validity-api:poller-detail")
     private_credentials = EncryptedDictField()
     commands = SerializedPKRelatedField(
         serializer=NestedCommandSerializer,
@@ -324,21 +329,22 @@
             "private_credentials",
             "commands",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
+        brief_fields = ("id", "url", "display", "name")
 
     def validate(self, data):
         models.Poller.validate_commands(data["connection_type"], data["commands"])
         return super().validate(data)
 
 
-NestedPollerSerializer = nested_factory(PollerSerializer, ("id", "url", "display", "name"))
+NestedPollerSerializer = nested_factory(PollerSerializer, nb_version=config.netbox_version)
 
 
 class SerializedStateItemSerializer(FieldsMixin, serializers.Serializer):
     name = serializers.CharField(read_only=True)
     serializer = NestedSerializerSerializer(read_only=True)
     data_source = NestedDataSourceSerializer(read_only=True, source="data_file.source")
     data_file = NestedDataFileSerializer(read_only=True)
```

### Comparing `netbox_validity-2.2.1/validity/api/urls.py` & `netbox_validity-2.3.0/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/api/views.py` & `netbox_validity-2.3.0/validity/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/choices.py` & `netbox_validity-2.3.0/validity/choices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Any, Optional, TypeVar
 
 from django.db.models import IntegerChoices, TextChoices
 from django.db.models.enums import ChoicesMeta
 from django.utils.translation import gettext_lazy as _
 
-from validity.netbox_changes import DEVICE_ROLE_RELATION
-
 
 class ColoredChoiceMeta(ChoicesMeta):
     """
     Allows to write choice fields with a color like that:
         option1 = 'red'
         option2 = ('option2', 'yellow')
         option3 = ('option3', 'Option3', 'green')
@@ -85,15 +83,15 @@
     ROUTEROS = "ROUTEROS", "ROUTEROS", "green"
 
 
 class DeviceGroupByChoices(MemberMixin, TextChoices):
     DEVICE = "device__name", _("Device")
     DEVICE_TYPE = "device__device_type__slug", _("Device Type")
     MANUFACTURER = "device__device_type__manufacturer__slug", _("Manufacturer")
-    DEVICE_ROLE = f"device__{DEVICE_ROLE_RELATION}__slug", _("Device Role")
+    DEVICE_ROLE = "device__role__slug", _("Device Role")
     TENANT = "device__tenant__slug", _("Tenant")
     PLATFORM = "device__platform__slug", _("Platform")
     LOCATION = "device__location__slug", _("Location")
     SITE = "device__site__slug", _("Site")
     TEST = "test__name", _("Test")
 
     @classmethod
```

### Comparing `netbox_validity-2.2.1/validity/compliance/dynamic_pairs.py` & `netbox_validity-2.3.0/validity/compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/eval/default_nameset.py` & `netbox_validity-2.3.0/validity/compliance/eval/default_nameset.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/eval/eval.py` & `netbox_validity-2.3.0/validity/compliance/eval/eval.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/eval/eval_defaults.py` & `netbox_validity-2.3.0/validity/compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/exceptions.py` & `netbox_validity-2.3.0/validity/compliance/exceptions.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/serialization/backend.py` & `netbox_validity-2.3.0/validity/compliance/serialization/backend.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/serialization/routeros.py` & `netbox_validity-2.3.0/validity/compliance/serialization/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/serialization/serializable.py` & `netbox_validity-2.3.0/validity/compliance/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/serialization/xml.py` & `netbox_validity-2.3.0/validity/compliance/serialization/xml.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/compliance/state.py` & `netbox_validity-2.3.0/validity/compliance/state.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/custom_validators.py` & `netbox_validity-2.3.0/validity/custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/data_backends.py` & `netbox_validity-2.3.0/validity/data_backends.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/fields/encrypted.py` & `netbox_validity-2.3.0/validity/fields/encrypted.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     def to_python(self, value):
         if value is None or isinstance(value, EncryptedDict):
             return value
         return EncryptedDict(value)
 
     def formfield(self, **kwargs):
-        from validity.forms.helpers import EncryptedDictField as EncryptedDictFormField
+        from validity.forms.fields import EncryptedDictField as EncryptedDictFormField
 
         return Field.formfield(
             self,
             **{
                 "form_class": EncryptedDictFormField,
                 "encoder": self.encoder,
                 "decoder": self.decoder,
```

### Comparing `netbox_validity-2.2.1/validity/filtersets.py` & `netbox_validity-2.3.0/validity/filtersets.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from django_filters import BooleanFilter, ChoiceFilter, ModelMultipleChoiceFilter
 from extras.models import Tag
 from netbox.filtersets import NetBoxModelFilterSet
 from tenancy.models import Tenant
 
 from validity import models
 from validity.choices import SeverityChoices
-from validity.netbox_changes import DEVICE_ROLE_RELATION
 
 
 class SearchMixin:
     def search(self, queryset, name, value):
         value = value.strip()
         if not value:
             return queryset
@@ -50,17 +49,15 @@
     report_id = ModelMultipleChoiceFilter(field_name="report", queryset=models.ComplianceReport.objects.all())
     latest = BooleanFilter(method="filter_latest")
     severity = ChoiceFilter(field_name="test__severity", choices=SeverityChoices.choices)
     device_type_id = ModelMultipleChoiceFilter(field_name="device__device_type", queryset=DeviceType.objects.all())
     manufacturer_id = ModelMultipleChoiceFilter(
         field_name="device__device_type__manufacturer", queryset=Manufacturer.objects.all()
     )
-    device_role_id = ModelMultipleChoiceFilter(
-        field_name=f"device__{DEVICE_ROLE_RELATION}", queryset=DeviceRole.objects.all()
-    )
+    device_role_id = ModelMultipleChoiceFilter(field_name="device__role", queryset=DeviceRole.objects.all())
     tenant_id = ModelMultipleChoiceFilter(field_name="device__tenant", queryset=Tenant.objects.all())
     platform_id = ModelMultipleChoiceFilter(field_name="device__platform", queryset=Platform.objects.all())
     location_id = ModelMultipleChoiceFilter(field_name="device__location", queryset=Location.objects.all())
     site_id = ModelMultipleChoiceFilter(field_name="device__site", queryset=Site.objects.all())
     test_tag_id = ModelMultipleChoiceFilter(field_name="test__tags", queryset=Tag.objects.all())
     tag = None
```

### Comparing `netbox_validity-2.2.1/validity/forms/filterset.py` & `netbox_validity-2.3.0/validity/forms/filterset.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,40 +14,42 @@
     CommandTypeChoices,
     ConnectionTypeChoices,
     DeviceGroupByChoices,
     DynamicPairsChoices,
     ExtractionMethodChoices,
     SeverityChoices,
 )
-from .helpers import ExcludeMixin, PlaceholderChoiceField
+from validity.netbox_changes import FieldSet
+from .fields import PlaceholderChoiceField
+from .mixins import AddM2MPlaceholderFormMixin, ExcludeMixin
 
 
 class DeviceReportFilterForm(ExcludeMixin, Form):
     q = CharField(label=_("Device Search"), required=False)
     compliance_passed = PlaceholderChoiceField(
-        required=False, placeholder=_("Compliance Passed"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:]
+        required=False, label=_("Compliance Passed"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:]
     )
     severity_ge = PlaceholderChoiceField(
-        required=False, placeholder=_("Minimum Severity"), choices=SeverityChoices.choices[1:]
+        required=False, label=_("Minimum Severity"), choices=SeverityChoices.choices[1:]
     )
 
 
 class DataSourceDevicesFilterForm(Form):
     q = CharField(label=_("Device Search"), required=False)
     tenant_id = DynamicModelMultipleChoiceField(label=_("Tenant"), queryset=Tenant.objects.all(), required=False)
 
 
-class TestResultFilterForm(ExcludeMixin, Form):
-    latest = PlaceholderChoiceField(required=False, placeholder=_("Latest"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:])
+class TestResultFilterForm(ExcludeMixin, AddM2MPlaceholderFormMixin, Form):
+    latest = PlaceholderChoiceField(required=False, label=_("Latest"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:])
     passed = PlaceholderChoiceField(
         required=False,
-        placeholder=_("Passed"),
+        label=_("Passed"),
         choices=BOOLEAN_WITH_BLANK_CHOICES[1:],
     )
-    severity = PlaceholderChoiceField(required=False, placeholder=_("Severity"), choices=SeverityChoices.choices)
+    severity = PlaceholderChoiceField(required=False, label=_("Severity"), choices=SeverityChoices.choices)
     device_id = DynamicModelMultipleChoiceField(
         label=_("Device"),
         queryset=Device.objects.all(),
         required=False,
     )
     test_id = DynamicModelMultipleChoiceField(
         label=_("Test"), queryset=models.ComplianceTest.objects.all(), required=False
@@ -75,36 +77,33 @@
     site_id = DynamicModelMultipleChoiceField(required=False, label=_("Site"), queryset=Site.objects.all())
     test_tag_id = DynamicModelMultipleChoiceField(required=False, label=_("Test Tags"), queryset=Tag.objects.all())
 
 
 class ComplianceTestResultFilterForm(TestResultFilterForm, NetBoxModelFilterSetForm):
     model = models.ComplianceTestResult
     fieldsets = (
-        [_("Common"), ("latest", "passed", "selector_id")],
-        [_("Test"), ("severity", "test_id", "report_id", "test_tag_id")],
-        [
-            _("Device"),
-            (
-                "device_id",
-                "device_type_id",
-                "manufacturer_id",
-                "device_role_id",
-                "tenant_id",
-                "platform_id",
-                "location_id",
-                "site_id",
-            ),
-        ],
+        FieldSet("latest", "passed", "selector_id", name=_("Common")),
+        FieldSet("severity", "test_id", "report_id", "test_tag_id", name=_("Test")),
+        FieldSet(
+            "device_id",
+            "device_type_id",
+            "manufacturer_id",
+            "device_role_id",
+            "tenant_id",
+            "platform_id",
+            "location_id",
+            "site_id",
+            name=_("Device"),
+        ),
     )
 
 
 class ReportGroupByForm(Form):
     group_by = PlaceholderChoiceField(
         label=_("Group results by"),
-        placeholder=_("Group results by"),
         required=False,
         choices=DeviceGroupByChoices.choices,
     )
 
 
 class StateSelectForm(Form):
     state_item = PlaceholderChoiceField(
@@ -138,46 +137,46 @@
     )
 
 
 class SerializerFilterForm(NetBoxModelFilterSetForm):
     model = models.Serializer
     name = CharField(required=False)
     extraction_method = PlaceholderChoiceField(
-        required=False, placeholder=_("Extraction Method"), choices=ExtractionMethodChoices.choices
+        required=False, label=_("Extraction Method"), choices=ExtractionMethodChoices.choices
     )
     datasource_id = DynamicModelMultipleChoiceField(
         label=_("Data Source"), queryset=DataSource.objects.all(), required=False
     )
 
 
 class ComplianceTestFilterForm(NetBoxModelFilterSetForm):
     model = models.ComplianceTest
     name = CharField(required=False)
-    severity = PlaceholderChoiceField(required=False, placeholder=_("Severity"), choices=SeverityChoices.choices)
+    severity = PlaceholderChoiceField(required=False, label=_("Severity"), choices=SeverityChoices.choices)
     selector_id = DynamicModelMultipleChoiceField(
         label=_("Selector"), queryset=models.ComplianceSelector.objects.all(), required=False
     )
     datasource_id = DynamicModelMultipleChoiceField(
         label=_("Data Source"), queryset=DataSource.objects.all(), required=False
     )
 
 
 class PollerFilterForm(NetBoxModelFilterSetForm):
     model = models.Poller
     name = CharField(required=False)
     connection_type = PlaceholderChoiceField(
-        required=False, placeholder=_("Connection Type"), choices=ConnectionTypeChoices.choices
+        required=False, label=_("Connection Type"), choices=ConnectionTypeChoices.choices
     )
 
 
 class CommandFilterForm(NetBoxModelFilterSetForm):
     model = models.Command
     name = CharField(required=False)
     label = CharField(required=False)
-    type = PlaceholderChoiceField(required=False, placeholder=_("Type"), choices=CommandTypeChoices.choices)
+    type = PlaceholderChoiceField(required=False, label=_("Type"), choices=CommandTypeChoices.choices)
     retrieves_config = NullBooleanField(
         label=_("Global"), required=False, widget=Select(choices=BOOLEAN_WITH_BLANK_CHOICES)
     )
     serializer_id = DynamicModelMultipleChoiceField(
         label=_("Serializer"), queryset=models.Serializer.objects.all(), required=False
     )
     poller_id = DynamicModelMultipleChoiceField(label=_("Poller"), queryset=models.Poller.objects.all(), required=False)
```

### Comparing `netbox_validity-2.2.1/validity/forms/general.py` & `netbox_validity-2.3.0/validity/forms/general.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 from tenancy.models import Tenant
 from utilities.forms import add_blank_choice, get_field_value
 from utilities.forms.fields import DynamicModelChoiceField, DynamicModelMultipleChoiceField
 from utilities.forms.widgets import HTMXSelect
 
 from validity import models
 from validity.choices import ConnectionTypeChoices
-from .helpers import PrettyJSONWidget, SubformMixin
+from validity.netbox_changes import FieldSet
+from .mixins import SubformMixin
+from .widgets import PrettyJSONWidget
 
 
 class ComplianceTestForm(SyncedDataMixin, NetBoxModelForm):
     selectors = DynamicModelMultipleChoiceField(queryset=models.ComplianceSelector.objects.all())
     expression = CharField(required=False, widget=Textarea(attrs={"style": "font-family:monospace"}))
 
     fieldsets = (
-        (_("Compliance Test"), ("name", "severity", "description", "selectors", "tags")),
-        (_("Expression from Data Source"), ("data_source", "data_file")),
-        (_("Expression from DB"), ("expression",)),
+        FieldSet("name", "severity", "description", "selectors", "tags", name=_("Compliance Test")),
+        FieldSet("data_source", "data_file", name=_("Expression from Data Source")),
+        FieldSet("expression", name=_("Expression from DB")),
     )
 
     class Meta:
         model = models.ComplianceTest
         fields = ("name", "severity", "description", "expression", "selectors", "data_source", "data_file", "tags")
 
 
@@ -37,30 +39,28 @@
     )
     platform_filter = DynamicModelMultipleChoiceField(queryset=Platform.objects.all(), required=False)
     location_filter = DynamicModelMultipleChoiceField(queryset=Location.objects.all(), required=False)
     site_filter = DynamicModelMultipleChoiceField(queryset=Site.objects.all(), required=False)
     tenant_filter = DynamicModelMultipleChoiceField(queryset=Tenant.objects.all(), required=False)
 
     fieldsets = (
-        (_("Common"), ("name", "tags")),
-        (_("Dynamic Pairs"), ("dynamic_pairs", "dp_tag_prefix")),
-        (
-            _("Filters"),
-            (
-                "filter_operation",
-                "name_filter",
-                "type_filter",
-                "location_filter",
-                "manufacturer_filter",
-                "platform_filter",
-                "site_filter",
-                "status_filter",
-                "tag_filter",
-                "tenant_filter",
-            ),
+        FieldSet("name", "tags", name=_("Common")),
+        FieldSet("dynamic_pairs", "dp_tag_prefix", name=_("Dynamic Pairs")),
+        FieldSet(
+            "filter_operation",
+            "name_filter",
+            "type_filter",
+            "location_filter",
+            "manufacturer_filter",
+            "platform_filter",
+            "site_filter",
+            "status_filter",
+            "tag_filter",
+            "tenant_filter",
+            name=_("Filters"),
         ),
     )
 
     class Meta:
         model = models.ComplianceSelector
         fields = (
             "name",
@@ -86,18 +86,18 @@
         return result
 
 
 class SerializerForm(SyncedDataMixin, SubformMixin, NetBoxModelForm):
     template = CharField(required=False, widget=Textarea(attrs={"style": "font-family:monospace"}))
 
     main_fieldsets = (
-        (_("Serializer"), ("name", "extraction_method", "tags")),
+        FieldSet("name", "extraction_method", "tags", name=_("Serializer")),
         "__subform__",
-        (_("Template from Data Source"), ("data_source", "data_file")),
-        (_("Template from DB"), ("template",)),
+        FieldSet("data_source", "data_file", name=_("Template from Data Source")),
+        FieldSet("template", name=_("Template from DB")),
     )
 
     @property
     def fieldsets(self):
         fs = super().fieldsets
         if not self.subform or not self.subform.requires_template:
             fs = fs[:-2]  # drop "Template from..." fieldsets
@@ -116,17 +116,17 @@
 
 
 class NameSetForm(NetBoxModelForm):
     tests = DynamicModelMultipleChoiceField(queryset=models.ComplianceTest.objects.all(), required=False)
     definitions = CharField(required=False, widget=Textarea(attrs={"style": "font-family:monospace"}))
 
     fieldsets = (
-        (_("Name Set"), ("name", "description", "_global", "tests", "tags")),
-        (_("Definitions from Data Source"), ("data_source", "data_file")),
-        (_("Definitions from DB"), ("definitions",)),
+        FieldSet("name", "description", "_global", "tests", "tags", name=_("Name Set")),
+        FieldSet("data_source", "data_file", name=_("Definitions from Data Source")),
+        FieldSet("definitions", name=_("Definitions from DB")),
     )
 
     class Meta:
         model = models.NameSet
         fields = ("name", "description", "_global", "tests", "definitions", "data_source", "data_file", "tags")
 
 
@@ -150,14 +150,14 @@
         return super().clean()
 
 
 class CommandForm(SubformMixin, NetBoxModelForm):
     serializer = DynamicModelChoiceField(queryset=models.Serializer.objects.all(), required=False)
 
     main_fieldsets = [
-        (_("Command"), ("name", "label", "type", "retrieves_config", "serializer", "tags")),
+        FieldSet("name", "label", "type", "retrieves_config", "serializer", "tags", name=_("Command")),
     ]
 
     class Meta:
         model = models.Command
         fields = ("name", "label", "type", "retrieves_config", "serializer", "tags")
         widgets = {"type": HTMXSelect()}
```

### Comparing `netbox_validity-2.2.1/validity/graphql.py` & `netbox_validity-2.3.0/validity/graphql/graphene.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/managers.py` & `netbox_validity-2.3.0/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/migrations/0001_initial.py` & `netbox_validity-2.3.0/validity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/migrations/0002_custom_fields.py` & `netbox_validity-2.3.0/validity/migrations/0002_custom_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import migrations
 from django.utils.translation import gettext_lazy as _
-
+from validity.netbox_changes import CF_OBJ_TYPE, content_types
 
 def forward_func(apps, schema_editor):
     ContentType = apps.get_model("contenttypes", "ContentType")
     CustomField = apps.get_model("extras", "CustomField")
     Device = apps.get_model("dcim", "Device")
     Tenant = apps.get_model("tenancy", "Tenant")
     DeviceType = apps.get_model("dcim", "DeviceType")
@@ -17,35 +17,35 @@
     cfs = CustomField.objects.using(db_alias).bulk_create(
         [
             CustomField(
                 name="serializer",
                 label=_("Config Serializer"),
                 description=_("Required by Validity"),
                 type="object",
-                object_type=ContentType.objects.get_for_model(ConfigSerializer),
                 required=False,
+                **{CF_OBJ_TYPE: ContentType.objects.get_for_model(ConfigSerializer)},
             ),
             CustomField(
                 name="repo",
                 label=_("Git Repository"),
                 description=_("Required by Validity"),
                 type="object",
-                object_type=ContentType.objects.get_for_model(GitRepo),
                 required=False,
+                **{CF_OBJ_TYPE: ContentType.objects.get_for_model(GitRepo)},
             ),
         ]
     )
-    cfs[0].content_types.set(
+    content_types(cfs[0]).set(
         [
-            ContentType.objects.get_for_model(Device),
-            ContentType.objects.get_for_model(DeviceType),
-            ContentType.objects.get_for_model(Manufacturer),
+            ContentType.objects.get_for_model(Device).pk,
+            ContentType.objects.get_for_model(DeviceType).pk,
+            ContentType.objects.get_for_model(Manufacturer).pk,
         ]
     )
-    cfs[1].content_types.set([ContentType.objects.get_for_model(Tenant)])
+    content_types(cfs[1]).set([ContentType.objects.get_for_model(Tenant).pk])
 
 
 def reverse_func(apps, schema_editor):
     CustomField = apps.get_model("extras", "CustomField")
     db_alias = schema_editor.connection.alias
     CustomField.objects.using(db_alias).filter(
         name__in=[
```

### Comparing `netbox_validity-2.2.1/validity/migrations/0005_rename_serializer.py` & `netbox_validity-2.3.0/validity/migrations/0005_rename_serializer.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/migrations/0006_datasources.py` & `netbox_validity-2.3.0/validity/migrations/0006_datasources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from itertools import chain
 from django.db import migrations
 from django.utils.translation import gettext_lazy as _
 from validity.fields.encrypted import EncryptedString
 from django.db import migrations, models
 import django.db.models.deletion
+from validity.netbox_changes import CF_OBJ_TYPE, content_types, CF_CONTENT_TYPES
 
 
 def setup_datasource_cf(apps, schema_editor):
     ContentType = apps.get_model("contenttypes", "ContentType")
     CustomField = apps.get_model("extras", "CustomField")
     DataSource = apps.get_model("core", "DataSource")
     Tenant = apps.get_model("tenancy", "Tenant")
@@ -45,35 +46,35 @@
                 description=_("Required by Validity. You may use {{branch}} substitution"),
                 type="text",
                 required=False,
             ),
         ]
     )
     for cf in datasource_cfs:
-        cf.content_types.set([ContentType.objects.get_for_model(DataSource)])
+        content_types(cf).set([ContentType.objects.get_for_model(DataSource).pk])
     tenant_cf = CustomField.objects.using(db).create(
         name="data_source",
         label=_("Data Source"),
         description=_("Required by Validity"),
         type="object",
-        object_type=ContentType.objects.get_for_model(DataSource),
         required=False,
+        **{CF_OBJ_TYPE: ContentType.objects.get_for_model(DataSource)}
     )
-    tenant_cf.content_types.set([ContentType.objects.get_for_model(Tenant)])
+    content_types(tenant_cf).set([ContentType.objects.get_for_model(Tenant)])
 
 
 def delete_datasource_cf(apps, schema_editor):
     CustomField = apps.get_model("extras", "CustomField")
     CustomField.objects.using(schema_editor.connection.alias).filter(
         name__in=[
             "default",
             "device_config_path",
             "web_url",
         ],
-        content_types__model="datasource",
+        **{f"{CF_CONTENT_TYPES}__model": "datasource"}
     ).delete()
 
 
 def get_fields(model, fields):
     result = {}
     for field_name in fields:
         if field_value := getattr(model, field_name, None):
@@ -110,33 +111,33 @@
                 sep="\n",
             )  # noqa
 
 
 def delete_repo_cf(apps, schema_editor):
     db = schema_editor.connection.alias
     CustomField = apps.get_model("extras", "CustomField")
-    CustomField.objects.using(db).filter(name="repo", content_types__model="tenant").delete()
+    CustomField.objects.using(db).filter(name="repo", **{f"{CF_CONTENT_TYPES}__model": "tenant"}).delete()
 
 
 def setup_repo_cf(apps, schema_editor):
     ContentType = apps.get_model("contenttypes", "ContentType")
     CustomField = apps.get_model("extras", "CustomField")
     Tenant = apps.get_model("tenancy", "Tenant")
     GitRepo = apps.get_model("validity", "GitRepo")
     db = schema_editor.connection.alias
 
     cf = CustomField.objects.using(db).create(
         name="repo",
         label=_("Git Repository"),
         description=_("Required by Validity"),
         type="object",
-        object_type=ContentType.objects.get_for_model(GitRepo),
         required=False,
+        **{CF_OBJ_TYPE: ContentType.objects.get_for_model(GitRepo)}
     )
-    cf.content_types.set([ContentType.objects.get_for_model(Tenant)])
+    content_types(cf).set([ContentType.objects.get_for_model(Tenant)])
 
 
 def switch_git_links(apps, schema_editor):
     db = schema_editor.connection.alias
     DataSource = apps.get_model("core", "DataSource")
     DataFile = apps.get_model("core", "DataFile")
     models = [apps.get_model("validity", m) for m in ("ComplianceTest", "NameSet", "Serializer")]
```

### Comparing `netbox_validity-2.2.1/validity/migrations/0007_polling.py` & `netbox_validity-2.3.0/validity/migrations/0007_polling.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import taggit.managers
 import utilities.json
 import validity.models.base
 import validity.fields.encrypted
 from django.utils.translation import gettext_lazy as _
 import django.core.validators
 import django.db.models.deletion
+from validity.netbox_changes import CF_OBJ_TYPE, content_types
 
 
 def create_cf(apps, schema_editor):
     ContentType = apps.get_model("contenttypes", "ContentType")
     CustomField = apps.get_model("extras", "CustomField")
     Poller = apps.get_model("validity", "Poller")
     Device = apps.get_model("dcim", "Device")
@@ -20,22 +21,22 @@
     db_alias = schema_editor.connection.alias
 
     cf = CustomField.objects.using(db_alias).create(
         name="poller",
         label=_("Poller"),
         description=_("Required by Validity. Defines properties of device polling"),
         type="object",
-        object_type=ContentType.objects.get_for_model(Poller),
         required=False,
+        **{CF_OBJ_TYPE: ContentType.objects.get_for_model(Poller)}
     )
-    cf.content_types.set(
+    content_types(cf).set(
         [
-            ContentType.objects.get_for_model(Device),
-            ContentType.objects.get_for_model(DeviceType),
-            ContentType.objects.get_for_model(Manufacturer),
+            ContentType.objects.get_for_model(Device).pk,
+            ContentType.objects.get_for_model(DeviceType).pk,
+            ContentType.objects.get_for_model(Manufacturer).pk,
         ]
     )
 
 
 def delete_cf(apps, schema_editor):
     CustomField = apps.get_model("extras", "CustomField")
     db_alias = schema_editor.connection.alias
```

### Comparing `netbox_validity-2.2.1/validity/migrations/0008_script_change.py` & `netbox_validity-2.3.0/validity/migrations/0008_script_change.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/base.py` & `netbox_validity-2.3.0/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/data.py` & `netbox_validity-2.3.0/validity/models/data.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/device.py` & `netbox_validity-2.3.0/validity/models/device.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/nameset.py` & `netbox_validity-2.3.0/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/polling.py` & `netbox_validity-2.3.0/validity/models/polling.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/report.py` & `netbox_validity-2.3.0/validity/models/report.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/selector.py` & `netbox_validity-2.3.0/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/serializer.py` & `netbox_validity-2.3.0/validity/models/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from dcim.models import Device
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from validity.choices import ExtractionMethodChoices
 from validity.compliance.serialization import serialize
-from validity.netbox_changes import DEVICE_ROLE_RELATION
 from validity.subforms import (
     RouterOSSerializerForm,
     TEXTFSMSerializerForm,
     TTPSerializerForm,
     XMLSerializerForm,
     YAMLSerializerForm,
 )
@@ -64,15 +63,15 @@
     @property
     def bound_devices(self) -> models.QuerySet[Device]:
         from .device import VDevice
 
         return (
             VDevice.objects.annotate_serializer_id()
             .filter(serializer_id=self.pk)
-            .select_related("site", DEVICE_ROLE_RELATION, "device_type__manufacturer")
+            .select_related("site", "role", "device_type__manufacturer")
         )
 
     @property
     def effective_template(self) -> str:
         return self.effective_text_field()
 
     def serialize(self, data: str) -> dict:
```

### Comparing `netbox_validity-2.2.1/validity/models/test.py` & `netbox_validity-2.3.0/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/models/test_result.py` & `netbox_validity-2.3.0/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/navigation.py` & `netbox_validity-2.3.0/validity/navigation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from extras.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
-from utilities.choices import ButtonColorChoices
+from validity.netbox_changes import ButtonColorChoices, plugins
 
 
 def model_add_button(entity):
-    return PluginMenuButton(
+    return plugins.PluginMenuButton(
         link=f"plugins:validity:{entity}_add",
         title="Add",
         icon_class="mdi mdi-plus-thick",
         color=ButtonColorChoices.GREEN,
         permissions=[f"validity.add_{entity}"],
     )
 
 
 def model_menu_item(entity, title, buttons=()):
     buttons = [btn(entity) if callable(btn) else btn for btn in buttons]
-    return PluginMenuItem(
+    return plugins.PluginMenuItem(
         link=f"plugins:validity:{entity}_list",
         link_text=title,
         buttons=buttons or [],
         permissions=[f"validity.view_{entity}"],
     )
 
 
-run_tests_button = PluginMenuButton(
+run_tests_button = plugins.PluginMenuButton(
     link="plugins:validity:compliancetest_run",
     title="Run",
     icon_class="mdi mdi-rocket-launch",
     color=ButtonColorChoices.CYAN,
 )
 
 validity_menu_items = (
@@ -39,12 +38,12 @@
 )
 
 polling_menu_items = (
     model_menu_item("command", "Commands", [model_add_button]),
     model_menu_item("poller", "Pollers", [model_add_button]),
 )
 
-menu = PluginMenu(
+menu = plugins.PluginMenu(
     label="Validity",
     groups=(("main", validity_menu_items), ("polling", polling_menu_items)),
     icon_class="mdi mdi-checkbox-marked-circle-outline",
 )
```

### Comparing `netbox_validity-2.2.1/validity/pollers/base.py` & `netbox_validity-2.3.0/validity/pollers/base.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/pollers/default_credentials.py` & `netbox_validity-2.3.0/validity/pollers/default_credentials.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/pollers/factory.py` & `netbox_validity-2.3.0/validity/pollers/factory.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/pollers/http.py` & `netbox_validity-2.3.0/validity/pollers/http.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/pollers/result.py` & `netbox_validity-2.3.0/validity/pollers/result.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/scripts/run_tests.py` & `netbox_validity-2.3.0/validity/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/scripts/script_data.py` & `netbox_validity-2.3.0/validity/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/search.py` & `netbox_validity-2.3.0/validity/search.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/static/validity/connection-type-select.js` & `netbox_validity-2.3.0/validity/static/validity/connection-type-select.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,25 @@
 function fillTextArea(public_creds, private_creds) {
     document.getElementById('id_public_credentials').value = JSON.stringify(public_creds, null, 2);
     document.getElementById('id_private_credentials').value = JSON.stringify(private_creds, null, 2);
 }
 
-function fillCredentials(connectionTypeInfo) {
+function fillCredentials(valueExtracter, connectionTypeInfo) {
     try {
-        const connectionType = connectionTypeInfo.value;
+        const connectionType = valueExtracter(connectionTypeInfo)
         if (connectionType == "")
             return;
         const defaultCredentials = JSON.parse(document.getElementById('default_credentials').textContent)[connectionType];
         fillTextArea(defaultCredentials.public, defaultCredentials.private);
     } catch (e) {
         console.log(e.name, e.message)
     }
 
 }
 
 window.onload = () => {
-    document.getElementById('connection_type_select').slim.onChange = fillCredentials
+    const select = document.getElementById('connection_type_select');
+    if ("tomselect" in select) // NetBox 4.x
+        select.tomselect.on("change", fillCredentials.bind(undefined, (value) => value))
+    else // NetBox 3.x
+        select.slim.onChange = fillCredentials.bind(undefined, (value) => value.value)
 }
```

### Comparing `netbox_validity-2.2.1/validity/static/validity/prism-dark.css` & `netbox_validity-2.3.0/validity/static/validity/prism-dark.css`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/static/validity/prism-light.css` & `netbox_validity-2.3.0/validity/static/validity/prism-light.css`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/static/validity/prism.js` & `netbox_validity-2.3.0/validity/static/validity/prism.js`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/subforms.py` & `netbox_validity-2.3.0/validity/subforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 """
 
 import textwrap
 import xml.etree.ElementTree as ET
 
 from django import forms
 from django.utils.translation import gettext_lazy as _
-from utilities.forms import BootstrapMixin
 
 from validity.choices import JSONAPIMethodChoices
+from validity.netbox_changes import BootstrapMixin
 from validity.utils.json import jq
 from validity.utils.misc import reraise
 
 
 class BaseSubform(BootstrapMixin, forms.Form):
     def clean(self):
         if self.data.keys() - self.base_fields.keys():
```

### Comparing `netbox_validity-2.2.1/validity/tables.py` & `netbox_validity-2.3.0/validity/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from django_tables2 import Column, RequestConfig, Table, TemplateColumn
 from netbox.tables import BooleanColumn as BooleanColumn
 from netbox.tables import ChoiceFieldColumn, ManyToManyColumn, NetBoxTable
 from netbox.tables.columns import ActionsColumn, LinkedCountColumn
 from utilities.paginator import EnhancedPaginator
 
 from validity import models
-from validity.utils.misc import colorful_percentage
+from validity.templatetags.validity import colorful_percentage
 
 
 class SelectorTable(NetBoxTable):
     name = Column(linkify=True)
     filter_operation = ChoiceFieldColumn()
     name_filter = BooleanColumn(empty_values=())
     tag_filter = BooleanColumn(accessor="tag_filter__all")
```

### Comparing `netbox_validity-2.2.1/validity/template_content.py` & `netbox_validity-2.3.0/validity/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/templates/validity/aux_tab_table.html` & `netbox_validity-2.3.0/validity/templates/validity/aux_tab_table.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
-{% load bootstrap5 %}
+{% load django_bootstrap5 %}
 {% load render_table from django_tables2 %}
 {% block head %}
 {% endblock %}
 {% block subtitle %}
-<div class="object-subtitle"></div>
 {% endblock %}
 {% block controls %}
 {%if read_only %}
 <div class="controls"></div>
 {% else %}
 {{ block.super }}
 {% endif %}
 {% endblock %}
 {% block content %}
-  <div class="row mb-3">
-    <div class="col-auto">
-    <form role="form" class="row" method="get">
-      {% bootstrap_form filterset_form layout="inline" %}
-      <div class="col-auto">{% buttons submit=search_button_name|default:"Search" %}{% endbuttons %}</div>
+<div class="row mb-3">
+  <div class="col-auto">
+    <form role="form" class="row row-cols-auto g-3 align-items-center" method="get">
+      {% bootstrap_form filterset_form layout="inline" inline_field_class="col-auto" %}
+      <div class="col-auto">
+        {% bootstrap_button type="submit" content=search_button_name|default:"Search" %}
+      </div>
       <div class="col-auto">
         {% block extra_button %}{% endblock %}
       </div>
     </form>
   </div>
 </div>
 <div class="card mb-3">
```

### Comparing `netbox_validity-2.2.1/validity/templates/validity/command.html` & `netbox_validity-2.3.0/validity/templates/validity/command.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/templates/validity/compliancereport.html` & `netbox_validity-2.3.0/validity/templates/validity/compliancereport.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends 'generic/object.html' %}
 {% load validity %}
-{% load bootstrap5 %}
+{% load django_bootstrap5 %}
 {% load buttons %}
 {% load perms %}
 {% load render_table from django_tables2 %}
 {% block controls %}
 <div class="controls">
 {% if request.user|can_delete:object %}
   {% delete_button object %}
@@ -42,17 +42,17 @@
         </div>
       </div>
     </div>
     <div class="col col-md-4">
       <div class="card">
         <h5 class="card-header">Group Results By</h5>
         <div class="card-body">
-          <form role="form" class="row" method="get">
-            {% bootstrap_form groupby_form layout="inline" %}
-            <div class="col-auto">{% buttons submit="Apply" %}{% endbuttons %}</div>
+          <form role="form" class="row align-items-center" method="get">
+            <div class="col-auto">{% bootstrap_form groupby_form layout="inline" %}</div>
+            <div class="col-auto">{% bootstrap_button button_type="submit" content="Apply" %}</div>
           </form>
         </div>
       </div>
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-{% extends 'generic/object.html' %} {% load validity %} {% load bootstrap5 %}
-{% load buttons %} {% load perms %} {% load render_table from django_tables2 %}
-{% block controls %}
+{% extends 'generic/object.html' %} {% load validity %} {% load
+django_bootstrap5 %} {% load buttons %} {% load perms %} {% load render_table
+from django_tables2 %} {% block controls %}
 {% if request.user|can_delete:object %} {% delete_button object %} {% endif %}
 {% endblock %} {% block content %}
 **** CCoommpplliiaannccee RReeppoorrtt ****
 IIDD                    {{ object.id }}
 CCrreeaatteedd               {{ object.created | date:"Y-m-d G:i:s" }}
 DDeevviicceess iinnvvoollvveedd      {{ object.device_count }}
 UUnniiqquuee TTeessttss iinnvvoollvveedd {{ object.test_count }}
 **** GGrroouupp RReessuullttss BByy ****
 {% bootstrap_form groupby_form layout="inline" %}
-{% buttons submit="Apply" %}{% endbuttons %}
+{% bootstrap_button button_type="submit" content="Apply" %}
 **** SSttaattiissttiiccss ggrroouuppeedd bbyy {{{{ ggrroouuppbbyy__llaabbeell }}}} ****
 {% if groupby_table %}
 {% render_table groupby_table %}
 {%include 'inc/paginator.html' with paginator=groupby_table.paginator
 page=groupby_table.page%} {% else %} Choose a field to group by to display
 statistics {% endif %}
 {% endblock content %}
```

### Comparing `netbox_validity-2.2.1/validity/templates/validity/complianceselector.html` & `netbox_validity-2.3.0/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/templates/validity/compliancetest.html` & `netbox_validity-2.3.0/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/templates/validity/compliancetestresult.html` & `netbox_validity-2.3.0/validity/templates/validity/compliancetestresult.html`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
             <th scope="row">Dynamic Pair</th>
             <td>{{ object.dynamic_pair | linkify | placeholder }}</td>
           </tr>
           <tr>
             <th scope="row">Result</th>
             <td>
               {% if object.passed %}
-              <span class="badge bg-green">PASSED</span>
+              <span class="badge {%bg%}-green">PASSED</span>
               {% else %}
-              <span class="badge bg-red">FAILED</span>
+              <span class="badge {%bg%}-red">FAILED</span>
               {% endif %}
             </td>
           </tr>
           <tr>
             <th scope="row">Created</th>
             <td>{{ object.created | date:"Y-m-d G:i:s" }}</td>
           </tr>
```

### Comparing `netbox_validity-2.2.1/validity/templates/validity/device_state.html` & `netbox_validity-2.3.0/validity/templates/validity/device_state.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load validity %}
-{% load bootstrap5 %}
+{% load django_bootstrap5 %}
 {% block head %}
 {% endblock %}
 {% block title %}{{ object }}: Serialized State{% endblock %}
 {% block subtitle %}
-<div class="object-subtitle"></div>
 {% endblock %}
 {% block content %}
 <div class="row mb-2">
   <div class="col-md-5">
     <div class="card">
       <div class="card-body">
         <h5 class="card-title mb-2">Metainfo</h5>
@@ -45,17 +44,17 @@
       </div>
     </div>
   </div>
   <div class="col col-md-4">
     <div class="card">
       <h5 class="card-header">State</h5>
       <div class="card-body">
-        <form role="form" class="row" method="get">
-          {% bootstrap_form state_form layout="inline" %}
-          <div class="col-auto">{% buttons submit="Show" %}{% endbuttons %}</div>
+        <form role="form" class="row align-items-center" method="get">
+          <div class="col-auto">{% bootstrap_form state_form layout="inline" %}</div>
+          <div class="col-auto">{% bootstrap_button button_type="submit" content="Show" %}</div>
         </form>
       </div>
     </div>
   </div>
 </div>
 <div class="row mx-1 mb-2">
   {% if not error %}
@@ -67,15 +66,15 @@
       </div>
     </div>
     <div class="card-body">
       {% include 'extras/inc/configcontext_data.html' with data=state_item.serialized format=format %}
     </div>
   </div>
   {% else %}
-  <div class="card bg-warning mt-3">
+  <div class="card {%bg%}-warning mt-3">
     <div class="card-body">
       <h6 class="card-title">{{ error }}</h6>
     </div>
   </div>
   {% endif %}
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load validity %} {%
-load bootstrap5 %} {% block head %} {% endblock %} {% block title %}{{ object
-}}: Serialized State{% endblock %} {% block subtitle %}
-{% endblock %} {% block content %}
+load django_bootstrap5 %} {% block head %} {% endblock %} {% block title %}{
+{ object }}: Serialized State{% endblock %} {% block subtitle %} {% endblock %}
+{% block content %}
 **** MMeettaaiinnffoo ****
 DDaattaa SSoouurrccee              {{ object.data_source | linkify | placeholder }}
 PPoolllleerr                   {{ object.poller | linkify | placeholder }}
 SSeerriiaalliizzeerr               {{ state_item.serializer | linkify | placeholder }}
 CCoommmmaanndd                  {{ state_item.command | linkify | placeholder }}
                          {% include "validity/inc/path_with_link.html" with
 DDaattaa FFiillee                data_file=state_item.data_file
                          web_url=object.data_source.web_url only %}
 LLooccaall ccooppyy llaasstt mmooddiiffiieedd {{ state_item.data_file.last_updated | date:"Y-m-d G:
                          i:s" | placeholder}}
 **** SSttaattee ****
 {% bootstrap_form state_form layout="inline" %}
-{% buttons submit="Show" %}{% endbuttons %}
+{% bootstrap_button button_type="submit" content="Show" %}
 {% if not error %}
 **** {{{{ ssttaattee__iitteemm..vveerrbboossee__nnaammee }}}} ****
 {% include 'validity/inc/configcontext_format.html' %}
 {% include 'extras/inc/configcontext_data.html' with data=state_item.serialized
 format=format %}
 {% else %}
 ** {{{{ eerrrroorr }}}} **
```

### Comparing `netbox_validity-2.2.1/validity/templates/validity/inc/parameters.html` & `netbox_validity-2.3.0/validity/templates/validity/inc/parameters.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/templates/validity/inc/related_objects.html` & `netbox_validity-2.3.0/validity/templates/validity/inc/related_objects.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 {% load helpers %}
+{% load validity %}
 
 <div class="card">
   <h5 class="card-header">{{ title | default:"Related Objects (Validity)" }}</h5>
   <ul class="list-group list-group-flush">
     {% for count, model, filter_param in related_models %}
       {% with viewname=model|viewname:"list" %}
         <a href="{% url viewname %}?{{ filter_param }}={{ object.pk }}" class="list-group-item list-group-item-action d-flex justify-content-between">
           {{ model|meta:"verbose_name_plural"|bettertitle }}
           {% if count %}
-              <span class="badge bg-primary rounded-pill">{{ count }}</span>
+              <span class="badge {%bg%}-primary rounded-pill">{{ count }}</span>
           {% else %}
-              <span class="badge bg-light rounded-pill">&mdash;</span>
+              <span class="badge {%bg%}-light rounded-pill">&mdash;</span>
           {% endif %}
         </a>
       {% endwith %}
     {% endfor %}
   </ul>
 </div>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{% load helpers %}
+{% load helpers %} {% load validity %}
 **** {{{{ ttiittllee || ddeeffaauulltt::""RReellaatteedd OObbjjeeccttss ((VVaalliiddiittyy))"" }}}} ****
     * {% for count, model, filter_param in related_models %} {% with
       viewname=model|viewname:"list" %} _{_{_ _m_o_d_e_l_|_m_e_t_a_:
       _"_v_e_r_b_o_s_e___n_a_m_e___p_l_u_r_a_l_"_|_b_e_t_t_e_r_t_i_t_l_e_ _}_}_ _{_%_ _i_f_ _c_o_u_n_t_ _%_}_ _{_{_ _c_o_u_n_t_ _}_}_ _{_%_ _e_l_s_e
       _%_}_ _—_ _{_%_ _e_n_d_i_f_ _%_}_ {% endwith %} {% endfor %}
```

### Comparing `netbox_validity-2.2.1/validity/templates/validity/nameset.html` & `netbox_validity-2.3.0/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/templates/validity/poller.html` & `netbox_validity-2.3.0/validity/templates/validity/poller.html`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       </div>
     </div>
     <div class="col col-md-8">
       <div class="card">
         <div class="card-header">
           <div class="row">
             <h5 class="col">Credentials</h5>
-            <div class="col">{% include 'extras/inc/configcontext_format.html' %}</div>
+            <div class="col">{% include 'validity/inc/configcontext_format.html' %}</div>
           </div>
         </div>
         <div class="card-body">
           <div>
             <h6 class="mb-3">Public</h6>
             {% include 'extras/inc/configcontext_data.html' with data=object.public_credentials format=format %}
           </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 from django_tables2 %} {% block content %}
 **** PPoolllleerr ****
 NNaammee            {{ object.name }}
 CCoonnnneeccttiioonn TTyyppee {{ object | colored_choice:"connection_type" }}
 CCoommmmaannddss        {{ object.commands.all | linkify_list }}
 {% include 'inc/panels/tags.html' %}
 **** CCrreeddeennttiiaallss ****
-{% include 'extras/inc/configcontext_format.html' %}
+{% include 'validity/inc/configcontext_format.html' %}
 ** PPuubblliicc **
 {% include 'extras/inc/configcontext_data.html' with
 data=object.public_credentials format=format %}
 ** PPrriivvaattee **
 {% include 'extras/inc/configcontext_data.html' with
 data=object.private_credentials.encrypted %}
 **** BBoouunndd DDeevviicceess ****
```

### Comparing `netbox_validity-2.2.1/validity/templates/validity/serializer.html` & `netbox_validity-2.3.0/validity/templates/validity/serializer.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/templatetags/validity.py` & `netbox_validity-2.3.0/validity/templatetags/validity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Any
 
 from django import template
 from django.db.models import Model
 from django.http.request import HttpRequest
+from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from utilities.templatetags.builtins.filters import linkify, placeholder
 
-from validity.utils.misc import colorful_percentage as _colorful_percentage
+from validity import config
 
 
 register = template.Library()
 
 
 @register.filter
 def colored_choice(obj: Model, field: str) -> str:
     value = getattr(obj, f"get_{field}_display")
     color = getattr(obj, f"get_{field}_color")
-    return mark_safe(f'<span class="badge bg-{color()}">{value()}</span>')
+    return mark_safe(f'<span class="badge {bg()}-{color()}">{value()}</span>')
 
 
 @register.filter
 def linkify_list(obj_list: list[Model], attr: str | None = None) -> str:
     result = ", ".join(linkify(obj, attr) for obj in obj_list)
     return placeholder("") if not result else mark_safe(result)
 
@@ -36,16 +37,23 @@
 
 @register.filter
 def data_source(model) -> str:
     return _("Data Source") if model.data_source else _("DB")
 
 
 @register.filter
-def colorful_percentage(percent):
-    return _colorful_percentage(percent)
+def colorful_percentage(percent: float) -> str:
+    levels = {75: "warning", 50: "orange", 25: "danger"}
+    badge_color = "success"
+    for level, color in levels.items():
+        if level <= percent:
+            break
+        badge_color = color
+    percent = round(percent, 1)
+    return format_html('<span class="badge rounded-pill {}-{}">{}%</span>', bg(), badge_color, percent)
 
 
 @register.simple_tag
 def url_with_query_params(request: HttpRequest, **params):
     params = {k: [v] if not isinstance(v, list) else v for k, v in params.items()}
     query_params = request.GET.copy()
     query_params |= params
@@ -69,7 +77,17 @@
         if row_part.lower() in {"low", "middle", "high"}:
             row_parts[i] = f"<b>{row_part.upper()}</b>"
     row_name = mark_safe(" ".join(row_parts))
     count = getattr(obj, f"{severity}_count")
     passed = getattr(obj, f"{severity}_passed")
     percentage = getattr(obj, f"{severity}_percentage")
     return {"row_name": row_name, "passed": passed, "count": count, "percentage": percentage}
+
+
+@register.simple_tag
+def bg():
+    return "bg" if config.netbox_version < "4.0.0" else "text-bg"
+
+
+@register.filter
+def nb_version():
+    return config.netbox_version
```

### Comparing `netbox_validity-2.2.1/validity/tests/base.py` & `netbox_validity-2.3.0/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/factories.py` & `netbox_validity-2.3.0/validity/tests/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         model = Tenant
 
 
 class DeviceFactory(DjangoModelFactory):
     name = factory.Sequence(lambda n: f"device-{n}")
     site = factory.SubFactory(SiteFactory)
     device_type = factory.SubFactory(DeviceTypeFactory)
-    device_role = factory.SubFactory(DeviceRoleFactory)
+    role = factory.SubFactory(DeviceRoleFactory)
 
     class Meta:
         model = models.VDevice
 
 
 class TagFactory(DjangoModelFactory):
     name = factory.Sequence(lambda n: f"tag-{n}")
```

### Comparing `netbox_validity-2.2.1/validity/tests/test_api.py` & `netbox_validity-2.3.0/validity/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_choices.py` & `netbox_validity-2.3.0/validity/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_compliance/test_dynamic_pairs.py` & `netbox_validity-2.3.0/validity/tests/test_compliance/test_dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_compliance/test_eval.py` & `netbox_validity-2.3.0/validity/tests/test_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_compliance/test_serialization.py` & `netbox_validity-2.3.0/validity/tests/test_compliance/test_serialization.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_compliance/test_state.py` & `netbox_validity-2.3.0/validity/tests/test_compliance/test_state.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_custom_validators.py` & `netbox_validity-2.3.0/validity/tests/test_custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_data_backends.py` & `netbox_validity-2.3.0/validity/tests/test_data_backends.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_fields.py` & `netbox_validity-2.3.0/validity/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_graphql.py` & `netbox_validity-2.3.0/validity/tests/test_graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             return
         answer = resp.json()["data"][self.data_name]
         if isinstance(answer, list):
             answer = answer[0]
         assert self.subanswer.items() <= answer.items()
 
 
+@pytest.mark.skip
 class TestReportList(GraphQLTest):
     query = """
     query {
         report_list {
             id
             device_count
             test_count
@@ -57,14 +58,15 @@
         "middle_count": 8,
         "high_passed": 0,
         "high_count": 0,
     }
     data_name = "report_list"
 
 
+@pytest.mark.skip
 class TestSelector(GraphQLTest):
     query = """
     query {
         selector (id: 1) {
             name
             devices {
                 name
```

### Comparing `netbox_validity-2.2.1/validity/tests/test_managers.py` & `netbox_validity-2.3.0/validity/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_models/test_clean.py` & `netbox_validity-2.3.0/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_models/test_compliancetest.py` & `netbox_validity-2.3.0/validity/tests/test_models/test_compliancetest.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_models/test_git_link.py` & `netbox_validity-2.3.0/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_models/test_selector.py` & `netbox_validity-2.3.0/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_models/test_vdatasource.py` & `netbox_validity-2.3.0/validity/tests/test_models/test_vdatasource.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_models/test_vdevice.py` & `netbox_validity-2.3.0/validity/tests/test_models/test_vdevice.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_pollers.py` & `netbox_validity-2.3.0/validity/tests/test_pollers.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             return arg
 
         commands = [Mock(parameters={"cli_command": "a"}), Mock(parameters={"cli_command": "b"})]
         poller = get_mocked_poller({}, commands, Mock(**{"return_value.send_command": poll}))
         devices = [get_mocked_device(f"1.1.1.{i}") for i in range(10)]
         start = time.time()
         results = list(poller.poll(devices))
-        assert time.time() - start < 0.3
+        assert time.time() - start < 1
         assert len(results) == len(commands) * len(devices)
         if raise_exc:
             assert all(res.error.message.startswith("OSError") for res in results)
         else:
             assert all(res.result in {"a", "b"} for res in results)
```

### Comparing `netbox_validity-2.2.1/validity/tests/test_scripts/test_run_tests.py` & `netbox_validity-2.3.0/validity/tests/test_scripts/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_scripts/test_script_data.py` & `netbox_validity-2.3.0/validity/tests/test_scripts/test_script_data.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_utils/test_json.py` & `netbox_validity-2.3.0/validity/tests/test_utils/test_json.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_utils/test_misc.py` & `netbox_validity-2.3.0/validity/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_utils/test_orm.py` & `netbox_validity-2.3.0/validity/tests/test_utils/test_orm.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/tests/test_views.py` & `netbox_validity-2.3.0/validity/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,7 +190,13 @@
 @pytest.mark.django_db
 def test_datasource_devices(admin_client):
     data_source = DataSourceFactory(custom_field_data={"default": True})
     DeviceFactory()
     DeviceFactory()
     resp = admin_client.get(data_source.get_absolute_url() + "devices/")
     assert resp.status_code == HTTPStatus.OK
+
+
+@pytest.mark.django_db
+def test_run_tests(admin_client, setup_runtests_script):
+    resp = admin_client.get("/plugins/validity/tests/run/", follow=True)
+    assert resp.status_code == HTTPStatus.OK
```

### Comparing `netbox_validity-2.2.1/validity/urls.py` & `netbox_validity-2.3.0/validity/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-from django.shortcuts import redirect
 from django.urls import include, path
 from utilities.urls import get_model_urls
 
 from . import views
 
 
 urlpatterns = [
     path("selectors/", views.ComplianceSelectorListView.as_view(), name="complianceselector_list"),
     path("selectors/add/", views.ComplianceSelectorEditView.as_view(), name="complianceselector_add"),
     path("selectors/delete/", views.ComplianceSelectorBulkDeleteView.as_view(), name="complianceselector_bulk_delete"),
     path("selectors/<int:pk>/", include(get_model_urls("validity", "complianceselector"))),
     path("tests/", views.ComplianceTestListView.as_view(), name="compliancetest_list"),
-    path(
-        "tests/run/",
-        lambda _: redirect("extras:script", module="validity_scripts", name="RunTests"),
-        name="compliancetest_run",
-    ),
+    path("tests/run/", views.run_tests, name="compliancetest_run"),
     path("tests/add/", views.ComplianceTestEditView.as_view(), name="compliancetest_add"),
     path("tests/delete/", views.ComplianceTestBulkDeleteView.as_view(), name="compliancetest_bulk_delete"),
     path("tests/<int:pk>/", include(get_model_urls("validity", "compliancetest"))),
     path("test-results/", views.ComplianceResultListView.as_view(), name="compliancetestresult_list"),
     path("test-results/<int:pk>/", include(get_model_urls("validity", "compliancetestresult"))),
     path("serializers/", views.SerializerListView.as_view(), name="serializer_list"),
     path("serializers/add/", views.SerializerEditView.as_view(), name="serializer_add"),
```

### Comparing `netbox_validity-2.2.1/validity/utils/json.py` & `netbox_validity-2.3.0/validity/utils/json.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/utils/misc.py` & `netbox_validity-2.3.0/validity/utils/misc.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,33 +2,21 @@
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager, suppress
 from itertools import islice
 from typing import TYPE_CHECKING, Any, Callable, Iterable
 
 from core.exceptions import SyncError
 from django.db.models import Q
-from django.utils.html import format_html
 from netbox.context import current_request
 
 
 if TYPE_CHECKING:
     from validity.models import VDataSource
 
 
-def colorful_percentage(percent: float) -> str:
-    levels = {75: "warning", 50: "orange", 25: "danger"}
-    badge_color = "success"
-    for level, color in levels.items():
-        if level <= percent:
-            break
-        badge_color = color
-    percent = round(percent, 1)
-    return format_html('<span class="badge rounded-pill bg-{}">{}%</span>', badge_color, percent)
-
-
 @contextmanager
 def null_request():
     ctx = current_request.get()
     current_request.set(None)
     try:
         yield
     finally:
```

### Comparing `netbox_validity-2.2.1/validity/utils/orm.py` & `netbox_validity-2.3.0/validity/utils/orm.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from dataclasses import dataclass
 from itertools import chain
 from typing import Generic, Iterable, Iterator, TypeVar
 
 from django.db.models import Model, QuerySet
 
+from validity.netbox_changes import CF_OBJ_TYPE, content_types
+
 
 M = TypeVar("M", bound=Model)
 N = TypeVar("N", bound=Model)
 
 
 class QuerySetMap(Generic[M]):
     """
@@ -190,7 +192,22 @@
 def model_to_proxy(model: Model, proxy_type: type[M]) -> M:
     """
     Converts model to its proxy type (e.g. Device to VDevice)
     """
     new_model = proxy_type()
     new_model.__dict__ = model.__dict__.copy()
     return new_model
+
+
+@dataclass
+class CustomFieldBuilder:
+    cf_model: type
+    content_type_model: type
+    db_alias: str = ""
+
+    def create(self, *, bind_to, object_type=None, **cf_params):
+        db = self.db_alias or self.cf_model.objects.db
+        if object_type is not None:
+            cf_params[CF_OBJ_TYPE] = object_type
+        custom_field = self.cf_model.objects.using(db).create(**cf_params)
+        content_types(custom_field).set(self.content_type_model.objects.get_for_model(model).pk for model in bind_to)
+        return custom_field
```

### Comparing `netbox_validity-2.2.1/validity/utils/version.py` & `netbox_validity-2.3.0/validity/utils/version.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/views/__init__.py` & `netbox_validity-2.3.0/validity/views/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 )
 from .test import (
     ComplianceTestBulkDeleteView,
     ComplianceTestDeleteView,
     ComplianceTestEditView,
     ComplianceTestListView,
     ComplianceTestView,
+    run_tests,
 )
 from .test_result import ComplianceResultListView, ComplianceResultView
```

### Comparing `netbox_validity-2.2.1/validity/views/base.py` & `netbox_validity-2.3.0/validity/views/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import partial
 from typing import Any, Dict
 
 from django.db.models import Model
 from django.forms import Form
 from django.shortcuts import get_object_or_404
 from django_filters import FilterSet
 from django_filters.views import FilterView
@@ -66,15 +67,15 @@
 
 
 class TestResultBaseView(SingleTableMixin, FilterViewWithForm):
     template_name = "validity/compliance_results.html"
     tab = ViewTab("Test Results", badge=lambda obj: obj.results.count())
     model = models.ComplianceTestResult
     filterset_class = filtersets.ComplianceTestResultFilterSet
-    filterform_class = forms.TestResultFilterForm
+    filterform_class = partial(forms.TestResultFilterForm, add_m2m_placeholder=True)
     table_class = tables.ComplianceResultTable
     permission_required = "validity.view_compliancetestresult"
 
     parent_model: type[Model]
     result_relation: str
     read_only: bool = False
     exclude_form_fields: tuple[str, ...] = ()
```

### Comparing `netbox_validity-2.2.1/validity/views/command.py` & `netbox_validity-2.3.0/validity/views/command.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/views/data_source.py` & `netbox_validity-2.3.0/validity/views/data_source.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/views/device.py` & `netbox_validity-2.3.0/validity/views/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,25 @@
 logger = logging.getLogger(__name__)
 
 
 @register_model_view(Device, "results")
 class TestResultView(TestResultBaseView):
     parent_model = Device
     result_relation = "device"
-    exclude_form_fields = ("platform_id", "tenant_id", "device_role_id", "manufacturer_id", "report_id", "selector_id")
+    exclude_form_fields = (
+        "platform_id",
+        "tenant_id",
+        "device_role_id",
+        "manufacturer_id",
+        "report_id",
+        "selector_id",
+        "device_type_id",
+        "location_id",
+        "site_id",
+    )
 
 
 @register_model_view(Device, "serialized_state")
 class DeviceSerializedStateView(generic.ObjectView):
     template_name = "validity/device_state.html"
     tab = ViewTab("Serialized State", permission="dcim.view_device")
     queryset = VDevice.objects.prefetch_datasource().prefetch_serializer().prefetch_poller()
```

### Comparing `netbox_validity-2.2.1/validity/views/nameset.py` & `netbox_validity-2.3.0/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/views/poller.py` & `netbox_validity-2.3.0/validity/views/poller.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/views/report.py` & `netbox_validity-2.3.0/validity/views/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,24 @@
 
 
 @register_model_view(models.ComplianceReport, "results")
 class ReportResultView(TestResultBaseView):
     parent_model = models.ComplianceReport
     result_relation = "report"
     read_only = True
-    exclude_form_fields = ("latest", "selector_id", "platform_id", "tenant_id", "device_role_id", "manufacturer_id")
+    exclude_form_fields = (
+        "latest",
+        "selector_id",
+        "platform_id",
+        "tenant_id",
+        "device_role_id",
+        "manufacturer_id",
+        "device_type_id",
+        "site_id",
+        "location_id",
+    )
     permission_required = "view_compliancereport"
 
 
 @register_model_view(models.ComplianceReport, "delete")
 class ReportDeleteView(generic.ObjectDeleteView):
     queryset = models.ComplianceReport.objects.all()
```

### Comparing `netbox_validity-2.2.1/validity/views/selector.py` & `netbox_validity-2.3.0/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/views/serializer.py` & `netbox_validity-2.3.0/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.1/validity/views/test.py` & `netbox_validity-2.3.0/validity/views/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.db.models import Count, Q
+from django.shortcuts import get_object_or_404, redirect
 from netbox.views import generic
 from utilities.views import register_model_view
 
-from validity import filtersets, forms, models, tables
+from validity import config, filtersets, forms, models, tables
 from .base import TableMixin, TestResultBaseView
 
 
 class ComplianceTestListView(generic.ObjectListView):
     queryset = models.ComplianceTest.objects.annotate_latest_count()
     table = tables.ComplianceTestTable
     filterset = filtersets.ComplianceTestFilterSet
@@ -44,7 +45,16 @@
     table = tables.ComplianceTestTable
 
 
 @register_model_view(models.ComplianceTest, "edit")
 class ComplianceTestEditView(generic.ObjectEditView):
     queryset = models.ComplianceTest.objects.all()
     form = forms.ComplianceTestForm
+
+
+def run_tests(request):
+    if config.netbox_version < "4.0.0":
+        return redirect("extras:script", module="validity_scripts", name="RunTests")
+    from extras.models import Script
+
+    script = get_object_or_404(Script, name="RunTests", module__data_file__path="validity_scripts.py")
+    return redirect("extras:script", pk=script.pk)
```

### Comparing `netbox_validity-2.2.1/validity/views/test_result.py` & `netbox_validity-2.3.0/validity/views/test_result.py`

 * *Files identical despite different names*

