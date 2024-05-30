# Comparing `tmp/lsst_pipe_base-27.2024.2100.tar.gz` & `tmp/lsst_pipe_base-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_pipe_base-27.2024.2100.tar", last modified: Thu May 23 10:09:14 2024, max compression
+gzip compressed data, was "lsst_pipe_base-27.2024.2200.tar", last modified: Thu May 30 09:56:48 2024, max compression
```

## Comparing `lsst_pipe_base-27.2024.2100.tar` & `lsst_pipe_base-27.2024.2200.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.106432 lsst_pipe_base-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 10:09:14.106432 lsst_pipe_base-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.082432 lsst_pipe_base-27.2024.2100/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.086432 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/creating-a-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/creating-a-pipelinetask.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/creating-a-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/task-framework-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/task-retargeting-howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/testing-a-pipeline-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.086432 lsst_pipe_base-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.086432 lsst_pipe_base-27.2024.2100/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.086432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.094432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_datasetQueryConstraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    30075 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_observation_dimension_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_quantumContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/automatic_connection_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/caching_limited_butler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.094432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.094432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.094432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/connectionTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    52230 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/executionButlerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/execution_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.094432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/formatters/pexConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.094432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/_implDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/_loadHelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27987 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/_versionDeserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    56203 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/graphSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/quantumNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    63434 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipelineTask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.098432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    32831 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    75567 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    39356 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.098432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
--rw-r--r--   0 runner    (1001) docker     (127)    28590 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/prerequisite_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54285 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/quantum_graph_skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.098432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/script/register_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/script/transfer_from_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/taskFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/testUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.098432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.102432 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/_data_id_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    27231 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    22758 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/no_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/pipelineStepTester.py
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/simpleQGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:09:13.000000 lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.106432 lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 10:09:14.000000 lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-23 10:09:14.000000 lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:09:14.000000 lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 10:09:14.000000 lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:09:14.000000 lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:09:13.000000 lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 10:09:14.106432 lsst_pipe_base-27.2024.2100/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:14.106432 lsst_pipe_base-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_caching_limited_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_cliCmdRegisterInstrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_config_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_dataid_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_dynamic_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_executionButler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_execution_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16055 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26529 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_pipelineLoadSubset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_pipelineTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    67752 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_quantumGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_taskmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_testUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-23 10:09:07.000000 lsst_pipe_base-27.2024.2100/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.085743 lsst_pipe_base-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-30 09:56:48.085743 lsst_pipe_base-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.057743 lsst_pipe_base-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.061743 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/creating-a-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/creating-a-pipelinetask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/creating-a-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/task-framework-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/task-retargeting-howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/testing-a-pipeline-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.057743 lsst_pipe_base-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.061743 lsst_pipe_base-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.061743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.069743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_datasetQueryConstraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30075 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_observation_dimension_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_quantumContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/automatic_connection_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/caching_limited_butler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.069743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.069743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.069743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/connectionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52230 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/executionButlerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/execution_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.073743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/formatters/pexConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.073743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/_implDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/_loadHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27987 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/_versionDeserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56203 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/graphSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/quantumNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63434 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipelineTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.077743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32831 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75567 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39356 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.077743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28590 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/prerequisite_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54285 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/quantum_graph_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.077743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/script/register_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/script/transfer_from_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/taskFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/testUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.077743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.077743 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/_data_id_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24352 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/no_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/pipelineStepTester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/simpleQGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:56:47.000000 lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.085743 lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-30 09:56:48.000000 lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-30 09:56:48.000000 lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:48.000000 lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 09:56:48.000000 lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:56:48.000000 lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:47.000000 lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 09:56:48.085743 lsst_pipe_base-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:48.085743 lsst_pipe_base-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_caching_limited_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_cliCmdRegisterInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_config_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_dataid_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_dynamic_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_executionButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_execution_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16055 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26529 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_pipelineLoadSubset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_pipelineTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67752 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_quantumGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_taskmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_testUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-30 09:56:41.000000 lsst_pipe_base-27.2024.2200/tests/test_utils.py
```

### Comparing `lsst_pipe_base-27.2024.2100/PKG-INFO` & `lsst_pipe_base-27.2024.2200/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_pipe_base-27.2024.2100/README.md` & `lsst_pipe_base-27.2024.2200/README.md`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/bsd_license.txt` & `lsst_pipe_base-27.2024.2200/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/CHANGES.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/creating-a-pipeline.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/creating-a-pipeline.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/creating-a-pipelinetask.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/creating-a-pipelinetask.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/creating-a-task.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/creating-a-task.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/index.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/task-framework-overview.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/task-framework-overview.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/task-retargeting-howto.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/task-retargeting-howto.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/testing-a-pipeline-task.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/testing-a-pipeline-task.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/doc/lsst.pipe.base/working-with-pipeline-graphs.rst` & `lsst_pipe_base-27.2024.2200/doc/lsst.pipe.base/working-with-pipeline-graphs.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/gpl-v3.0.txt` & `lsst_pipe_base-27.2024.2200/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/pyproject.toml` & `lsst_pipe_base-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/__init__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_datasetQueryConstraints.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_datasetQueryConstraints.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_dataset_handle.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_dataset_handle.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_instrument.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_observation_dimension_packer.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_observation_dimension_packer.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_quantumContext.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_quantumContext.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_status.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_status.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/_task_metadata.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/_task_metadata.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/automatic_connection_constants.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/automatic_connection_constants.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/caching_limited_butler.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/caching_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/cmd/__init__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/cmd/commands.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/opt/__init__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/opt/arguments.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/cli/opt/options.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/config.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/config.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/configOverrides.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/connectionTypes.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/connectionTypes.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/connections.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/connections.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/executionButlerBuilder.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/executionButlerBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/execution_reports.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/execution_reports.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/formatters/pexConfig.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/formatters/pexConfig.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/_implDetails.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/_implDetails.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/_loadHelpers.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/_loadHelpers.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/_versionDeserializers.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/_versionDeserializers.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/graph.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/graphSummary.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/graphSummary.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graph/quantumNode.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graph/quantumNode.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/graphBuilder.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/graphBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeTools.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeTools.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipelineIR.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipelineIR.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipelineTask.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipelineTask.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/__init__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/__main__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/__main__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_dataset_types.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_dataset_types.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_edges.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_edges.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_exceptions.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_mapping_views.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_mapping_views.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_nodes.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_nodes.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_task_subsets.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_task_subsets.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/_tasks.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/_tasks.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/io.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/io.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_options.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_options.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/pipeline_graph/visualization/_show.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/pipeline_graph/visualization/_show.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/prerequisite_helpers.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/prerequisite_helpers.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/quantum_graph_builder.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/quantum_graph_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/quantum_graph_skeleton.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/quantum_graph_skeleton.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/script/__init__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/script/register_instrument.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/script/register_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/script/transfer_from_graph.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/script/transfer_from_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/struct.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/struct.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/task.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/task.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/taskFactory.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/taskFactory.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/testUtils.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/testUtils.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/__init__.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/_data_id_match.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/_data_id_match.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/_pipeline_task.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/_pipeline_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,22 +46,27 @@
 from astropy.units import Quantity
 from lsst.daf.butler import DataCoordinate, DatasetRef, DeferredDatasetHandle, SerializedDatasetType
 from lsst.pex.config import Config, ConfigDictField, ConfigurableField, Field, ListField
 from lsst.utils.doImport import doImportType
 from lsst.utils.introspection import get_full_type_name
 from lsst.utils.iteration import ensure_iterable
 
-from ... import automatic_connection_constants as acc
 from ... import connectionTypes as cT
 from ...config import PipelineTaskConfig
 from ...connections import InputQuantizedConnection, OutputQuantizedConnection, PipelineTaskConnections
 from ...pipeline_graph import PipelineGraph
 from ...pipelineTask import PipelineTask
 from ._data_id_match import DataIdMatch
-from ._storage_class import MockDataset, MockDatasetQuantum, MockStorageClass, get_mock_name
+from ._storage_class import (
+    ConvertedUnmockedDataset,
+    MockDataset,
+    MockDatasetQuantum,
+    MockStorageClass,
+    get_mock_name,
+)
 
 _LOG = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from ..._quantumContext import QuantumContext
 
 
@@ -103,29 +108,35 @@
 
     Parameters
     ----------
     original_graph : `~..pipeline_graph.PipelineGraph`
         Original tasks and configuration to mock.
     unmocked_dataset_types : `~collections.abc.Iterable` [ `str` ], optional
         Names of overall-input dataset types that should not be replaced with
-        mocks.
+        mocks.  "Automatic" datasets written by the execution framework such
+        as configs, logs, and metadata are implicitly included.
     force_failures : `~collections.abc.Mapping` [ `str`, `ForcedFailure` ]
         Mapping from original task label to information about an exception one
         or more quanta for this task should raise.
 
     Returns
     -------
     mocked : `~..pipeline_graph.PipelineGraph`
         Pipeline graph using `MockPipelineTask` configurations that target the
         original tasks.  Never resolved.
     """
-    unmocked_dataset_types = tuple(unmocked_dataset_types)
+    unmocked_dataset_types = list(unmocked_dataset_types)
     if force_failures is None:
         force_failures = {}
     result = PipelineGraph(description=original_graph.description)
+    for task_node in original_graph.tasks.values():
+        unmocked_dataset_types.append(task_node.init.config_output.dataset_type_name)
+        if task_node.log_output is not None:
+            unmocked_dataset_types.append(task_node.log_output.dataset_type_name)
+        unmocked_dataset_types.append(task_node.metadata_output.dataset_type_name)
     for original_task_node in original_graph.tasks.values():
         config = MockPipelineTaskConfig()
         config.original.retarget(original_task_node.task_class)
         config.original = original_task_node.config
         config.unmocked_dataset_types.extend(unmocked_dataset_types)
         if original_task_node.label in force_failures:
             force_failures[original_task_node.label].set_config(config)
@@ -302,22 +313,23 @@
             inputs_list = []
             ref: DatasetRef
             for ref in ensure_iterable(refs):
                 if isinstance(ref.datasetType.storageClass, MockStorageClass):
                     input_dataset = butlerQC.get(ref)
                     if isinstance(input_dataset, DeferredDatasetHandle):
                         input_dataset = input_dataset.get()
-                    if not isinstance(input_dataset, MockDataset):
+                    if isinstance(input_dataset, MockDataset):
+                        # To avoid very deep provenance we trim inputs to a
+                        # single level.
+                        input_dataset.quantum = None
+                    elif not isinstance(input_dataset, ConvertedUnmockedDataset):
                         raise TypeError(
-                            f"Expected MockDataset instance for {ref}; "
+                            f"Expected MockDataset or ConvertedUnmockedDataset instance for {ref}; "
                             f"got {input_dataset!r} of type {type(input_dataset)!r}."
                         )
-                    # To avoid very deep provenance we trim inputs to a single
-                    # level.
-                    input_dataset.quantum = None
                 else:
                     input_dataset = MockDataset(
                         dataset_id=ref.id,
                         dataset_type=ref.datasetType.to_simple(),
                         data_id=dict(ref.dataId.mapping),
                         run=ref.run,
                     )
@@ -377,30 +389,20 @@
         self.original: PipelineTaskConnections = config.original.connections.ConnectionsClass(
             config=config.original.value
         )
         self.dimensions.update(self.original.dimensions)
         self.unmocked_dataset_types = frozenset(config.unmocked_dataset_types)
         for name, connection in self.original.allConnections.items():
             if connection.name not in self.unmocked_dataset_types:
-                if connection.storageClass in (
-                    acc.CONFIG_INIT_OUTPUT_STORAGE_CLASS,
-                    acc.METADATA_OUTPUT_STORAGE_CLASS,
-                    acc.LOG_OUTPUT_STORAGE_CLASS,
-                ):
-                    # We don't mock the automatic output connections, so if
-                    # they're used as an input in any other connection, we
-                    # can't mock them there either.
-                    storage_class_name = connection.storageClass
-                else:
-                    # We register the mock storage class with the global
-                    # singleton here, but can only put its name in the
-                    # connection. That means the same global singleton (or one
-                    # that also has these registrations) has to be available
-                    # whenever this dataset type is used.
-                    storage_class_name = MockStorageClass.get_or_register_mock(connection.storageClass).name
+                # We register the mock storage class with the global
+                # singleton here, but can only put its name in the
+                # connection. That means the same global singleton (or one
+                # that also has these registrations) has to be available
+                # whenever this dataset type is used.
+                storage_class_name = MockStorageClass.get_or_register_mock(connection.storageClass).name
                 kwargs: dict[str, Any] = {}
                 if hasattr(connection, "dimensions"):
                     connection_dimensions = set(connection.dimensions)
                     # Replace the generic "skypix" placeholder with htm7, since
                     # that requires the dataset type to have already been
                     # registered.
                     if "skypix" in connection_dimensions:
```

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/mocks/_storage_class.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/mocks/_storage_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 __all__ = (
+    "ConvertedUnmockedDataset",
     "MockDataset",
     "MockStorageClass",
     "MockDatasetQuantum",
     "MockStorageClassDelegate",
     "get_mock_name",
     "get_original_name",
     "is_mock_name",
@@ -225,28 +226,62 @@
 
         @classmethod
         def model_json_schema(cls, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_json_schema`."""
             return super().model_json_schema(*args, **kwargs)
 
 
+class ConvertedUnmockedDataset(pydantic.BaseModel):
+    """A marker class that represents a conversion from a regular in-memory
+    dataset to a mock storage class.
+    """
+
+    original_type: str
+    """The full Python type of the original unmocked in-memory dataset."""
+
+    # Work around the fact that Sphinx chokes on Pydantic docstring formatting,
+    # when we inherit those docstrings in our public classes.
+    if "sphinx" in sys.modules:
+
+        def copy(self, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.copy`."""
+            return super().copy(*args, **kwargs)
+
+        def model_dump(self, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.model_dump`."""
+            return super().model_dump(*args, **kwargs)
+
+        def model_dump_json(self, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.model_dump_json`."""
+            return super().model_dump(*args, **kwargs)
+
+        def model_copy(self, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.model_copy`."""
+            return super().model_copy(*args, **kwargs)
+
+        @classmethod
+        def model_json_schema(cls, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.model_json_schema`."""
+            return super().model_json_schema(*args, **kwargs)
+
+
 class MockDatasetQuantum(pydantic.BaseModel):
     """Description of the quantum that produced a mock dataset.
 
     This is also used to represent task-init operations for init-output mock
     datasets.
     """
 
     task_label: str
     """Label of the producing PipelineTask in its pipeline."""
 
     data_id: dict[str, DataIdValue]
     """Data ID for the quantum."""
 
-    inputs: dict[str, list[MockDataset]]
+    inputs: dict[str, list[MockDataset | ConvertedUnmockedDataset]]
     """Mock datasets provided as input to the quantum.
 
     Keys are task-internal connection names, not dataset type names.
     """
 
     # Work around the fact that Sphinx chokes on Pydantic docstring formatting,
     # when we inherit those docstrings in our public classes.
@@ -406,24 +441,25 @@
     def derivedComponents(self) -> Mapping[str, MockStorageClass]:
         # Docstring inherited.
         return cast(Mapping[str, MockStorageClass], super().derivedComponents)
 
     def can_convert(self, other: StorageClass) -> bool:
         # Docstring inherited.
         if not isinstance(other, MockStorageClass):
-            return False
+            # Allow conversions from an original type (and others compatible
+            # with it) to a mock, to allow for cases where an upstream task
+            # did not use a mock to write something but the downstream one is
+            # trying to us a mock to read it.
+            return self.original.can_convert(other)
         return self.original.can_convert(other.original)
 
     def coerce_type(self, incorrect: Any) -> Any:
         # Docstring inherited.
         if not isinstance(incorrect, MockDataset):
-            raise TypeError(
-                f"Mock storage class {self.name!r} can only convert in-memory datasets "
-                f"corresponding to other mock storage classes, not {incorrect!r}."
-            )
+            return ConvertedUnmockedDataset(original_type=get_full_type_name(incorrect))
         factory = StorageClassFactory()
         other_storage_class = factory.getStorageClass(incorrect.storage_class)
         assert isinstance(other_storage_class, MockStorageClass), "Should not get a MockDataset otherwise."
         if other_storage_class.name == self.name:
             return incorrect
         if not self.can_convert(other_storage_class):
             raise TypeError(
```

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/no_dimensions.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/no_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/pipelineStepTester.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/pipelineStepTester.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/simpleQGraph.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/simpleQGraph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/tests/util.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/tests/util.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst/pipe/base/utils.py` & `lsst_pipe_base-27.2024.2200/python/lsst/pipe/base/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/PKG-INFO` & `lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_pipe_base-27.2024.2100/python/lsst_pipe_base.egg-info/SOURCES.txt` & `lsst_pipe_base-27.2024.2200/python/lsst_pipe_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_caching_limited_butler.py` & `lsst_pipe_base-27.2024.2200/tests/test_caching_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_cliCmdRegisterInstrument.py` & `lsst_pipe_base-27.2024.2200/tests/test_cliCmdRegisterInstrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_configOverrides.py` & `lsst_pipe_base-27.2024.2200/tests/test_configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_config_formatter.py` & `lsst_pipe_base-27.2024.2200/tests/test_config_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_connections.py` & `lsst_pipe_base-27.2024.2200/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_dataid_match.py` & `lsst_pipe_base-27.2024.2200/tests/test_dataid_match.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_dataset_handle.py` & `lsst_pipe_base-27.2024.2200/tests/test_dataset_handle.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_dynamic_connections.py` & `lsst_pipe_base-27.2024.2200/tests/test_dynamic_connections.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_executionButler.py` & `lsst_pipe_base-27.2024.2200/tests/test_executionButler.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_execution_reports.py` & `lsst_pipe_base-27.2024.2200/tests/test_execution_reports.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_graphBuilder.py` & `lsst_pipe_base-27.2024.2200/tests/test_graphBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_instrument.py` & `lsst_pipe_base-27.2024.2200/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_pipeline.py` & `lsst_pipe_base-27.2024.2200/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_pipelineIR.py` & `lsst_pipe_base-27.2024.2200/tests/test_pipelineIR.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_pipelineLoadSubset.py` & `lsst_pipe_base-27.2024.2200/tests/test_pipelineLoadSubset.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_pipelineTask.py` & `lsst_pipe_base-27.2024.2200/tests/test_pipelineTask.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_pipeline_graph.py` & `lsst_pipe_base-27.2024.2200/tests/test_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_quantumGraph.py` & `lsst_pipe_base-27.2024.2200/tests/test_quantumGraph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_struct.py` & `lsst_pipe_base-27.2024.2200/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_task.py` & `lsst_pipe_base-27.2024.2200/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_taskmetadata.py` & `lsst_pipe_base-27.2024.2200/tests/test_taskmetadata.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_testUtils.py` & `lsst_pipe_base-27.2024.2200/tests/test_testUtils.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.2100/tests/test_utils.py` & `lsst_pipe_base-27.2024.2200/tests/test_utils.py`

 * *Files identical despite different names*

