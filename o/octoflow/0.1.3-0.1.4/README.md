# Comparing `tmp/octoflow-0.1.3.tar.gz` & `tmp/octoflow-0.1.4.tar.gz`

## Comparing `octoflow-0.1.3.tar` & `octoflow-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/config.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/constants.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/core.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/exceptions.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/logging.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/plugin.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/typing.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/base.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/dataclass.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/dataset.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/expression.py
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/loaders.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/metadata.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/sampler.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/schema.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/data/types.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/tracking/__init__.py
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/tracking/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/tracking/artifact/__init__.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/tracking/artifact/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/cache.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/collections.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/config.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/func.py
--rw-r--r--   0        0        0    11582 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/hashing.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/objects.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/rsync.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.3/octoflow/utils/string.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.3/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.3/AUTHORS.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.3/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.3/README.md
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/config.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/constants.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/core.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/exceptions.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/logging.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/plugin.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/typing.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/base.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/dataclass.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/dataset.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/expression.py
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/loaders.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/metadata.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/sampler.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/schema.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/types.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/__init__.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/artifact/__init__.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/artifact/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/cache.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/collections.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/config.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/func.py
+-rw-r--r--   0        0        0    11582 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/hashing.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/objects.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/rsync.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/string.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.4/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.4/AUTHORS.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.4/README.md
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.4/PKG-INFO
```

### Comparing `octoflow-0.1.3/octoflow/__init__.py` & `octoflow-0.1.4/octoflow/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 
 from octoflow import logging
 from octoflow.config import config
 from octoflow.utils.config import Config
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 __all__ = [
     "Config",
     "config",
     "logger",
     "logging",
 ]
```

### Comparing `octoflow-0.1.3/octoflow/config.py` & `octoflow-0.1.4/octoflow/config.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/core.py` & `octoflow-0.1.4/octoflow/core.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/logging.py` & `octoflow-0.1.4/octoflow/logging.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/plugin.py` & `octoflow-0.1.4/octoflow/plugin.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/__init__.py` & `octoflow-0.1.4/octoflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/base.py` & `octoflow-0.1.4/octoflow/data/base.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/dataclass.py` & `octoflow-0.1.4/octoflow/data/dataclass.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/dataset.py` & `octoflow-0.1.4/octoflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/expression.py` & `octoflow-0.1.4/octoflow/data/expression.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/loaders.py` & `octoflow-0.1.4/octoflow/data/loaders.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/metadata.py` & `octoflow-0.1.4/octoflow/data/metadata.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/sampler.py` & `octoflow-0.1.4/octoflow/data/sampler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/schema.py` & `octoflow-0.1.4/octoflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/data/types.py` & `octoflow-0.1.4/octoflow/data/types.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/tracking/models.py` & `octoflow-0.1.4/octoflow/tracking/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import enum
 import json
+import re
 import shutil
 import sqlite3 as sqlite
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 from packaging.version import Version
@@ -31,18 +32,18 @@
         self,
         path: Union[Path, str],
         /,
         name: str,
         description: Optional[str] = None,
     ):
         self.path = Path(path)
-        if not name.isidentifier():
+        if not re.match(r"^[a-zA-Z_-][a-zA-Z0-9_-]*$", name):
             msg = f"invalid name: {name}"
             raise ValueError(msg)
-        self.name = name
+        self.name = name.strip()
         self.description = description
         self.save(exist_ok=True)
 
     def save(self, exist_ok: bool = False) -> None:
         path = Path(self.path) / self.name / "metadata.json"
         if not exist_ok and path.exists():
             msg = f"already exists: {path}"
@@ -129,15 +130,15 @@
             return Run.from_existing(run_path)
         return None
 
 
 TABLE_CREATE_SQL = """CREATE TABLE IF NOT EXISTS runs (
 id INTEGER PRIMARY KEY AUTOINCREMENT,
 key TEXT,
-value JSON,
+value TEXT,
 type TEXT,
 step INTEGER,
 FOREIGN KEY (step) REFERENCES runs (id) ON DELETE CASCADE,
 CHECK (type IN ('param', 'metric'))
 )"""
 
 """,
@@ -238,15 +239,15 @@
             if step_type != "param":
                 msg = f"step '{step}' is not a param type"
                 raise ValueError(msg)
         try:
             cursor = conn.cursor()
             result = cursor.execute(
                 "INSERT INTO runs VALUES (NULL, ?, ?, ?, ?)",
-                (key, value, type, step),
+                (key, json.dumps(value), type, step),
             )
             conn.commit()
         except sqlite.Error as e:
             conn.rollback()
             msg = f"failed to log {type} '{key}' with value '{value}'"
             raise ValueError(msg) from e
         finally:
@@ -311,15 +312,18 @@
         edges: Dict[int, List[int]] = {}
         for id, _, _, _, step in results:
             if step is None:
                 step = -1
             if step not in edges:
                 edges[step] = []
             edges[step].append(id)
-        nodes = {id: (key, value, type) for id, key, value, type, _ in results}
+        nodes = {
+            id: (key, json.loads(value), type)
+            for id, key, value, type, _ in results
+        }
         tree = build_nested_tree(nodes, edges)
         values = filter_by_var(tree, var)
         return pd.DataFrame(values)
 
 
 def build_nested_tree(
     nodes: Dict[int, Tuple[str, Any, str]],
```

### Comparing `octoflow-0.1.3/octoflow/tracking/artifact/handler.py` & `octoflow-0.1.4/octoflow/tracking/artifact/handler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/cache.py` & `octoflow-0.1.4/octoflow/utils/cache.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/collections.py` & `octoflow-0.1.4/octoflow/utils/collections.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/config.py` & `octoflow-0.1.4/octoflow/utils/config.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/func.py` & `octoflow-0.1.4/octoflow/utils/func.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/hashing.py` & `octoflow-0.1.4/octoflow/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/objects.py` & `octoflow-0.1.4/octoflow/utils/objects.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/rsync.py` & `octoflow-0.1.4/octoflow/utils/rsync.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/octoflow/utils/string.py` & `octoflow-0.1.4/octoflow/utils/string.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/.gitignore` & `octoflow-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/LICENSE` & `octoflow-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/README.md` & `octoflow-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/pyproject.toml` & `octoflow-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.3/PKG-INFO` & `octoflow-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoflow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Streamlining machine learning tracking for seamless experiment management.
 Project-URL: Documentation, https://github.com/ysenarath/octoflow
 Project-URL: Source, https://github.com/ysenarath/octoflow
 Author-email: Yasas Senarath <email@example.com>
 License-Expression: MIT
 License-File: AUTHORS.md
 License-File: LICENSE
```

