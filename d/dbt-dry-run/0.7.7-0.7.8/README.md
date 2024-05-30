# Comparing `tmp/dbt_dry_run-0.7.7.tar.gz` & `tmp/dbt_dry_run-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_dry_run-0.7.7.tar", max compression
+gzip compressed data, was "dbt_dry_run-0.7.8.tar", max compression
```

## Comparing `dbt_dry_run-0.7.7.tar` & `dbt_dry_run-0.7.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    11356 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/LICENSE
--rw-r--r--   0        0        0    12787 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/README.md
--rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/__init__.py
--rw-r--r--   0        0        0      110 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/__main__.py
--rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/adapter/__init__.py
--rw-r--r--   0        0        0     2144 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/adapter/service.py
--rw-r--r--   0        0        0      122 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/adapter/utils.py
--rw-r--r--   0        0        0     4409 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/cli.py
--rw-r--r--   0        0        0     4153 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/columns_metadata.py
--rw-r--r--   0        0        0     1327 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/exception.py
--rw-r--r--   0        0        0     4212 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/execution.py
--rw-r--r--   0        0        0      715 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/flags.py
--rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/linting/__init__.py
--rw-r--r--   0        0        0     1783 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/linting/column_linting.py
--rw-r--r--   0        0        0     4967 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/literals.py
--rw-r--r--   0        0        0      264 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/__init__.py
--rw-r--r--   0        0        0     4567 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/manifest.py
--rw-r--r--   0        0        0     2491 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/profile.py
--rw-r--r--   0        0        0      733 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/report.py
--rw-r--r--   0        0        0     2176 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/table.py
--rw-r--r--   0        0        0     1686 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_dispatch.py
--rw-r--r--   0        0        0     1494 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/__init__.py
--rw-r--r--   0        0        0     7654 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/incremental_runner.py
--rw-r--r--   0        0        0      860 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/node_test_runner.py
--rw-r--r--   0        0        0     1927 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/seed_runner.py
--rw-r--r--   0        0        0     4089 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/snapshot_runner.py
--rw-r--r--   0        0        0     1798 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/source_runner.py
--rw-r--r--   0        0        0     1066 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/table_runner.py
--rw-r--r--   0        0        0     1192 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/view_runner.py
--rw-r--r--   0        0        0     4747 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/result_reporter.py
--rw-r--r--   0        0        0     2670 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/results.py
--rw-r--r--   0        0        0     4899 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/scheduler.py
--rw-r--r--   0        0        0      970 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/__init__.py
--rw-r--r--   0        0        0     3578 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/big_query_sql_runner.py
--rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/__init__.py
--rw-r--r--   0        0        0      231 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/conftest.py
--rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/linting/__init__.py
--rw-r--r--   0        0        0     1846 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/linting/test_column_linting.py
--rw-r--r--   0        0        0     1691 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_manifest.py
--rw-r--r--   0        0        0     2761 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_profile.py
--rw-r--r--   0        0        0        0 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/__init__.py
--rw-r--r--   0        0        0    19372 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_incremental_runner.py
--rw-r--r--   0        0        0     1633 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_node_runner.py
--rw-r--r--   0        0        0     3406 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_seed_runner.py
--rw-r--r--   0        0        0     9714 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py
--rw-r--r--   0        0        0     1238 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_source_runner.py
--rw-r--r--   0        0        0     4896 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_table_runner.py
--rw-r--r--   0        0        0     2941 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_test_runner.py
--rw-r--r--   0        0        0     5886 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_view_runner.py
--rw-r--r--   0        0        0        0 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/sql_runner/__init__.py
--rw-r--r--   0        0        0     4439 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
--rw-r--r--   0        0        0     5503 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_columns_metadata.py
--rw-r--r--   0        0        0     2678 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_execution.py
--rw-r--r--   0        0        0     8855 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_literals.py
--rw-r--r--   0        0        0     2442 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_result_reporter.py
--rw-r--r--   0        0        0     3831 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_scheduler.py
--rw-r--r--   0        0        0     2631 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/utils.py
--rw-r--r--   0        0        0      167 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/version.py
--rw-r--r--   0        0        0     2171 2024-05-03 13:02:59.734599 dbt_dry_run-0.7.7/pyproject.toml
--rw-r--r--   0        0        0    13728 1970-01-01 00:00:00.000000 dbt_dry_run-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/LICENSE
+-rw-r--r--   0        0        0    12787 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/adapter/__init__.py
+-rw-r--r--   0        0        0     2264 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/adapter/service.py
+-rw-r--r--   0        0        0      122 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/adapter/utils.py
+-rw-r--r--   0        0        0     4409 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/cli.py
+-rw-r--r--   0        0        0     4153 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/columns_metadata.py
+-rw-r--r--   0        0        0     1327 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/exception.py
+-rw-r--r--   0        0        0     4212 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/execution.py
+-rw-r--r--   0        0        0      715 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/flags.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/linting/__init__.py
+-rw-r--r--   0        0        0     1783 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/linting/column_linting.py
+-rw-r--r--   0        0        0     5135 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/literals.py
+-rw-r--r--   0        0        0      264 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/models/__init__.py
+-rw-r--r--   0        0        0     4567 2024-05-30 12:14:49.962626 dbt_dry_run-0.7.8/dbt_dry_run/models/manifest.py
+-rw-r--r--   0        0        0     2491 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/models/profile.py
+-rw-r--r--   0        0        0      733 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/models/report.py
+-rw-r--r--   0        0        0     2196 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/models/table.py
+-rw-r--r--   0        0        0     1686 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_dispatch.py
+-rw-r--r--   0        0        0     1494 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/__init__.py
+-rw-r--r--   0        0        0     7654 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/incremental_runner.py
+-rw-r--r--   0        0        0      860 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/node_test_runner.py
+-rw-r--r--   0        0        0     1927 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/seed_runner.py
+-rw-r--r--   0        0        0     4089 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/snapshot_runner.py
+-rw-r--r--   0        0        0     1798 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/source_runner.py
+-rw-r--r--   0        0        0     1066 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/table_runner.py
+-rw-r--r--   0        0        0     1192 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/node_runner/view_runner.py
+-rw-r--r--   0        0        0     4747 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/result_reporter.py
+-rw-r--r--   0        0        0     2670 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/results.py
+-rw-r--r--   0        0        0     4899 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/scheduler.py
+-rw-r--r--   0        0        0      970 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/sql_runner/__init__.py
+-rw-r--r--   0        0        0     3578 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/sql_runner/big_query_sql_runner.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/linting/__init__.py
+-rw-r--r--   0        0        0     1846 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/linting/test_column_linting.py
+-rw-r--r--   0        0        0     1691 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/models/test_manifest.py
+-rw-r--r--   0        0        0     2761 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/models/test_profile.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/__init__.py
+-rw-r--r--   0        0        0    19372 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_incremental_runner.py
+-rw-r--r--   0        0        0     1633 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_node_runner.py
+-rw-r--r--   0        0        0     3406 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_seed_runner.py
+-rw-r--r--   0        0        0     9714 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_snapshot_runner.py
+-rw-r--r--   0        0        0     1238 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_source_runner.py
+-rw-r--r--   0        0        0     4896 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_table_runner.py
+-rw-r--r--   0        0        0     2941 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_test_runner.py
+-rw-r--r--   0        0        0     5886 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_view_runner.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/sql_runner/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
+-rw-r--r--   0        0        0     5503 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/test_columns_metadata.py
+-rw-r--r--   0        0        0     2678 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/test_execution.py
+-rw-r--r--   0        0        0     8855 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/test_literals.py
+-rw-r--r--   0        0        0     2442 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/test_result_reporter.py
+-rw-r--r--   0        0        0     3831 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/test_scheduler.py
+-rw-r--r--   0        0        0     2631 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/test/utils.py
+-rw-r--r--   0        0        0      167 2024-05-30 12:14:49.966626 dbt_dry_run-0.7.8/dbt_dry_run/version.py
+-rw-r--r--   0        0        0     2171 2024-05-30 12:14:49.974626 dbt_dry_run-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0    13728 1970-01-01 00:00:00.000000 dbt_dry_run-0.7.8/PKG-INFO
```

### Comparing `dbt_dry_run-0.7.7/LICENSE` & `dbt_dry_run-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/README.md` & `dbt_dry_run-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/adapter/service.py` & `dbt_dry_run-0.7.8/dbt_dry_run/adapter/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 from argparse import Namespace
 from dataclasses import asdict, dataclass, field
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from dbt.adapters.base import BaseAdapter
+from dbt.adapters.contracts.connection import Connection
 from dbt.adapters.factory import get_adapter, register_adapter, reset_adapters
 from dbt.config import RuntimeConfig
-from dbt.contracts.connection import Connection
 from dbt.flags import set_from_args
+from dbt.mp_context import get_mp_context
+from dbt_common.context import set_invocation_context
 
 from dbt_dry_run.adapter.utils import default_profiles_dir
 from dbt_dry_run.models import Manifest
 
 
 @dataclass(frozen=True)
 class DbtArgs:
@@ -19,33 +21,34 @@
     project_dir: str = os.getcwd()
     profile: Optional[str] = None
     target: Optional[str] = None
     target_path: Optional[str] = None
     vars: Dict[str, Any] = field(default_factory=dict)
     threads: Optional[int] = None
 
+    dependencies: List[str] = field(default_factory=list)
+
     def to_namespace(self) -> Namespace:
         self_as_dict = asdict(self)
         # self_as_dict["vars"] = json.loads(self_as_dict["vars"])
         return Namespace(**self_as_dict)
 
 
 def set_dbt_args(args: DbtArgs) -> None:
     set_from_args(args.to_namespace(), args)
 
 
 class ProjectService:
     def __init__(self, args: DbtArgs):
         self._args = args
-        set_dbt_args(self._args)
-        dbt_project, dbt_profile = RuntimeConfig.collect_parts(self._args)
-        self._profile = dbt_profile
-        self._config = RuntimeConfig.from_parts(dbt_project, dbt_profile, self._args)
+        set_from_args(self._args.to_namespace(), self._args)
+        set_invocation_context(os.environ)
+        self._config = RuntimeConfig.from_args(self._args)
         reset_adapters()
-        register_adapter(self._config)
+        register_adapter(self._config, get_mp_context())
         self._adapter = get_adapter(self._config)
 
     def get_connection(self) -> Connection:
         connection = self._adapter.connections.set_connection_name("dbt-dry-run")
         return connection
 
     @property
@@ -57,12 +60,12 @@
     def get_dbt_manifest(self) -> Manifest:
         manifest = Manifest.from_filepath(self.manifest_filepath)
 
         return manifest
 
     @property
     def threads(self) -> int:
-        return self._profile.threads
+        return self._config.threads
 
     @property
     def adapter(self) -> BaseAdapter:
         return self._adapter
```

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/cli.py` & `dbt_dry_run-0.7.8/dbt_dry_run/cli.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/columns_metadata.py` & `dbt_dry_run-0.7.8/dbt_dry_run/columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/exception.py` & `dbt_dry_run-0.7.8/dbt_dry_run/exception.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/execution.py` & `dbt_dry_run-0.7.8/dbt_dry_run/execution.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/flags.py` & `dbt_dry_run-0.7.8/dbt_dry_run/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/linting/column_linting.py` & `dbt_dry_run-0.7.8/dbt_dry_run/linting/column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/literals.py` & `dbt_dry_run-0.7.8/dbt_dry_run/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     BigQueryFieldType.TIME: lambda: "TIME(12,0,0)",
     BigQueryFieldType.DATETIME: lambda: "DATETIME(2021,1,1,12,0,0)",
     BigQueryFieldType.GEOGRAPHY: lambda: "ST_GeogPoint(0.0, 0.0)",
     BigQueryFieldType.INTERVAL: lambda: "MAKE_INTERVAL(1)",
     BigQueryFieldType.NUMERIC: lambda: "CAST(1 AS NUMERIC)",
     BigQueryFieldType.BIGNUMERIC: lambda: "CAST(2 AS BIGNUMERIC)",
     BigQueryFieldType.JSON: lambda: "PARSE_JSON('{\"a\": 1}')",
+    BigQueryFieldType.RANGE: lambda: "RANGE(DATE '2022-12-01', DATE '2022-12-31')",
 }
 
 _EXAMPLE_VALUES_TEST: Dict[BigQueryFieldType, Callable[[], str]] = {
     BigQueryFieldType.STRING: lambda: f"'foo'",
     BigQueryFieldType.BYTES: lambda: f"b'foo'",
     BigQueryFieldType.INTEGER: lambda: "1",
     BigQueryFieldType.INT64: lambda: "1",
@@ -41,14 +42,15 @@
     BigQueryFieldType.TIME: lambda: "TIME(12,0,0)",
     BigQueryFieldType.DATETIME: lambda: "DATETIME(2021,1,1,12,0,0)",
     BigQueryFieldType.INTERVAL: lambda: "MAKE_INTERVAL(1)",
     BigQueryFieldType.GEOGRAPHY: lambda: "ST_GeogPoint(0.0, 0.0)",
     BigQueryFieldType.NUMERIC: lambda: "CAST(1 AS NUMERIC)",
     BigQueryFieldType.BIGNUMERIC: lambda: "CAST(2 AS BIGNUMERIC)",
     BigQueryFieldType.JSON: lambda: "PARSE_JSON('{\"a\": 1}')",
+    BigQueryFieldType.RANGE: lambda: "RANGE(DATE '2022-12-01', DATE '2022-12-31')",
 }
 
 _ACTIVE_EXAMPLE_VALUES = _EXAMPLE_VALUES
 
 
 def enable_test_example_values(enabled: bool) -> None:
     global _ACTIVE_EXAMPLE_VALUES
```

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/models/manifest.py` & `dbt_dry_run-0.7.8/dbt_dry_run/models/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/models/profile.py` & `dbt_dry_run-0.7.8/dbt_dry_run/models/profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/models/report.py` & `dbt_dry_run-0.7.8/dbt_dry_run/models/report.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/models/table.py` & `dbt_dry_run-0.7.8/dbt_dry_run/models/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     INTERVAL = "INTERVAL"
     GEOGRAPHY = "GEOGRAPHY"
     NUMERIC = "NUMERIC"
     BIGNUMERIC = "BIGNUMERIC"
     STRUCT = "STRUCT"
     JSON = "JSON"
     RECORD = "RECORD"
+    RANGE = "RANGE"
 
 
 class TableField(BaseModel):
     name: str
     type_: BigQueryFieldType = Field(..., alias="type")
     mode: Optional[BigQueryFieldMode]
     fields: Optional[List["TableField"]] = None
```

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_dispatch.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_dispatch.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/__init__.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/incremental_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/incremental_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/node_test_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/node_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/seed_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/snapshot_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/source_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/source_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/table_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/table_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/view_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/node_runner/view_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/result_reporter.py` & `dbt_dry_run-0.7.8/dbt_dry_run/result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/results.py` & `dbt_dry_run-0.7.8/dbt_dry_run/results.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/scheduler.py` & `dbt_dry_run-0.7.8/dbt_dry_run/scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/__init__.py` & `dbt_dry_run-0.7.8/dbt_dry_run/sql_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/big_query_sql_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/sql_runner/big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/linting/test_column_linting.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/linting/test_column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_manifest.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/models/test_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_profile.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/models/test_profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_incremental_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_incremental_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_node_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_node_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_seed_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_source_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_source_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_table_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_table_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_test_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_view_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/node_runner/test_view_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/test_columns_metadata.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/test_columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/test_execution.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/test_literals.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/test_literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/test_result_reporter.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/test_result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/test_scheduler.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/dbt_dry_run/test/utils.py` & `dbt_dry_run-0.7.8/dbt_dry_run/test/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.7/pyproject.toml` & `dbt_dry_run-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-dry-run"
-version = "0.7.7"
+version = "0.7.8"
 description = "Dry run dbt projects"
 authors = ["Connor Charles <connor.charles@autotrader.co.uk>",
            "Phil hope <philip.hope@autotrader.co.uk>",
            "Angelos Georgiadis <angelos.georgiadis@autotrader.co.uk>",
            "Richard Wilmer <richard.wilmer@autotrader.co.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
@@ -23,21 +23,21 @@
 pyyaml = "~6"
 typer = "~0"
 
 [tool.poetry.dev-dependencies]
 black = "^22"
 isort = "^5.10.1"
 pytest = "^7.2.0"
-mypy = "^0.931"
+mypy = "^0.981"
 types-PyYAML = "^6.0.4"
 pytest-cov = "^4.0.0"
 twine = "^3.8.0"
 types-setuptools = "^57.4.9"
 pytest-mock = "^3.7.0"
-dbt-bigquery = "~1.7.0"
+dbt-bigquery = "~1.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "dbt_dry_run/test"
```

### Comparing `dbt_dry_run-0.7.7/PKG-INFO` & `dbt_dry_run-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-dry-run
-Version: 0.7.7
+Version: 0.7.8
 Summary: Dry run dbt projects
 Home-page: https://github.com/autotraderuk/dbt-dry-run
 License: Apache-2.0
 Author: Connor Charles
 Author-email: connor.charles@autotrader.co.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

