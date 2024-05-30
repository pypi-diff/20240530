# Comparing `tmp/pyiron_workflow-0.7.1.tar.gz` & `tmp/pyiron_workflow-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_workflow-0.7.1.tar", last modified: Wed May  8 21:43:19 2024, max compression
+gzip compressed data, was "pyiron_workflow-0.8.0.tar", last modified: Thu May 30 02:04:14 2024, max compression
```

## Comparing `pyiron_workflow-0.7.1.tar` & `pyiron_workflow-0.8.0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.180070 pyiron_workflow-0.7.1/pyiron_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/pyiron_workflow/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/draw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/executors/cloudpickleprocesspool.py
--rw-r--r--   0 runner    (1001) docker     (127)    17951 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/has_interface_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/has_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/injection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/io_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)    39869 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/node_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/pyiron_atomistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/semantics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/single_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/has_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/type_hinting.py
--rw-r--r--   0 runner    (1001) docker     (127)    23787 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/working.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 21:43:18.000000 pyiron_workflow-0.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.784209 pyiron_workflow-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-05-30 02:04:14.784209 pyiron_workflow-0.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.772209 pyiron_workflow-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.780209 pyiron_workflow-0.8.0/pyiron_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 02:04:14.784209 pyiron_workflow-0.8.0/pyiron_workflow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/draw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.780209 pyiron_workflow-0.8.0/pyiron_workflow/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/executors/cloudpickleprocesspool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17951 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/has_interface_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/has_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/io_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39869 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.780209 pyiron_workflow-0.8.0/pyiron_workflow/node_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.780209 pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/pyiron_atomistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_library/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/node_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/single_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.784209 pyiron_workflow-0.8.0/pyiron_workflow/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/has_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/snippets/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/type_hinting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23787 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/pyiron_workflow/working.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:04:14.784209 pyiron_workflow-0.8.0/pyiron_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-05-30 02:04:14.000000 pyiron_workflow-0.8.0/pyiron_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-30 02:04:14.000000 pyiron_workflow-0.8.0/pyiron_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:04:14.000000 pyiron_workflow-0.8.0/pyiron_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-30 02:04:14.000000 pyiron_workflow-0.8.0/pyiron_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 02:04:14.000000 pyiron_workflow-0.8.0/pyiron_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-30 02:04:12.000000 pyiron_workflow-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 02:04:14.784209 pyiron_workflow-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-30 02:02:54.000000 pyiron_workflow-0.8.0/setup.py
```

### Comparing `pyiron_workflow-0.7.1/LICENSE` & `pyiron_workflow-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/__init__.py` & `pyiron_workflow-0.8.0/pyiron_workflow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,8 +25,12 @@
 - Support for more complex remote execution, especially leveraging :mod:`pympipool`
 - Infrastructure that supports and encourages of FAIR principles for node packages and
   finished workflows
 - Ontological hinting for data channels in order to provide guided workflow design
 - GUI on top for code-lite/code-free visual scripting
 """
 
+from ._version import get_versions
+
+__version__ = get_versions()["version"]
+
 from pyiron_workflow.workflow import Workflow
```

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/channels.py` & `pyiron_workflow-0.8.0/pyiron_workflow/channels.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/composite.py` & `pyiron_workflow-0.8.0/pyiron_workflow/composite.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/create.py` & `pyiron_workflow-0.8.0/pyiron_workflow/create.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/draw.py` & `pyiron_workflow-0.8.0/pyiron_workflow/draw.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/executors/cloudpickleprocesspool.py` & `pyiron_workflow-0.8.0/pyiron_workflow/executors/cloudpickleprocesspool.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/for_loop.py` & `pyiron_workflow-0.8.0/pyiron_workflow/for_loop.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/function.py` & `pyiron_workflow-0.8.0/pyiron_workflow/function.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/has_interface_mixins.py` & `pyiron_workflow-0.8.0/pyiron_workflow/has_interface_mixins.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/injection.py` & `pyiron_workflow-0.8.0/pyiron_workflow/injection.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/io.py` & `pyiron_workflow-0.8.0/pyiron_workflow/io.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/io_preview.py` & `pyiron_workflow-0.8.0/pyiron_workflow/io_preview.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from pyiron_workflow.injection import OutputDataWithInjection, OutputsWithInjection
 from pyiron_workflow.io import Inputs
 from pyiron_workflow.node import Node
 from pyiron_workflow.output_parser import ParseOutput
 from pyiron_workflow.snippets.dotdict import DotDict
 
 if TYPE_CHECKING:
+    from pandas import DataFrame
     from pyiron_workflow.composite import Composite
 
 
 class HasIOPreview(ABC):
     """
     An interface mixin guaranteeing the class-level availability of input and output
     previews.
@@ -360,7 +361,71 @@
     @property
     def inputs(self) -> Inputs:
         return self._inputs
 
     @property
     def outputs(self) -> OutputsWithInjection:
         return self._outputs
+
+    def iter(
+        self,
+        body_node_executor=None,
+        output_column_map: Optional[dict[str, str]] = None,
+        **iterating_inputs,
+    ) -> DataFrame:
+        return self._loop(
+            "iter_on",
+            body_node_executor=body_node_executor,
+            output_column_map=output_column_map,
+            **iterating_inputs,
+        )
+
+    def zip(
+        self,
+        body_node_executor=None,
+        output_column_map: Optional[dict[str, str]] = None,
+        **iterating_inputs,
+    ) -> DataFrame:
+        return self._loop(
+            "zip_on",
+            body_node_executor=body_node_executor,
+            output_column_map=output_column_map,
+            **iterating_inputs,
+        )
+
+    def _loop(
+        self,
+        loop_style_key,
+        body_node_executor=None,
+        output_column_map=None,
+        **looping_inputs,
+    ):
+        loop_on = tuple(looping_inputs.keys())
+        self._guarantee_names_are_input_channels(loop_on)
+
+        broadcast_inputs = {
+            label: self.inputs[label].value
+            for label in set(self.inputs.labels).difference(loop_on)
+        }
+
+        from pyiron_workflow.for_loop import for_node
+
+        for_instance = for_node(
+            self.__class__,
+            **{
+                loop_style_key: loop_on,
+                "output_column_map": output_column_map,
+                **looping_inputs,
+                **broadcast_inputs,
+            },
+        )
+        for_instance.body_node_executor = body_node_executor
+
+        return for_instance().df
+
+    def _guarantee_names_are_input_channels(self, presumed_input_keys: tuple[str]):
+        non_input_kwargs = set(presumed_input_keys).difference(self.inputs.labels)
+        if len(non_input_kwargs) > 0:
+            raise ValueError(
+                f"{self.label} cannot iterate on {non_input_kwargs} because they are "
+                f"not among input channels {self.inputs.labels}"
+            )
```

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/job.py` & `pyiron_workflow-0.8.0/pyiron_workflow/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/loops.py` & `pyiron_workflow-0.8.0/pyiron_workflow/loops.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/macro.py` & `pyiron_workflow-0.8.0/pyiron_workflow/macro.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/node.py` & `pyiron_workflow-0.8.0/pyiron_workflow/node.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/calculator.py` & `pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/calculator.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/macro.py` & `pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/macro.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/task.py` & `pyiron_workflow-0.8.0/pyiron_workflow/node_library/atomistics/task.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/node_library/pyiron_atomistics.py` & `pyiron_workflow-0.8.0/pyiron_workflow/node_library/pyiron_atomistics.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/node_library/standard.py` & `pyiron_workflow-0.8.0/pyiron_workflow/node_library/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,20 @@
     elif stop is None:
         raise ValueError("If start is provided, stop _must_ be provided")
     else:
         s = slice(start, stop, step)
     return s
 
 
+@as_function_node("object")
+def SetAttr(obj, key: str, val):
+    setattr(obj, key, val)
+    return obj
+
+
 # A bunch of (but not all) standard operators
 # Return values based on dunder methods, where available
 
 
 @as_function_node("str")
 def String(obj):
     return str(obj)
@@ -294,14 +300,15 @@
     NotEquals,
     Or,
     Positive,
     Power,
     RandomFloat,
     RightMultiply,
     Round,
+    SetAttr,
     Sleep,
     Slice,
     String,
     Subtract,
     UserInput,
     XOr,
 ]
```

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/node_package.py` & `pyiron_workflow-0.8.0/pyiron_workflow/node_package.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/output_parser.py` & `pyiron_workflow-0.8.0/pyiron_workflow/output_parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/run.py` & `pyiron_workflow-0.8.0/pyiron_workflow/run.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/semantics.py` & `pyiron_workflow-0.8.0/pyiron_workflow/semantics.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/single_output.py` & `pyiron_workflow-0.8.0/pyiron_workflow/single_output.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/colors.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/colors.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/dotdict.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/factory.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/files.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/files.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/has_post.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/has_post.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/logger.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/singleton.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/snippets/testcase.py` & `pyiron_workflow-0.8.0/pyiron_workflow/snippets/testcase.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/storage.py` & `pyiron_workflow-0.8.0/pyiron_workflow/storage.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/topology.py` & `pyiron_workflow-0.8.0/pyiron_workflow/topology.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/transform.py` & `pyiron_workflow-0.8.0/pyiron_workflow/transform.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/type_hinting.py` & `pyiron_workflow-0.8.0/pyiron_workflow/type_hinting.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/workflow.py` & `pyiron_workflow-0.8.0/pyiron_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow/working.py` & `pyiron_workflow-0.8.0/pyiron_workflow/working.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.1/pyiron_workflow.egg-info/SOURCES.txt` & `pyiron_workflow-0.8.0/pyiron_workflow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
-setup.cfg
+pyproject.toml
 setup.py
-versioneer.py
+docs/README.md
 pyiron_workflow/__init__.py
 pyiron_workflow/_tests.py
 pyiron_workflow/_version.py
 pyiron_workflow/channels.py
 pyiron_workflow/composite.py
 pyiron_workflow/create.py
 pyiron_workflow/draw.py
```

