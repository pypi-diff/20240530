# Comparing `tmp/gempyp-1.0.90b3.tar.gz` & `tmp/gempyp-1.0.90b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempyp-1.0.90b3.tar", max compression
+gzip compressed data, was "gempyp-1.0.90b4.tar", max compression
```

## Comparing `gempyp-1.0.90b3.tar` & `gempyp-1.0.90b4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0       25 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/__init__.py
--rw-r--r--   0        0        0      108 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/cli.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/config/__init__.py
--rw-r--r--   0        0        0     7753 2024-04-23 05:32:45.965360 gempyp-1.0.90b3/gempyp/config/baseConfig.py
--rw-r--r--   0        0        0      198 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/config/customParser.py
--rw-r--r--   0        0        0     2226 2024-05-20 07:24:06.014963 gempyp-1.0.90b3/gempyp/config/DefaultSettings.py
--rw-r--r--   0        0        0       62 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/config/gempyp.conf
--rw-r--r--   0        0        0     2145 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/config/GitLinkXML.py
--rw-r--r--   0        0        0    21143 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/config/Result.html
--rw-r--r--   0        0        0       26 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/config/suite_conf.json
--rw-r--r--   0        0        0       28 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/config/testcase_conf.json
--rw-r--r--   0        0        0     8234 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/config/xmlConfig.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/data_compare/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/data_compare/common/__init__.py
--rw-r--r--   0        0        0     3627 2024-04-23 05:31:05.678699 gempyp-1.0.90b3/gempyp/data_compare/common/common_functions.py
--rw-r--r--   0        0        0      956 2024-04-23 05:31:05.693479 gempyp-1.0.90b3/gempyp/data_compare/compare.py
--rw-r--r--   0        0        0      149 2024-04-23 05:31:05.694480 gempyp-1.0.90b3/gempyp/data_compare/config/dvm.json
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/configurator/__init__.py
--rw-r--r--   0        0        0     4635 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/configurator/configurator.py
--rw-r--r--   0        0        0      320 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/configurator/validator.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/core/__init__.py
--rw-r--r--   0        0        0      589 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/core/comparator.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/core/Compare.py
--rw-r--r--   0        0        0    10157 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/core/python_obj_comparator.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/__init__.py
--rw-r--r--   0        0        0     5498 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/data.py
--rw-r--r--   0        0        0      869 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/database.py
--rw-r--r--   0        0        0     1903 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/db_mysql.py
--rw-r--r--   0        0        0     2646 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/db_oracle.py
--rw-r--r--   0        0        0     2436 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/db_postgre.py
--rw-r--r--   0        0        0     1999 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/db_sqlite.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data/file_processor.py
--rw-r--r--   0        0        0    11161 2024-04-23 05:31:05.695706 gempyp-1.0.90b3/gempyp/data_compare/data_comp.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711228 gempyp-1.0.90b3/gempyp/data_compare/report/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/data_compare/tools/__init__.py
--rw-r--r--   0        0        0     6758 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/data_uploader.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/dv/__init__.py
--rw-r--r--   0        0        0     2286 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/dv/dfOperations.py
--rw-r--r--   0        0        0    10231 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/dv/dvCompare.py
--rw-r--r--   0        0        0      682 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/dv/dvDatabases.py
--rw-r--r--   0        0        0    10760 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/dv/dvDataframe.py
--rw-r--r--   0        0        0     1441 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/dv/dvObj.py
--rw-r--r--   0        0        0     3789 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/dv/dvReporting.py
--rw-r--r--   0        0        0    23225 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/dv/dvRunner.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/engine/__init__.py
--rw-r--r--   0        0        0     5092 2024-04-23 05:31:05.711975 gempyp-1.0.90b3/gempyp/engine/baseTemplate.py
--rw-r--r--   0        0        0     8515 2024-05-20 07:22:40.024225 gempyp-1.0.90b3/gempyp/engine/dataUpload.py
--rw-r--r--   0        0        0    51385 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/engine/engine.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.728857 gempyp-1.0.90b3/gempyp/engine/executors/__init__.py
--rw-r--r--   0        0        0      443 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/engine/executors/baseExecutor.py
--rw-r--r--   0        0        0      656 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/engine/gempypHelper.py
--rw-r--r--   0        0        0     5483 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/engine/runner.py
--rw-r--r--   0        0        0     5533 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/engine/simpleTestcase.py
--rw-r--r--   0        0        0    12428 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/engine/testData.py
--rw-r--r--   0        0        0    64741 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/final_report.html
--rw-r--r--   0        0        0     5666 2024-04-23 05:32:45.980999 gempyp-1.0.90b3/gempyp/gemPyp.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/jira/__init__.py
--rw-r--r--   0        0        0     2312 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/jira/jiraIntegration.py
--rw-r--r--   0        0        0     4474 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/jira/jiraIntegrationCopy.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.729072 gempyp-1.0.90b3/gempyp/libs/__init__.py
--rw-r--r--   0        0        0     9328 2024-04-23 05:37:15.962177 gempyp-1.0.90b3/gempyp/libs/common.py
--rw-r--r--   0        0        0      131 2024-04-23 05:31:05.743503 gempyp-1.0.90b3/gempyp/libs/enums/run_types.py
--rw-r--r--   0        0        0      318 2024-04-23 05:31:05.744504 gempyp-1.0.90b3/gempyp/libs/enums/status.py
--rw-r--r--   0        0        0       47 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/libs/exceptions/__init__.py
--rw-r--r--   0        0        0     4352 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/libs/gem_s3_common.py
--rw-r--r--   0        0        0     2642 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/libs/logConfig.py
--rw-r--r--   0        0        0     1465 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/libs/parsers.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/pyprest/__init__.py
--rw-r--r--   0        0        0     7073 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/pyprest/apiCommon.py
--rw-r--r--   0        0        0      491 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/pyprest/beforeAfterSample.py
--rw-r--r--   0        0        0    14091 2024-04-23 06:32:44.195355 gempyp-1.0.90b3/gempyp/pyprest/compareFunctions.py
--rw-r--r--   0        0        0    13569 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/pyprest/keyCheck.py
--rw-r--r--   0        0        0    15661 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/pyprest/legacyComparison.py
--rw-r--r--   0        0        0     1933 2024-04-23 05:31:05.745590 gempyp-1.0.90b3/gempyp/pyprest/miscVariables.py
--rw-r--r--   0        0        0    10827 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/pyprest/postAssertion.py
--rw-r--r--   0        0        0     5987 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/pyprest/postVariables.py
--rw-r--r--   0        0        0     8271 2024-04-23 05:31:05.762677 gempyp-1.0.90b3/gempyp/pyprest/predefinedFunctions.py
--rw-r--r--   0        0        0     4388 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/pyprest/preVariables.py
--rw-r--r--   0        0        0    38424 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/pyprest/pypRest.py
--rw-r--r--   0        0        0     4432 2024-04-23 05:32:45.996783 gempyp-1.0.90b3/gempyp/pyprest/reporting.py
--rw-r--r--   0        0        0     2725 2024-04-23 05:31:05.762677 gempyp-1.0.90b3/gempyp/pyprest/restEngine.py
--rw-r--r--   0        0        0     1031 2024-04-23 05:31:05.762677 gempyp-1.0.90b3/gempyp/pyprest/restObj.py
--rw-r--r--   0        0        0     6308 2024-04-23 05:31:05.762677 gempyp-1.0.90b3/gempyp/pyprest/utils.py
--rw-r--r--   0        0        0     6157 2024-04-23 05:32:46.012474 gempyp-1.0.90b3/gempyp/pyprest/variableReplacement.py
--rw-r--r--   0        0        0        0 2024-04-23 05:31:05.762677 gempyp-1.0.90b3/gempyp/reporter/__init__.py
--rw-r--r--   0        0        0     8517 2024-04-23 05:32:46.012474 gempyp-1.0.90b3/gempyp/reporter/reportGenerator.py
--rw-r--r--   0        0        0    13032 2024-04-23 05:32:46.012474 gempyp-1.0.90b3/gempyp/sdk/executor.py
--rw-r--r--   0        0        0     2490 2024-04-23 05:31:05.762677 gempyp-1.0.90b3/gempyp/sdk/worker.py
--rw-r--r--   0        0        0    11547 2024-04-23 05:31:05.762677 gempyp-1.0.90b3/gempyp/testcase.html
--rw-r--r--   0        0        0        2 2024-04-23 05:31:05.660636 gempyp-1.0.90b3/LICENSE
--rw-r--r--   0        0        0     1431 2024-05-20 07:24:30.607221 gempyp-1.0.90b3/pyproject.toml
--rw-r--r--   0        0        0     3161 2024-04-23 05:31:05.660636 gempyp-1.0.90b3/README.md
--rw-r--r--   0        0        0     4992 1970-01-01 00:00:00.000000 gempyp-1.0.90b3/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/cli.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/config/__init__.py
+-rw-r--r--   0        0        0     7753 2024-04-23 05:32:45.965360 gempyp-1.0.90b4/gempyp/config/baseConfig.py
+-rw-r--r--   0        0        0      198 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/config/customParser.py
+-rw-r--r--   0        0        0     2226 2024-05-20 07:24:06.014963 gempyp-1.0.90b4/gempyp/config/DefaultSettings.py
+-rw-r--r--   0        0        0       62 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/config/gempyp.conf
+-rw-r--r--   0        0        0     2145 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/config/GitLinkXML.py
+-rw-r--r--   0        0        0    21143 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/config/Result.html
+-rw-r--r--   0        0        0       26 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/config/suite_conf.json
+-rw-r--r--   0        0        0       28 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/config/testcase_conf.json
+-rw-r--r--   0        0        0     8234 2024-04-23 05:32:45.980999 gempyp-1.0.90b4/gempyp/config/xmlConfig.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/data_compare/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/data_compare/common/__init__.py
+-rw-r--r--   0        0        0     3627 2024-04-23 05:31:05.678699 gempyp-1.0.90b4/gempyp/data_compare/common/common_functions.py
+-rw-r--r--   0        0        0      956 2024-04-23 05:31:05.693479 gempyp-1.0.90b4/gempyp/data_compare/compare.py
+-rw-r--r--   0        0        0      149 2024-04-23 05:31:05.694480 gempyp-1.0.90b4/gempyp/data_compare/config/dvm.json
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/configurator/__init__.py
+-rw-r--r--   0        0        0     4635 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/configurator/configurator.py
+-rw-r--r--   0        0        0      320 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/configurator/validator.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/core/__init__.py
+-rw-r--r--   0        0        0      589 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/core/comparator.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/core/Compare.py
+-rw-r--r--   0        0        0    10157 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/core/python_obj_comparator.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/__init__.py
+-rw-r--r--   0        0        0     5498 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/data.py
+-rw-r--r--   0        0        0      869 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/database.py
+-rw-r--r--   0        0        0     1903 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/db_mysql.py
+-rw-r--r--   0        0        0     2646 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/db_oracle.py
+-rw-r--r--   0        0        0     2436 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/db_postgre.py
+-rw-r--r--   0        0        0     1999 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/db_sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data/file_processor.py
+-rw-r--r--   0        0        0    11161 2024-04-23 05:31:05.695706 gempyp-1.0.90b4/gempyp/data_compare/data_comp.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711228 gempyp-1.0.90b4/gempyp/data_compare/report/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/data_compare/tools/__init__.py
+-rw-r--r--   0        0        0     6758 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/data_uploader.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/dv/__init__.py
+-rw-r--r--   0        0        0     2286 2024-04-23 05:32:45.980999 gempyp-1.0.90b4/gempyp/dv/dfOperations.py
+-rw-r--r--   0        0        0    10231 2024-04-23 05:32:45.980999 gempyp-1.0.90b4/gempyp/dv/dvCompare.py
+-rw-r--r--   0        0        0      682 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/dv/dvDatabases.py
+-rw-r--r--   0        0        0    10786 2024-05-30 08:57:11.883075 gempyp-1.0.90b4/gempyp/dv/dvDataframe.py
+-rw-r--r--   0        0        0     1441 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/dv/dvObj.py
+-rw-r--r--   0        0        0     3789 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/dv/dvReporting.py
+-rw-r--r--   0        0        0    23225 2024-04-23 05:32:45.980999 gempyp-1.0.90b4/gempyp/dv/dvRunner.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/engine/__init__.py
+-rw-r--r--   0        0        0     5092 2024-04-23 05:31:05.711975 gempyp-1.0.90b4/gempyp/engine/baseTemplate.py
+-rw-r--r--   0        0        0     8515 2024-05-20 07:22:40.024225 gempyp-1.0.90b4/gempyp/engine/dataUpload.py
+-rw-r--r--   0        0        0    51524 2024-05-30 09:13:53.648688 gempyp-1.0.90b4/gempyp/engine/engine.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.728857 gempyp-1.0.90b4/gempyp/engine/executors/__init__.py
+-rw-r--r--   0        0        0      443 2024-04-23 05:31:05.729072 gempyp-1.0.90b4/gempyp/engine/executors/baseExecutor.py
+-rw-r--r--   0        0        0      656 2024-04-23 05:31:05.729072 gempyp-1.0.90b4/gempyp/engine/gempypHelper.py
+-rw-r--r--   0        0        0     5486 2024-05-30 08:57:46.850262 gempyp-1.0.90b4/gempyp/engine/runner.py
+-rw-r--r--   0        0        0     5533 2024-04-23 05:32:45.980999 gempyp-1.0.90b4/gempyp/engine/simpleTestcase.py
+-rw-r--r--   0        0        0    12428 2024-04-23 05:31:05.729072 gempyp-1.0.90b4/gempyp/engine/testData.py
+-rw-r--r--   0        0        0    64741 2024-04-23 05:31:05.729072 gempyp-1.0.90b4/gempyp/final_report.html
+-rw-r--r--   0        0        0     5666 2024-04-23 05:32:45.980999 gempyp-1.0.90b4/gempyp/gemPyp.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.729072 gempyp-1.0.90b4/gempyp/jira/__init__.py
+-rw-r--r--   0        0        0     2312 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/jira/jiraIntegration.py
+-rw-r--r--   0        0        0     4474 2024-04-23 05:31:05.729072 gempyp-1.0.90b4/gempyp/jira/jiraIntegrationCopy.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.729072 gempyp-1.0.90b4/gempyp/libs/__init__.py
+-rw-r--r--   0        0        0     9354 2024-05-30 08:58:24.582803 gempyp-1.0.90b4/gempyp/libs/common.py
+-rw-r--r--   0        0        0      131 2024-04-23 05:31:05.743503 gempyp-1.0.90b4/gempyp/libs/enums/run_types.py
+-rw-r--r--   0        0        0      318 2024-04-23 05:31:05.744504 gempyp-1.0.90b4/gempyp/libs/enums/status.py
+-rw-r--r--   0        0        0       47 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/libs/exceptions/__init__.py
+-rw-r--r--   0        0        0     4352 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/libs/gem_s3_common.py
+-rw-r--r--   0        0        0     2642 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/libs/logConfig.py
+-rw-r--r--   0        0        0     1465 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/libs/parsers.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/pyprest/__init__.py
+-rw-r--r--   0        0        0     7073 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/pyprest/apiCommon.py
+-rw-r--r--   0        0        0      491 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/pyprest/beforeAfterSample.py
+-rw-r--r--   0        0        0    14091 2024-04-23 06:32:44.195355 gempyp-1.0.90b4/gempyp/pyprest/compareFunctions.py
+-rw-r--r--   0        0        0    13569 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/pyprest/keyCheck.py
+-rw-r--r--   0        0        0    15661 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/pyprest/legacyComparison.py
+-rw-r--r--   0        0        0     1933 2024-04-23 05:31:05.745590 gempyp-1.0.90b4/gempyp/pyprest/miscVariables.py
+-rw-r--r--   0        0        0    10827 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/pyprest/postAssertion.py
+-rw-r--r--   0        0        0     5987 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/pyprest/postVariables.py
+-rw-r--r--   0        0        0     8271 2024-04-23 05:31:05.762677 gempyp-1.0.90b4/gempyp/pyprest/predefinedFunctions.py
+-rw-r--r--   0        0        0     4388 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/pyprest/preVariables.py
+-rw-r--r--   0        0        0    38424 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/pyprest/pypRest.py
+-rw-r--r--   0        0        0     4432 2024-04-23 05:32:45.996783 gempyp-1.0.90b4/gempyp/pyprest/reporting.py
+-rw-r--r--   0        0        0     2725 2024-04-23 05:31:05.762677 gempyp-1.0.90b4/gempyp/pyprest/restEngine.py
+-rw-r--r--   0        0        0     1031 2024-04-23 05:31:05.762677 gempyp-1.0.90b4/gempyp/pyprest/restObj.py
+-rw-r--r--   0        0        0     6308 2024-04-23 05:31:05.762677 gempyp-1.0.90b4/gempyp/pyprest/utils.py
+-rw-r--r--   0        0        0     6157 2024-04-23 05:32:46.012474 gempyp-1.0.90b4/gempyp/pyprest/variableReplacement.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.762677 gempyp-1.0.90b4/gempyp/reporter/__init__.py
+-rw-r--r--   0        0        0     8517 2024-04-23 05:32:46.012474 gempyp-1.0.90b4/gempyp/reporter/reportGenerator.py
+-rw-r--r--   0        0        0    13032 2024-04-23 05:32:46.012474 gempyp-1.0.90b4/gempyp/sdk/executor.py
+-rw-r--r--   0        0        0     2490 2024-04-23 05:31:05.762677 gempyp-1.0.90b4/gempyp/sdk/worker.py
+-rw-r--r--   0        0        0    11547 2024-04-23 05:31:05.762677 gempyp-1.0.90b4/gempyp/testcase.html
+-rw-r--r--   0        0        0        2 2024-04-23 05:31:05.660636 gempyp-1.0.90b4/LICENSE
+-rw-r--r--   0        0        0     1431 2024-05-30 09:14:55.942563 gempyp-1.0.90b4/pyproject.toml
+-rw-r--r--   0        0        0     3161 2024-04-23 05:31:05.660636 gempyp-1.0.90b4/README.md
+-rw-r--r--   0        0        0     4992 1970-01-01 00:00:00.000000 gempyp-1.0.90b4/PKG-INFO
```

### Comparing `gempyp-1.0.90b3/gempyp/config/baseConfig.py` & `gempyp-1.0.90b4/gempyp/config/baseConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/config/DefaultSettings.py` & `gempyp-1.0.90b4/gempyp/config/DefaultSettings.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/config/GitLinkXML.py` & `gempyp-1.0.90b4/gempyp/config/GitLinkXML.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/config/Result.html` & `gempyp-1.0.90b4/gempyp/config/Result.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/config/xmlConfig.py` & `gempyp-1.0.90b4/gempyp/config/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/common/common_functions.py` & `gempyp-1.0.90b4/gempyp/data_compare/common/common_functions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/compare.py` & `gempyp-1.0.90b4/gempyp/data_compare/compare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/configurator/configurator.py` & `gempyp-1.0.90b4/gempyp/data_compare/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/core/comparator.py` & `gempyp-1.0.90b4/gempyp/data_compare/core/comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/core/python_obj_comparator.py` & `gempyp-1.0.90b4/gempyp/data_compare/core/python_obj_comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/data/data.py` & `gempyp-1.0.90b4/gempyp/data_compare/data/data.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/data/database.py` & `gempyp-1.0.90b4/gempyp/data_compare/data/database.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/data/db_mysql.py` & `gempyp-1.0.90b4/gempyp/data_compare/data/db_mysql.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/data/db_oracle.py` & `gempyp-1.0.90b4/gempyp/data_compare/data/db_oracle.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/data/db_postgre.py` & `gempyp-1.0.90b4/gempyp/data_compare/data/db_postgre.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/data/db_sqlite.py` & `gempyp-1.0.90b4/gempyp/data_compare/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_compare/data_comp.py` & `gempyp-1.0.90b4/gempyp/data_compare/data_comp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/data_uploader.py` & `gempyp-1.0.90b4/gempyp/data_uploader.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/dv/dfOperations.py` & `gempyp-1.0.90b4/gempyp/dv/dfOperations.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/dv/dvCompare.py` & `gempyp-1.0.90b4/gempyp/dv/dvCompare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/dv/dvDatabases.py` & `gempyp-1.0.90b4/gempyp/dv/dvDatabases.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/dv/dvDataframe.py` & `gempyp-1.0.90b4/gempyp/dv/dvDataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
     def setConnection(self, lib, conn):
         lib = importlib.import_module(lib)
         conn = getattr(lib, conn)
 
     def csvFileReader(self, path, delimiter, db):
         try:
+            path=path[0]
             self.logger.info(f"Reading data from {db} CSV File")
             df = pd.read_csv(path, delimiter)
             df = df.loc[:, ~df.columns.str.contains('^Unnamed')]
             columns = df.columns.values.tolist()
             self.reporter.addRow(
                 f"Parsing {db} file", "Parsing file is successful", status.PASS)
             return df, columns
```

### Comparing `gempyp-1.0.90b3/gempyp/dv/dvObj.py` & `gempyp-1.0.90b4/gempyp/dv/dvObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/dv/dvReporting.py` & `gempyp-1.0.90b4/gempyp/dv/dvReporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/dv/dvRunner.py` & `gempyp-1.0.90b4/gempyp/dv/dvRunner.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/engine/baseTemplate.py` & `gempyp-1.0.90b4/gempyp/engine/baseTemplate.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/engine/dataUpload.py` & `gempyp-1.0.90b4/gempyp/engine/dataUpload.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/engine/engine.py` & `gempyp-1.0.90b4/gempyp/engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,27 +361,31 @@
             version1 = version(package_name)
         except Exception:
             version1=None
 
         # If package is not installed, try to get version from setup.py
         if version1 is None:
             version1 = self.get_version_from_setup()
+        if(platform.system().upper()=="WINDOWS"):
+            osName=platform.system().upper()+" "+platform.version().split(".")[0]
+        else:
+            osName=platform.system().upper()
         suite_details = {
             "s_run_id": self.s_run_id,
             "s_start_time": self.start_time,
             "s_end_time": None,
             "s_id": self.PARAMS.get("S_ID", "test_id"),
             "status": status.EXE.name,
             "project_name": self.project_name,
             "report_name": self.report_name,  # earlier it was report info
             "user": self.user,
             "env": self.project_env,
             "machine": self.machine,
             "framework_version":version1,
-            "os": platform.system().upper()+" "+platform.version().split(".")[0],
+            "os": osName,
             "meta_data": [],
             "expected_testcases": self.total_runable_testcase,
             "testcase_info": None,
             "framework_name": "GEMPYP",
         }
         self.DATA.suite_detail = self.DATA.suite_detail.append(
             suite_details, ignore_index=True
```

### Comparing `gempyp-1.0.90b3/gempyp/engine/gempypHelper.py` & `gempyp-1.0.90b4/gempyp/engine/gempypHelper.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/engine/runner.py` & `gempyp-1.0.90b4/gempyp/engine/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     if testcase_meta.get("default_urls", None):
         DefaultSettings.urls.update(testcase_meta.get("default_urls"))  # only for optimized mode, urls not shared between processes
     logger = config_data.get("LOGGER")
     testcase_meta.pop("config_data")
     try:
         file_name = config_data.get("PATH")
         file_path = download_common_file(file_name,testcase_meta.get("SUITE_VARS",None))
-        dynamic_testcase = moduleImports(file_path)
+        dynamic_testcase = moduleImports(file_path[0])
         try:
             # TODO update the config_data to contain some default values
             # GEMPYPFOLDER
             all_classes = inspect.getmembers(dynamic_testcase, inspect.isclass)
             for name, cls in all_classes:
                 # currently running only one class easily extensible to run multiple classes
                 # from single file
```

### Comparing `gempyp-1.0.90b3/gempyp/engine/simpleTestcase.py` & `gempyp-1.0.90b4/gempyp/engine/simpleTestcase.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/engine/testData.py` & `gempyp-1.0.90b4/gempyp/engine/testData.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/final_report.html` & `gempyp-1.0.90b4/gempyp/final_report.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/gemPyp.py` & `gempyp-1.0.90b4/gempyp/gemPyp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/jira/jiraIntegration.py` & `gempyp-1.0.90b4/gempyp/jira/jiraIntegration.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/jira/jiraIntegrationCopy.py` & `gempyp-1.0.90b4/gempyp/jira/jiraIntegrationCopy.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/libs/common.py` & `gempyp-1.0.90b4/gempyp/libs/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             script_path, script_name = importFromPath(file_name)
             script_name = script_name.split(".")[0]
             if script_path is not None:
                 sys.path.append(script_path)
             try:
                 dynamicTestcase = importlib.import_module(script_name) 
             except Exception:
-                logging.info("when absolute and module import both failed")
+                logging.info("when absolute and module import both failed. Trying relative path....")
                 try:
                     for each in sys.path:
                         if isinstance(each,dict) and each is not None:
                             logging.info("Fetching config path - {}".format( each['XMLConfigDir']))
                             lib_path = os.path.join(each['XMLConfigDir'], script_path)
                     sys.path.append(lib_path)
                     dynamicTestcase = importlib.import_module(script_name.split(".")[0])
```

### Comparing `gempyp-1.0.90b3/gempyp/libs/gem_s3_common.py` & `gempyp-1.0.90b4/gempyp/libs/gem_s3_common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/libs/logConfig.py` & `gempyp-1.0.90b4/gempyp/libs/logConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/libs/parsers.py` & `gempyp-1.0.90b4/gempyp/libs/parsers.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/apiCommon.py` & `gempyp-1.0.90b4/gempyp/pyprest/apiCommon.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/compareFunctions.py` & `gempyp-1.0.90b4/gempyp/pyprest/compareFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/keyCheck.py` & `gempyp-1.0.90b4/gempyp/pyprest/keyCheck.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/legacyComparison.py` & `gempyp-1.0.90b4/gempyp/pyprest/legacyComparison.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/miscVariables.py` & `gempyp-1.0.90b4/gempyp/pyprest/miscVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/postAssertion.py` & `gempyp-1.0.90b4/gempyp/pyprest/postAssertion.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/postVariables.py` & `gempyp-1.0.90b4/gempyp/pyprest/postVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/predefinedFunctions.py` & `gempyp-1.0.90b4/gempyp/pyprest/predefinedFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/preVariables.py` & `gempyp-1.0.90b4/gempyp/pyprest/preVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/pypRest.py` & `gempyp-1.0.90b4/gempyp/pyprest/pypRest.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/reporting.py` & `gempyp-1.0.90b4/gempyp/pyprest/reporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/restEngine.py` & `gempyp-1.0.90b4/gempyp/pyprest/restEngine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/restObj.py` & `gempyp-1.0.90b4/gempyp/pyprest/restObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/utils.py` & `gempyp-1.0.90b4/gempyp/pyprest/utils.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/pyprest/variableReplacement.py` & `gempyp-1.0.90b4/gempyp/pyprest/variableReplacement.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/reporter/reportGenerator.py` & `gempyp-1.0.90b4/gempyp/reporter/reportGenerator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/sdk/executor.py` & `gempyp-1.0.90b4/gempyp/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/sdk/worker.py` & `gempyp-1.0.90b4/gempyp/sdk/worker.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/gempyp/testcase.html` & `gempyp-1.0.90b4/gempyp/testcase.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/pyproject.toml` & `gempyp-1.0.90b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gempyp"
-version = "1.0.90b3"
+version = "1.0.90b4"
 description = "An ecosystem of libraries useful for software development"
 authors = ["Gemini Solutions-QA"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://gempyp.readthedocs.io/en/latest/"
 homepage = "https://github.com/Gemini-Solutions/gempyp"
 repository = "https://github.com/Gemini-Solutions/gempyp"
```

### Comparing `gempyp-1.0.90b3/README.md` & `gempyp-1.0.90b4/README.md`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b3/PKG-INFO` & `gempyp-1.0.90b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gempyp
-Version: 1.0.90b3
+Version: 1.0.90b4
 Summary: An ecosystem of libraries useful for software development
 Home-page: https://github.com/Gemini-Solutions/gempyp
 License: MIT
 Author: Gemini Solutions-QA
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gempyp Version: 1.0.90b3 Summary: An ecosystem of
+Metadata-Version: 2.1 Name: gempyp Version: 1.0.90b4 Summary: An ecosystem of
 libraries useful for software development Home-page: https://github.com/Gemini-
 Solutions/gempyp License: MIT Author: Gemini Solutions-QA Requires-Python:
 >=3.6.8,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

