# Comparing `tmp/laktory-0.3.2.tar.gz` & `tmp/laktory-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laktory-0.3.2.tar", last modified: Tue May 28 18:11:58 2024, max compression
+gzip compressed data, was "laktory-0.3.3.tar", last modified: Thu May 30 04:45:09 2024, max compression
```

## Comparing `laktory-0.3.2.tar` & `laktory-0.3.3.tar`

### file list

```diff
@@ -1,513 +1,515 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.406434 laktory-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.310434 laktory-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.322435 laktory-0.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/ISSUE_TEMPLATE/bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/ISSUE_TEMPLATE/feature.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.322435 laktory-0.3.2/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/scripts/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/scripts/update_quickstart_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/scripts/write_release_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.322435 laktory-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/workflows/publish-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/workflows/run_quickstart.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-28 18:11:49.000000 laktory-0.3.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 18:11:49.000000 laktory-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-28 18:11:49.000000 laktory-0.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 18:11:49.000000 laktory-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 18:11:49.000000 laktory-0.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-28 18:11:58.406434 laktory-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-28 18:11:49.000000 laktory-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.322435 laktory-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.322435 laktory-0.3.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/datetime.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.326434 laktory-0.3.2/docs/api/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dispatcher/dispatcher.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dispatcher/dispatcherrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dispatcher/jobrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dispatcher/pipelinerunner.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.326434 laktory-0.3.2/docs/api/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dlt/apply_changes.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dlt/get_df.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dlt/is_debug.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dlt/is_mocked.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dlt/read.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/dlt/read_stream.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.326434 laktory-0.3.2/docs/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/basemodel.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/dataproducer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.326434 laktory-0.3.2/docs/api/models/datasinks/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasinks/basedatasink.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasinks/filedatasink.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasinks/tabledatasink.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.330434 laktory-0.3.2/docs/api/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasources/basedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasources/filedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasources/memorydatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasources/pipelinenodedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/datasources/tabledatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/pipelinenode.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/pipelinenodeexpectation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.330434 laktory-0.3.2/docs/api/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/baseresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.334434 laktory-0.3.2/docs/api/models/resources/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/accesscontrol.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/cluster.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/column.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/directory.md
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/dltpipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/externallocation.md
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/grants.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/group.md
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/job.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/metastore.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/metastoreassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/metastoredataaccess.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/mwspermissionassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/notebook.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/secret.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/secretacl.md
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/secretscope.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/serviceprincipal.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/serviceprincipalrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/sqlquery.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/user.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/userrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/volume.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/warehouse.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/databricks/workspacefile.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.334434 laktory-0.3.2/docs/api/models/resources/providers/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/providers/aws.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/providers/azure.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/providers/azurepulumi.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/providers/databricks.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/pulumiresource.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/resources/terraformresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.334434 laktory-0.3.2/docs/api/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/spark/sparkchain.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/spark/sparkchainnode.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/spark/sparkfuncarg.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.338435 laktory-0.3.2/docs/api/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/stacks/pulumistack.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/stacks/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/models/stacks/terraformstack.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.310434 laktory-0.3.2/docs/api/spark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.338435 laktory-0.3.2/docs/api/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/dataframe/groupby_and_agg.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/dataframe/has_column.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/dataframe/schema_flat.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/dataframe/show_string.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/dataframe/smart_join.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/dataframe/window_filter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.342435 laktory-0.3.2/docs/api/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/_constants.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/add.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/convert_units.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/div.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/mul.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/poly1.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/poly2.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/roundp.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/scaled_power.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/string_split.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/sub.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/api/spark/functions/uuid.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.342435 laktory-0.3.2/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/governance.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.342435 laktory-0.3.2/docs/concepts/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/models/models.md
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/models/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/models/sourcessinks.md
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/models/sparkchain.md
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/spark.md
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/concepts/variables.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/demos.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.342435 laktory-0.3.2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/guides/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/guides/compute.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/guides/job.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/guides/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/guides/secrets.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/guides/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/guides/users.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.354434 laktory-0.3.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/databricks.png
--rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/delta_live_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)   240172 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/dlt_debug.png
--rw-r--r--   0 runner    (1001) docker     (127)   256333 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/dlt_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   221423 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/job_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/kappa.png
--rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/lakehouse.png
--rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/logo_sg.png
--rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/logo_sg_ltb.png
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/logo_sw.png
--rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/logo_sw_ltw.png
--rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/medaillon_complex.png
--rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/medallion.png
--rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/okube.png
--rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/pl_quickstart.png
--rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/pl_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/pl_stock_prices_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/pulumi.png
--rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/stock_prices_lineage.png
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/terraform.png
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/images/what_is_laktory.png
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/lakehouseascode.md
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.354434 laktory-0.3.2/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-28 18:11:49.000000 laktory-0.3.2/docs/stylesheets/mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.354434 laktory-0.3.2/laktory/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.358435 laktory-0.3.2/laktory/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_testing/stackvalidator.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_testing/stockprices.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.358435 laktory-0.3.2/laktory/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/_quickstart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/cli/quickstart_stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.362434 laktory-0.3.2/laktory/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/dispatcher/dispatcherrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/dispatcher/dltpipelinerunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/dispatcher/jobrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.362434 laktory-0.3.2/laktory/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/dlt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.362434 laktory-0.3.2/laktory/models/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.362434 laktory-0.3.2/laktory/models/azurenative/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/azurenative/storageblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16431 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/dataproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.362434 laktory-0.3.2/laktory/models/datasinks/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasinks/basedatasink.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasinks/filedatasink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasinks/tabledatasink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.366434 laktory-0.3.2/laktory/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasources/basedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasources/filedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasources/memorydatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasources/pipelinenodedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/datasources/tabledatasource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.366434 laktory-0.3.2/laktory/models/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/cataloggrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/connectiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/externallocationgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/functiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/metastoregrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/registeredmodelgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/schemagrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/sharegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/storagecredentialgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/tablegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/viewgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/grants/volumegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)    24180 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/pipelinenode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/pipelinenodeexpectation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.366434 laktory-0.3.2/laktory/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/baseresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.374435 laktory-0.3.2/laktory/models/resources/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/accesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/dltpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/externallocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/groupmember.py
--rw-r--r--   0 runner    (1001) docker     (127)    24460 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/metastoreassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/metastoredataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/mwspermissionassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/secretacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/secretscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/serviceprincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/serviceprincipalrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/sqlquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/userrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/databricks/workspacefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.374435 laktory-0.3.2/laktory/models/resources/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/providers/awsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/providers/azureprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/providers/azurepulumiprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/providers/baseprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/providers/databricksprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/pulumiresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/resources/terraformresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.374435 laktory-0.3.2/laktory/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/spark/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/spark/sparkchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/spark/sparkchainnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/spark/sparkfuncarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.374435 laktory-0.3.2/laktory/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/stacks/pulumistack.py
--rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/stacks/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/models/stacks/terraformstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.374435 laktory-0.3.2/laktory/polars/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/polars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.314434 laktory-0.3.2/laktory/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.374435 laktory-0.3.2/laktory/resources/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/resources/data/stock_prices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.378435 laktory-0.3.2/laktory/resources/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/resources/notebooks/dlt_laktory_pl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/resources/notebooks/job_laktory_pl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.378435 laktory-0.3.2/laktory/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.378435 laktory-0.3.2/laktory/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/groupby_and_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/has_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/schema_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/show_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/smart_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/watermark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/dataframe/window_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.378435 laktory-0.3.2/laktory/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/functions/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/functions/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/functions/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/spark/functions/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-28 18:11:49.000000 laktory-0.3.2/laktory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.402434 laktory-0.3.2/laktory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-28 18:11:58.000000 laktory-0.3.2/laktory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-05-28 18:11:58.000000 laktory-0.3.2/laktory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:11:58.000000 laktory-0.3.2/laktory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 18:11:58.000000 laktory-0.3.2/laktory.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 18:11:58.000000 laktory-0.3.2/laktory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 18:11:58.000000 laktory-0.3.2/laktory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-28 18:11:49.000000 laktory-0.3.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-28 18:11:49.000000 laktory-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.378435 laktory-0.3.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-28 18:11:49.000000 laktory-0.3.2/scripts/databricks_api_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 18:11:49.000000 laktory-0.3.2/scripts/polars_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 18:11:49.000000 laktory-0.3.2/scripts/test_computed_filed.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 18:11:49.000000 laktory-0.3.2/scripts/test_db_connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.378435 laktory-0.3.2/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 18:11:49.000000 laktory-0.3.2/settings/dev.env
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:11:58.406434 laktory-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.386434 laktory-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/build_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.386434 laktory-0.3.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.390435 laktory-0.3.2/tests/data/brz_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/brz_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/brz_stock_prices/.part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/brz_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.314434 laktory-0.3.2/tests/data/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.314434 laktory-0.3.2/tests/data/events/yahoo-finance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.314434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.314434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.318434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.390435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/01/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.390435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/05/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.390435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/06/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.390435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/07/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.390435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/08/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.394435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/11/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.394435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/12/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.394435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/13/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.394435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/14/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.394435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/15/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.394435 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/18/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.398434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/19/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.398434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/20/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.398434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/21/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.398434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/22/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.398434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/25/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.398434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/26/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.402434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/27/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.402434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/28/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.402434 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/29/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/pl-spark-dlt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/pl-spark-job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/pl-spark-local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/pl-spark-streaming.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.402434 laktory-0.3.2/tests/data/slv_stock_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_meta/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_meta/.part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_meta/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:58.402434 laktory-0.3.2/tests/data/slv_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_prices/.part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/stack_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/stockprices0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/stockprices1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/data/stockprices2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_datasinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_dlt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_dltpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_pipeline_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_spark_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_spark_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    27005 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-28 18:11:49.000000 laktory-0.3.2/tests/test_workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.537009 laktory-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.433008 laktory-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.441008 laktory-0.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/ISSUE_TEMPLATE/feature.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.445008 laktory-0.3.3/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/scripts/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/scripts/update_quickstart_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/scripts/write_release_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.445008 laktory-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/workflows/publish-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/workflows/run_quickstart.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-30 04:45:00.000000 laktory-0.3.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-30 04:45:00.000000 laktory-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-05-30 04:45:00.000000 laktory-0.3.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 04:45:00.000000 laktory-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 04:45:00.000000 laktory-0.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-30 04:45:09.537009 laktory-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-30 04:45:00.000000 laktory-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.445008 laktory-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.445008 laktory-0.3.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/datetime.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.445008 laktory-0.3.3/docs/api/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dispatcher/dispatcher.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dispatcher/dispatcherrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dispatcher/jobrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dispatcher/pipelinerunner.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.449008 laktory-0.3.3/docs/api/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dlt/apply_changes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dlt/get_df.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dlt/is_debug.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dlt/is_mocked.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dlt/read.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/dlt/read_stream.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.449008 laktory-0.3.3/docs/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/basemodel.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/dataproducer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.449008 laktory-0.3.3/docs/api/models/datasinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasinks/basedatasink.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasinks/filedatasink.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasinks/tabledatasink.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.449008 laktory-0.3.3/docs/api/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasources/basedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasources/filedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasources/memorydatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasources/pipelinenodedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/datasources/tabledatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/pipelinenode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/pipelinenodeexpectation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.453008 laktory-0.3.3/docs/api/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/baseresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.457008 laktory-0.3.3/docs/api/models/resources/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/accesscontrol.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/cluster.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/directory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/dltpipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/externallocation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/grants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/group.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/metastore.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/metastoreassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/metastoredataaccess.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/mwspermissionassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/notebook.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/secretacl.md
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/secretscope.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/serviceprincipal.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/serviceprincipalrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/sqlquery.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/user.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/userrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/volume.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/warehouse.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/databricks/workspacefile.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.457008 laktory-0.3.3/docs/api/models/resources/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/providers/aws.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/providers/azure.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/providers/azurepulumi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/providers/databricks.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/pulumiresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/resources/terraformresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.457008 laktory-0.3.3/docs/api/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/spark/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/spark/sparkchainnode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/spark/sparkfuncarg.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.457008 laktory-0.3.3/docs/api/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/stacks/pulumistack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/stacks/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/models/stacks/terraformstack.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.433008 laktory-0.3.3/docs/api/spark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.461008 laktory-0.3.3/docs/api/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/dataframe/display.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/dataframe/groupby_and_agg.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/dataframe/has_column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/dataframe/schema_flat.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/dataframe/show_string.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/dataframe/smart_join.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/dataframe/window_filter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.461008 laktory-0.3.3/docs/api/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/_constants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/add.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/convert_units.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/div.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/mul.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/poly1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/poly2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/roundp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/scaled_power.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/string_split.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/sub.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/api/spark/functions/uuid.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.465008 laktory-0.3.3/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/governance.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.465008 laktory-0.3.3/docs/concepts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/models/models.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/models/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/models/sourcessinks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/models/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/spark.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/concepts/variables.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/demos.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.465008 laktory-0.3.3/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/guides/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/guides/compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/guides/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/guides/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/guides/secrets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/guides/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/guides/users.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.473008 laktory-0.3.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/databricks.png
+-rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/delta_live_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)   240172 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/dlt_debug.png
+-rw-r--r--   0 runner    (1001) docker     (127)   256333 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/dlt_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   221423 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/job_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/kappa.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/lakehouse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/logo_sg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/logo_sg_ltb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/logo_sw.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/logo_sw_ltw.png
+-rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/medaillon_complex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/medallion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/okube.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/pl_quickstart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/pl_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/pl_stock_prices_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/pulumi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/stock_prices_lineage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/terraform.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/images/what_is_laktory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/lakehouseascode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.477008 laktory-0.3.3/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-30 04:45:00.000000 laktory-0.3.3/docs/stylesheets/mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.477008 laktory-0.3.3/laktory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.481008 laktory-0.3.3/laktory/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_testing/stackvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_testing/stockprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.481008 laktory-0.3.3/laktory/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/_quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/cli/quickstart_stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.481008 laktory-0.3.3/laktory/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/dispatcher/dispatcherrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/dispatcher/dltpipelinerunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/dispatcher/jobrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.481008 laktory-0.3.3/laktory/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/dlt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.485008 laktory-0.3.3/laktory/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.485008 laktory-0.3.3/laktory/models/azurenative/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/azurenative/storageblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16431 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/dataproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.485008 laktory-0.3.3/laktory/models/datasinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasinks/basedatasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasinks/filedatasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasinks/tabledatasink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.485008 laktory-0.3.3/laktory/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasources/basedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasources/filedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasources/memorydatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasources/pipelinenodedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/datasources/tabledatasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.489009 laktory-0.3.3/laktory/models/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/cataloggrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/connectiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/externallocationgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/functiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/metastoregrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/registeredmodelgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/schemagrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/sharegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/storagecredentialgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/tablegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/viewgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/grants/volumegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24304 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/pipelinenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/pipelinenodeexpectation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.489009 laktory-0.3.3/laktory/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/baseresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.497008 laktory-0.3.3/laktory/models/resources/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/accesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/dltpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/externallocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/groupmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24460 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/metastoreassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/metastoredataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/mwspermissionassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/secretacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/secretscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/serviceprincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/serviceprincipalrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/sqlquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/userrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/databricks/workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.497008 laktory-0.3.3/laktory/models/resources/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/providers/awsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/providers/azureprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/providers/azurepulumiprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/providers/baseprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/providers/databricksprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/pulumiresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/resources/terraformresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.497008 laktory-0.3.3/laktory/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/spark/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/spark/sparkchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/spark/sparkchainnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/spark/sparkfuncarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.497008 laktory-0.3.3/laktory/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/stacks/pulumistack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22331 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/stacks/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/models/stacks/terraformstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.497008 laktory-0.3.3/laktory/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/polars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.437008 laktory-0.3.3/laktory/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.501009 laktory-0.3.3/laktory/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/resources/data/stock_prices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.501009 laktory-0.3.3/laktory/resources/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/resources/notebooks/dlt_laktory_pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/resources/notebooks/job_laktory_pl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.501009 laktory-0.3.3/laktory/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.501009 laktory-0.3.3/laktory/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/groupby_and_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/has_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/schema_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/show_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/smart_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/dataframe/window_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.501009 laktory-0.3.3/laktory/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/functions/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/functions/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/functions/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/spark/functions/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-30 04:45:00.000000 laktory-0.3.3/laktory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.529009 laktory-0.3.3/laktory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-30 04:45:09.000000 laktory-0.3.3/laktory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20411 2024-05-30 04:45:09.000000 laktory-0.3.3/laktory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 04:45:09.000000 laktory-0.3.3/laktory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 04:45:09.000000 laktory-0.3.3/laktory.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-30 04:45:09.000000 laktory-0.3.3/laktory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 04:45:09.000000 laktory-0.3.3/laktory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-30 04:45:00.000000 laktory-0.3.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-30 04:45:00.000000 laktory-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.505009 laktory-0.3.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-30 04:45:00.000000 laktory-0.3.3/scripts/databricks_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 04:45:00.000000 laktory-0.3.3/scripts/polars_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 04:45:00.000000 laktory-0.3.3/scripts/test_computed_filed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 04:45:00.000000 laktory-0.3.3/scripts/test_db_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.505009 laktory-0.3.3/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 04:45:00.000000 laktory-0.3.3/settings/dev.env
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 04:45:09.537009 laktory-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.513009 laktory-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/build_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.513009 laktory-0.3.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.513009 laktory-0.3.3/tests/data/brz_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/brz_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/brz_stock_prices/.part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/brz_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.437008 laktory-0.3.3/tests/data/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.437008 laktory-0.3.3/tests/data/events/yahoo-finance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.437008 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.437008 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.441008 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.513009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.517009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/05/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.517009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/06/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.517009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/07/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.517009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/08/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.517009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/11/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.517009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/12/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.521009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/13/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.521009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/14/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.521009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/15/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.521009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/18/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.521009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/19/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.525009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/20/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.525009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/21/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.525009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/22/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.525009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/25/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.525009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/26/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.529009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/27/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.529009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/28/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.529009 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/29/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/pl-spark-dlt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/pl-spark-job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/pl-spark-local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/pl-spark-streaming.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.529009 laktory-0.3.3/tests/data/slv_stock_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_meta/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_meta/.part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_meta/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:09.529009 laktory-0.3.3/tests/data/slv_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_prices/.part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/stack_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/stockprices0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/stockprices1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/data/stockprices2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_datasinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_dlt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_dltpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14079 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_pipeline_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_spark_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_spark_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27040 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-30 04:45:00.000000 laktory-0.3.3/tests/test_workspacefile.py
```

### Comparing `laktory-0.3.2/.github/ISSUE_TEMPLATE/bug.yaml` & `laktory-0.3.3/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.github/ISSUE_TEMPLATE/feature.yaml` & `laktory-0.3.3/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.github/scripts/bump_version.py` & `laktory-0.3.3/.github/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.github/scripts/update_quickstart_stack.py` & `laktory-0.3.3/.github/scripts/update_quickstart_stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.github/scripts/write_release_body.py` & `laktory-0.3.3/.github/scripts/write_release_body.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.github/workflows/release.yml` & `laktory-0.3.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.github/workflows/run_quickstart.yml` & `laktory-0.3.3/.github/workflows/run_quickstart.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.github/workflows/test.yml` & `laktory-0.3.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/.gitignore` & `laktory-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/CHANGELOG.md` & `laktory-0.3.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 # Release History
 
-## [0.3.2] - Unreleased
+## [0.3.3] - Unreleased
+### Added
+* Support for SQL expression in SparkChain node
+* Limit option to Data Sources
+* Sample option to Data Sources
+* Display method for Spark DataFrames
+### Updated
+* Stack model environments to support overwrite of individual list element
+### Fixed
+* Pipeline Node data source read with DLT in debug mode
+
+## [0.3.2] - 2024-05-28
 ### Updated
 * Install instructions
 ### Breaking changes
 * Re-organized optional dependencies
 * Remove support for Pulumi python
 
 ## [0.3.1] - 2024-05-28
```

### Comparing `laktory-0.3.2/LICENSE` & `laktory-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/PKG-INFO` & `laktory-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.3.2
+Version: 0.3.3
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laktory-0.3.2/README.md` & `laktory-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/api/models/resources/databricks/cluster.md` & `laktory-0.3.3/docs/api/models/resources/databricks/cluster.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/api/models/resources/databricks/grants.md` & `laktory-0.3.3/docs/api/models/resources/databricks/grants.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/api/models/resources/databricks/job.md` & `laktory-0.3.3/docs/api/models/resources/databricks/job.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/api/models/resources/databricks/metastoredataaccess.md` & `laktory-0.3.3/docs/api/models/resources/databricks/metastoredataaccess.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/cli.md` & `laktory-0.3.3/docs/concepts/cli.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/deployment.md` & `laktory-0.3.3/docs/concepts/deployment.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/design.md` & `laktory-0.3.3/docs/concepts/design.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/governance.md` & `laktory-0.3.3/docs/concepts/governance.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/models/dataevent.md` & `laktory-0.3.3/docs/concepts/models/dataevent.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/models/models.md` & `laktory-0.3.3/docs/concepts/models/models.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/models/pipeline.md` & `laktory-0.3.3/docs/concepts/models/pipeline.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/models/sourcessinks.md` & `laktory-0.3.3/docs/concepts/models/sourcessinks.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/models/sparkchain.md` & `laktory-0.3.3/docs/concepts/models/sparkchain.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/spark.md` & `laktory-0.3.3/docs/concepts/spark.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/stack.md` & `laktory-0.3.3/docs/concepts/stack.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/concepts/variables.md` & `laktory-0.3.3/docs/concepts/variables.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/databricks.png` & `laktory-0.3.3/docs/images/databricks.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/delta_live_tables.png` & `laktory-0.3.3/docs/images/delta_live_tables.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/dlt_debug.png` & `laktory-0.3.3/docs/images/dlt_debug.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/dlt_stock_prices.png` & `laktory-0.3.3/docs/images/dlt_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/job_stock_prices.png` & `laktory-0.3.3/docs/images/job_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/kappa.png` & `laktory-0.3.3/docs/images/kappa.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/lakehouse.png` & `laktory-0.3.3/docs/images/lakehouse.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/logo_sg.png` & `laktory-0.3.3/docs/images/logo_sg.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/logo_sg_ltb.png` & `laktory-0.3.3/docs/images/logo_sg_ltb.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/logo_sw.png` & `laktory-0.3.3/docs/images/logo_sw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/logo_sw_ltw.png` & `laktory-0.3.3/docs/images/logo_sw_ltw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/medaillon_complex.png` & `laktory-0.3.3/docs/images/medaillon_complex.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/medallion.png` & `laktory-0.3.3/docs/images/medallion.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/okube.png` & `laktory-0.3.3/docs/images/okube.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/pl_quickstart.png` & `laktory-0.3.3/docs/images/pl_quickstart.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/pl_stock_prices.png` & `laktory-0.3.3/docs/images/pl_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/pl_stock_prices_simple.png` & `laktory-0.3.3/docs/images/pl_stock_prices_simple.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/pulumi.png` & `laktory-0.3.3/docs/images/pulumi.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/stock_prices_lineage.png` & `laktory-0.3.3/docs/images/stock_prices_lineage.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/terraform.png` & `laktory-0.3.3/docs/images/terraform.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/images/what_is_laktory.png` & `laktory-0.3.3/docs/images/what_is_laktory.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/index.md` & `laktory-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/install.md` & `laktory-0.3.3/docs/install.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/lakehouseascode.md` & `laktory-0.3.3/docs/lakehouseascode.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/quickstart.md` & `laktory-0.3.3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/docs/stylesheets/mkdocstrings.css` & `laktory-0.3.3/docs/stylesheets/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/__init__.py` & `laktory-0.3.3/laktory/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/_logger.py` & `laktory-0.3.3/laktory/_logger.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/_parsers.py` & `laktory-0.3.3/laktory/_parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,13 +51,20 @@
 def merge_dicts(d1: dict, d2: dict) -> dict:
     dm = copy.deepcopy(d1)
 
     def _merge_dicts(d1, d2):
         for key, value in d2.items():
             if key in d1 and isinstance(d1[key], dict) and isinstance(value, dict):
                 _merge_dicts(d1[key], value)
+            elif key in d1 and isinstance(d1[key], list) and isinstance(value, dict):
+                for index, sub_value in value.items():
+                    idx = int(index)
+                    if isinstance(d1[key][idx], dict):
+                        _merge_dicts(d1[key][idx], sub_value)
+                    else:
+                        d1[key][idx] = sub_value
             else:
                 d1[key] = value
 
     _merge_dicts(dm, d2)
 
     return dm
```

### Comparing `laktory-0.3.2/laktory/_settings.py` & `laktory-0.3.3/laktory/_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/_testing/stackvalidator.py` & `laktory-0.3.3/laktory/_testing/stackvalidator.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/_testing/stockprices.py` & `laktory-0.3.3/laktory/_testing/stockprices.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/cli/_common.py` & `laktory-0.3.3/laktory/cli/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     def pulumi_stack_name(self):
         return self.organization + "/" + self.env
 
     def pulumi_call(self, cmd):
         if self.pulumi_stack_name is None:
             raise ValueError("Argument `stack` must be specified with pulumi backend")
 
-        pstack = self.stack.to_pulumi(env=self.env)
+        pstack = self.stack.to_pulumi(env_name=self.env)
         getattr(pstack, cmd)(stack=self.pulumi_stack_name, flags=self.pulumi_options)
 
     def terraform_call(self, cmd):
-        pstack = self.stack.to_terraform(env=self.env)
+        pstack = self.stack.to_terraform(env_name=self.env)
         getattr(pstack, cmd)(flags=self.terraform_options)
 
 
 class Worker:
     def run(self, cmd, cwd=None, raise_exceptions=True):
         try:
             completed_process = subprocess.run(
```

### Comparing `laktory-0.3.2/laktory/cli/_deploy.py` & `laktory-0.3.3/laktory/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/cli/_init.py` & `laktory-0.3.3/laktory/cli/_init.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/cli/_preview.py` & `laktory-0.3.3/laktory/cli/_preview.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/cli/_quickstart.py` & `laktory-0.3.3/laktory/cli/_quickstart.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/cli/_run.py` & `laktory-0.3.3/laktory/cli/_run.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/cli/_write.py` & `laktory-0.3.3/laktory/cli/_write.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/cli/quickstart_stack.yaml` & `laktory-0.3.3/laktory/cli/quickstart_stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/constants.py` & `laktory-0.3.3/laktory/constants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/datetime.py` & `laktory-0.3.3/laktory/datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/dispatcher/dispatcher.py` & `laktory-0.3.3/laktory/dispatcher/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,21 +90,23 @@
     # Workspace Client                                                        #
     # ----------------------------------------------------------------------- #
 
     @property
     def _workspace_arguments(self):
         data = {}
         if self.stack.backend == "pulumi":
-            config = self.stack.to_pulumi(env=self.env).model_dump()["config"]
+            config = self.stack.to_pulumi(env_name=self.env).model_dump()["config"]
             for k, v in config.items():
                 if k.startswith("databricks"):
                     _k = k.split(":")[1]
                     data[_k] = v
         elif self.stack.backend == "terraform":
-            providers = self.stack.to_terraform(env=self.env).model_dump()["provider"]
+            providers = self.stack.to_terraform(env_name=self.env).model_dump()[
+                "provider"
+            ]
             for k in providers:
                 if "databricks" in k.lower():
                     data = providers[k]
                     break
 
         kwargs = {}
         for k in [
```

### Comparing `laktory-0.3.2/laktory/dispatcher/dispatcherrunner.py` & `laktory-0.3.3/laktory/dispatcher/dispatcherrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/dispatcher/dltpipelinerunner.py` & `laktory-0.3.3/laktory/dispatcher/dltpipelinerunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/dispatcher/jobrunner.py` & `laktory-0.3.3/laktory/dispatcher/jobrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/dlt/__init__.py` & `laktory-0.3.3/laktory/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/azurenative/storageblob.py` & `laktory-0.3.3/laktory/models/azurenative/storageblob.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/basemodel.py` & `laktory-0.3.3/laktory/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/dataevent.py` & `laktory-0.3.3/laktory/models/dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/dataproducer.py` & `laktory-0.3.3/laktory/models/dataproducer.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/datasinks/basedatasink.py` & `laktory-0.3.3/laktory/models/datasinks/basedatasink.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/datasinks/filedatasink.py` & `laktory-0.3.3/laktory/models/datasinks/filedatasink.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/datasinks/tabledatasink.py` & `laktory-0.3.3/laktory/models/datasinks/tabledatasink.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/datasources/basedatasource.py` & `laktory-0.3.3/laktory/models/datasources/basedatasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 from laktory.polars import is_polars_dataframe
 from laktory.types import AnyDataFrame
 from laktory._logger import get_logger
 
 logger = get_logger(__name__)
 
 
+class DataFrameSample(BaseModel):
+    fraction: float
+    seed: Union[int, None] = None
+
+
 class Watermark(BaseModel):
     """
     Definition of a spark structured streaming watermark for joining data
     streams.
 
     Attributes
     ----------
@@ -129,16 +134,18 @@
 
     as_stream: bool = False
     broadcast: Union[bool, None] = False
     cdc: Union[DataSourceCDC, None] = None
     dataframe_type: Literal["SPARK", "POLARS"] = "SPARK"
     drops: Union[list, None] = None
     filter: Union[str, None] = None
+    limit: Union[int, None] = None
     mock_df: Any = Field(default=None, exclude=True)
     renames: Union[dict[str, str], None] = None
+    sample: Union[DataFrameSample, None] = None
     selects: Union[list[str], dict[str, str], None] = None
     watermark: Union[Watermark, None] = None
     _pipeline_node: "PipelineNode" = None
 
     @model_validator(mode="after")
     def options(self) -> Any:
 
@@ -256,14 +263,22 @@
                 self.watermark.threshold,
             )
 
         # Broadcast
         if self.broadcast:
             df = F.broadcast(df)
 
+        # Sample
+        if self.sample:
+            df = df.sample(fraction=self.sample.fraction, seed=self.sample.seed)
+
+        # Limit
+        if self.limit:
+            df = df.limit(self.limit)
+
         # SparkChain
         # if self.spark_chain:
         #     df = self.spark_chain.execute(df, udfs=None, spark=df.sparkSession)
 
         return df
 
     def _post_read_polars(self, df: PolarsDataFrame) -> PolarsDataFrame:
```

### Comparing `laktory-0.3.2/laktory/models/datasources/filedatasource.py` & `laktory-0.3.3/laktory/models/datasources/filedatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/datasources/memorydatasource.py` & `laktory-0.3.3/laktory/models/datasources/memorydatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/datasources/pipelinenodedatasource.py` & `laktory-0.3.3/laktory/models/datasources/pipelinenodedatasource.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
     # pl.execute(spark=spark)
     ```
     """
 
     node_name: Union[str, None]
     node: Any = Field(None, exclude=True)  # Add suggested type?
+    # include_failed_expectations: bool = True  # TODO: Implement
+    # include_passed_expectations: bool = True  # TODO: Implement
 
     # ----------------------------------------------------------------------- #
     # Properties                                                              #
     # ----------------------------------------------------------------------- #
 
     @property
     def _id(self) -> str:
@@ -70,47 +72,57 @@
         if self.is_orchestrator_dlt:
 
             from laktory.dlt import read as dlt_read
             from laktory.dlt import read_stream as dlt_read_stream
             from laktory.dlt import is_debug
 
             if is_debug():
-                logger.info(f"Reading pipeline node {self._id} from sink (DLT debug)")
                 df = None
-                if self.node.sink:
+                if self.node.output_df:
+                    logger.info(
+                        f"Reading pipeline node {self._id} from output DataFrame (DLT debug)"
+                    )
+                    df = self.node.output_df
+                elif self.node.sink:
+                    logger.info(
+                        f"Reading pipeline node {self._id} from sink (DLT debug)"
+                    )
                     df = self.node.sink.read(spark=spark, as_stream=self.as_stream)
+                else:
+                    logger.info(f"Can't read pipeline node {self._id} (DLT DEBUG)")
+
             else:
                 if self.as_stream:
                     logger.info(f"Reading pipeline node {self._id} with DLT as stream")
                     df = dlt_read_stream(self.node.name)
                 else:
                     logger.info(f"Reading pipeline node {self._id} with DLT as static")
                     df = dlt_read(self.node.name)
 
         # Read from node output DataFrame (if available)
-        elif self.node._output_df:
+        elif self.node.output_df:
             logger.info(f"Reading pipeline node {self._id} from output DataFrame")
-            df = self.node._output_df
+            df = self.node.output_df
 
         # Read from node sink
         elif self.node.sink:
             logger.info(f"Reading pipeline node {self._id} from sink")
             df = self.node.sink.read(spark=spark, as_stream=self.as_stream)
 
         else:
             raise ValueError(f"Pipeline Node {self._id} can't read DataFrame")
 
         return df
 
     def _read_polars(self) -> PolarsDataFrame:
 
         # Read from node output DataFrame (if available)
-        if self.node._output_df:
+        if self.node.output_df:
             logger.info(f"Reading pipeline node {self._id} from output DataFrame")
-            df = self.node._output_df
+            df = self.node.output_df
 
         # Read from node sink
         elif self.node.sink:
             logger.info(f"Reading pipeline node {self._id} from sink")
             df = self.node.sink.read(as_stream=self.as_stream)
 
         else:
```

### Comparing `laktory-0.3.2/laktory/models/datasources/tabledatasource.py` & `laktory-0.3.3/laktory/models/datasources/tabledatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/__init__.py` & `laktory-0.3.3/laktory/models/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/cataloggrant.py` & `laktory-0.3.3/laktory/models/grants/cataloggrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/connectiongrant.py` & `laktory-0.3.3/laktory/models/grants/connectiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/externallocationgrant.py` & `laktory-0.3.3/laktory/models/grants/externallocationgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/functiongrant.py` & `laktory-0.3.3/laktory/models/grants/functiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/metastoregrant.py` & `laktory-0.3.3/laktory/models/grants/metastoregrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/registeredmodelgrant.py` & `laktory-0.3.3/laktory/models/grants/registeredmodelgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/schemagrant.py` & `laktory-0.3.3/laktory/models/grants/schemagrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/sharegrant.py` & `laktory-0.3.3/laktory/models/grants/sharegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/storagecredentialgrant.py` & `laktory-0.3.3/laktory/models/grants/storagecredentialgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/tablegrant.py` & `laktory-0.3.3/laktory/models/grants/tablegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/viewgrant.py` & `laktory-0.3.3/laktory/models/grants/viewgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/grants/volumegrant.py` & `laktory-0.3.3/laktory/models/grants/volumegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/pipeline.py` & `laktory-0.3.3/laktory/models/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -537,31 +537,33 @@
 
         return nodes
 
     # ----------------------------------------------------------------------- #
     # Methods                                                                 #
     # ----------------------------------------------------------------------- #
 
-    def execute(self, spark, udfs=None) -> None:
+    def execute(self, spark, udfs=None, write_sinks=True) -> None:
         """
         Execute the pipeline (read sources and write sinks) by sequentially
         executing each node. The selected orchestrator might impact how
         data sources or sinks are processed.
 
         Parameters
         ----------
         spark:
             Spark Session
         udfs:
             List of user-defined functions used in transformation chains.
+        write_sinks:
+            If `False` writing of node sinks will be skipped
         """
         logger.info("Executing Pipeline")
 
         for inode, node in enumerate(self.sorted_nodes):
-            node.execute(spark=spark, udfs=udfs)
+            node.execute(spark=spark, udfs=udfs, write_sink=write_sinks)
 
     def dag_figure(self) -> Figure:
         """
         [UNDER DEVELOPMENT] Generate a figure representation of the pipeline
         DAG.
 
         Returns
```

### Comparing `laktory-0.3.2/laktory/models/pipelinenode.py` & `laktory-0.3.3/laktory/models/pipelinenode.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,19 @@
             "stored_as_scd_type": cdc.scd_type,
             "target": self.sink.table_name,
             "track_history_column_list": cdc.track_history_columns,
             "track_history_except_column_list": cdc.track_history_except_columns,
         }
 
     @property
+    def output_df(self) -> AnyDataFrame:
+        """Node Dataframe after reading source and applying transformer."""
+        return self._output_df
+
+    @property
     def layer_spark_chain(self):
         nodes = []
 
         if self.layer == "BRONZE":
             if self.add_layer_columns:
                 nodes += [
                     SparkChainNode(
```

### Comparing `laktory-0.3.2/laktory/models/pipelinenodeexpectation.py` & `laktory-0.3.3/laktory/models/pipelinenodeexpectation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/baseresource.py` & `laktory-0.3.3/laktory/models/resources/baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/__init__.py` & `laktory-0.3.3/laktory/models/resources/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/accesscontrol.py` & `laktory-0.3.3/laktory/models/resources/databricks/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/catalog.py` & `laktory-0.3.3/laktory/models/resources/databricks/catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/cluster.py` & `laktory-0.3.3/laktory/models/resources/databricks/cluster.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/column.py` & `laktory-0.3.3/laktory/models/resources/databricks/column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/dbfsfile.py` & `laktory-0.3.3/laktory/models/resources/databricks/dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/directory.py` & `laktory-0.3.3/laktory/models/resources/databricks/directory.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/dltpipeline.py` & `laktory-0.3.3/laktory/models/resources/databricks/dltpipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/externallocation.py` & `laktory-0.3.3/laktory/models/resources/databricks/externallocation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/grants.py` & `laktory-0.3.3/laktory/models/resources/databricks/grants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/group.py` & `laktory-0.3.3/laktory/models/resources/databricks/group.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/groupmember.py` & `laktory-0.3.3/laktory/models/resources/databricks/groupmember.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/job.py` & `laktory-0.3.3/laktory/models/resources/databricks/job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/metastore.py` & `laktory-0.3.3/laktory/models/resources/databricks/metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/metastoreassignment.py` & `laktory-0.3.3/laktory/models/resources/databricks/metastoreassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/metastoredataaccess.py` & `laktory-0.3.3/laktory/models/resources/databricks/metastoredataaccess.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/mwspermissionassignment.py` & `laktory-0.3.3/laktory/models/resources/databricks/mwspermissionassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/notebook.py` & `laktory-0.3.3/laktory/models/resources/databricks/notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/permissions.py` & `laktory-0.3.3/laktory/models/resources/databricks/permissions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/schema.py` & `laktory-0.3.3/laktory/models/resources/databricks/schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/secret.py` & `laktory-0.3.3/laktory/models/resources/databricks/secret.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/secretacl.py` & `laktory-0.3.3/laktory/models/resources/databricks/secretacl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/secretscope.py` & `laktory-0.3.3/laktory/models/resources/databricks/secretscope.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/serviceprincipal.py` & `laktory-0.3.3/laktory/models/resources/databricks/serviceprincipal.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/serviceprincipalrole.py` & `laktory-0.3.3/laktory/models/resources/databricks/serviceprincipalrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/sqlquery.py` & `laktory-0.3.3/laktory/models/resources/databricks/sqlquery.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/table.py` & `laktory-0.3.3/laktory/models/resources/databricks/table.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/user.py` & `laktory-0.3.3/laktory/models/resources/databricks/user.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/userrole.py` & `laktory-0.3.3/laktory/models/resources/databricks/userrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/volume.py` & `laktory-0.3.3/laktory/models/resources/databricks/volume.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/warehouse.py` & `laktory-0.3.3/laktory/models/resources/databricks/warehouse.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/databricks/workspacefile.py` & `laktory-0.3.3/laktory/models/resources/databricks/workspacefile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/providers/awsprovider.py` & `laktory-0.3.3/laktory/models/resources/providers/awsprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/providers/azureprovider.py` & `laktory-0.3.3/laktory/models/resources/providers/azureprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/providers/azurepulumiprovider.py` & `laktory-0.3.3/laktory/models/resources/providers/azurepulumiprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/providers/baseprovider.py` & `laktory-0.3.3/laktory/models/resources/providers/baseprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/providers/databricksprovider.py` & `laktory-0.3.3/laktory/models/resources/providers/databricksprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/pulumiresource.py` & `laktory-0.3.3/laktory/models/resources/pulumiresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/resources/terraformresource.py` & `laktory-0.3.3/laktory/models/resources/terraformresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/spark/_common.py` & `laktory-0.3.3/laktory/models/spark/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/spark/sparkchain.py` & `laktory-0.3.3/laktory/models/spark/sparkchain.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/spark/sparkchainnode.py` & `laktory-0.3.3/laktory/models/spark/sparkchainnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         To support spark functions expecting column argument, col("x"),
         lit("3") and expr("x*2") can be provided.
     spark_func_name:
         Name of the spark function to build the dataframe. If `column` is
         specified, the spark function should return a column instead. Mutually
          exclusive to `sql_expression`.
     sql_expression:
-        Expression defining how to build the column. If `column` is
+        SQL Expression using `{df}` to reference upstream dataframe and
+        defining how to build the output dataframe. If `column` is
         specified, the sql expression should define a column instead. Mutually
          exclusive to `spark_func_name`
 
     Examples
     --------
     ```py
     import pandas as pd
@@ -210,16 +211,14 @@
                 col = F.expr(self.sql_expression).alias(self.column.name)
                 if self.column.type not in ["_any"]:
                     col = col.cast(self.column.type)
                 if return_col:
                     return col
                 return self.add_column(df, col)
             else:
-                raise NotImplementedError("sql_expression not supported yet")
-                # TODO: This implementation should workd, but it should be tested and documented
                 df = df.sparkSession.sql(self.sql_expression, df=df)
                 return df
 
         # From Spark Function
         func_name = self.spark_func_name
         if self.spark_func_name is None:
             if self.is_column:
```

### Comparing `laktory-0.3.2/laktory/models/spark/sparkfuncarg.py` & `laktory-0.3.3/laktory/models/spark/sparkfuncarg.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/stacks/pulumistack.py` & `laktory-0.3.3/laktory/models/stacks/pulumistack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/models/stacks/stack.py` & `laktory-0.3.3/laktory/models/stacks/stack.py`

 * *Files 3% similar despite different names*

```diff
@@ -337,24 +337,28 @@
     pulumi: Pulumi = Pulumi()
     resources: Union[StackResources, None] = StackResources()
     terraform: Terraform = Terraform()
     variables: dict[str, Any] = {}
     _envs: dict[str, EnvironmentStack] = None
 
     # ----------------------------------------------------------------------- #
-    # Properties                                                              #
+    # Methods                                                                 #
     # ----------------------------------------------------------------------- #
 
-    @property
-    def envs(self) -> dict[str, EnvironmentStack]:
+    def get_env(self, env_name: str, inject_vars=True) -> EnvironmentStack:
         """
-        Complete definition of each of the stack environments. It takes into
+        Complete definition the stack for a given environment. It takes into
         account both the default stack values and environment-specific
         overwrites.
 
+        Parameters
+        ----------
+        env_name:
+            Name of the environment
+
         Returns
         -------
         :
             Environment definitions.
         """
 
         if self._envs is None:
@@ -406,46 +410,51 @@
 
                 return data
 
             d = dump_with_options(self)
             _envs = d.pop("environments")
 
             envs = {}
-            for env_name, env in self.environments.items():
+            for _env_name, env in self.environments.items():
                 for k in ENV_FIELDS:
                     if k in d:
-                        d[k] = merge_dicts(d[k], _envs[env_name].get(k, {}))
-                envs[env_name] = EnvironmentStack(**d)
+                        d[k] = merge_dicts(d[k], _envs[_env_name].get(k, {}))
+
+                # Inject Variables
+                if inject_vars:
+                    d = self.environments[_env_name].inject_vars(d)
+
+                envs[_env_name] = EnvironmentStack(**d)
 
             self._envs = envs
 
-        return self._envs
+        return self._envs[env_name]
 
     # ----------------------------------------------------------------------- #
     # Pulumi Methods                                                          #
     # ----------------------------------------------------------------------- #
 
-    def to_pulumi(self, env: Union[str, None] = None):
+    def to_pulumi(self, env_name: Union[str, None] = None):
         """
         Create a pulumi stack for a given environment `env`.
 
         Parameters
         ----------
-        env:
+        env_name:
             Target environment. If `None`, used default stack values only.
 
         Returns
         -------
         : PulumiStack
             Pulumi-specific stack definition
         """
         from laktory.models.stacks.pulumistack import PulumiStack
 
-        if env is not None and env in self.envs:
-            env = self.envs[env]
+        if env_name is not None and env_name in self.environments.keys():
+            env = self.get_env(env_name=env_name, inject_vars=False)
         else:
             env = self
 
         # Resources
         resources = {}
         for r in env.resources._get_all().values():
             r.variables = env.variables
@@ -462,32 +471,32 @@
             outputs=env.pulumi.outputs,
         )
 
     # ----------------------------------------------------------------------- #
     # Terraform Methods                                                       #
     # ----------------------------------------------------------------------- #
 
-    def to_terraform(self, env: Union[str, None] = None):
+    def to_terraform(self, env_name: Union[str, None] = None):
         """
         Create a terraform stack for a given environment `env`.
 
         Parameters
         ----------
-        env:
+        env_name:
             Target environment. If `None`, used default stack values only.
 
         Returns
         -------
         : TerraformStack
             Terraform-specific stack definition
         """
         from laktory.models.stacks.terraformstack import TerraformStack
 
-        if env is not None and env in self.envs:
-            env = self.envs[env]
+        if env_name is not None and env_name in self.environments.keys():
+            env = self.get_env(env_name=env_name, inject_vars=False)
         else:
             env = self
 
         # Providers
         providers = {}
         for r in env.resources._get_all(providers_only=True).values():
             for _r in r.core_resources:
```

### Comparing `laktory-0.3.2/laktory/models/stacks/terraformstack.py` & `laktory-0.3.3/laktory/models/stacks/terraformstack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/resources/data/stock_prices.json` & `laktory-0.3.3/laktory/resources/data/stock_prices.json`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/resources/notebooks/dlt_laktory_pl.py` & `laktory-0.3.3/laktory/resources/notebooks/dlt_laktory_pl.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from laktory import get_logger
 from laktory import settings
 
 dlt.spark = spark
 logger = get_logger(__name__)
 
 # Read pipeline definition
-pl_name = spark.conf.get("pipeline_name", "pl-stock-prices")
+pl_name = spark.conf.get("pipeline_name", "dlt-stock-prices")
 filepath = f"/Workspace{settings.workspace_laktory_root}pipelines/{pl_name}.json"
 with open(filepath, "r") as fp:
     pl = models.Pipeline.model_validate_json(fp.read())
 
 
 # Import User Defined Functions
 sys.path.append(f"/Workspace{settings.workspace_laktory_root}pipelines/")
```

### Comparing `laktory-0.3.2/laktory/resources/notebooks/job_laktory_pl.py` & `laktory-0.3.3/laktory/resources/notebooks/job_laktory_pl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/__init__.py` & `laktory-0.3.3/laktory/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/dataframe/__init__.py` & `laktory-0.3.3/laktory/spark/dataframe/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from pyspark.sql.dataframe import DataFrame
 
-from laktory.spark.dataframe.schema_flat import schema_flat
+from laktory.spark.dataframe.display import display
+from laktory.spark.dataframe.groupby_and_agg import groupby_and_agg
 from laktory.spark.dataframe.has_column import has_column
+from laktory.spark.dataframe.schema_flat import schema_flat
 from laktory.spark.dataframe.show_string import show_string
 from laktory.spark.dataframe.smart_join import smart_join
 from laktory.spark.dataframe.watermark import watermark
-from laktory.spark.dataframe.groupby_and_agg import groupby_and_agg
 from laktory.spark.dataframe.window_filter import window_filter
 
 
 # DataFrame Extensions
-DataFrame.schema_flat = schema_flat
+DataFrame.display = display
+DataFrame.groupby_and_agg = groupby_and_agg
 DataFrame.has_column = has_column
+DataFrame.schema_flat = schema_flat
 DataFrame.show_string = show_string
 DataFrame.smart_join = smart_join
 DataFrame.watermark = watermark
-DataFrame.groupby_and_agg = groupby_and_agg
 DataFrame.window_filter = window_filter
 
 # Spark Connect DataFrame Extensions
 try:
     from pyspark.sql.connect.dataframe import DataFrame
 
-    DataFrame.schema_flat = schema_flat
+    DataFrame.display = display
+    DataFrame.groupby_and_agg = groupby_and_agg
     DataFrame.has_column = has_column
+    DataFrame.schema_flat = schema_flat
     DataFrame.show_string = show_string
     DataFrame.smart_join = smart_join
     DataFrame.watermark = watermark
-    DataFrame.groupby_and_agg = groupby_and_agg
     DataFrame.window_filter = window_filter
 except:
     pass
```

### Comparing `laktory-0.3.2/laktory/spark/dataframe/groupby_and_agg.py` & `laktory-0.3.3/laktory/spark/dataframe/groupby_and_agg.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/dataframe/has_column.py` & `laktory-0.3.3/laktory/spark/dataframe/has_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/dataframe/schema_flat.py` & `laktory-0.3.3/laktory/spark/dataframe/schema_flat.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/dataframe/show_string.py` & `laktory-0.3.3/laktory/spark/dataframe/show_string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/dataframe/smart_join.py` & `laktory-0.3.3/laktory/spark/dataframe/smart_join.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/dataframe/watermark.py` & `laktory-0.3.3/laktory/spark/dataframe/watermark.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/dataframe/window_filter.py` & `laktory-0.3.3/laktory/spark/dataframe/window_filter.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/functions/_common.py` & `laktory-0.3.3/laktory/spark/functions/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/functions/logical.py` & `laktory-0.3.3/laktory/spark/functions/logical.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/functions/math.py` & `laktory-0.3.3/laktory/spark/functions/math.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/functions/string.py` & `laktory-0.3.3/laktory/spark/functions/string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/spark/functions/units.py` & `laktory-0.3.3/laktory/spark/functions/units.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory/version.py` & `laktory-0.3.3/laktory/version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/laktory.egg-info/PKG-INFO` & `laktory-0.3.3/laktory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.3.2
+Version: 0.3.3
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laktory-0.3.2/laktory.egg-info/SOURCES.txt` & `laktory-0.3.3/laktory.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 docs/api/models/resources/providers/databricks.md
 docs/api/models/spark/sparkchain.md
 docs/api/models/spark/sparkchainnode.md
 docs/api/models/spark/sparkfuncarg.md
 docs/api/models/stacks/pulumistack.md
 docs/api/models/stacks/stack.md
 docs/api/models/stacks/terraformstack.md
+docs/api/spark/dataframe/display.md
 docs/api/spark/dataframe/groupby_and_agg.md
 docs/api/spark/dataframe/has_column.md
 docs/api/spark/dataframe/schema_flat.md
 docs/api/spark/dataframe/show_string.md
 docs/api/spark/dataframe/smart_join.md
 docs/api/spark/dataframe/window_filter.md
 docs/api/spark/functions/_constants.md
@@ -268,14 +269,15 @@
 laktory/models/stacks/terraformstack.py
 laktory/polars/__init__.py
 laktory/resources/data/stock_prices.json
 laktory/resources/notebooks/dlt_laktory_pl.py
 laktory/resources/notebooks/job_laktory_pl.py
 laktory/spark/__init__.py
 laktory/spark/dataframe/__init__.py
+laktory/spark/dataframe/display.py
 laktory/spark/dataframe/groupby_and_agg.py
 laktory/spark/dataframe/has_column.py
 laktory/spark/dataframe/schema_flat.py
 laktory/spark/dataframe/show_string.py
 laktory/spark/dataframe/smart_join.py
 laktory/spark/dataframe/watermark.py
 laktory/spark/dataframe/window_filter.py
```

### Comparing `laktory-0.3.2/mkdocs.yml` & `laktory-0.3.3/mkdocs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,15 @@
       - Stacks:
           - Stack: api/models/stacks/stack.md
           - PulumiStack: api/models/stacks/pulumistack.md
           - TerraformStack: api/models/stacks/terraformstack.md
     - CLI: api/cli.md
     - Spark:
       - DataFrame:
+        - display: api/spark/dataframe/display.md
         - groupby_and_agg: api/spark/dataframe/groupby_and_agg.md
         - has_column: api/spark/dataframe/has_column.md
         - schema_flat: api/spark/dataframe/schema_flat.md
         - smart_join: api/spark/dataframe/smart_join.md
         - show_string: api/spark/dataframe/show_string.md
         - window_filter: api/spark/dataframe/window_filter.md
       - Functions:
```

### Comparing `laktory-0.3.2/pyproject.toml` & `laktory-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/scripts/databricks_api_call.py` & `laktory-0.3.3/scripts/databricks_api_call.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/build_test_data.py` & `laktory-0.3.3/tests/build_test_data.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet` & `laktory-0.3.3/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/pl-spark-dlt.yaml` & `laktory-0.3.3/tests/data/pl-spark-dlt.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/pl-spark-job.yaml` & `laktory-0.3.3/tests/data/pl-spark-job.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/pl-spark-local.yaml` & `laktory-0.3.3/tests/data/pl-spark-local.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/pl-spark-streaming.yaml` & `laktory-0.3.3/tests/data/pl-spark-streaming.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet` & `laktory-0.3.3/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet` & `laktory-0.3.3/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/data/stack.yaml` & `laktory-0.3.3/tests/data/stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_basemodel.py` & `laktory-0.3.3/tests/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_baseresource.py` & `laktory-0.3.3/tests/test_baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_catalog.py` & `laktory-0.3.3/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_cli.py` & `laktory-0.3.3/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def test_preview_terraform():
     filepath = os.path.join(paths.data, "stack.yaml")
 
     # Ideally, we would run `laktory init`, but the runner does not seem to handle running multiple commands
     with open(filepath, "r") as fp:
-        pstack = models.Stack.model_validate_yaml(fp).to_terraform(env="dev")
+        pstack = models.Stack.model_validate_yaml(fp).to_terraform(env_name="dev")
         pstack.init(flags=["-migrate-state", "-upgrade"])
 
     result = runner.invoke(
         app,
         ["preview", "--backend", "terraform", "--env", "dev", "--filepath", filepath],
     )
     assert result.exit_code == 0
```

### Comparing `laktory-0.3.2/tests/test_column.py` & `laktory-0.3.3/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_dataevent.py` & `laktory-0.3.3/tests/test_dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_datasinks.py` & `laktory-0.3.3/tests/test_datasinks.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_datasources.py` & `laktory-0.3.3/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_datetime.py` & `laktory-0.3.3/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_dbfsfile.py` & `laktory-0.3.3/tests/test_dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_dispatcher.py` & `laktory-0.3.3/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_dltpipeline.py` & `laktory-0.3.3/tests/test_dltpipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_docstrings.py` & `laktory-0.3.3/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_job.py` & `laktory-0.3.3/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_metastore.py` & `laktory-0.3.3/tests/test_metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_notebook.py` & `laktory-0.3.3/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_pipeline.py` & `laktory-0.3.3/tests/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,46 +62,46 @@
     fig.write_html(os.path.join(paths.tmp, "dag.html"), auto_open=OPEN_FIGURES)
 
 
 def test_execute():
     pl.execute(spark)
 
     # In memory DataFrames
-    assert pl.nodes_dict["brz_stock_prices"]._output_df.columns == [
+    assert pl.nodes_dict["brz_stock_prices"].output_df.columns == [
         "name",
         "description",
         "producer",
         "data",
         "_bronze_at",
     ]
-    assert pl.nodes_dict["brz_stock_prices"]._output_df.count() == 80
-    assert pl.nodes_dict["slv_stock_meta"]._output_df.columns == [
+    assert pl.nodes_dict["brz_stock_prices"].output_df.count() == 80
+    assert pl.nodes_dict["slv_stock_meta"].output_df.columns == [
         "symbol2",
         "currency",
         "first_traded",
         "_silver_at",
     ]
-    assert pl.nodes_dict["slv_stock_meta"]._output_df.count() == 3
-    assert pl.nodes_dict["slv_stock_prices"]._output_df.columns == [
+    assert pl.nodes_dict["slv_stock_meta"].output_df.count() == 3
+    assert pl.nodes_dict["slv_stock_prices"].output_df.columns == [
         "_bronze_at",
         "created_at",
         "close",
         "currency",
         "first_traded",
         "_silver_at",
         "symbol",
     ]
-    assert pl.nodes_dict["slv_stock_prices"]._output_df.count() == 80
-    assert pl.nodes_dict["gld_max_stock_prices"]._output_df.columns == [
+    assert pl.nodes_dict["slv_stock_prices"].output_df.count() == 80
+    assert pl.nodes_dict["gld_max_stock_prices"].output_df.columns == [
         "symbol",
         "max_price",
         "min_price",
         "_gold_at",
     ]
-    assert pl.nodes_dict["gld_max_stock_prices"]._output_df.count() == 4
+    assert pl.nodes_dict["gld_max_stock_prices"].output_df.count() == 4
 
     # Sinks
     _df_slv = spark.read.format("PARQUET").load(slv_sink_path)
     _df_gld = spark.read.format("PARQUET").load(gld_sink_path)
     assert _df_slv.columns == [
         "_bronze_at",
         "created_at",
@@ -131,15 +131,17 @@
     assert data == {
         "as_stream": True,
         "broadcast": False,
         "cdc": None,
         "dataframe_type": "SPARK",
         "drops": None,
         "filter": None,
+        "limit": None,
         "renames": None,
+        "sample": None,
         "selects": None,
         "watermark": None,
         "catalog_name": "dev",
         "table_name": "brz_stock_prices",
         "schema_name": "sandbox",
         "warehouse": "DATABRICKS",
     }
@@ -198,15 +200,17 @@
                 "source": {
                     "as_stream": True,
                     "broadcast": False,
                     "cdc": None,
                     "dataframe_type": "SPARK",
                     "drops": None,
                     "filter": None,
+                    "limit": None,
                     "renames": None,
+                    "sample": None,
                     "selects": None,
                     "watermark": None,
                     "format": "JSON",
                     "header": True,
                     "multiline": False,
                     "path": "/Volumes/dev/sources/landing/events/yahoo-finance/stock_price/",
                     "read_options": {},
@@ -285,15 +289,17 @@
                 "source": {
                     "as_stream": True,
                     "broadcast": False,
                     "cdc": None,
                     "dataframe_type": "SPARK",
                     "drops": None,
                     "filter": None,
+                    "limit": None,
                     "renames": None,
+                    "sample": None,
                     "selects": None,
                     "watermark": None,
                     "node_name": "brz_stock_prices",
                 },
                 "timestamp_key": None,
             },
         ],
```

### Comparing `laktory-0.3.2/tests/test_pipeline_node.py` & `laktory-0.3.3/tests/test_pipeline_node.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_schema.py` & `laktory-0.3.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_settings.py` & `laktory-0.3.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_spark_chain.py` & `laktory-0.3.3/tests/test_spark_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,36 @@
     df = sc.execute(df)
 
     # Test
     assert df.count() == df0.count() * 2
     assert df.columns == df0.columns
 
 
+def test_dataframe_sql_expression(df0=df0):
+    df = df0.select(df0.columns)
+
+    sc = models.SparkChain(
+        nodes=[
+            {
+                "sql_expression": "SELECT *, x*2 AS x2 FROM {df}",
+            },
+        ]
+    )
+
+    # Execute Chain
+    df = sc.execute(df)
+
+    # Test
+    pdf = df.toPandas()
+    assert pdf.columns.tolist() == ["x", "a", "b", "c", "n", "pi", "p", "word", "x2"]
+    assert pdf["x2"].tolist() == (pdf["x"] * 2).tolist()
+
+    df.show()
+
+
 def test_dataframe_table_input(df0=df0):
     df = df0.select(df0.columns)
 
     sc = models.SparkChain(
         nodes=[
             {
                 "spark_func_name": "union",
@@ -275,14 +297,15 @@
         ]
     )
     with pytest.raises(MissingColumnsError):
         df = sc.execute(df)
 
 
 if __name__ == "__main__":
-    test_spark_func_arg()
-    test_dataframe_df_input()
-    test_dataframe_table_input()
-    test_column()
-    test_udfs()
-    test_nested()
-    test_exceptions()
+    # test_spark_func_arg()
+    # test_dataframe_df_input()
+    test_dataframe_sql_expression()
+    # test_dataframe_table_input()
+    # test_column()
+    # test_udfs()
+    # test_nested()
+    # test_exceptions()
```

### Comparing `laktory-0.3.2/tests/test_spark_dataframe.py` & `laktory-0.3.3/tests/test_spark_dataframe.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_spark_functions.py` & `laktory-0.3.3/tests/test_spark_functions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_sql_query.py` & `laktory-0.3.3/tests/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_stack.py` & `laktory-0.3.3/tests/test_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         },
     }
 
     return stack
 
 
 def test_pulumi_stack():
-    pstack = stack.to_pulumi(env=None)
+    pstack = stack.to_pulumi(env_name=None)
     assert pstack.organization == "okube"
     data_default = pstack.model_dump()
     data_default["config"]["databricks:token"] = "***"
     data_default["resources"]["databricks"]["properties"]["token"] = "***"
     print(data_default)
     assert data_default == {
         "variables": {},
@@ -419,30 +419,30 @@
                 "options": {"dependsOn": [], "deleteBeforeReplace": True},
             },
         },
         "outputs": {},
     }
 
     # Dev
-    data = stack.to_pulumi(env="dev").model_dump()
+    data = stack.to_pulumi(env_name="dev").model_dump()
     data["config"]["databricks:token"] = "***"
     data["resources"]["databricks"]["properties"]["token"] = "***"
     data0 = copy.deepcopy(data_default)
     data0["variables"]["env"] = "dev"
     data0["variables"]["is_dev"] = True
     data0["variables"]["node_type_id"] = "Standard_DS3_v2"
     cluster = data0["resources"]["job-stock-prices-ut-stack"]["properties"][
         "jobClusters"
     ][0]["newCluster"]
     cluster["nodeTypeId"] = "Standard_DS3_v2"
     cluster["sparkEnvVars"]["LAKTORY_WORKSPACE_ENV"] = "dev"
     assert data == data0
 
     # Prod
-    data = stack.to_pulumi(env="prod").model_dump()
+    data = stack.to_pulumi(env_name="prod").model_dump()
     data["config"]["databricks:token"] = "***"
     data["resources"]["databricks"]["properties"]["token"] = "***"
     data0 = copy.deepcopy(data_default)
     data0["variables"]["env"] = "prod"
     data0["variables"]["is_dev"] = False
     data0["variables"]["node_type_id"] = "Standard_DS4_v2"
     cluster = data0["resources"]["job-stock-prices-ut-stack"]["properties"][
@@ -451,15 +451,15 @@
     cluster["nodeTypeId"] = "Standard_DS4_v2"
     cluster["sparkEnvVars"]["LAKTORY_WORKSPACE_ENV"] = "prod"
     data0["resources"]["dlt-custom-name"]["properties"]["development"] = False
     assert data == data0
 
 
 def test_pulumi_preview():
-    pstack = stack.to_pulumi(env="dev")
+    pstack = stack.to_pulumi(env_name="dev")
     pstack.preview(stack="okube/dev")
 
 
 def test_terraform_stack():
     data_default = stack.to_terraform().model_dump()
     data_default["provider"]["databricks"]["token"] = "***"
     print(data_default)
@@ -566,40 +566,40 @@
                     "source": "./tmp-pl-stock-prices-ut-stack.json",
                 }
             },
         },
     }
 
     # Dev
-    data = stack.to_terraform(env="dev").model_dump()
+    data = stack.to_terraform(env_name="dev").model_dump()
     data["provider"]["databricks"]["token"] = "***"
     data0 = copy.deepcopy(data_default)
     print(data0["resource"]["databricks_job"]["job-stock-prices-ut-stack"])
     cluster = data0["resource"]["databricks_job"]["job-stock-prices-ut-stack"][
         "job_cluster"
     ][0]["new_cluster"]
     cluster["node_type_id"] = "Standard_DS3_v2"
     cluster["spark_env_vars"]["LAKTORY_WORKSPACE_ENV"] = "dev"
     assert data == data0
 
     # Prod
-    data = stack.to_terraform(env="prod").model_dump()
+    data = stack.to_terraform(env_name="prod").model_dump()
     data["provider"]["databricks"]["token"] = "***"
     data0 = copy.deepcopy(data_default)
     cluster = data0["resource"]["databricks_job"]["job-stock-prices-ut-stack"][
         "job_cluster"
     ][0]["new_cluster"]
     cluster["node_type_id"] = "Standard_DS4_v2"
     cluster["spark_env_vars"]["LAKTORY_WORKSPACE_ENV"] = "prod"
     data0["resource"]["databricks_pipeline"]["dlt-custom-name"]["development"] = False
     assert data == data0
 
 
 def test_terraform_plan():
-    tstack = stack.to_terraform(env="dev")
+    tstack = stack.to_terraform(env_name="dev")
     tstack.terraform.backend = (
         None  # TODO: Add credentials to git actions to use azure backend
     )
     tstack.init(flags=["-migrate-state", "-upgrade"])
     tstack.plan()
```

### Comparing `laktory-0.3.2/tests/test_table.py` & `laktory-0.3.3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.2/tests/test_workspacefile.py` & `laktory-0.3.3/tests/test_workspacefile.py`

 * *Files identical despite different names*

