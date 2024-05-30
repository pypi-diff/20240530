# Comparing `tmp/lsst_daf_butler-27.2024.2100.tar.gz` & `tmp/lsst_daf_butler-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_daf_butler-27.2024.2100.tar", last modified: Thu May 23 10:23:11 2024, max compression
+gzip compressed data, was "lsst_daf_butler-27.2024.2200.tar", last modified: Thu May 30 10:11:32 2024, max compression
```

## Comparing `lsst_daf_butler-27.2024.2100.tar` & `lsst_daf_butler-27.2024.2200.tar`

### file list

```diff
@@ -1,461 +1,463 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.346766 lsst_daf_butler-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-23 10:23:11.346766 lsst_daf_butler-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.266765 lsst_daf_butler-27.2024.2100/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.274765 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/
--rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/concreteStorageClasses.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/datastores.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/dimensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/formatters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/organizing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/use-in-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/writing-subcommands.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.270765 lsst_daf_butler-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.274765 lsst_daf_butler-27.2024.2100/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.274765 lsst_daf_butler-27.2024.2100/python/lsst/daf/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.282765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75170 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_instance_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_column_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_column_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_config_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_existence.py
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_deferredDatasetHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_exceptions_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_file_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_file_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_labeled_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_limited_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_named.py
--rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_quantum_backed.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_registry_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_storage_class_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)    23377 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.282765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/locked_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/named_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/thread_safe_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/arrow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.282765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cliLog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.282765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/_remove_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/_remove_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.282765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/optionGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/column_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.286765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastore.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.286765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/composites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/formatters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/dimensions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.286765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/storageClasses.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.286765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57480 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    34999 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/file_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/generic_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/record_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/stored_file_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.290765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/chainedDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)   120549 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/fileDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/fileDatastoreClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.290765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/file_datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/file_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/file_datastore/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/inMemoryDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/ddl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.290765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrowastropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrownumpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrownumpydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrowtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.294765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    55578 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_governor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22884 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    20940 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_record_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_record_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19925 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_skypix.py
--rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/construction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.294765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_butler/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100744 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_butler/_direct_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.294765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58712 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_query_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.298766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/astropyTable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/mapping_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/name_shrinker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/persistence_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/pydantic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.298766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_data_coordinate_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_dataset_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_dimension_record_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_expression_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/convert_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/expression_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/overlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/result_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.302765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    16403 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_query_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.306765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_caching_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_record_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_summary_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_dataset_type_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    60859 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_registry_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.306765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/bridge/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/bridge/monolithic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.306765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27734 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/nameKey.py
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/synthIntKey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/connectionString.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.306765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25550 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/databases/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/databases/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.306765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.310765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    51063 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.310765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54687 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/dimensions/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.310765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    26746 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    79984 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_opaque.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/nameShrinker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.314766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/default_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/pgsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/opaque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.314766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    33980 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36701 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_sql_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.314766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/categorize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.318765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.318765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/find_first_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   114911 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/sql_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.318765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64445 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/tests/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)   186202 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/tests/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/wildcards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.322765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_collection_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_http_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_query_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_ref_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18508 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    22666 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_remote_butler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.322765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/_query_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/_query_data_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.322765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.322765 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_query_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/repo_relocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.326766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/_pruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/butlerImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/certifyCalibrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/collectionChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/configDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/configValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/createRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/exportCalibs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/ingest_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/register_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/removeCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/removeDatasetType.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/removeRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/retrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/transferDatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.330766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_datasetsHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_dummyRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_examplePythonTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    40160 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/butler_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/cliCmdTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/cliLogTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/deferredFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/dict_convertible_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14769 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/hybrid_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/hybrid_butler_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/server_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/testFormatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24302 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/timespan_database_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.330766 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    32431 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:23:11.000000 lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.346766 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-23 10:23:11.000000 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-23 10:23:11.000000 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:23:11.000000 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 10:23:11.000000 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 10:23:11.000000 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:23:11.000000 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:23:10.000000 lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-23 10:23:11.346766 lsst_daf_butler-27.2024.2100/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:23:11.346766 lsst_daf_butler-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_astropyTableFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)   128241 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdAssociate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdConfigDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdConfigValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdCreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdIngestFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdPruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdRemoveCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdRemoveRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliCmdRetrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliPluginLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliUtilSplitCommas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliUtilSplitKv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliUtilToUpper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_cliUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_composites.py
--rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_connectionString.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    84810 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_dimension_record_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    45224 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_exprParserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_exprParserYacc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_logFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_matplotlibFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_normalFormExpression.py
--rw-r--r--   0 runner    (1001) docker     (127)    27146 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    87941 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_pydantic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_quantumBackedButler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_query_direct_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_query_direct_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    90454 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_query_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_query_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_query_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    24404 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_query_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_remote_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    38408 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_simpleButler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_storageClass.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-23 10:23:05.000000 lsst_daf_butler-27.2024.2100/tests/test_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.871721 lsst_daf_butler-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-30 10:11:32.871721 lsst_daf_butler-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.787721 lsst_daf_butler-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.795721 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/
+-rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/concreteStorageClasses.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/datastores.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/dimensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/formatters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/organizing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/use-in-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/writing-subcommands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.791721 lsst_daf_butler-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.795721 lsst_daf_butler-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.795721 lsst_daf_butler-27.2024.2200/python/lsst/daf/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.803721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75170 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_instance_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_column_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_column_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_config_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_existence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_deferredDatasetHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_exceptions_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_file_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_file_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_labeled_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_limited_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_named.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_quantum_backed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_registry_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_storage_class_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23377 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.807721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/locked_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/named_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/thread_safe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/arrow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.807721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cliLog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.807721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/_remove_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/_remove_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.807721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/optionGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/column_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.807721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastore.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.811721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/composites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/formatters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/dimensions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.811721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/storageClasses.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.815721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57480 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34999 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/file_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/generic_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/record_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/stored_file_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.815721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/chainedDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120549 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/fileDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/fileDatastoreClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.815721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/file_datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/file_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/file_datastore/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/inMemoryDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/ddl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.815721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrowastropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrownumpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrownumpydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrowtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.819721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55578 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_governor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22884 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20940 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_record_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19925 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_skypix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.819721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100744 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_butler/_direct_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.823721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54473 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_query_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_result_page_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.823721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/astropyTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/mapping_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/name_shrinker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/persistence_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/pydantic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.827721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_data_coordinate_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_dataset_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_dimension_record_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_expression_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/convert_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/expression_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/result_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.827721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16403 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23244 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_query_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.831721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_caching_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_record_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_summary_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_dataset_type_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60859 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_registry_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.831721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/bridge/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/bridge/monolithic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.831721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27734 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/nameKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/synthIntKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/connectionString.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.831721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25550 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/databases/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/databases/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.831721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.835721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52543 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.835721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54687 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/dimensions/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.835721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26746 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79984 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_opaque.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/nameShrinker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.839721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/default_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/pgsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/opaque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.839721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33980 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32311 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_sql_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.843721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/categorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.843721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.843721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/find_first_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114870 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/sql_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.843721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64445 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/tests/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189306 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/tests/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/wildcards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.847721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_collection_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_http_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_query_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_ref_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21093 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22666 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_remote_butler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.847721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/_query_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/_query_data_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/_query_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.847721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.847721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_query_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/repo_relocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.851721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/_pruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/butlerImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/certifyCalibrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/collectionChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/configDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/configValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/createRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/exportCalibs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/ingest_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/register_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/removeCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/removeDatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/removeRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/retrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/transferDatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.855721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_datasetsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_dummyRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_examplePythonTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/butler_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/cliCmdTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/cliLogTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/deferredFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/dict_convertible_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14769 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/hybrid_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/hybrid_butler_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/testFormatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24302 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/timespan_database_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.855721 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32431 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.871721 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:11:32.000000 lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 10:11:32.871721 lsst_daf_butler-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:11:32.871721 lsst_daf_butler-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_astropyTableFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128241 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdAssociate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdConfigDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdConfigValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdCreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdIngestFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdPruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdRemoveCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdRemoveRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliCmdRetrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliPluginLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliUtilSplitCommas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliUtilSplitKv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliUtilToUpper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_cliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_connectionString.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84810 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_ddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_dimension_record_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45224 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_exprParserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_exprParserYacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_logFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_matplotlibFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_normalFormExpression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27146 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87941 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_pydantic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_quantumBackedButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_query_direct_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_query_direct_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_query_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_query_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_query_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24404 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_query_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_remote_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38408 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_simpleButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_storageClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-30 10:11:26.000000 lsst_daf_butler-27.2024.2200/tests/test_versioning.py
```

### Comparing `lsst_daf_butler-27.2024.2100/PKG-INFO` & `lsst_daf_butler-27.2024.2200/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_daf_butler-27.2024.2100/README.md` & `lsst_daf_butler-27.2024.2200/README.md`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/bsd_license.txt` & `lsst_daf_butler-27.2024.2200/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/CHANGES.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/concreteStorageClasses.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/concreteStorageClasses.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/configuring.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/configuring.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/datastores.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/datastores.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/dimensions.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/dimensions.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/formatters.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/formatters.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/index.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/organizing.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/organizing.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/queries.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/queries.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/use-in-tests.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/use-in-tests.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/doc/lsst.daf.butler/writing-subcommands.rst` & `lsst_daf_butler-27.2024.2200/doc/lsst.daf.butler/writing-subcommands.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/gpl-v3.0.txt` & `lsst_daf_butler-27.2024.2200/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/pyproject.toml` & `lsst_daf_butler-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_collections.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_config.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_instance_options.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_instance_options.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_butler_repo_index.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_butler_repo_index.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_column_categorization.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_column_categorization.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_column_tags.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_column_tags.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_column_type_info.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_column_type_info.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_config.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_config_support.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_config_support.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_association.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_association.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_existence.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_existence.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_ref.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_ref.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_dataset_type.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_dataset_type.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_deferredDatasetHandle.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_deferredDatasetHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_exceptions.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,24 @@
     """
 
     def __init__(self, detail: str):
         return super().__init__(detail)
 
 
 class CalibrationLookupError(LookupError, ButlerUserError):
-    """Exception raised for failures to look up a calibration dataset."""
+    """Exception raised for failures to look up a calibration dataset.
+
+    For a find-first query involving a calibration dataset to work, either the
+    query's result rows need to include a temporal dimension or needs to be
+    constrained temporally, such that each result row corresponds to a unique
+    calibration dataset.  This exception can be raised if those dimensions or
+    constraint are missing, or if a temporal dimension timespan overlaps
+    multiple validity ranges (e.g. the recommended bias changes in the middle
+    of an exposure).
+    """
 
     error_type = "calibration_lookup"
 
 
 class CollectionCycleError(ValueError, ButlerUserError):
     """Raised when an operation would cause a chained collection to be a child
     of itself.
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_exceptions_legacy.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_exceptions_legacy.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_file_dataset.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_file_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_file_descriptor.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_file_descriptor.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_formatter.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_labeled_butler_factory.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_labeled_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_limited_butler.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_location.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_location.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_named.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_named.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_quantum.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_quantum.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_quantum_backed.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_quantum_backed.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_registry_shim.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_registry_shim.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_storage_class.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_storage_class.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_storage_class_delegate.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_storage_class_delegate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_timespan.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_timespan.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_topology.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_topology.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/locked_object.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/locked_object.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/named_locks.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/named_locks.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/_utilities/thread_safe_cache.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/_utilities/thread_safe_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/arrow_utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/butler.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cliLog.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cliLog.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/_remove_collections.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/_remove_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/_remove_runs.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/_remove_runs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/cmd/commands.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/arguments.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/optionGroups.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/optionGroups.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/opt/options.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/progress.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/progress.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/cli/utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/column_spec.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/column_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,34 @@
 from lsst.sphgeom import Region
 
 from . import arrow_utils, ddl
 from ._timespan import Timespan
 from .name_shrinker import NameShrinker
 
 ColumnType: TypeAlias = Literal[
-    "int", "string", "hash", "float", "datetime", "bool", "uuid", "timespan", "region"
+    "int",
+    "string",
+    "hash",
+    "float",
+    "datetime",
+    "bool",
+    "uuid",
+    "timespan",
+    "region",
+    # The ingest_date column in the datasets table can be one of two column
+    # types:
+    # 1. TIMESTAMP column (which is not used anywhere else in the DB)
+    # 2. Integer nanoseconds TAI (same as "datetime" column type)
+    # Which it is depends on the database schema in use for the "datasets"
+    # manager.  (v1 is TIMESTAMP, v2 is integer).  See makeStaticTableSpecs in
+    # lsst.daf.butler.registry.datasets.byDimensions.tables.
+    #
+    # We don't know which it is until we go to resolve the query against
+    # a database, so it has to be its own data type.
+    "ingest_date",
 ]
 
 
 COLLECTION_NAME_MAX_LENGTH = 64
 # TODO: DM-42541 would bee a good opportunity to move this constant to a
 # better home; this file is the least-bad home I can think of for now.  Note
 # that actually changing the value is a (minor) schema change.
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/composites.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/composites.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/formatters.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/formatters.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/dimensions.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/dimensions.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/registry.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/registry.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/configs/storageClasses.yaml` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/configs/storageClasses.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/_datastore.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/_datastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/cache_manager.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/cache_manager.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/composites.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/composites.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/constraints.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/constraints.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/file_templates.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/file_templates.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/generic_base.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/generic_base.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/record_data.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/record_data.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastore/stored_file_info.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastore/stored_file_info.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/chainedDatastore.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/chainedDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/fileDatastore.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/fileDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/fileDatastoreClient.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/fileDatastoreClient.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/file_datastore/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/file_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/file_datastore/get.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/file_datastore/get.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/datastores/inMemoryDatastore.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/datastores/inMemoryDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/ddl.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/ddl.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrowastropy.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrowastropy.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrownumpy.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrownumpy.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrownumpydict.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrownumpydict.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/arrowtable.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/arrowtable.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/delegates/dataframe.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/delegates/dataframe.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_config.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_coordinate.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_coordinate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_database.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_database.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_elements.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_elements.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_governor.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_governor.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_graph.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_group.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_group.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_packer.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_packer.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_record_set.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_record_set.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_record_table.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_record_table.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_records.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_records.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_schema.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_skypix.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_skypix.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/_universe.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/_universe.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/construction.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/construction.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/dimensions/record_cache.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/dimensions/record_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_butler/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_butler/_direct_butler.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_butler/_direct_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_driver.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,23 +39,15 @@
 from typing import TYPE_CHECKING, Any, cast, overload
 
 import sqlalchemy
 
 from .. import ddl
 from .._dataset_type import DatasetType
 from .._exceptions import InvalidQueryError
-from ..dimensions import (
-    DataCoordinate,
-    DataIdValue,
-    DimensionGroup,
-    DimensionRecordSet,
-    DimensionUniverse,
-    SkyPixDimension,
-)
-from ..name_shrinker import NameShrinker
+from ..dimensions import DataCoordinate, DataIdValue, DimensionGroup, DimensionUniverse
 from ..queries import tree as qt
 from ..queries.driver import (
     DataCoordinateResultPage,
     DatasetRefResultPage,
     DimensionRecordResultPage,
     GeneralResultPage,
     PageKey,
@@ -77,14 +69,20 @@
 from ._query_plan import (
     QueryFindFirstPlan,
     QueryJoinsPlan,
     QueryPlan,
     QueryProjectionPlan,
     ResolvedDatasetSearch,
 )
+from ._result_page_converter import (
+    DataCoordinateResultPageConverter,
+    DatasetRefResultPageConverter,
+    DimensionRecordResultPageConverter,
+    ResultPageConverter,
+)
 from ._sql_column_visitor import SqlColumnVisitor
 
 if TYPE_CHECKING:
     from ..registry.interfaces import Database
 
 
 _LOG = logging.getLogger(__name__)
@@ -218,27 +216,38 @@
         else:
             raw_page_size = self._raw_page_size
         # Execute the query by initializing a _Cursor object that manages the
         # lifetime of the result.
         cursor = _Cursor(
             self.db,
             sql_select,
-            result_spec=result_spec,
-            name_shrinker=builder.joiner.name_shrinker,
             postprocessing=builder.postprocessing,
             raw_page_size=raw_page_size,
-            column_order=builder.columns.get_column_order(),
+            page_converter=self._create_result_page_converter(result_spec, builder),
         )
         result_page = cursor.next()
         if result_page.next_key is not None:
             # Cursor has not been exhausted; add it to the driver for use by
             # fetch_next_page.
             self._cursors[result_page.next_key] = cursor
         return result_page
 
+    def _create_result_page_converter(self, spec: ResultSpec, builder: QueryBuilder) -> ResultPageConverter:
+        match spec:
+            case DimensionRecordResultSpec():
+                return DimensionRecordResultPageConverter(spec, self.db)
+            case DataCoordinateResultSpec():
+                return DataCoordinateResultPageConverter(spec, builder.columns.get_column_order())
+            case DatasetRefResultSpec():
+                return DatasetRefResultPageConverter(
+                    spec, self.get_dataset_type(spec.dataset_type_name), builder.columns.get_column_order()
+                )
+            case _:
+                raise NotImplementedError(f"Result type '{spec.result_type}' not yet implemented")
+
     @overload
     def fetch_next_page(
         self, result_spec: DataCoordinateResultSpec, key: PageKey
     ) -> DataCoordinateResultPage: ...
 
     @overload
     def fetch_next_page(
@@ -1081,46 +1090,35 @@
 
     Parameters
     ----------
     db : `.registry.interface.Database`
         Database to run the query against.
     sql : `sqlalchemy.Executable`
         SQL query to execute.
-    result : `ResultSpec`
-        Specification of the result type.
-    name_shrinker : `NameShrinker` or `None`
-        Object that was used to shrink dataset column names to fit within the
-        database identifier limit.
     postprocessing : `Postprocessing`
         Post-query filtering and checks to perform.
     raw_page_size : `int`
         Maximum number of SQL result rows to return in each page, before
         postprocessing.
-    column_order : `ColumnOrder`
-        Definition of the columns available in the rows returned by the SQL
-        query.
+    page_converter : `ResultPageConverter`
+        Object for converting raw SQL result rows into ResultPage instances.
     """
 
     def __init__(
         self,
         db: Database,
         sql: sqlalchemy.Executable,
-        result_spec: ResultSpec,
-        name_shrinker: NameShrinker | None,
         postprocessing: Postprocessing,
         raw_page_size: int,
-        column_order: qt.ColumnOrder,
+        page_converter: ResultPageConverter,
     ):
-        self._result_spec = result_spec
-        self._name_shrinker = name_shrinker
         self._raw_page_size = raw_page_size
         self._postprocessing = postprocessing
-        self._timespan_repr_cls = db.getTimespanRepresentation()
         self._context = db.query(sql, execution_options=dict(yield_per=raw_page_size))
-        self._column_order = column_order
+        self._page_converter = page_converter
         cursor = self._context.__enter__()
         try:
             self._iterator = cursor.partitions()
         except:  # noqa: E722
             self._context.__exit__(*sys.exc_info())
             raise
 
@@ -1157,116 +1155,11 @@
                 # always fetching the next page up front.
                 next_key = uuid.uuid4()
             else:
                 next_key = None
                 self.close()
 
             postprocessed_rows = self._postprocessing.apply(raw_page)
-            match self._result_spec:
-                case DimensionRecordResultSpec():
-                    return self._convert_dimension_record_results(postprocessed_rows, next_key)
-                case DataCoordinateResultSpec():
-                    return self._convert_data_coordinate_results(postprocessed_rows, next_key)
-                case _:
-                    raise NotImplementedError("TODO")
+            return self._page_converter.convert(postprocessed_rows, next_key)
         except:  # noqa: E722
             self._context.__exit__(*sys.exc_info())
             raise
-
-    def _convert_dimension_record_results(
-        self,
-        raw_rows: Iterable[sqlalchemy.Row],
-        next_key: PageKey | None,
-    ) -> DimensionRecordResultPage:
-        """Convert a raw SQL result iterable into a page of `DimensionRecord`
-        query results.
-
-        Parameters
-        ----------
-        raw_rows : `~collections.abc.Iterable` [ `sqlalchemy.Row` ]
-            Iterable of SQLAlchemy rows, with `Postprocessing` filters already
-            applied.
-        next_key : `PageKey` or `None`
-            Key for the next page to add into the returned page object.
-
-        Returns
-        -------
-        result_page : `DimensionRecordResultPage`
-            Page object that holds a `DimensionRecord` container.
-        """
-        result_spec = cast(DimensionRecordResultSpec, self._result_spec)
-        record_set = DimensionRecordSet(result_spec.element)
-        record_cls = result_spec.element.RecordClass
-        if isinstance(result_spec.element, SkyPixDimension):
-            pixelization = result_spec.element.pixelization
-            id_qualified_name = qt.ColumnSet.get_qualified_name(result_spec.element.name, None)
-            for raw_row in raw_rows:
-                pixel_id = raw_row._mapping[id_qualified_name]
-                record_set.add(record_cls(id=pixel_id, region=pixelization.pixel(pixel_id)))
-        else:
-            # Mapping from DimensionRecord attribute name to qualified column
-            # name, but as a list of tuples since we'd just iterate over items
-            # anyway.
-            column_map = list(
-                zip(
-                    result_spec.element.schema.dimensions.names,
-                    result_spec.element.dimensions.names,
-                )
-            )
-            for field in result_spec.element.schema.remainder.names:
-                if field != "timespan":
-                    column_map.append(
-                        (field, qt.ColumnSet.get_qualified_name(result_spec.element.name, field))
-                    )
-            if result_spec.element.temporal:
-                timespan_qualified_name = qt.ColumnSet.get_qualified_name(
-                    result_spec.element.name, "timespan"
-                )
-            else:
-                timespan_qualified_name = None
-            for raw_row in raw_rows:
-                m = raw_row._mapping
-                d = {k: m[v] for k, v in column_map}
-                if timespan_qualified_name is not None:
-                    d["timespan"] = self._timespan_repr_cls.extract(m, name=timespan_qualified_name)
-                record_set.add(record_cls(**d))
-        return DimensionRecordResultPage(spec=result_spec, next_key=next_key, rows=record_set)
-
-    def _convert_data_coordinate_results(
-        self,
-        raw_rows: Iterable[sqlalchemy.Row],
-        next_key: PageKey | None,
-    ) -> DataCoordinateResultPage:
-        """Convert a raw SQL result iterable into a page of `DataCoordinate`
-        query results.
-
-        Parameters
-        ----------
-        spec : `DataCoordinateResultSpec`
-            Specification for the output values.
-        raw_rows : `~collections.abc.Iterable` [ `sqlalchemy.Row` ]
-            Iterable of SQLAlchemy rows, with `Postprocessing` filters already
-            applied.
-        next_key : `PageKey` or `None`
-            Key for the next page to add into the returned page object.
-
-        Returns
-        -------
-        result_page : `DataCoordinateResultPage`
-            Page object that holds a `DataCoordinate` container.
-        """
-        spec = self._result_spec
-        assert isinstance(spec, DataCoordinateResultSpec)
-
-        dimensions = spec.dimensions
-        column_order = self._column_order
-        assert (
-            list(dimensions.data_coordinate_keys) == column_order.dimension_key_names
-        ), "Dimension keys in result row should be in same order as those specified by the result spec"
-
-        rows = [
-            DataCoordinate.from_full_values(
-                dimensions, tuple(column_order.extract_dimension_key_columns(row))
-            )
-            for row in raw_rows
-        ]
-        return DataCoordinateResultPage(spec=spec, rows=rows, next_key=next_key)
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_postprocessing.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_postprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 from collections.abc import Iterable, Iterator
 from typing import TYPE_CHECKING, ClassVar
 
 import sqlalchemy
 from lsst.sphgeom import DISJOINT, Region
 
-from ..queries import ValidityRangeMatchError
+from .._exceptions import CalibrationLookupError
 from ..queries import tree as qt
 
 if TYPE_CHECKING:
     from ..dimensions import DimensionElement
 
 
 class Postprocessing:
@@ -79,15 +79,15 @@
     non-overlap pair will be filtered out.
     """
 
     check_validity_match_count: bool
     """If `True`, result rows will include a special column that counts the
     number of matching datasets in each collection for each data ID, and
     postprocessing should check that the value of this column is one for
-    every row (and raise `.queries.ValidityRangeMatchError` if it is not).
+    every row (and raise `CalibrationLookupError` if it is not).
     """
 
     @property
     def limit(self) -> int | None:
         """The maximum number of rows to return, or `None` for no limit.
 
         This is only set when other postprocess filtering makes it impossible
@@ -198,15 +198,15 @@
         for row in rows:
             m = row._mapping
             if any(m[a].relate(m[b]) & DISJOINT for a, b in joins) or any(
                 m[field].relate(region) & DISJOINT for field, region in where
             ):
                 continue
             if self.check_validity_match_count and m[self.VALIDITY_MATCH_COUNT] > 1:
-                raise ValidityRangeMatchError(
+                raise CalibrationLookupError(
                     "Ambiguous calibration validity range match. This usually means a temporal join or "
                     "'where' needs to be added, but it could also mean that multiple validity ranges "
                     "overlap a single output data ID."
                 )
             yield row
             if self._limit is not None:
                 self._limit -= 1
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_query_builder.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_query_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_query_plan.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_query_plan.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 __all__ = ("SqlColumnVisitor",)
 
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy
 
 from .. import ddl
+from .._exceptions import InvalidQueryError
 from ..queries import tree as qt
 from ..queries.visitors import ColumnExpressionVisitor, PredicateVisitFlags, PredicateVisitor
 from ..timespan_database_representation import TimespanDatabaseRepresentation
 
 if TYPE_CHECKING:
     from ._driver import DirectQueryDriver
     from ._query_builder import QueryJoiner
@@ -146,14 +147,22 @@
                 # Spatial overlaps should be transformed away by now.
                 raise AssertionError(
                     f"Unexpected types {a.column_type},{b.column_type} in overlaps operator."
                 )
 
         lhs = self.expect_scalar(a)
         rhs = self.expect_scalar(b)
+        # Special case to handle awkward situation where ingest_date is not
+        # always the same type as other datetime columns.
+        if qt.is_one_datetime_and_one_ingest_date(a, b):
+            if a.column_type == "datetime":
+                lhs = self._convert_datetime_to_ingest_date(a)
+            elif b.column_type == "datetime":
+                rhs = self._convert_datetime_to_ingest_date(b)
+
         match operator:
             case "==":
                 return lhs == rhs
             case "!=":
                 return lhs != rhs
             case "<":
                 return lhs < rhs
@@ -265,11 +274,30 @@
         return sqlalchemy.not_(result)
 
     def expect_scalar(self, expression: qt.OrderExpression) -> sqlalchemy.ColumnElement[Any]:
         result = expression.visit(self)
         assert isinstance(result, sqlalchemy.ColumnElement)
         return result
 
+    def _convert_datetime_to_ingest_date(self, expression: qt.ColumnExpression) -> sqlalchemy.ColumnElement:
+        assert expression.column_type == "datetime"
+        if self._driver.managers.datasets.ingest_date_dtype() == sqlalchemy.TIMESTAMP:
+            # Datasets manager v1 schema has "datasets" table's "ingest_date"
+            # column as TIMESTAMP, but the rest of the database schema and
+            # query system uses integer TAI nanoseconds.  So we have to convert
+            # the nanoseconds value to a timestamp.
+            # Note that this loses precision.
+            if expression.expression_type != "datetime":
+                # Conversion between TAI and UTC can't be done in the database,
+                # so we are only able to handle literal values here.
+                raise InvalidQueryError("Only literal date-time values can be compared with ingest date.")
+
+            return sqlalchemy.literal(expression.value.utc.to_datetime())
+        else:
+            # For v2 schema, ingest_date uses TAI nanoseconds like everything
+            # else, so no conversion is required.
+            return self.expect_scalar(expression)
+
     def expect_timespan(self, expression: qt.ColumnExpression) -> TimespanDatabaseRepresentation:
         result = expression.visit(self)
         assert isinstance(result, TimespanDatabaseRepresentation)
         return result
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/astropyTable.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/astropyTable.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/file.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/file.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/json.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/json.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/logs.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/logs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/matplotlib.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/matplotlib.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/packages.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/packages.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/parquet.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/parquet.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/pickle.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/pickle.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/formatters/yaml.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/formatters/yaml.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/json.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/json.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/logging.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/logging.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/mapping_factory.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/mapping_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/name_shrinker.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/name_shrinker.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/nonempty_mapping.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/persistence_context.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/persistence_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/progress.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/progress.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/pydantic_utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_base.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,41 +23,27 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
-__all__ = ("QueryBase", "QueryResultsBase", "ValidityRangeMatchError")
+__all__ = ("QueryBase", "QueryResultsBase")
 
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Mapping, Set
 from typing import Any, Self
 
 from ..dimensions import DataId, DimensionGroup
 from .convert_args import convert_order_by_args, convert_where_args
 from .driver import QueryDriver
 from .expression_factory import ExpressionProxy
 from .tree import OrderExpression, Predicate, QueryTree
 
 
-class ValidityRangeMatchError(RuntimeError):
-    """Exception raised when a find-first calibration dataset query does not
-    fully resolve validity ranges.
-
-    For a find-first query involving a calibration dataset to work, either the
-    query's result rows need to include a temporal dimension or needs to be
-    constrained temporally, such that each result row corresponds to a unique
-    calibration dataset.  This exception can be raised if those dimensions or
-    constraint are missing, or if a temporal dimension timespan overlaps
-    multiple validity ranges (e.g. the recommended bias changes in the middle
-    of an exposure).
-    """
-
-
 class QueryBase(ABC):
     """Common base class for `Query` and all `QueryResult` objects.
 
     This class should rarely be referenced directly; it is public only because
     it provides public methods to its subclasses.
 
     Parameters
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_data_coordinate_query_results.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_data_coordinate_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_dataset_query_results.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_dataset_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_dimension_record_query_results.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_dimension_record_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_expression_strings.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_expression_strings.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_identifiers.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_identifiers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/_query.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/_query.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/convert_args.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/convert_args.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/driver.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/driver.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/expression_factory.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/expression_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/overlaps.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/overlaps.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/result_specs.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/result_specs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_base.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_base.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_expression.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "ColumnExpression",
     "OrderExpression",
     "UnaryExpression",
     "BinaryExpression",
     "Reversed",
     "UnaryOperator",
     "BinaryOperator",
+    "is_one_datetime_and_one_ingest_date",
     "is_one_timespan_and_one_datetime",
     "validate_order_expression",
 )
 
 from typing import TYPE_CHECKING, Annotated, Literal, NamedTuple, TypeAlias, TypeVar, final
 
 import pydantic
@@ -235,15 +236,15 @@
         validator.
 
     Raises
     ------
     InvalidQueryError
         Raised if this expression is not one that can be used for sorting.
     """
-    if expression.column_type not in ("int", "string", "float", "datetime"):
+    if expression.column_type not in ("int", "string", "float", "datetime", "ingest_date"):
         raise InvalidQueryError(f"Column type {expression.column_type} of {expression} is not ordered.")
     return expression
 
 
 OrderExpression: TypeAlias = Annotated[
     _ColumnExpression | Reversed,
     pydantic.Field(discriminator="expression_type"),
@@ -270,7 +271,18 @@
     """
     if a.column_type == "timespan" and b.column_type == "datetime":
         return TimespanAndDatetime(a, b)
     elif a.column_type == "datetime" and b.column_type == "timespan":
         return TimespanAndDatetime(b, a)
     else:
         return None
+
+
+def is_one_datetime_and_one_ingest_date(
+    a: ColumnExpression, b: ColumnExpression
+) -> bool:  # numpydoc ignore=PR01
+    """Return `True` if the two columns ``a`` and `b`` include one datetime
+    column and one ingest_date column.
+    """
+    return (a.column_type == "datetime" and b.column_type == "ingest_date") or (
+        a.column_type == "ingest_date" and b.column_type == "datetime"
+    )
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_literal.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_literal.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,29 +29,32 @@
 
 __all__ = (
     "ColumnLiteral",
     "LiteralValue",
     "make_column_literal",
 )
 
+import datetime
 import uuid
 import warnings
 from base64 import b64decode, b64encode
 from functools import cached_property
 from typing import Literal, TypeAlias, Union, final
 
 import astropy.time
 import erfa
 from lsst.sphgeom import Region
 
 from ..._timespan import Timespan
 from ...time_utils import TimeConverter
 from ._base import ColumnLiteralBase
 
-LiteralValue: TypeAlias = int | str | float | bytes | uuid.UUID | astropy.time.Time | Timespan | Region
+LiteralValue: TypeAlias = (
+    int | str | float | bytes | uuid.UUID | astropy.time.Time | datetime.datetime | Timespan | Region
+)
 
 
 @final
 class IntColumnLiteral(ColumnLiteralBase):
     """A literal `int` value in a column expression."""
 
     expression_type: Literal["int"] = "int"
@@ -363,12 +366,14 @@
             return FloatColumnLiteral.from_value(value)
         case uuid.UUID():
             return UUIDColumnLiteral.from_value(value)
         case bytes():
             return HashColumnLiteral.from_value(value)
         case astropy.time.Time():
             return DateTimeColumnLiteral.from_value(value)
+        case datetime.date():
+            return DateTimeColumnLiteral.from_value(astropy.time.Time(value))
         case Timespan():
             return TimespanColumnLiteral.from_value(value)
         case Region():
             return RegionColumnLiteral.from_value(value)
     raise TypeError(f"Invalid type {type(value).__name__!r} of value {value!r} for column literal.")
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_reference.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,16 @@
     @property
     def column_type(self) -> ColumnType:
         # Docstring inherited.
         match self.field:
             case "dataset_id":
                 return "uuid"
             case "ingest_date":
-                return "datetime"
+                # See comment at definition of `ColumnType` type alias.
+                return "ingest_date"
             case "run":
                 return "string"
             case "collection":
                 return "string"
             case "timespan":
                 return "timespan"
         raise AssertionError(f"Invalid field {self.field!r} for dataset.")
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_column_set.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_column_set.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_predicate.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_predicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,19 @@
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Annotated, Literal, TypeAlias, TypeVar, cast, final
 
 import pydantic
 
 from ..._exceptions import InvalidQueryError
 from ._base import QueryTreeBase
-from ._column_expression import ColumnExpression, is_one_timespan_and_one_datetime
+from ._column_expression import (
+    ColumnExpression,
+    is_one_datetime_and_one_ingest_date,
+    is_one_timespan_and_one_datetime,
+)
 
 if TYPE_CHECKING:
     from ..visitors import PredicateVisitFlags, PredicateVisitor
     from ._column_set import ColumnSet
     from ._query_tree import QueryTree
 
 ComparisonOperator: TypeAlias = Literal["==", "!=", "<", ">", ">=", "<=", "overlaps"]
@@ -457,18 +461,24 @@
     def visit(self, visitor: PredicateVisitor[_A, _O, _L], flags: PredicateVisitFlags) -> _L:
         # Docstring inherited.
         return visitor.visit_comparison(self.a, self.operator, self.b, flags)
 
     @pydantic.model_validator(mode="after")
     def _validate_column_types(self) -> Comparison:
         if self.operator == "overlaps" and is_one_timespan_and_one_datetime(self.a, self.b):
-            # Special case for datetime overlaps timespan, which is currently
-            # the only mixed-type comparison allowed.
+            # Allow mixed-type comparison of datetime overlaps timespan.
             pass
+        elif is_one_datetime_and_one_ingest_date(self.a, self.b):
+            if self.operator in ("==", "!=", "<", ">", ">=", "<="):
+                # ingest_date might be one of two different column types
+                # (integer TAI nanoseconds like "datetime", or TIMESTAMP), but
+                # either one can be compared with a "datetime" column.
+                pass
         elif self.a.column_type == self.b.column_type:
+            # Most operators require matching column types.
             match (self.operator, self.a.column_type):
                 case ("==" | "!=", _):
                     pass
                 case ("<" | ">" | ">=" | "<=", "int" | "string" | "float" | "datetime"):
                     pass
                 case ("overlaps", "region" | "timespan"):
                     pass
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/tree/_query_tree.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/tree/_query_tree.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/queries/visitors.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/queries/visitors.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_caching_context.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_caching_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_record_cache.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_record_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_summary.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_summary.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_summary_cache.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_summary_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_collection_type.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_collection_type.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_config.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_dataset_type_cache.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_dataset_type_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_defaults.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_defaults.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_exceptions.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_registry.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/_registry_factory.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/_registry_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/attributes.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/attributes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/bridge/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/bridge/ephemeral.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/bridge/ephemeral.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/bridge/monolithic.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/bridge/monolithic.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/_base.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/_base.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/nameKey.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/nameKey.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/collections/synthIntKey.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/collections/synthIntKey.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/connectionString.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/databases/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/databases/postgresql.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/databases/sqlite.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -679,16 +679,16 @@
                 fields_provided["collection"] = sqlalchemy.literal("NO COLLECTIONS")
         else:
             sql_projection.joiner.where(collection_col.in_([collection.key for collection in collections]))
             if "collection" in fields:
                 # Avoid a join to the collection table to get the name by using
                 # a CASE statement.  The SQL will be a bit more verbose but
                 # more efficient.
-                fields_provided["collection"] = sqlalchemy.case(
-                    {record.key: record.name for record in collections}, value=collection_col
+                fields_provided["collection"] = _create_case_expression_for_collections(
+                    collections, collection_col
                 )
         # Add more column definitions, starting with the data ID.
         sql_projection.joiner.extract_dimensions(self.datasetType.dimensions.required.names)
         # We can always get the dataset_id from the tags/calibs table, even if
         # could also get it from the 'static' dataset table.
         if "dataset_id" in fields:
             fields_provided["dataset_id"] = dataset_id_col
@@ -703,17 +703,16 @@
                 # know that if we find the dataset in that collection,
                 # then that's the datasets's run; we don't need to
                 # query for it.
                 fields_provided["run"] = sqlalchemy.literal(only_collection_record.name)
             elif run_collections_only:
                 # Once again we can avoid joining to the collection table by
                 # adding a CASE statement.
-                fields_provided["run"] = sqlalchemy.case(
-                    {record.key: record.name for record in collections},
-                    value=self._static.dataset.c[self._runKeyColumn],
+                fields_provided["run"] = _create_case_expression_for_collections(
+                    collections, self._static.dataset.c[self._runKeyColumn]
                 )
                 need_static_table = True
             else:
                 # Here we can't avoid a join to the collection table, because
                 # we might find a dataset via something other than its RUN
                 # collection.
                 (
@@ -1058,7 +1057,40 @@
                 existing_collection = self._collections[getattr(row, collFkName)].name
                 new_collection = self._collections[getattr(row, f"new_{collFkName}")].name
                 raise ConflictingDefinitionError(
                     f"Dataset with type {self.datasetType.name!r} and data ID {data_id} "
                     f"has ID {row.dataset_id} in existing collection {existing_collection!r} "
                     f"but ID {row.new_dataset_id} in new collection {new_collection!r}."
                 )
+
+
+def _create_case_expression_for_collections(
+    collections: Iterable[CollectionRecord], id_column: sqlalchemy.ColumnElement
+) -> sqlalchemy.Case | sqlalchemy.Null:
+    """Return a SQLAlchemy Case expression that converts collection IDs to
+    collection names for the given set of collections.
+
+    Parameters
+    ----------
+    collections : `~collections.abc.Iterable` [ `CollectionRecord` ]
+        List of collections to include in conversion table.  This should be an
+        exhaustive list of collections that could appear in `id_column`.
+    id_column : `sqlalchemy.ColumnElement`
+        The column containing the collection ID that we want to convert to a
+        collection name.
+    """
+    mapping = {record.key: record.name for record in collections}
+    if not mapping:
+        # SQLAlchemy does not correctly handle an empty mapping in case() -- it
+        # crashes when trying to compile the expression with an
+        # "AttributeError('NoneType' object has no attribute 'dialect_impl')"
+        # when trying to access the 'type' property of the Case object.  If you
+        # explicitly specify a type via type_coerce it instead generates
+        # invalid SQL syntax.
+        #
+        # We can end up with empty mappings here in certain "doomed query" edge
+        # cases, e.g.  we start with a list of valid collections but they are
+        # all filtered out by higher-level code on the basis of collection
+        # summaries.
+        return sqlalchemy.null()
+
+    return sqlalchemy.case(mapping, value=id_column)
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/dimensions/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/dimensions/static.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/dimensions/static.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_attributes.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_attributes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_bridge.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_bridge.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_collections.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_database.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_database.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_datasets.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_datasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_dimensions.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_obscore.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_obscore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_opaque.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_opaque.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/interfaces/_versioning.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/interfaces/_versioning.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/managers.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/managers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/nameShrinker.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/nameShrinker.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_config.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_manager.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_manager.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_records.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_records.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_schema.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/_spatial.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/default_spatial.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/default_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/obscore/pgsphere.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/obscore/pgsphere.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/opaque.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/opaque.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_builder.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_query.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_query.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_query_backend.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_query_backend.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_query_context.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_query_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_readers.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_readers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_results.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_results.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = (
     "ChainedDatasetQueryResults",
     "DatabaseDataCoordinateQueryResults",
     "DatabaseDimensionRecordQueryResults",
+    "DatabaseParentDatasetQueryResults",
     "DataCoordinateQueryResults",
     "DatasetQueryResults",
     "DimensionRecordQueryResults",
     "ParentDatasetQueryResults",
     "QueryResultsBase",
 )
 
@@ -56,17 +57,17 @@
     DimensionGroup,
     DimensionRecord,
 )
 from ._query import Query
 from ._structs import OrderByClause
 
 
-class QueryResultsBase:
-    """Abstract base class defining functions used by several of the other
-    QueryResults classes.
+class LimitedQueryResultsBase:
+    """Abstract base class defining functions that are shared by all of the
+    other QueryResults classes.
     """
 
     @abstractmethod
     def count(self, *, exact: bool = True, discard: bool = False) -> int:
         """Count the number of rows this query would return.
 
         Parameters
@@ -137,14 +138,20 @@
         -------
         messages : `~collections.abc.Iterable` [ `str` ]
             String messages that describe reasons the query might not yield any
             results.
         """
         raise NotImplementedError()
 
+
+class QueryResultsBase(LimitedQueryResultsBase):
+    """Abstract base class defining functions shared by several of the other
+    QueryResults classes.
+    """
+
     @abstractmethod
     def order_by(self, *args: str) -> Self:
         """Make the iterator return ordered results.
 
         Parameters
         ----------
         *args : `str`
@@ -496,18 +503,17 @@
             raise DatasetTypeError(
                 "Dataset component queries are no longer supported by Registry.  Use "
                 "DatasetType methods to obtain components from parent dataset types instead."
             )
         resolved_dataset_type = self._query.backend.resolve_single_dataset_type_wildcard(
             datasetType, explicit_only=True
         )
-        return ParentDatasetQueryResults(
+        return DatabaseParentDatasetQueryResults(
             self._query.find_datasets(resolved_dataset_type, collections, find_first=findFirst, defer=True),
             resolved_dataset_type,
-            [None],
         )
 
     def findRelatedDatasets(
         self,
         datasetType: DatasetType | str,
         collections: Any,
         *,
@@ -541,34 +547,33 @@
     def limit(self, limit: int, offset: int | None = 0) -> Self:
         if offset is None:
             offset = 0
         self._query = self._query.sliced(offset, offset + limit, defer=True)
         return self
 
 
-class DatasetQueryResults(Iterable[DatasetRef]):
+class DatasetQueryResults(LimitedQueryResultsBase, Iterable[DatasetRef]):
     """An interface for objects that represent the results of queries for
     datasets.
     """
 
     @abstractmethod
     def byParentDatasetType(self) -> Iterator[ParentDatasetQueryResults]:
         """Group results by parent dataset type.
 
         Returns
         -------
         iter : `~collections.abc.Iterator` [ `ParentDatasetQueryResults` ]
             An iterator over `DatasetQueryResults` instances that are each
-            responsible for a single parent dataset type (either just that
-            dataset type, one or more of its component dataset types, or both).
+            responsible for a single parent dataset type.
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def materialize(self) -> AbstractContextManager[DatasetQueryResults]:
+    def materialize(self) -> AbstractContextManager[Self]:
         """Insert this query's results into a temporary table.
 
         Returns
         -------
         context : `typing.ContextManager` [ `DatasetQueryResults` ]
             A context manager that ensures the temporary table is created and
             populated in ``__enter__`` (returning a results object backed by
@@ -576,15 +581,15 @@
             materialized, the context manager may do nothing (reflecting the
             fact that an outer context manager should already take care of
             everything else).
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def expanded(self) -> DatasetQueryResults:
+    def expanded(self) -> Self:
         """Return a `DatasetQueryResults` for which `DataCoordinate.hasRecords`
         returns `True` for all data IDs in returned `DatasetRef` objects.
 
         Returns
         -------
         expanded : `DatasetQueryResults`
             Either a new `DatasetQueryResults` instance or ``self``, if it is
@@ -594,215 +599,117 @@
         -----
         As with `DataCoordinateQueryResults.expanded`, it may be more efficient
         to call `materialize` before expanding data IDs for very large result
         sets.
         """
         raise NotImplementedError()
 
-    @abstractmethod
-    def count(self, *, exact: bool = True, discard: bool = False) -> int:
-        """Count the number of rows this query would return.
-
-        Parameters
-        ----------
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed to account for that filtering in the count.  If `False`, the
-            result may be an upper bound.
-        discard : `bool`, optional
-            If `True`, compute the exact count even if it would require running
-            the full query and then throwing away the result rows after
-            counting them.  If `False`, this is an error, as the user would
-            usually be better off executing the query first to fetch its rows
-            into a new query (or passing ``exact=False``).  Ignored if
-            ``exact=False``.
-
-        Returns
-        -------
-        count : `int`
-            The number of rows the query would return, or an upper bound if
-            ``exact=False``.
+    def _iter_by_dataset_type(self) -> Iterator[tuple[DatasetType, Iterable[DatasetRef]]]:
+        """Group results by dataset type.
 
-        Notes
-        -----
-        This counts the number of rows returned, not the number of unique rows
-        returned, so even with ``exact=True`` it may provide only an upper
-        bound on the number of *deduplicated* result rows.
+        This is a private hook for the interface defined by
+        `DatasetRef.iter_by_type`, enabling much more efficient
+        processing of heterogeneous `DatasetRef` iterables when they come
+        directly from queries.
         """
-        raise NotImplementedError()
+        for parent_results in self.byParentDatasetType():
+            dataset_type = parent_results.parentDatasetType
+            yield dataset_type, parent_results
 
-    @abstractmethod
-    def any(
-        self,
-        *,
-        execute: bool = True,
-        exact: bool = True,
-    ) -> bool:
-        """Test whether this query returns any results.
 
-        Parameters
-        ----------
-        execute : `bool`, optional
-            If `True`, execute at least a ``LIMIT 1`` query if it cannot be
-            determined prior to execution that the query would return no rows.
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed, until at least one result row is found.  If `False`, the
-            returned result does not account for post-query filtering, and
-            hence may be `True` even when all result rows would be filtered
-            out.
+class ParentDatasetQueryResults(DatasetQueryResults):
+    """An object that represents results from a query for datasets with a
+    single parent `DatasetType`.
+    """
 
-        Returns
-        -------
-        any : `bool`
-            `True` if the query would (or might, depending on arguments) yield
-            result rows.  `False` if it definitely would not.
+    @property
+    @abstractmethod
+    def parentDatasetType(self) -> DatasetType:
+        """The parent dataset type for all datasets in this iterable
+        (`DatasetType`).
         """
         raise NotImplementedError()
 
+    @property
     @abstractmethod
-    def explain_no_results(self, execute: bool = True) -> Iterable[str]:
-        """Return human-readable messages that may help explain why the query
-        yields no results.
-
-        Parameters
-        ----------
-        execute : `bool`, optional
-            If `True` (default) execute simplified versions (e.g. ``LIMIT 1``)
-            of aspects of the tree to more precisely determine where rows were
-            filtered out.
+    def dataIds(self) -> DataCoordinateQueryResults:
+        """A lazy-evaluation object representing a query for just the data
+        IDs of the datasets that would be returned by this query
+        (`DataCoordinateQueryResults`).
 
-        Returns
-        -------
-        messages : `~collections.abc.Iterable` [ `str` ]
-            String messages that describe reasons the query might not yield any
-            results.
+        The returned object is not in general `zip`-iterable with ``self``;
+        it may be in a different order or have (or not have) duplicates.
         """
         raise NotImplementedError()
 
-    def _iter_by_dataset_type(self) -> Iterator[tuple[DatasetType, Iterable[DatasetRef]]]:
-        """Group results by dataset type.
-
-        This is a private hook for the interface defined by
-        `DatasetRef.iter_by_type`, enabling much more efficient
-        processing of heterogeneous `DatasetRef` iterables when they come
-        directly from queries.
-        """
-        for parent_results in self.byParentDatasetType():
-            for component in parent_results._components:
-                dataset_type = parent_results.parentDatasetType
-                if component is not None:
-                    dataset_type = dataset_type.makeComponentDatasetType(component)
-                if tuple(parent_results._components) == (component,):
-                    # Usual case, and in the future (after component support
-                    # has been fully removed) the only case.
-                    yield dataset_type, parent_results
-                else:
-                    # General case that emits a deprecation warning.
-                    yield (dataset_type, parent_results.withComponents((component,)))
-
 
-class ParentDatasetQueryResults(DatasetQueryResults):
+class DatabaseParentDatasetQueryResults(ParentDatasetQueryResults):
     """An object that represents results from a query for datasets with a
     single parent `DatasetType`.
 
     Parameters
     ----------
     query : `Query`
         Low-level query object that backs these results.
     dataset_type : `DatasetType`
         Parent dataset type for all datasets returned by this query.
-    components : `~collections.abc.Sequence` [ `str` or `None` ], optional
-        Names of components to include in iteration.  `None` may be included
-        (at most once) to include the parent dataset type.
 
     Notes
     -----
     The `Query` class now implements essentially all of this class's
     functionality; "QueryResult" classes like this one now exist only to
     provide interface backwards compatibility and more specific iterator
     types.
     """
 
     def __init__(
         self,
         query: Query,
         dataset_type: DatasetType,
-        components: Sequence[str | None] = (None,),
     ):
         self._query = query
         self._dataset_type = dataset_type
-        self._components = components
 
-    __slots__ = ("_query", "_dataset_type", "_components")
+    __slots__ = ("_query", "_dataset_type")
 
     def __iter__(self) -> Iterator[DatasetRef]:
-        return self._query.iter_dataset_refs(self._dataset_type, self._components)
+        return self._query.iter_dataset_refs(self._dataset_type)
 
     def __repr__(self) -> str:
-        return f"<DatasetRef iterator for [components of] {self._dataset_type.name}>"
-
-    @property
-    @deprecated("Deprecated, will be removed after v27.", version="v27", category=FutureWarning)
-    def components(self) -> Sequence[str | None]:
-        """The components of the parent dataset type included in these results
-        (`~collections.abc.Sequence` [ `str` or `None` ]).
-        """
-        return self._components
+        return f"<DatasetRef iterator for {self._dataset_type.name}>"
 
     def byParentDatasetType(self) -> Iterator[ParentDatasetQueryResults]:
         # Docstring inherited from DatasetQueryResults.
         yield self
 
     @contextmanager
-    def materialize(self) -> Iterator[ParentDatasetQueryResults]:
+    def materialize(self) -> Iterator[DatabaseParentDatasetQueryResults]:
         # Docstring inherited from DatasetQueryResults.
         with self._query.open_context():
-            yield ParentDatasetQueryResults(self._query.materialized(), self._dataset_type, self._components)
+            yield DatabaseParentDatasetQueryResults(self._query.materialized(), self._dataset_type)
 
     @property
     def parentDatasetType(self) -> DatasetType:
-        """The parent dataset type for all datasets in this iterable
-        (`DatasetType`).
-        """
+        # Docstring inherited.
         return self._dataset_type
 
     @property
     def dataIds(self) -> DataCoordinateQueryResults:
-        """A lazy-evaluation object representing a query for just the data
-        IDs of the datasets that would be returned by this query
-        (`DataCoordinateQueryResults`).
-
-        The returned object is not in general `zip`-iterable with ``self``;
-        it may be in a different order or have (or not have) duplicates.
-        """
+        # Docstring inherited.
         return DatabaseDataCoordinateQueryResults(self._query.projected(defer=True))
 
-    @deprecated("Deprecated, will be removed after v27.", version="v27", category=FutureWarning)
-    def withComponents(self, components: Sequence[str | None]) -> ParentDatasetQueryResults:
-        """Return a new query results object for the same parent datasets but
-        different components.
-
-        Parameters
-        ----------
-        components :  `~collections.abc.Sequence` [ `str` or `None` ]
-            Names of components to include in iteration.  `None` may be
-            included (at most once) to include the parent dataset type.
-        """
-        return ParentDatasetQueryResults(self._query, self._dataset_type, components)
-
-    def expanded(self) -> ParentDatasetQueryResults:
+    def expanded(self) -> DatabaseParentDatasetQueryResults:
         # Docstring inherited from DatasetQueryResults.
-        return ParentDatasetQueryResults(
-            self._query.with_record_columns(defer=True), self._dataset_type, self._components
+        return DatabaseParentDatasetQueryResults(
+            self._query.with_record_columns(defer=True), self._dataset_type
         )
 
     def count(self, *, exact: bool = True, discard: bool = False) -> int:
         # Docstring inherited.
-        return len(self._components) * self._query.count(exact=exact, discard=discard)
+        return self._query.count(exact=exact, discard=discard)
 
     def any(self, *, execute: bool = True, exact: bool = True) -> bool:
         # Docstring inherited.
         return self._query.any(execute=execute, exact=exact)
 
     def explain_no_results(self, execute: bool = True) -> Iterable[str]:
         # Docstring inherited.
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_sql_query_backend.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_sql_query_backend.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_sql_query_context.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_sql_query_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/_structs.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/_structs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/butler_sql_engine.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/butler_sql_engine.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/_predicate.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/_predicate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/categorize.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/categorize.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/check.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/check.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/normalForm.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/normalForm.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/queries/find_first_dataset.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/queries/find_first_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/sql_registry.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/sql_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -2127,17 +2127,15 @@
             # only if we need to findFirst.  Note that if any of the
             # collections are actually wildcard expressions, and
             # findFirst=True, this will raise TypeError for us.
             builder.joinDataset(
                 resolved_dataset_type, collection_wildcard, isResult=True, findFirst=findFirst
             )
             query = builder.finish()
-            parent_results.append(
-                queries.ParentDatasetQueryResults(query, resolved_dataset_type, components=[None])
-            )
+            parent_results.append(queries.DatabaseParentDatasetQueryResults(query, resolved_dataset_type))
         if not parent_results:
             doomed_by.extend(
                 f"No registered dataset type matching {t!r} found, so no matching datasets can "
                 "exist in any collection."
                 for t in ensure_iterable(datasetType)
             )
             return queries.ChainedDatasetQueryResults([], doomed_by=doomed_by)
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/tests/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/tests/_database.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/tests/_database.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/tests/_registry.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/tests/_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 import lsst.sphgeom
 from lsst.daf.relation import Relation, RelationalAlgebraError, Transfer, iteration, sql
 
 from ..._dataset_association import DatasetAssociation
 from ..._dataset_ref import DatasetIdFactory, DatasetIdGenEnum, DatasetRef
 from ..._dataset_type import DatasetType
 from ..._exceptions import (
+    CalibrationLookupError,
     CollectionTypeError,
     DataIdValueError,
     InconsistentDataIdError,
     InvalidQueryError,
     MissingCollectionError,
     MissingDatasetTypeError,
 )
@@ -135,14 +136,21 @@
 
     supportsExtendedTimeQueryOperators: bool = True
     """True if the registry class being tested supports ``<`` and ``>``
     operators in expression strings for comparisons of `Timespan` vs
     `Timespan`, or `Timespan` vs `Time`.
     """
 
+    supportsCalibrationCollectionInFindFirst: bool = True
+    """True if the registry class being tested supports searching in
+    calibration collections in queryDatasets(findFirst=True).
+    (The old query system would ignore/"skip" calibration collections in these
+    searches.  The new one is able to search in these collections.)
+    """
+
     @classmethod
     @abstractmethod
     def getDataDir(cls) -> str:
         """Return the root directory containing test data YAML files."""
         raise NotImplementedError()
 
     def makeRegistryConfig(self) -> RegistryConfig:
@@ -1543,14 +1551,57 @@
                 registry.findDataset("bias", instrument="Cam1", detector=1, collections="imported_g"),
                 registry.findDataset("bias", instrument="Cam1", detector=2, collections="imported_r"),
                 registry.findDataset("bias", instrument="Cam1", detector=3, collections="imported_r"),
                 registry.findDataset("bias", instrument="Cam1", detector=4, collections="imported_r"),
             ],
         )
 
+        with self.assertRaises(TypeError):
+            # Collection wildcards not allowed in find-first searches because
+            # they do not guarantee the ordering of collections.
+            registry.queryDatasets("bias", collections="imported_*", findFirst=True)
+
+    def testQueryDatasetsExtraDimensions(self):
+        registry = self.makeRegistry()
+        self.loadData(registry, "base.yaml")
+        self.loadData(registry, "datasets.yaml")
+        # Bias dataset type does not include physical filter.  By adding
+        # "physical_filter" to dimensions, we are effectively searching here
+        # for bias datasets with an instrument that has a specific filter
+        # available, even though that filter has nothing to do with the bias
+        # datasets we are finding.
+        self.assertEqual(
+            0,
+            registry.queryDatasets(
+                "bias",
+                collections=...,
+                dimensions=["physical_filter"],
+                dataId={
+                    "instrument": "Cam1",
+                    "band": "not_a_real_band",
+                },
+            ).count(),
+        )
+        self.assertEqual(
+            6,
+            len(
+                set(
+                    registry.queryDatasets(
+                        "bias",
+                        collections=...,
+                        dimensions=["physical_filter"],
+                        dataId={
+                            "instrument": "Cam1",
+                            "band": "r",
+                        },
+                    )
+                )
+            ),
+        )
+
     def testQueryResults(self):
         """Test querying for data IDs and then manipulating the QueryResults
         object returned to perform other queries.
         """
         registry = self.makeRegistry()
         self.loadData(registry, "base.yaml")
         self.loadData(registry, "datasets.yaml")
@@ -2596,18 +2647,26 @@
         registry.certify(coll_calib, registry.queryDatasets("bias", collections=...), Timespan(None, None))
 
         coll_list = [coll_calib, "imported_g", "imported_r"]
         chain = "Cam1/chain"
         registry.registerCollection(chain, type=CollectionType.CHAINED)
         registry.setCollectionChain(chain, coll_list)
 
-        # explicit list will raise if findFirst=True or there are temporal
-        # dimensions
-        with self.assertRaises(NotImplementedError):
-            registry.queryDatasets("bias", collections=coll_list, findFirst=True)
+        # explicit list will raise if findFirst=True.
+        # For old query system, this is because it couldn't handle find-first
+        # lookups in calibration collections.
+        # For new query system, it's because it correctly determines that the
+        # lookup is ambiguous due to multiple datasets with the same data ID
+        # in the calibration collection.
+        exception_type = (
+            CalibrationLookupError if self.supportsCalibrationCollectionInFindFirst else NotImplementedError
+        )
+        with self.assertRaises(exception_type):
+            list(registry.queryDatasets("bias", collections=coll_list, findFirst=True))
+        # explicit list will raise if there are temporal dimensions
         with self.assertRaises(NotImplementedError):
             registry.queryDataIds(
                 ["instrument", "detector", "exposure"], datasets="bias", collections=coll_list
             ).count()
 
         # chain will skip
         datasets = list(registry.queryDatasets("bias", collections=chain))
@@ -2617,47 +2676,56 @@
         self.assertGreater(len(dataIds), 0)
 
         # glob will skip too
         datasets = list(registry.queryDatasets("bias", collections="*d*"))
         self.assertGreater(len(datasets), 0)
 
         # regular expression will skip too
-        pattern = re.compile(".*")
-        datasets = list(registry.queryDatasets("bias", collections=pattern))
-        self.assertGreater(len(datasets), 0)
+        if self.supportsCollectionRegex:
+            pattern = re.compile(".*")
+            datasets = list(registry.queryDatasets("bias", collections=pattern))
+            self.assertGreater(len(datasets), 0)
 
         # ellipsis should work as usual
         datasets = list(registry.queryDatasets("bias", collections=...))
         self.assertGreater(len(datasets), 0)
 
-        # few tests with findFirst
-        datasets = list(registry.queryDatasets("bias", collections=chain, findFirst=True))
-        self.assertGreater(len(datasets), 0)
+        if self.supportsCalibrationCollectionInFindFirst:
+            # New query system correctly determines that this search is
+            # ambiguous, because there are multiple datasets with the same
+            # {instrument=Cam1, detector=2} data ID in the calibration
+            # collection at the beginning of the chain.
+            with self.assertRaises(CalibrationLookupError):
+                datasets = list(registry.queryDatasets("bias", collections=chain, findFirst=True))
+        else:
+            # Old query system ignores calibration collection entirely.
+            datasets = list(registry.queryDatasets("bias", collections=chain, findFirst=True))
+            self.assertGreater(len(datasets), 0)
 
     def testIngestTimeQuery(self):
         registry = self.makeRegistry()
         self.loadData(registry, "base.yaml")
         dt0 = datetime.datetime.now(datetime.UTC)
         self.loadData(registry, "datasets.yaml")
         dt1 = datetime.datetime.now(datetime.UTC)
 
         datasets = list(registry.queryDatasets(..., collections=...))
         len0 = len(datasets)
         self.assertGreater(len0, 0)
 
-        where = "ingest_date > T'2000-01-01'"
-        datasets = list(registry.queryDatasets(..., collections=..., where=where))
-        len1 = len(datasets)
-        self.assertEqual(len0, len1)
+        for where in ("ingest_date > T'2000-01-01'", "T'2000-01-01' < ingest_date"):
+            datasets = list(registry.queryDatasets(..., collections=..., where=where))
+            len1 = len(datasets)
+            self.assertEqual(len0, len1)
 
         # no one will ever use this piece of software in 30 years
-        where = "ingest_date > T'2050-01-01'"
-        datasets = list(registry.queryDatasets(..., collections=..., where=where))
-        len2 = len(datasets)
-        self.assertEqual(len2, 0)
+        for where in ("ingest_date > T'2050-01-01'", "T'2050-01-01' < ingest_date"):
+            datasets = list(registry.queryDatasets(..., collections=..., where=where))
+            len2 = len(datasets)
+            self.assertEqual(len2, 0)
 
         # Check more exact timing to make sure there is no 37 seconds offset
         # (after fixing DM-30124). SQLite time precision is 1 second, make
         # sure that we don't test with higher precision.
         tests = [
             # format: (timestamp, operator, expected_len)
             (dt0 - timedelta(seconds=1), ">", len0),
@@ -2909,15 +2977,15 @@
             (
                 # No datasets of this type in this collection.
                 base_query.findDatasets("flat", collections=["biases"]),
                 ["flat", "biases"],
             ),
             (
                 # No collections matching at all.
-                registry.queryDatasets("flat", collections=re.compile("potato.+")),
+                registry.queryDatasets("flat", collections="potato*"),
                 ["potato"],
             ),
         ]
         with self.assertRaises(MissingDatasetTypeError):
             # Dataset type name doesn't match any existing dataset types.
             registry.queryDataIds(["detector"], datasets=["nonexistent"], collections=...)
         with self.assertRaises(MissingDatasetTypeError):
@@ -3026,15 +3094,14 @@
         query5 = registry.queryDatasets(["bias", "nonexistent"], collections=["biases"])
         self.assertTrue(set(query5))
         self.assertTrue(query5.any(execute=False, exact=False))
         self.assertTrue(query5.any(execute=True, exact=False))
         self.assertTrue(query5.any(execute=True, exact=True))
         self.assertGreaterEqual(query5.count(exact=False), 1)
         self.assertGreaterEqual(query5.count(exact=True), 1)
-        self.assertFalse(list(query5.explain_no_results()))
         # This query applies a selection that yields no results, fully in the
         # database.  Explaining why it fails involves traversing the relation
         # tree and running a LIMIT 1 query at each level that has the potential
         # to remove rows.
         query6 = registry.queryDimensionRecords(
             "detector", where="detector.purpose = 'no-purpose'", instrument="Cam1"
         )
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/versions.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/versions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/registry/wildcards.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/registry/wildcards.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_authentication.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_authentication.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_collection_args.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_collection_args.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_config.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_factory.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_http_connection.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_http_connection.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_query_driver.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_query_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 __all__ = ("RemoteQueryDriver",)
 
 
 from collections.abc import Iterable
 from typing import Any, overload
 
 from ...butler import Butler
+from .._dataset_ref import DatasetRef
 from .._dataset_type import DatasetType
 from ..dimensions import DataCoordinate, DataIdValue, DimensionGroup, DimensionRecord, DimensionUniverse
 from ..queries.driver import (
     DataCoordinateResultPage,
     DatasetRefResultPage,
     DimensionRecordResultPage,
     GeneralResultPage,
@@ -128,14 +129,21 @@
         elif result_spec.result_type == "data_coordinate":
             assert result.type == "data_coordinate"
             return DataCoordinateResultPage(
                 spec=result_spec,
                 next_key=None,
                 rows=[DataCoordinate.from_simple(r, universe) for r in result.rows],
             )
+        elif result_spec.result_type == "dataset_ref":
+            assert result.type == "dataset_ref"
+            return DatasetRefResultPage(
+                spec=result_spec,
+                next_key=None,
+                rows=[DatasetRef.from_simple(r, universe) for r in result.rows],
+            )
         else:
             raise NotImplementedError(f"Unhandled result type {result_spec.result_type}")
 
     @overload
     def fetch_next_page(
         self, result_spec: DataCoordinateResultSpec, key: PageKey
     ) -> DataCoordinateResultPage: ...
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_ref_utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_ref_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_registry.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,24 +56,30 @@
     CollectionTypeError,
     DatasetTypeError,
     DatasetTypeExpressionError,
     NoDefaultCollectionError,
     Registry,
     RegistryDefaults,
 )
-from ..registry.queries import DataCoordinateQueryResults, DatasetQueryResults, DimensionRecordQueryResults
+from ..registry.queries import (
+    ChainedDatasetQueryResults,
+    DataCoordinateQueryResults,
+    DatasetQueryResults,
+    DimensionRecordQueryResults,
+)
 from ..registry.wildcards import CollectionWildcard, DatasetTypeWildcard
 from ..remote_butler import RemoteButler
 from ._collection_args import (
     convert_collection_arg_to_glob_string_list,
     convert_dataset_type_arg_to_glob_string_list,
 )
 from ._http_connection import RemoteButlerHttpConnection, parse_model
 from .registry._query_common import CommonQueryArguments
 from .registry._query_data_coordinates import QueryDriverDataCoordinateQueryResults
+from .registry._query_datasets import QueryDriverDatasetRefQueryResults
 from .registry._query_dimension_records import QueryDriverDimensionRecordQueryResults
 from .server_models import (
     ExpandDataIdRequestModel,
     ExpandDataIdResponseModel,
     GetCollectionInfoResponseModel,
     GetCollectionSummaryResponseModel,
     QueryCollectionsRequestModel,
@@ -368,15 +374,70 @@
         where: str = "",
         findFirst: bool = False,
         components: bool = False,
         bind: Mapping[str, Any] | None = None,
         check: bool = True,
         **kwargs: Any,
     ) -> DatasetQueryResults:
-        raise NotImplementedError()
+        doomed_by: list[str] = []
+        dimension_group = self.dimensions.conform(dimensions) if dimensions is not None else None
+
+        if collections is None and not self.defaults.collections:
+            raise NoDefaultCollectionError("No collections provided, and no default collections set")
+        if findFirst and collections is not None:
+            wildcard = CollectionWildcard.from_expression(collections)
+            if wildcard.patterns:
+                raise TypeError(
+                    "Collection search patterns not allowed in findFirst search, "
+                    "because collections must be in a specific order."
+                )
+
+        args = self._convert_common_query_arguments(
+            dataId=dataId,
+            where=where,
+            bind=bind,
+            kwargs=kwargs,
+            datasets=None,
+            collections=collections,
+            doomed_by=doomed_by,
+        )
+
+        if not args.collections:
+            doomed_by.append("No datasets can be found because collection list is empty.")
+
+        missing_dataset_types: list[str] = []
+        dataset_types = list(self.queryDatasetTypes(datasetType, missing=missing_dataset_types))
+        if missing_dataset_types:
+            doomed_by.extend(f"Dataset type {name} is not registered." for name in missing_dataset_types)
+
+        if len(dataset_types) == 0:
+            doomed_by.extend(
+                [
+                    f"No registered dataset type matching {t!r} found, so no matching datasets can "
+                    "exist in any collection."
+                    for t in ensure_iterable(datasetType)
+                ]
+            )
+            return ChainedDatasetQueryResults([], doomed_by=doomed_by)
+
+        query_results = [
+            QueryDriverDatasetRefQueryResults(
+                self._butler._query,
+                args,
+                dataset_type=dt,
+                find_first=findFirst,
+                extra_dimensions=dimension_group,
+                doomed_by=doomed_by,
+            )
+            for dt in dataset_types
+        ]
+        if len(query_results) == 1:
+            return query_results[0]
+        else:
+            return ChainedDatasetQueryResults(query_results)
 
     def queryDataIds(
         self,
         # TODO: Drop `Dimension` objects on DM-41326.
         dimensions: DimensionGroup | Iterable[Dimension | str] | Dimension | str,
         *,
         dataId: DataId | None = None,
@@ -421,25 +482,26 @@
         *,
         dataId: DataId | None = None,
         datasets: object | None = None,
         collections: CollectionArgType | None = None,
         where: str = "",
         bind: Mapping[str, Any] | None = None,
         kwargs: dict[str, int | str],
+        doomed_by: list[str] | None = None,
     ) -> CommonQueryArguments:
         dataset_types = self._resolve_dataset_types(datasets)
         if dataset_types and collections is None and not self.defaults.collections:
             raise NoDefaultCollectionError("'collections' must be provided if 'datasets' is provided")
         return CommonQueryArguments(
             dataId=dataId,
             where=where,
             bind=dict(bind) if bind else None,
             kwargs=dict(kwargs),
             dataset_types=dataset_types,
-            collections=self._resolve_collections(collections),
+            collections=self._resolve_collections(collections, doomed_by),
         )
 
     def queryDatasetAssociations(
         self,
         datasetType: str | DatasetType,
         collections: CollectionArgType | None = ...,
         *,
@@ -452,21 +514,26 @@
     def storageClasses(self) -> StorageClassFactory:
         return self._butler.storageClasses
 
     @storageClasses.setter
     def storageClasses(self, value: StorageClassFactory) -> None:
         raise NotImplementedError()
 
-    def _resolve_collections(self, collections: CollectionArgType | None) -> list[str] | None:
+    def _resolve_collections(
+        self, collections: CollectionArgType | None, doomed_by: list[str] | None = None
+    ) -> list[str] | None:
         if collections is None:
             return list(self.defaults.collections)
 
         wildcard = CollectionWildcard.from_expression(collections)
         if wildcard.patterns:
-            return list(self.queryCollections(collections))
+            result = list(self.queryCollections(collections))
+            if not result and doomed_by is not None:
+                doomed_by.append(f"No collections found matching expression {wildcard}")
+            return result
         else:
             return list(wildcard.strings)
 
     def _resolve_dataset_types(self, dataset_types: object | None) -> list[str]:
         if dataset_types is None:
             return []
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/_remote_butler.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/_remote_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/_query_common.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/_query_common.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/_query_data_coordinates.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/_query_data_coordinates.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/_dependencies.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/_dependencies.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/_factory.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/_server.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/_server.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_external.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_external.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server/handlers/_query_serialization.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server/handlers/_query_serialization.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,16 +25,27 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 from collections.abc import Iterator
 
-from ....queries.driver import DataCoordinateResultPage, DimensionRecordResultPage, ResultPage, ResultSpec
-from ...server_models import DataCoordinateResultModel, DimensionRecordsResultModel, QueryExecuteResultData
+from ....queries.driver import (
+    DataCoordinateResultPage,
+    DatasetRefResultPage,
+    DimensionRecordResultPage,
+    ResultPage,
+    ResultSpec,
+)
+from ...server_models import (
+    DataCoordinateResultModel,
+    DatasetRefResultModel,
+    DimensionRecordsResultModel,
+    QueryExecuteResultData,
+)
 
 
 def convert_query_pages(spec: ResultSpec, pages: Iterator[ResultPage]) -> QueryExecuteResultData:
     """Convert pages of result data from the query system to a serializable
     format.
 
     Parameters
@@ -45,14 +56,16 @@
         Raw pages of data from the query driver.
     """
     match spec.result_type:
         case "dimension_record":
             return _convert_dimension_record_pages(pages)
         case "data_coordinate":
             return _convert_data_coordinate_pages(pages)
+        case "dataset_ref":
+            return _convert_dataset_ref_pages(pages)
         case _:
             raise NotImplementedError(f"Unhandled query result type {spec.result_type}")
 
 
 def _convert_dimension_record_pages(pages: Iterator[ResultPage]) -> DimensionRecordsResultModel:
     response = DimensionRecordsResultModel(rows=[])
     for page in pages:
@@ -63,7 +76,15 @@
 
 def _convert_data_coordinate_pages(pages: Iterator[ResultPage]) -> DataCoordinateResultModel:
     response = DataCoordinateResultModel(rows=[])
     for page in pages:
         assert isinstance(page, DataCoordinateResultPage)
         response.rows.extend(coordinate.to_simple() for coordinate in page.rows)
     return response
+
+
+def _convert_dataset_ref_pages(pages: Iterator[ResultPage]) -> DatasetRefResultModel:
+    response = DatasetRefResultModel(rows=[])
+    for page in pages:
+        assert isinstance(page, DatasetRefResultPage)
+        response.rows.extend(ref.to_simple() for ref in page.rows)
+    return response
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/remote_butler/server_models.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/remote_butler/server_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,26 @@
     results.
     """
 
     type: Literal["dimension_record"] = "dimension_record"
     rows: list[SerializedDimensionRecord]
 
 
-QueryExecuteResultData: TypeAlias = DataCoordinateResultModel | DimensionRecordsResultModel
+class DatasetRefResultModel(pydantic.BaseModel):
+    """Result model for /query/execute/ when user requested DatasetRef
+    results.
+    """
+
+    type: Literal["dataset_ref"] = "dataset_ref"
+    rows: list[SerializedDatasetRef]
+
+
+QueryExecuteResultData: TypeAlias = (
+    DataCoordinateResultModel | DimensionRecordsResultModel | DatasetRefResultModel
+)
 
 
 class QueryExecuteResponseModel(pydantic.BaseModel):
     """Response model for /query/execute/. Results may be in several different
     formats depending what the user requested.
     """
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/repo_relocation.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/repo_relocation.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/_associate.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/_associate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/_pruneDatasets.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/_pruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/butlerImport.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/butlerImport.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/certifyCalibrations.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/certifyCalibrations.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/collectionChain.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/collectionChain.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/configDump.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/configDump.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/configValidate.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/configValidate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/createRepo.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/createRepo.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/exportCalibs.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/exportCalibs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/ingest_files.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/ingest_files.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryCollections.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDataIds.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDatasetTypes.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDatasetTypes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDatasets.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/queryDimensionRecords.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/queryDimensionRecords.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/register_dataset_type.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/register_dataset_type.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/removeCollections.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/removeCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/removeDatasetType.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/removeDatasetType.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/removeRuns.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/removeRuns.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/retrieveArtifacts.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/retrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/script/transferDatasets.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/script/transferDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_datasetsHelper.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_datasetsHelper.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_dummyRegistry.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_dummyRegistry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_examplePythonTypes.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_examplePythonTypes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/_testRepo.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/_testRepo.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/butler_queries.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/butler_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 __all__ = ()
 
 import os
 import unittest
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Sequence
 from typing import ClassVar
+from uuid import UUID
 
 import astropy.time
 
 from .._butler import Butler
 from .._dataset_type import DatasetType
 from .._exceptions import InvalidQueryError
 from .._timespan import Timespan
@@ -188,14 +189,27 @@
             universe = butler.dimensions
             expected_coordinates = [
                 DataCoordinate.standardize({"instrument": "Cam1", "detector": x}, universe=universe)
                 for x in expected_detectors
             ]
             self.assertCountEqual(list(results), expected_coordinates)
 
+    def test_simple_dataset_query(self) -> None:
+        butler = self.make_butler("base.yaml", "datasets.yaml")
+        with butler._query() as query:
+            refs = list(query.datasets("bias", "imported_g").order_by("detector"))
+            self.assertEqual(len(refs), 3)
+            self.assertEqual(refs[0].id, UUID("e15ab039-bc8b-4135-87c5-90902a7c0b22"))
+            self.assertEqual(refs[1].id, UUID("51352db4-a47a-447c-b12d-a50b206b17cd"))
+            for detector, ref in enumerate(refs, 1):
+                self.assertEqual(ref.datasetType.name, "bias")
+                self.assertEqual(ref.dataId["instrument"], "Cam1")
+                self.assertEqual(ref.dataId["detector"], detector)
+                self.assertEqual(ref.run, "imported_g")
+
     def test_implied_union_record_query(self) -> None:
         """Test queries for a dimension ('band') that uses "implied union"
         storage, in which its values are the union of the values for it in a
         another dimension (physical_filter) that implies it.
         """
         butler = self.make_butler("base.yaml")
         band = butler.dimensions["band"]
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/cliCmdTestBase.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/cliCmdTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/cliLogTestBase.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/cliLogTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/deferredFormatter.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/deferredFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/dict_convertible_model.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/dict_convertible_model.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/hybrid_butler.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/hybrid_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/hybrid_butler_registry.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/hybrid_butler_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         where: str = "",
         findFirst: bool = False,
         components: bool = False,
         bind: Mapping[str, Any] | None = None,
         check: bool = True,
         **kwargs: Any,
     ) -> DatasetQueryResults:
-        return self._direct.queryDatasets(
+        return self._remote.queryDatasets(
             datasetType,
             collections=collections,
             dimensions=dimensions,
             dataId=dataId,
             where=where,
             findFirst=findFirst,
             bind=bind,
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/server.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/server.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/server_utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/server_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/testFormatters.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/testFormatters.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/tests/utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/time_utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/timespan_database_representation.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/timespan_database_representation.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/__init__.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/_context.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/_interfaces.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/_interfaces.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/transfers/_yaml.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/transfers/_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst/daf/butler/utils.py` & `lsst_daf_butler-27.2024.2200/python/lsst/daf/butler/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/PKG-INFO` & `lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_daf_butler-27.2024.2100/python/lsst_daf_butler.egg-info/SOURCES.txt` & `lsst_daf_butler-27.2024.2200/python/lsst_daf_butler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 python/lsst/daf/butler/direct_butler/_direct_butler.py
 python/lsst/daf/butler/direct_butler/_direct_butler_collections.py
 python/lsst/daf/butler/direct_query_driver/__init__.py
 python/lsst/daf/butler/direct_query_driver/_driver.py
 python/lsst/daf/butler/direct_query_driver/_postprocessing.py
 python/lsst/daf/butler/direct_query_driver/_query_builder.py
 python/lsst/daf/butler/direct_query_driver/_query_plan.py
+python/lsst/daf/butler/direct_query_driver/_result_page_converter.py
 python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py
 python/lsst/daf/butler/formatters/__init__.py
 python/lsst/daf/butler/formatters/astropyTable.py
 python/lsst/daf/butler/formatters/file.py
 python/lsst/daf/butler/formatters/json.py
 python/lsst/daf/butler/formatters/logs.py
 python/lsst/daf/butler/formatters/matplotlib.py
@@ -279,14 +280,15 @@
 python/lsst/daf/butler/remote_butler/_ref_utils.py
 python/lsst/daf/butler/remote_butler/_registry.py
 python/lsst/daf/butler/remote_butler/_remote_butler.py
 python/lsst/daf/butler/remote_butler/server_models.py
 python/lsst/daf/butler/remote_butler/registry/__init__.py
 python/lsst/daf/butler/remote_butler/registry/_query_common.py
 python/lsst/daf/butler/remote_butler/registry/_query_data_coordinates.py
+python/lsst/daf/butler/remote_butler/registry/_query_datasets.py
 python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py
 python/lsst/daf/butler/remote_butler/server/__init__.py
 python/lsst/daf/butler/remote_butler/server/_dependencies.py
 python/lsst/daf/butler/remote_butler/server/_factory.py
 python/lsst/daf/butler/remote_butler/server/_server.py
 python/lsst/daf/butler/remote_butler/server/handlers/_external.py
 python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py
```

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_astropyTableFormatter.py` & `lsst_daf_butler-27.2024.2200/tests/test_astropyTableFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_authentication.py` & `lsst_daf_butler-27.2024.2200/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_butler.py` & `lsst_daf_butler-27.2024.2200/tests/test_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_butler_factory.py` & `lsst_daf_butler-27.2024.2200/tests/test_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdAssociate.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdAssociate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdConfigDump.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdConfigDump.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdConfigValidate.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdConfigValidate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdCreate.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdCreate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdImport.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdImport.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdIngestFiles.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdIngestFiles.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdPruneDatasets.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdPruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryCollections.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDataIds.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDatasetTypes.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDatasetTypes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDatasets.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdQueryDimensionRecords.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdQueryDimensionRecords.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdRemoveCollections.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdRemoveCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdRemoveRuns.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdRemoveRuns.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliCmdRetrieveArtifacts.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliCmdRetrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliLog.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliLog.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliPluginLoader.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliPluginLoader.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliUtilSplitCommas.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliUtilSplitCommas.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliUtilSplitKv.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliUtilSplitKv.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliUtilToUpper.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliUtilToUpper.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_cliUtils.py` & `lsst_daf_butler-27.2024.2200/tests/test_cliUtils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_composites.py` & `lsst_daf_butler-27.2024.2200/tests/test_composites.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_config.py` & `lsst_daf_butler-27.2024.2200/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_connectionString.py` & `lsst_daf_butler-27.2024.2200/tests/test_connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_constraints.py` & `lsst_daf_butler-27.2024.2200/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_datasets.py` & `lsst_daf_butler-27.2024.2200/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_datastore.py` & `lsst_daf_butler-27.2024.2200/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_ddl.py` & `lsst_daf_butler-27.2024.2200/tests/test_ddl.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_dimension_record_containers.py` & `lsst_daf_butler-27.2024.2200/tests/test_dimension_record_containers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_dimensions.py` & `lsst_daf_butler-27.2024.2200/tests/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_exprParserLex.py` & `lsst_daf_butler-27.2024.2200/tests/test_exprParserLex.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_exprParserYacc.py` & `lsst_daf_butler-27.2024.2200/tests/test_exprParserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_expressions.py` & `lsst_daf_butler-27.2024.2200/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_formatter.py` & `lsst_daf_butler-27.2024.2200/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_location.py` & `lsst_daf_butler-27.2024.2200/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_logFormatter.py` & `lsst_daf_butler-27.2024.2200/tests/test_logFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_logging.py` & `lsst_daf_butler-27.2024.2200/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_matplotlibFormatter.py` & `lsst_daf_butler-27.2024.2200/tests/test_matplotlibFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_nonempty_mapping.py` & `lsst_daf_butler-27.2024.2200/tests/test_nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_normalFormExpression.py` & `lsst_daf_butler-27.2024.2200/tests/test_normalFormExpression.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_obscore.py` & `lsst_daf_butler-27.2024.2200/tests/test_obscore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_packages.py` & `lsst_daf_butler-27.2024.2200/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_parquet.py` & `lsst_daf_butler-27.2024.2200/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_postgresql.py` & `lsst_daf_butler-27.2024.2200/tests/test_postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,15 @@
     -----
     This is not a subclass of `unittest.TestCase` but to avoid repetition it
     defines methods that override `unittest.TestCase` methods. To make this
     work subclasses have to have this class first in the bases list.
     """
 
     sometimesHasDuplicateQueryRows = True
+    supportsCalibrationCollectionInFindFirst = False
 
     @classmethod
     def setUpClass(cls):
         cls.root = makeTestTempDir(TESTDIR)
         cls.server = _startServer(cls.root)
 
     @classmethod
```

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_progress.py` & `lsst_daf_butler-27.2024.2200/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_pydantic_utils.py` & `lsst_daf_butler-27.2024.2200/tests/test_pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_quantum.py` & `lsst_daf_butler-27.2024.2200/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_quantumBackedButler.py` & `lsst_daf_butler-27.2024.2200/tests/test_quantumBackedButler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_query_direct_postgresql.py` & `lsst_daf_butler-27.2024.2200/tests/test_query_direct_postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_query_direct_sqlite.py` & `lsst_daf_butler-27.2024.2200/tests/test_query_direct_sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_query_interface.py` & `lsst_daf_butler-27.2024.2200/tests/test_query_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,15 +592,15 @@
         self.assertEqual(columns.dataset_fields["raw"], {"ingest_date"})
         self.assertEqual(qt.DatasetFieldReference(dataset_type="raw", field="dataset_id").column_type, "uuid")
         self.assertEqual(
             qt.DatasetFieldReference(dataset_type="raw", field="collection").column_type, "string"
         )
         self.assertEqual(qt.DatasetFieldReference(dataset_type="raw", field="run").column_type, "string")
         self.assertEqual(
-            qt.DatasetFieldReference(dataset_type="raw", field="ingest_date").column_type, "datetime"
+            qt.DatasetFieldReference(dataset_type="raw", field="ingest_date").column_type, "ingest_date"
         )
         self.assertEqual(
             qt.DatasetFieldReference(dataset_type="raw", field="timespan").column_type, "timespan"
         )
         value = astropy.time.Time("2020-01-01T00:00:00", format="isot", scale="tai")
         self.assertEqual(expr.visit(_TestVisitor(dataset_fields={("raw", "ingest_date"): value})), value)
```

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_query_relations.py` & `lsst_daf_butler-27.2024.2200/tests/test_query_relations.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_query_remote.py` & `lsst_daf_butler-27.2024.2200/tests/test_query_remote.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_query_utilities.py` & `lsst_daf_butler-27.2024.2200/tests/test_query_utilities.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_remote_butler.py` & `lsst_daf_butler-27.2024.2200/tests/test_remote_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_server.py` & `lsst_daf_butler-27.2024.2200/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_simpleButler.py` & `lsst_daf_butler-27.2024.2200/tests/test_simpleButler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_sqlite.py` & `lsst_daf_butler-27.2024.2200/tests/test_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
     -----
     This is not a subclass of `unittest.TestCase` but to avoid repetition it
     defines methods that override `unittest.TestCase` methods. To make this
     work sublasses have to have this class first in the bases list.
     """
 
     sometimesHasDuplicateQueryRows = True
+    supportsCalibrationCollectionInFindFirst = False
 
     def setUp(self):
         self.root = makeTestTempDir(TESTDIR)
 
     def tearDown(self):
         removeTestTempDir(self.root)
 
@@ -254,14 +255,15 @@
     )
 
 
 class SqliteMemoryRegistryTests(RegistryTests):
     """Tests for `Registry` backed by a SQLite in-memory database."""
 
     sometimesHasDuplicateQueryRows = True
+    supportsCalibrationCollectionInFindFirst = False
 
     @classmethod
     def getDataDir(cls) -> str:
         return os.path.normpath(os.path.join(os.path.dirname(__file__), "data", "registry"))
 
     def makeRegistry(self, share_repo_with: SqlRegistry | None = None) -> SqlRegistry | None:
         if share_repo_with is not None:
```

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_storageClass.py` & `lsst_daf_butler-27.2024.2200/tests/test_storageClass.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_templates.py` & `lsst_daf_butler-27.2024.2200/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_testRepo.py` & `lsst_daf_butler-27.2024.2200/tests/test_testRepo.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_thread_utils.py` & `lsst_daf_butler-27.2024.2200/tests/test_thread_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_time_utils.py` & `lsst_daf_butler-27.2024.2200/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_timespan.py` & `lsst_daf_butler-27.2024.2200/tests/test_timespan.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_utils.py` & `lsst_daf_butler-27.2024.2200/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.2100/tests/test_versioning.py` & `lsst_daf_butler-27.2024.2200/tests/test_versioning.py`

 * *Files identical despite different names*

