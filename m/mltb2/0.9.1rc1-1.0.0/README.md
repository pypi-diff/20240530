# Comparing `tmp/mltb2-0.9.1rc1.tar.gz` & `tmp/mltb2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.9.1rc1.tar", max compression
+gzip compressed data, was "mltb2-1.0.0.tar", max compression
```

## Comparing `mltb2-0.9.1rc1.tar` & `mltb2-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     9405 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1118 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/LICENSE
--rw-r--r--   0        0        0      592 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/Makefile
--rw-r--r--   0        0        0     2154 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/README.md
--rw-r--r--   0        0        0      185 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/__init__.py
--rw-r--r--   0        0        0     7894 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/arangodb.py
--rw-r--r--   0        0        0     8100 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/data.py
--rw-r--r--   0        0        0     1759 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/db.py
--rw-r--r--   0        0        0     3281 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/fasttext.py
--rw-r--r--   0        0        0     2150 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/files.py
--rw-r--r--   0        0        0     3750 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/md.py
--rw-r--r--   0        0        0    10195 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/openai.py
--rw-r--r--   0        0        0     6853 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/optuna.py
--rw-r--r--   0        0        0     4697 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/plot.py
--rw-r--r--   0        0        0        0 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/py.typed
--rw-r--r--   0        0        0     7038 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/somajo.py
--rw-r--r--   0        0        0     3124 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/somajo_transformers.py
--rw-r--r--   0        0        0     9708 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/text.py
--rw-r--r--   0        0        0     3847 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/mltb2/transformers.py
--rw-r--r--   0        0        0     6054 2023-12-31 22:16:18.524764 mltb2-0.9.1rc1/pyproject.toml
--rw-r--r--   0        0        0     5149 1970-01-01 00:00:00.000000 mltb2-0.9.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     9405 2024-05-30 12:56:39.550498 mltb2-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1128 2024-05-30 12:56:39.550498 mltb2-1.0.0/LICENSE
+-rw-r--r--   0        0        0      604 2024-05-30 12:56:39.550498 mltb2-1.0.0/Makefile
+-rw-r--r--   0        0        0     2190 2024-05-30 12:56:39.550498 mltb2-1.0.0/README.md
+-rw-r--r--   0        0        0      185 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/__init__.py
+-rw-r--r--   0        0        0    11923 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/arangodb.py
+-rw-r--r--   0        0        0     4719 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/bs.py
+-rw-r--r--   0        0        0     8115 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/data.py
+-rw-r--r--   0        0        0     1738 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/db.py
+-rw-r--r--   0        0        0     3759 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/fasttext.py
+-rw-r--r--   0        0        0     8767 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/files.py
+-rw-r--r--   0        0        0     3758 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/md.py
+-rw-r--r--   0        0        0    13131 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/openai.py
+-rw-r--r--   0        0        0     6841 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/optuna.py
+-rw-r--r--   0        0        0     4665 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/plot.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/py.typed
+-rw-r--r--   0        0        0     7532 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/somajo.py
+-rw-r--r--   0        0        0     3130 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/somajo_transformers.py
+-rw-r--r--   0        0        0    10963 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/text.py
+-rw-r--r--   0        0        0     3847 2024-05-30 12:56:39.554498 mltb2-1.0.0/mltb2/transformers.py
+-rw-r--r--   0        0        0     6714 2024-05-30 12:56:39.554498 mltb2-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 mltb2-1.0.0/PKG-INFO
```

### Comparing `mltb2-0.9.1rc1/CONTRIBUTING.md` & `mltb2-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mltb2-0.9.1rc1/LICENSE` & `mltb2-1.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
-Copyright (c) 2023 Philip May
-Copyright (c) 2023 Philip May, Deutsche Telekom AG
+Copyright (c) 2023-2024 Philip May
+Copyright (c) 2023-2024 Philip May, Deutsche Telekom AG
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mltb2-0.9.1rc1/Makefile` & `mltb2-1.0.0/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 src := mltb2
 other-src := tests docs
 
 check:
 	poetry run black $(src) $(other-src) --check --diff
 	poetry run mypy --install-types --non-interactive $(src) $(other-src)
-	poetry run ruff $(src) $(other-src)
+	poetry run ruff check $(src) $(other-src)
 	poetry run mdformat --check --number .
 	poetry run make -C docs clean doctest
 
 format:
 	poetry run black $(src) $(other-src)
-	poetry run ruff $(src) $(other-src) --fix
+	poetry run ruff check $(src) $(other-src) --fix
 	poetry run mdformat --number .
 
 test:
 	poetry run pytest $(other-src)
 
 sphinx:
 	poetry run make -C docs clean html
```

### Comparing `mltb2-0.9.1rc1/README.md` & `mltb2-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,38 +6,34 @@
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://github.com/telekom/mltb2/blob/main/pyproject.toml)
 <br/>
 [![pytest](https://github.com/telekom/mltb2/actions/workflows/pytest.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/pytest.yml)
 [![Static Code Checks](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml)
 [![Build & Deploy Doc](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml)
 [![GitHub issues](https://img.shields.io/github/issues-raw/telekom/mltb2)](https://github.com/telekom/mltb2/issues)
 
-📦 A box of machine learning tools. 📦
+📦 A box full of machine learning tools. 📦
 
 - [Documentation Page](https://telekom.github.io/mltb2/)
 - [How to contribute](https://github.com/telekom/mltb2/blob/main/CONTRIBUTING.md)
 
 ## Installation
 
 MLTB2 is available at [the Python Package Index (PyPI)](https://pypi.org/project/mltb2/).
 It can be installed with pip:
 
 ```bash
 pip install mltb2
 ```
 
-Some optional dependencies might be necessary. You can install all of them with:
-
-```bash
-pip install mltb2[files,fasttext,optuna,plot,somajo,transformers,somajo_transformers,openai]
-```
-
-If you don't want to install all dependencies, see
+For many modules optional dependencies are necessary.
+Those optional dependencies must be installed when you want to use the module.
+To install those module specific dependencies see
 [the description of the individual modules](https://telekom.github.io/mltb2/api-reference.html).
 
 ## Licensing
 
-Copyright (c) 2023 Philip May\
-Copyright (c) 2023 Philip May, Deutsche Telekom AG
+Copyright (c) 2023-2024 [Philip May](https://philipmay.org)\
+Copyright (c) 2023-2024 [Philip May](https://philipmay.org), [Deutsche Telekom AG](https://www.telekom.de/)
 
 Licensed under the **MIT License** (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License by reviewing the file
 [LICENSE](https://github.com/telekom/mltb2/blob/main/LICENSE) in the repository.
```

### Comparing `mltb2-0.9.1rc1/mltb2/arangodb.py` & `mltb2-1.0.0/mltb2/arangodb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Philip May
+# Copyright (c) 2023-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """ArangoDB utils module.
 
 Hint:
     Use pip to install the necessary dependencies for this module:
@@ -10,20 +10,21 @@
 """
 
 
 import gzip
 from argparse import ArgumentParser
 from contextlib import closing
 from dataclasses import dataclass
-from typing import Dict, Optional, Sequence, Union
+from typing import Any, Dict, Optional, Sequence, Union
 
 import jsonlines
 from arango import ArangoClient
 from arango.database import StandardDatabase
 from dotenv import dotenv_values
+from pandas import DataFrame
 from tqdm import tqdm
 
 from mltb2.db import AbstractBatchDataManager
 
 
 def _check_config_keys(config: Dict[str, Optional[str]], expected_config_keys: Sequence[str]) -> None:
     """Check if all expected keys are in config.
@@ -32,15 +33,48 @@
     """
     for expected_config_key in expected_config_keys:
         if expected_config_key not in config:
             raise ValueError(f"Config file must contain '{expected_config_key}'!")
 
 
 @dataclass
-class ArangoBatchDataManager(AbstractBatchDataManager):
+class ArangoConnectionManager:
+    """ArangoDB connection manager.
+
+    Base class to manage / create ArangoDB connections.
+
+    Args:
+        hosts: ArangoDB host or hosts.
+        db_name: ArangoDB database name.
+        username: ArangoDB username.
+        password: ArangoDB password.
+    """
+
+    hosts: Union[str, Sequence[str]]
+    db_name: str
+    username: str
+    password: str
+
+    def _arango_client_factory(self) -> ArangoClient:
+        """Create an ArangoDB client."""
+        arango_client = ArangoClient(hosts=self.hosts)
+        return arango_client
+
+    def _connection_factory(self, arango_client: ArangoClient) -> StandardDatabase:
+        """Create an ArangoDB connection.
+
+        Args:
+            arango_client: ArangoDB client.
+        """
+        connection = arango_client.db(self.db_name, username=self.username, password=self.password)
+        return connection
+
+
+@dataclass
+class ArangoBatchDataManager(AbstractBatchDataManager, ArangoConnectionManager):
     """ArangoDB implementation of the ``AbstractBatchDataManager``.
 
     Args:
         hosts: ArangoDB host or hosts.
         db_name: ArangoDB database name.
         username: ArangoDB username.
         password: ArangoDB password.
@@ -48,18 +82,14 @@
         attribute_name: This attribute is used to check if a document is already processed.
             If the attribute is not present in a document, the document is processed.
             If it is available the document is considered as already processed.
         batch_size: The batch size.
         aql_overwrite: AQL string to overwrite the default.
     """
 
-    hosts: Union[str, Sequence[str]]
-    db_name: str
-    username: str
-    password: str
     collection_name: str
     attribute_name: str
     batch_size: int = 20
     aql_overwrite: Optional[str] = None
 
     @classmethod
     def from_config_file(cls, config_file_name, aql_overwrite: Optional[str] = None):
@@ -103,38 +133,24 @@
             "collection_name",
             "attribute_name",
             "batch_size",
         ]
         _check_config_keys(arango_config, expected_config_file_keys)
 
         return cls(
-            hosts=arango_config["hosts"],  # type: ignore
-            db_name=arango_config["db_name"],  # type: ignore
-            username=arango_config["username"],  # type: ignore
-            password=arango_config["password"],  # type: ignore
-            collection_name=arango_config["collection_name"],  # type: ignore
-            attribute_name=arango_config["attribute_name"],  # type: ignore
-            batch_size=int(arango_config["batch_size"]),  # type: ignore
+            hosts=arango_config["hosts"],  # type: ignore[arg-type]
+            db_name=arango_config["db_name"],  # type: ignore[arg-type]
+            username=arango_config["username"],  # type: ignore[arg-type]
+            password=arango_config["password"],  # type: ignore[arg-type]
+            collection_name=arango_config["collection_name"],  # type: ignore[arg-type]
+            attribute_name=arango_config["attribute_name"],  # type: ignore[arg-type]
+            batch_size=int(arango_config["batch_size"]),  # type: ignore[arg-type]
             aql_overwrite=aql_overwrite,
         )
 
-    def _arango_client_factory(self) -> ArangoClient:
-        """Create an ArangoDB client."""
-        arango_client = ArangoClient(hosts=self.hosts)
-        return arango_client
-
-    def _connection_factory(self, arango_client: ArangoClient) -> StandardDatabase:
-        """Create an ArangoDB connection.
-
-        Args:
-            arango_client: ArangoDB client.
-        """
-        connection = arango_client.db(self.db_name, username=self.username, password=self.password)
-        return connection
-
     def load_batch(self) -> Sequence:
         """Load a batch of data from the ArangoDB database.
 
         Returns:
             The loaded batch of data.
         """
         with closing(self._arango_client_factory()) as arango_client:
@@ -146,20 +162,20 @@
             }
             if self.aql_overwrite is None:
                 aql = "FOR doc IN @@coll FILTER !HAS(doc, @attribute) LIMIT @batch_size RETURN doc"
             else:
                 aql = self.aql_overwrite
             cursor = connection.aql.execute(
                 aql,
-                bind_vars=bind_vars,  # type: ignore
+                bind_vars=bind_vars,  # type: ignore[arg-type]
                 batch_size=self.batch_size,
             )
-            with closing(cursor) as closing_cursor:  # type: ignore
-                batch = closing_cursor.batch()  # type: ignore
-        return batch  # type: ignore
+            with closing(cursor) as closing_cursor:  # type: ignore[type-var]
+                batch = closing_cursor.batch()  # type: ignore[union-attr]
+        return batch  # type: ignore[return-value]
 
     def save_batch(self, batch: Sequence) -> None:
         """Save a batch of data to the ArangoDB database.
 
         Args:
             batch: The batch of data to save.
         """
@@ -191,28 +207,132 @@
     arango_config = dotenv_values(args.conf)
     expected_config_file_keys = ["hosts", "db_name", "username", "password"]
     _check_config_keys(arango_config, expected_config_file_keys)
 
     output_file_name = f"./{args.col}_backup.jsonl.gz"
     print(f"Writing backup to '{output_file_name}'...")
 
-    with closing(ArangoClient(hosts=arango_config["hosts"])) as arango_client, gzip.open(  # type: ignore
+    with closing(ArangoClient(hosts=arango_config["hosts"])) as arango_client, gzip.open(  # type: ignore[arg-type]
         output_file_name, "w"
     ) as gzip_out:
         connection = arango_client.db(
-            arango_config["db_name"],  # type: ignore
-            arango_config["username"],  # type: ignore
-            arango_config["password"],  # type: ignore
+            arango_config["db_name"],  # type: ignore[arg-type]
+            arango_config["username"],  # type: ignore[arg-type]
+            arango_config["password"],  # type: ignore[arg-type]
         )
-        jsonlines_writer = jsonlines.Writer(gzip_out)  # type: ignore
+        jsonlines_writer = jsonlines.Writer(gzip_out)  # type: ignore[arg-type]
         try:
             cursor = connection.aql.execute(
                 "FOR doc IN @@coll RETURN doc",
                 bind_vars={"@coll": args.col},
                 batch_size=100,
-                max_runtime=60 * 60,  # type: ignore # 1 hour
+                max_runtime=60 * 60,  # type: ignore[arg-type] # 1 hour
                 stream=True,
             )
             for doc in tqdm(cursor):
                 jsonlines_writer.write(doc)
         finally:
-            cursor.close(ignore_missing=True)  # type: ignore
+            cursor.close(ignore_missing=True)  # type: ignore[union-attr]
+
+
+@dataclass
+class ArangoImportDataManager(ArangoConnectionManager):
+    """ArangoDB import tool to fill data into a collection.
+
+    Args:
+        hosts: ArangoDB host or hosts.
+        db_name: ArangoDB database name.
+        username: ArangoDB username.
+        password: ArangoDB password.
+    """
+
+    @classmethod
+    def from_config_file(cls, config_file_name):
+        """Construct this from config file.
+
+        The config file must contain at least these values:
+
+        - ``hosts``
+        - ``db_name``
+        - ``username``
+        - ``password``
+
+        Config file example:
+
+        .. code-block::
+
+            hosts="https://arangodb.com"
+            db_name="my_ml_database"
+            username="my_username"
+            password="secret"
+
+        Args:
+            config_file_name: The config file name (path).
+        """
+        # load config file data
+        arango_config = dotenv_values(config_file_name)
+
+        # check if all necessary keys are in config file
+        expected_config_file_keys = [
+            "hosts",
+            "db_name",
+            "username",
+            "password",
+        ]
+        _check_config_keys(arango_config, expected_config_file_keys)
+
+        return cls(
+            hosts=arango_config["hosts"],
+            db_name=arango_config["db_name"],
+            username=arango_config["username"],
+            password=arango_config["password"],
+        )
+
+    def import_dicts(
+        self, dicts: Sequence[Dict[str, Any]], collection_name: str, create_collection: bool = False
+    ) -> None:
+        """Import data to ArangoDB.
+
+        Args:
+            dicts: The data to import.
+            collection_name: The collection name to import to.
+            create_collection: If ``True`` the collection is created if it does not exist.
+        Raises:
+            arango.exceptions.DocumentInsertError: If import fails.
+        """
+        with closing(self._arango_client_factory()) as arango_client:
+            connection = self._connection_factory(arango_client)
+
+            # get (or create) collection
+            if not connection.has_collection(collection_name):
+                if create_collection:
+                    collection = connection.create_collection(collection_name)
+                else:
+                    raise ValueError(
+                        f"Collection '{collection_name}' does not exist! "
+                        "Create it or specify 'create_collection=True'."
+                    )
+            else:
+                collection = connection.collection(collection_name)
+
+            collection.import_bulk(  # type: ignore[union-attr]
+                dicts,
+                halt_on_error=True,
+                details=False,
+                overwrite=False,
+                on_duplicate="error",
+                sync=True,
+                batch_size=100,
+            )
+
+    def import_dataframe(self, dataframe: DataFrame, collection_name: str, create_collection: bool = False) -> None:
+        """Import Pandas data to ArangoDB.
+
+        Args:
+            dataframe: The Pandas data to import.
+            collection_name: The collection name to import to.
+            create_collection: If ``True`` the collection is created if it does not exist.
+        Raises:
+            arango.exceptions.DocumentInsertError: If import fails.
+        """
+        dicts = dataframe.to_dict(orient="records")
+        self.import_dicts(dicts, collection_name, create_collection)
```

### Comparing `mltb2-0.9.1rc1/mltb2/data.py` & `mltb2-1.0.0/mltb2/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 - 2023 Philip May
+# Copyright (c) 2020-2024 Philip May
 # Copyright (c) 2021 Sigrun May, Helmholtz-Zentrum für Infektionsforschung GmbH (HZI)
 # Copyright (c) 2021 Sigrun May, Ostfalia Hochschule für angewandte Wissenschaften
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """This module offers tools for loading data.
 
@@ -89,15 +89,15 @@
 
     label = []
 
     for line in page_text_lines:
         try:
             i = int(line)
             label.append(0 if i > 0 else 1)
-        except ValueError:
+        except ValueError:  # noqa: PERF203
             pass  # we ignore this
 
     assert len(label) == 62
     label_series = pd.Series(label)
     return label_series
```

### Comparing `mltb2-0.9.1rc1/mltb2/db.py` & `mltb2-1.0.0/mltb2/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Philip May
+# Copyright (c) 2023-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """Database utils module."""
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
@@ -15,20 +15,18 @@
     This class (respectively an implementation of it) is intended to be
     used in conjunction with the :class:`BatchDataProcessor`.
     """
 
     @abstractmethod
     def load_batch(self) -> Sequence:
         """Load a batch of data from the database."""
-        pass
 
     @abstractmethod
     def save_batch(self, batch: Sequence) -> None:
         """Save a batch of data to the database."""
-        pass
 
 
 @dataclass
 class BatchDataProcessor:
     """Process batches of data from a database.
 
     Args:
```

### Comparing `mltb2-0.9.1rc1/mltb2/fasttext.py` & `mltb2-1.0.0/mltb2/fasttext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright (c) 2023 Philip May
+# Copyright (c) 2023-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """This module offers tools for `fastText <https://fasttext.cc/docs/en/support.html>`_.
 
 Hint:
     Use pip to install the necessary dependencies for this module:
     ``pip install mltb2[fasttext]``
 """
 
 import os
 from dataclasses import dataclass, field
+from typing import List, Optional
 
 import fasttext
 from fasttext.FastText import _FastText
 
 from mltb2.files import fetch_remote_file, get_and_create_mltb2_data_dir
 
 
@@ -47,20 +48,23 @@
                 url=model_url,
                 sha256_checksum=sha256_checksum,
             )
             assert fetch_remote_file_path == model_full_path
 
         return model_full_path
 
-    def __call__(self, text: str, num_lang: int = 10):
+    def __call__(self, text: str, num_lang: int = 10, always_detect_lang: Optional[List[str]] = None):
         """Identify languages of a given text.
 
         Args:
             text: the text for which the language is to be recognized
-            num_lang: number of returned languages
+            num_lang: number of returned language probabilities
+            always_detect_lang: A list of languages that should always be returned
+                even if not detected. If the language is not detected, the probability
+                is set to 0.0.
         Returns:
             A dict from language to probability.
             This dict contains no more than ``num_lang`` elements.
             So it is not guaranteed that the language you want to recognize is
             included in the dict. This is the case when the probability is very low.
             Possible languages are: ``af als am an ar arz as ast av az azb ba bar
             bcl be bg bh bn bo bpy br bs bxr ca cbk ce ceb ckb co cs cv cy da de
@@ -72,8 +76,12 @@
             si sk sl so sq sr su sv sw ta te tg th tk tl tr tt tyv ug uk ur uz vec
             vep vi vls vo wa war wuu xal xmf yi yo yue zh``
         """
         predictions = self.model.predict(text, k=num_lang)
         languages = predictions[0]
         probabilities = predictions[1]
         lang_to_prob = {lang[9:]: prob for lang, prob in zip(languages, probabilities)}
+        if always_detect_lang is not None:
+            for lang in always_detect_lang:
+                if lang not in lang_to_prob:
+                    lang_to_prob[lang] = 0.0
         return lang_to_prob
```

### Comparing `mltb2-0.9.1rc1/mltb2/md.py` & `mltb2-1.0.0/mltb2/md.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) 2023 Philip May, Deutsche Telekom AG
-# Copyright (c) 2023 Philip May
+# Copyright (c) 2023-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """Markdown specific module.
 
 Hint:
     Use pip to install the necessary dependencies for this module:
@@ -30,15 +30,15 @@
     Returns:
         The list of Markdown chunks.
     """
     positions: List[int] = [m.start() for m in re.finditer(_HEADLINE_REGEX, md_text)]
 
     # extend positions
     if 0 not in positions:
-        positions = [0] + positions
+        positions = [0] + positions  # noqa: RUF005
     positions.append(len(md_text))
 
     result = [md_text[x:y].strip() for x, y in zip(positions, positions[1:])]
     return result
 
 
 def chunk_md(md_text: str) -> List[str]:
@@ -92,15 +92,15 @@
             md_text: The Markdown text to be split.
         Returns:
             The list of Markdown section splits.
         """
         md_chunks = chunk_md(md_text)
         counts = self.transformers_token_counter(md_chunks)
 
-        assert len(md_chunks) == len(counts)  # type: ignore[arg-type] # noqa: S101
+        assert len(md_chunks) == len(counts)  # type: ignore[arg-type]
 
         result_merges: List[str] = []
         temp_merges: List[str] = []
         current_count: int = 0
 
         for md_chunk, count in zip(
             tqdm(md_chunks, disable=not self.show_progress_bar), counts  # type: ignore[arg-type]
```

### Comparing `mltb2-0.9.1rc1/mltb2/openai.py` & `mltb2-1.0.0/mltb2/openai.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-# Copyright (c) 2023 Philip May
+# Copyright (c) 2023-2024 Philip May
+# Copyright (c) 2024 Philip May, Deutsche Telekom AG
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """OpenAI specific module.
 
 Hint:
     Use pip to install the necessary dependencies for this module:
     ``pip install mltb2[openai]``
 """
 
 
-from abc import ABC, abstractmethod
+import os
 from dataclasses import dataclass, field
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional, Union
 
 import tiktoken
 import yaml
-from openai import ChatCompletion, Completion
-from openai.openai_object import OpenAIObject
+from openai import AsyncAzureOpenAI, AsyncOpenAI, AzureOpenAI, OpenAI
+from openai.types.chat import ChatCompletion
 from tiktoken.core import Encoding
 from tqdm import tqdm
 
 
 @dataclass
 class OpenAiTokenCounter:
     """Count OpenAI tokens.
@@ -63,214 +64,270 @@
             for t in tqdm(text, disable=not self.show_progress_bar):
                 tokenized_text = self.encoding.encode(t)
                 counts.append(len(tokenized_text))
             return counts
 
 
 @dataclass
-class OpenAiCompletionAnswer:
-    """Answer of an OpenAI completion.
+class OpenAiChatResult:
+    """Result of an OpenAI chat completion.
+
+    If you want to convert this to a ``dict`` use ``asdict(open_ai_chat_result)``
+    from the ``dataclasses`` module.
+
+    See Also:
+        OpenAI API reference: `The chat completion object <https://platform.openai.com/docs/api-reference/chat/object>`_
 
     Args:
-        text: the result of the OpenAI completion
+        content: the result of the OpenAI completion
         model: model name which has been used
         prompt_tokens: number of tokens of the prompt
-        completion_tokens: number of tokens of the completion (``text``)
-        total_tokens: number of total tokens (``prompt_tokens + completion_tokens``)
+        completion_tokens: number of tokens of the completion (``content``)
+        total_tokens: number of total tokens (``prompt_tokens + content_tokens``)
         finish_reason: The reason why the completion stopped.
 
             * ``stop``: Means the API returned the full completion without running into any token limit.
             * ``length``: Means the API stopped the completion because of running into a token limit.
-            * ``function_call``: When the model called a function.
-
-    See Also:
-        * `The chat completion object <https://platform.openai.com/docs/api-reference/chat/object>`_
-        * `The completion object <https://platform.openai.com/docs/api-reference/completions/object>`_
+            * ``content_filter``: When content was omitted due to a flag from the OpenAI content filters.
+            * ``tool_calls``: When the model called a tool.
+            * ``function_call`` (deprecated): When the model called a function.
+
+        completion_args: The arguments which have been used for the completion. Examples:
+
+            * ``model``: always set
+            * ``max_tokens``: only set if ``completion_kwargs`` contained ``max_tokens``
+            * ``temperature``: only set if ``completion_kwargs`` contained ``temperature``
+            * ``top_p``: only set if ``completion_kwargs`` contained ``top_p``
     """
 
-    text: Optional[str] = None
+    content: Optional[str] = None
     model: Optional[str] = None
     prompt_tokens: Optional[int] = None
     completion_tokens: Optional[int] = None
     total_tokens: Optional[int] = None
     finish_reason: Optional[str] = None
+    completion_args: Optional[Dict[str, Any]] = None
 
     @classmethod
-    def from_open_ai_object(cls, open_ai_object: OpenAIObject):
-        """Construct this class from ``OpenAIObject``."""
+    def from_chat_completion(
+        cls,
+        chat_completion: ChatCompletion,
+        completion_kwargs: Optional[Dict[str, Any]] = None,
+    ):
+        """Construct this class from an OpenAI ``ChatCompletion`` object.
+
+        Args:
+            chat_completion: The OpenAI ``ChatCompletion`` object.
+            completion_kwargs: The arguments which have been used for the completion.
+        Returns:
+            The constructed class.
+        """
         result = {}
-        result["model"] = open_ai_object.get("model")
-        usage = open_ai_object.get("usage")
+        result["completion_args"] = completion_kwargs
+        chat_completion_dict = chat_completion.model_dump()
+        result["model"] = chat_completion_dict.get("model")
+        usage = chat_completion_dict.get("usage")
         if usage is not None:
             result["prompt_tokens"] = usage.get("prompt_tokens")
             result["completion_tokens"] = usage.get("completion_tokens")
             result["total_tokens"] = usage.get("total_tokens")
-        choices = open_ai_object.get("choices")
+        choices = chat_completion_dict.get("choices")
         if choices is not None and len(choices) > 0:
             choice = choices[0]
             result["finish_reason"] = choice.get("finish_reason")
-            if "text" in choice:  # non chat models
-                result["text"] = choice.get("text")
-            elif "message" in choice:  # chat models
-                message = choice.get("message")
-                if message is not None:
-                    result["text"] = message.get("content")
-        return cls(**result)
+            message = choice.get("message")
+            if message is not None:
+                result["content"] = message.get("content")
+        return cls(**result)  # type: ignore[arg-type]
 
 
 @dataclass
-class OpenAiBaseCompletion(ABC):
-    """Abstract base class for OpenAI completion.
+class OpenAiChat:
+    """Tool to interact with OpenAI chat models.
 
-    Args:
-        completion_kwargs: kwargs for the OpenAI completion function
+    This also be constructed with :meth:`~OpenAiChat.from_yaml`.
 
     See Also:
-        * `Create chat completion <https://platform.openai.com/docs/api-reference/chat/create>`_
-        * `Create completion <https://platform.openai.com/docs/api-reference/completions/create>`_
+        OpenAI API reference: `Create chat completion <https://platform.openai.com/docs/api-reference/chat/create>`_
+
+    Args:
+        api_key: The OpenAI API key.
+        model: The OpenAI model name.
     """
 
-    completion_kwargs: Dict[str, Any]
+    api_key: str
+    model: str
+    client: Union[OpenAI, AzureOpenAI] = field(init=False, repr=False)
+    async_client: Union[AsyncOpenAI, AsyncAzureOpenAI] = field(init=False, repr=False)
+
+    def __post_init__(self) -> None:
+        """Do post init."""
+        self.client = OpenAI(api_key=self.api_key)
+        self.async_client = AsyncOpenAI(api_key=self.api_key)
 
     @classmethod
     def from_yaml(cls, yaml_file):
-        """Construct this class from a yaml file."""
-        with open(yaml_file, "r") as file:
-            completion_kwargs = yaml.safe_load(file)
-        return cls(completion_kwargs)
+        """Construct this class from a yaml file.
 
-    @abstractmethod
-    def _completion(
-        self, prompt: Union[str, List[Dict[str, str]]], completion_kwargs_for_this_call: Mapping[str, Any]
-    ) -> OpenAIObject:
-        """Abstract method to call the OpenAI completion."""
-        pass
-
-    def __call__(
-        self, prompt: Union[str, List[Dict[str, str]]], completion_kwargs: Optional[Mapping[str, Any]] = None
-    ) -> OpenAiCompletionAnswer:
-        """Call the OpenAI prompt completion.
+        If the ``api_key`` is not set in the yaml file,
+        it will be loaded from the environment variable ``OPENAI_API_KEY``.
 
         Args:
-            prompt: The prompt to be completed by the LLM.
-                In case of chat models this can be a string or a list.
-                In case of "non chat" models only a string is allowed.
-            completion_kwargs: Overwrite the ``completion_kwargs`` for this call.
-                This allows you, for example, to change the temperature for this call only.
+            yaml_file: The yaml file.
+        Returns:
+            The constructed class.
         """
-        completion_kwargs_for_this_call = self.completion_kwargs.copy()
-        if completion_kwargs is not None:
-            completion_kwargs_for_this_call.update(completion_kwargs)
-        open_ai_object: OpenAIObject = self._completion(prompt, completion_kwargs_for_this_call)
-        open_ai_completion_answer = OpenAiCompletionAnswer.from_open_ai_object(open_ai_object)
-        return open_ai_completion_answer
+        with open(yaml_file, "r") as file:
+            completion_kwargs = yaml.safe_load(file)
 
+        # load api_key from environment variable if it is not set in the yaml file
+        if "api_key" not in completion_kwargs:
+            api_key = os.getenv("OPENAI_API_KEY")
+            if api_key is not None:
+                completion_kwargs["api_key"] = api_key
+
+        return cls(**completion_kwargs)
+
+    def create_completions(
+        self,
+        prompt: Union[str, List[Dict[str, str]]],
+        completion_kwargs: Optional[Dict[str, Any]] = None,
+    ) -> OpenAiChatResult:
+        """Create a model response for the given prompt (chat conversation).
 
-@dataclass
-class OpenAiChatCompletion(OpenAiBaseCompletion):
-    """OpenAI chat completion.
+        Args:
+            prompt: The prompt for the model.
+            completion_kwargs: Keyword arguments for the OpenAI completion.
 
-    This also be constructed with :meth:`OpenAiBaseCompletion.from_yaml`.
+                - ``model`` can not be set via ``completion_kwargs``! Please set the ``model`` in the initializer.
+                - ``messages`` can not be set via ``completion_kwargs``! Please set the ``prompt`` argument.
 
-    Args:
-        completion_kwargs: The kwargs for the OpenAI completion function.
+                Also see:
 
-    See Also:
-        `Create chat completion <https://platform.openai.com/docs/api-reference/chat/create>`_
-    """
+                    - ``openai.resources.chat.completions.Completions.create()``
+                    - OpenAI API reference: `Create chat completion <https://platform.openai.com/docs/api-reference/chat/create>`_
 
-    def _completion(
-        self, prompt: Union[str, List[Dict[str, str]]], completion_kwargs_for_this_call: Mapping[str, Any]
-    ) -> OpenAIObject:
-        """Call to the OpenAI chat completion."""
-        if isinstance(prompt, str):
-            messages = [{"role": "user", "content": prompt}]
+        Returns:
+            The result of the OpenAI completion.
+        """
+        if isinstance(prompt, list):
+            for message in prompt:
+                if "role" not in message or "content" not in message:
+                    raise ValueError(
+                        "If prompt is a list of messages, each message must have a 'role' and 'content' key!"
+                    )
+                if message["role"] not in ["system", "user", "assistant", "tool"]:
+                    raise ValueError(
+                        "If prompt is a list of messages, each message must have a 'role' key with one of the values "
+                        "'system', 'user', 'assistant' or 'tool'!"
+                    )
+
+        if completion_kwargs is not None:
+            # check keys of completion_kwargs
+            if "model" in completion_kwargs:
+                raise ValueError(
+                    "'model' can not be set via 'completion_kwargs'! Please set the 'model' in the initializer."
+                )
+            if "messages" in completion_kwargs:
+                raise ValueError(
+                    "'messages' can not be set via 'completion_kwargs'! Please set the 'prompt' argument."
+                )
         else:
-            messages = prompt
-        open_ai_object: OpenAIObject = ChatCompletion.create(
-            messages=messages,
-            **completion_kwargs_for_this_call,
+            completion_kwargs = {}  # set default value
+        completion_kwargs["model"] = self.model
+        messages = [{"role": "user", "content": prompt}] if isinstance(prompt, str) else prompt
+        chat_completion = self.client.chat.completions.create(
+            messages=messages,  # type: ignore[arg-type]
+            **completion_kwargs,
         )
-        return open_ai_object
-
+        result = OpenAiChatResult.from_chat_completion(chat_completion, completion_kwargs=completion_kwargs)
+        return result
 
-def _check_mandatory_azure_completion_kwargs(completion_kwargs: Mapping[str, Any]) -> None:
-    """Check mandatory Azure ``completion_kwargs``."""
-    for mandatory_azure_completion_kwarg in ("api_base", "engine", "api_type", "api_version"):
-        if mandatory_azure_completion_kwarg not in completion_kwargs:
-            raise ValueError(f"You must set '{mandatory_azure_completion_kwarg}' for Azure completion!")
-    if completion_kwargs["api_type"] != "azure":
-        raise ValueError("You must set 'api_type' to 'azure' for Azure completion!")
-
-
-@dataclass
-class OpenAiAzureChatCompletion(OpenAiChatCompletion):
-    """OpenAI Azure chat completion.
-
-    This also be constructed with :meth:`OpenAiBaseCompletion.from_yaml`.
-
-    Args:
-        completion_kwargs: The kwargs for the OpenAI completion function.
-            The following Azure specific properties must be specified:
-
-                * ``api_type``
-                * ``api_version``
-                * ``api_base``
-                * ``engine``
-
-    See Also:
-        * `Create chat completion <https://platform.openai.com/docs/api-reference/chat/create>`_
-        * `Quickstart: Get started using GPT-35-Turbo and GPT-4 with Azure OpenAI Service <https://learn.microsoft.com/en-us/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line&pivots=programming-language-python>`_
-    """
-
-    def __post_init__(self) -> None:
-        """Do post init."""
-        _check_mandatory_azure_completion_kwargs(self.completion_kwargs)
+    async def create_completions_async(
+        self,
+        prompt: Union[str, List[Dict[str, str]]],
+        completion_kwargs: Optional[Dict[str, Any]] = None,
+    ) -> OpenAiChatResult:
+        """Create a model response for the given prompt (chat conversation).
 
+        Args:
+            prompt: The prompt for the model.
+            completion_kwargs: Keyword arguments for the OpenAI completion.
 
-@dataclass
-class OpenAiCompletion(OpenAiBaseCompletion):
-    """OpenAI (non chat) completion.
+                - ``model`` can not be set via ``completion_kwargs``! Please set the ``model`` in the initializer.
+                - ``messages`` can not be set via ``completion_kwargs``! Please set the ``prompt`` argument.
 
-    This also be constructed with :meth:`OpenAiBaseCompletion.from_yaml`.
+                Also see:
 
-    Args:
-        completion_kwargs: The kwargs for the OpenAI completion function.
+                    - ``openai.resources.chat.completions.Completions.create()``
+                    - OpenAI API reference: `Create chat completion <https://platform.openai.com/docs/api-reference/chat/create>`_
 
-    See Also:
-        `Create completion <https://platform.openai.com/docs/api-reference/completions/create>`_
-    """
+        Returns:
+            The result of the OpenAI completion.
+        """
+        if isinstance(prompt, list):
+            for message in prompt:
+                if "role" not in message or "content" not in message:
+                    raise ValueError(
+                        "If prompt is a list of messages, each message must have a 'role' and 'content' key!"
+                    )
+                if message["role"] not in ["system", "user", "assistant", "tool"]:
+                    raise ValueError(
+                        "If prompt is a list of messages, each message must have a 'role' key with one of the values "
+                        "'system', 'user', 'assistant' or 'tool'!"
+                    )
 
-    def _completion(
-        self, prompt: Union[str, List[Dict[str, str]]], completion_kwargs_for_this_call: Mapping[str, Any]
-    ) -> OpenAIObject:
-        """Call to the OpenAI (not chat) completion."""
-        open_ai_object: OpenAIObject = Completion.create(
-            prompt=prompt,
-            **completion_kwargs_for_this_call,
+        if completion_kwargs is not None:
+            # check keys of completion_kwargs
+            if "model" in completion_kwargs:
+                raise ValueError(
+                    "'model' can not be set via 'completion_kwargs'! Please set the 'model' in the initializer."
+                )
+            if "messages" in completion_kwargs:
+                raise ValueError(
+                    "'messages' can not be set via 'completion_kwargs'! Please set the 'prompt' argument."
+                )
+        else:
+            completion_kwargs = {}  # set default value
+        completion_kwargs["model"] = self.model
+        messages = [{"role": "user", "content": prompt}] if isinstance(prompt, str) else prompt
+        chat_completion = await self.async_client.chat.completions.create(
+            messages=messages,  # type: ignore[arg-type]
+            **completion_kwargs,
         )
-        return open_ai_object
+        result = OpenAiChatResult.from_chat_completion(chat_completion, completion_kwargs=completion_kwargs)
+        return result
 
 
 @dataclass
-class OpenAiAzureCompletion(OpenAiCompletion):
-    """OpenAI Azure (non chat) completion.
+class OpenAiAzureChat(OpenAiChat):
+    """Tool to interact with Azure OpenAI chat models.
 
-    This also be constructed with :meth:`OpenAiBaseCompletion.from_yaml`.
-
-    Args:
-        completion_kwargs: The kwargs for the OpenAI completion function.
-            The following Azure specific properties must be specified:
-
-                * ``api_type``
-                * ``api_version``
-                * ``api_base``
-                * ``engine``
+    This can also be constructed with :meth:`~OpenAiChat.from_yaml`.
 
     See Also:
-        * `Create completion <https://platform.openai.com/docs/api-reference/completions/create>`_
+        * OpenAI API reference: `Create chat completion <https://platform.openai.com/docs/api-reference/chat/create>`_
         * `Quickstart: Get started generating text using Azure OpenAI Service <https://learn.microsoft.com/en-us/azure/ai-services/openai/quickstart?tabs=command-line&pivots=programming-language-python>`_
+
+    Args:
+        api_key: The OpenAI API key.
+        model: The OpenAI model name.
+        api_version: The OpenAI API version.
+            A common value for this is ``2023-05-15``.
+        azure_endpoint: The Azure endpoint.
     """
 
+    api_version: str
+    azure_endpoint: str
+
     def __post_init__(self) -> None:
         """Do post init."""
-        _check_mandatory_azure_completion_kwargs(self.completion_kwargs)
+        self.client = AzureOpenAI(
+            api_key=self.api_key,
+            api_version=self.api_version,
+            azure_endpoint=self.azure_endpoint,
+        )
+        self.async_client = AsyncAzureOpenAI(
+            api_key=self.api_key,
+            api_version=self.api_version,
+            azure_endpoint=self.azure_endpoint,
+        )
```

### Comparing `mltb2-0.9.1rc1/mltb2/optuna.py` & `mltb2-1.0.0/mltb2/optuna.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright (c) 2021 Philip May
+# Copyright (c) 2021-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """This module offers tools for `Optuna <https://optuna.readthedocs.io/en/stable/>`_.
 
 Hint:
     Use pip to install the necessary dependencies for this module:
     ``pip install mltb2[optuna]``
 """
 
 
+import contextlib
 import logging
 
 import numpy as np
 import optuna
 from optuna.pruners import BasePruner
 from optuna.study import StudyDirection
 from scipy import stats
@@ -110,30 +111,28 @@
         n_warmup_steps: Pruning is disabled until the trial reaches or exceeds the given number
             of steps.
     """
 
     def __init__(self, alpha: float = 0.1, n_warmup_steps: int = 4) -> None:
         # input value check
         if n_warmup_steps < 0:
-            raise ValueError("'n_warmup_steps' must not be negative! n_warmup_steps: {}".format(n_warmup_steps))
+            raise ValueError(f"'n_warmup_steps' must not be negative! n_warmup_steps: {n_warmup_steps}")
         if alpha >= 1:
-            raise ValueError("'alpha' must be smaller than 1! {}".format(alpha))
+            raise ValueError(f"'alpha' must be smaller than 1! {alpha}")
         if alpha <= 0:
-            raise ValueError("'alpha' must be greater than 0! {}".format(alpha))
+            raise ValueError(f"'alpha' must be greater than 0! {alpha}")
 
         self.n_warmup_steps = n_warmup_steps
         self.alpha = alpha
 
     def prune(self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial) -> bool:  # noqa: D102
         # get best tial - best trial is not available for first trial
         best_trial = None
-        try:
+        with contextlib.suppress(ValueError):
             best_trial = study.best_trial
-        except ValueError:
-            pass
 
         if best_trial is not None:
             trial_intermediate_values = list(trial.intermediate_values.values())
 
             _logger.debug("trial_intermediate_values: %s", trial_intermediate_values)
 
             # wait until the trial reaches or exceeds n_warmup_steps number of steps
```

### Comparing `mltb2-0.9.1rc1/mltb2/plot.py` & `mltb2-1.0.0/mltb2/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018 Philip May
+# Copyright (c) 2018-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """Plot tools module.
 
 This module is based on `Matplotlib <https://matplotlib.org/>`_.
 
@@ -112,22 +112,16 @@
     if xlabel is not None:
         ax.set(xlabel=xlabel)
 
     if ylabel is not None:
         ax.set(ylabel=ylabel)
 
     ax.boxplot(values, labels=labels, vert=vert)
-
-    if vert:
-        grid_axis = "y"
-    else:
-        grid_axis = "x"
-
+    grid_axis = "y" if vert else "x"
     plt.grid(b=True, axis=grid_axis, linestyle="--")
-
     plt.xticks(rotation=90)
 
 
 def boxplot_dict(
     values_dict,
     title: Optional[str] = None,
     xlabel: Optional[str] = None,
```

### Comparing `mltb2-0.9.1rc1/mltb2/somajo.py` & `mltb2-1.0.0/mltb2/somajo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright (c) 2023 Philip May
+# Copyright (c) 2023-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """This module offers `SoMaJo <https://github.com/tsproisl/SoMaJo>`_ specific tools.
 
 Hint:
     Use pip to install the necessary dependencies for this module:
     ``pip install mltb2[somajo]``
 """
 
 
 from abc import ABC
 from dataclasses import dataclass, field
-from typing import Container, Dict, Iterable, List, Literal, Optional, Set, Tuple, Union
+from typing import Dict, Iterable, List, Literal, Optional, Set, Tuple, Union
 
 from somajo import SoMaJo
 from tqdm import tqdm
 
 
 @dataclass
 class SoMaJoBaseClass(ABC):
@@ -58,29 +58,27 @@
         if token.space_after:
             result_list.append(" ")
     result = "".join(result_list)
     result = result.strip()
     return result
 
 
-def extract_token_class_set(sentences: Iterable, keep_token_classes: Optional[Container[str]] = None) -> Set[str]:
+def extract_token_class_set(sentences: Iterable, keep_token_classes: Optional[str] = None) -> Set[str]:
     """Extract token from sentences by token class.
 
     Args:
         sentences: The sentences from which to extract.
         keep_token_classes: The token classes to keep. If ``None`` all will be kept.
     Returns:
         The set of extracted token texts.
     """
     result = set()
     for sentence in sentences:
         for token in sentence:
-            if keep_token_classes is None:
-                result.add(token.text)
-            elif token.token_class in keep_token_classes:
+            if keep_token_classes is None or token.token_class in keep_token_classes:
                 result.add(token.text)
             # else ignore
     return result
 
 
 @dataclass
 class SoMaJoSentenceSplitter(SoMaJoBaseClass):
@@ -185,14 +183,29 @@
         """
         if isinstance(text, str):
             text = [text]
         sentences = self.somajo.tokenize_text(text)
         result = extract_token_class_set(sentences, keep_token_classes="URL")
         return result
 
+    def extract_token_set(self, text: Union[Iterable, str], keep_token_classes: Optional[str] = None) -> Set[str]:
+        """Extract tokens from text.
+
+        Args:
+            text: the text
+            keep_token_classes: The token classes to keep. If ``None`` all will be kept.
+        Returns:
+            Set of tokens.
+        """
+        if isinstance(text, str):
+            text = [text]
+        sentences = self.somajo.tokenize_text(text)
+        result = extract_token_class_set(sentences, keep_token_classes=keep_token_classes)
+        return result
+
 
 @dataclass
 class UrlSwapper:
     """Tool to swap (and reverse swap) links with a numbered replacement link.
 
     Args:
         token_extractor: The sentence token extractor to be used.
```

### Comparing `mltb2-0.9.1rc1/mltb2/somajo_transformers.py` & `mltb2-1.0.0/mltb2/somajo_transformers.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,20 +53,20 @@
             text: The text to be split.
         Returns:
             The list of section splits.
         """
         sentences = self.somajo_sentence_splitter(text)
         counts = self.transformers_token_counter(sentences)
 
-        assert len(sentences) == len(counts)  # type: ignore  # noqa: S101
+        assert len(sentences) == len(counts)  # type: ignore[arg-type]
 
         result_splits: List[str] = []
         current_sentences: List[str] = []
         current_count: int = 0
-        for sentence, count in zip(tqdm(sentences, disable=not self.show_progress_bar), counts):  # type: ignore
+        for sentence, count in zip(tqdm(sentences, disable=not self.show_progress_bar), counts):  # type: ignore[arg-type]
             if count > self.max_token:
                 if self.ignore_overly_long_sentences:
                     continue
                 else:
                     raise ValueError("No sentence may be longer than 'max_token'.")
             if current_count + count <= self.max_token:
                 current_count += count
```

### Comparing `mltb2-0.9.1rc1/mltb2/text.py` & `mltb2-1.0.0/mltb2/text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Philip May
+# Copyright (c) 2023-2024 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """This module offers text specific tools.
 
 It offers the following functionality:
 
@@ -50,14 +50,37 @@
 
 SPECIAL_WHITESPACES_TRANS: Final[Dict[int, str]] = str.maketrans({char: " " for char in SPECIAL_WHITESPACES})
 
 INVISIBLE_CHARACTERS_AND_SPECIAL_WHITESPACES_TRANS = {**SPECIAL_WHITESPACES_TRANS, **INVISIBLE_CHARACTERS_TRANS}
 
 MULTI_SPACE_PATTERN: Pattern = re.compile(r" {2,}")
 
+XML_TAG_PATTERN: Pattern = re.compile(r"<\/?[\w:]+( \/|\/|)>")
+
+
+def has_xml_tag(text: str) -> bool:
+    """Check if text contains XML tags (one or multiple).
+
+    These are some XML tags we detect:
+
+    - ``<xml_tag>``
+    - ``<xml:tag>``
+    - ``</xml_tag>``
+    - ``<xml_tag/>``
+    - ``<xml_tag />``
+
+    While we do not detect ``a < b but x > y``.
+
+    Args:
+        text: The text to check.
+    Returns:
+        ``True`` if the text contains XML tags, ``False`` otherwise.
+    """
+    return re.search(XML_TAG_PATTERN, text) is not None
+
 
 def remove_invisible_characters(text: str) -> str:
     """Remove invisible characters from text.
 
     The invisible characters are defined in the constant ``INVISIBLE_CHARACTERS``.
 
     Args:
@@ -142,14 +165,35 @@
     """
     text = text.translate(INVISIBLE_CHARACTERS_AND_SPECIAL_WHITESPACES_TRANS)
     text = replace_multiple_whitespaces(text)
     text = text.strip()
     return text
 
 
+def clean_all_invisible_chars_and_strip(text: str) -> str:
+    """Clean text form invisible characters and strip the text.
+
+    - Remove invisible characters from text.
+    - Replace special whitespaces with normal whitespaces.
+    - Remove leading and trailing whitespaces.
+
+    The invisible characters are defined in the constant ``INVISIBLE_CHARACTERS``.
+    The special whitespaces are defined in the constant ``SPECIAL_WHITESPACES``.
+
+    Args:
+        text: The text to clean.
+
+    Rteturns:
+        The cleaned text.
+    """
+    text = text.translate(INVISIBLE_CHARACTERS_AND_SPECIAL_WHITESPACES_TRANS)
+    text = text.strip()
+    return text
+
+
 def _normalize_counter_to_defaultdict(counter: Counter, max_dimensions: int) -> defaultdict:
     """Normalize a counter to to ``max_dimensions``.
 
     The number of dimensions is limited to ``max_dimensions``
     of the most commen characters.
     The counter values are normalized by deviding them by the total count.
 
@@ -221,28 +265,28 @@
             ValueError: If :func:`~TextDistance.fit` is called after
                 :func:`~TextDistance.distance`.
         """
         if self._distance_called:
             raise ValueError("fit must not be called after distance calculation!")
 
         if isinstance(text, str):
-            self._char_counter.update(text)  # type: ignore
+            self._char_counter.update(text)  # type: ignore[union-attr]
         else:
             for t in tqdm(text, disable=not self.show_progress_bar):
-                self._char_counter.update(t)  # type: ignore
+                self._char_counter.update(t)  # type: ignore[union-attr]
 
         self._fit_called = True
 
     def _normalize_char_counter(self) -> None:
         """Normalize the char counter to a defaultdict.
 
         This supports lazy postprocessing of the char counter.
         """
         if not self._distance_called:
-            self._normalized_char_counts = _normalize_counter_to_defaultdict(self._char_counter, self.max_dimensions)  # type: ignore
+            self._normalized_char_counts = _normalize_counter_to_defaultdict(self._char_counter, self.max_dimensions)  # type: ignore[arg-type]
             self._char_counter = None
             self._counted_char_set = set(self._normalized_char_counts)
             self._distance_called = True
 
     def distance(self, text) -> float:
         """Calculate the distance between the fitted text and the given text.
 
@@ -256,13 +300,13 @@
         if not self._fit_called:
             raise ValueError("fit must not be called before distance!")
         self._normalize_char_counter()
         all_vector = []
         text_vector = []
         text_count = Counter(text)
         text_count_defaultdict = _normalize_counter_to_defaultdict(text_count, self.max_dimensions)
-        for c in self._counted_char_set.union(text_count_defaultdict):  # type: ignore
+        for c in self._counted_char_set.union(text_count_defaultdict):  # type: ignore[union-attr]
             all_vector.append(
-                self._normalized_char_counts[c]  # type: ignore
+                self._normalized_char_counts[c]  # type: ignore[index]
             )  # if c is not in defaultdict, it will return 0
             text_vector.append(text_count_defaultdict[c])  # if c is not in defaultdict, it will return 0
         return cityblock(all_vector, text_vector)
```

### Comparing `mltb2-0.9.1rc1/mltb2/transformers.py` & `mltb2-1.0.0/mltb2/transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.9.1rc1/pyproject.toml` & `mltb2-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mltb2"
-version = "0.9.1rc1"
+version = "1.0.0"
 description = "Machine Learning Toolbox 2"
 authors = ["PhilipMay <philip@may.la>"]
 readme = "README.md"
 homepage = "https://github.com/telekom/mltb2"
 documentation = "https://telekom.github.io/mltb2/"
 include = ["LICENSE", "CONTRIBUTING.md", "Makefile"]
 keywords = [
@@ -60,106 +60,126 @@
 scipy = "*"
 tqdm = "*"
 platformdirs = {version = "*", optional = true}
 scikit-learn = {version = "*", optional = true}
 fasttext-wheel = {version = "*", optional = true}
 optuna = {version = "*", optional = true}
 matplotlib = {version = "*", optional = true}
-SoMaJo = {version = ">=2.3.1", optional = true}
-torch = {version = "!=2.0.1,!=2.1.0", optional = true}  # some versions have poetry issues
+SoMaJo = {version = ">=2.4.1", optional = true}
+
+# some versions have poetry issues
+# 2.3.0 does not work with Intel Mac
+torch = {version = "!=2.0.1,!=2.1.0,!=2.3.0", optional = true}
+
 transformers = {version = "*", optional = true}
 tiktoken = {version = "*", optional = true}
 safetensors = {version = "!=0.3.2", optional = true}  # version 0.3.2 has poetry issues
-openai = {version = "^0", optional = true}
+openai = {version = "^1", optional = true}
 pyyaml = {version = "*", optional = true}
 pandas = {version = "*", optional = true}
 beautifulsoup4 = {version = "*", optional = true}
 joblib = {version = "*", optional = true}
 python-dotenv = {version = "*", optional = true}
 python-arango = {version = "*", optional = true}
 jsonlines = {version = "*", optional = true}
+markdownify = {version = "*", optional = true}
+mdformat = {version = "*", optional = true}
 
 [tool.poetry.extras]
-files = ["platformdirs", "scikit-learn"]
+files = ["platformdirs", "scikit-learn", "joblib"]
 fasttext = ["fasttext-wheel", "platformdirs", "scikit-learn"]
 data = ["platformdirs", "scikit-learn", "pandas", "beautifulsoup4", "joblib"]
 optuna = ["optuna"]
 plot = ["matplotlib"]
 somajo = ["SoMaJo"]
 transformers = ["scikit-learn", "torch", "transformers", "safetensors"]
 md = ["scikit-learn", "torch", "transformers", "safetensors"]
 somajo_transformers = ["SoMaJo", "scikit-learn", "torch", "transformers", "safetensors"]
 openai = ["tiktoken", "openai", "pyyaml"]
 arangodb = ["python-dotenv", "python-arango", "jsonlines"]
+bs = ["beautifulsoup4", "markdownify", "mdformat"]
 
 [tool.poetry.group.lint.dependencies]
 black = "*"
 ruff = "*"
 mypy = "*"
-mdformat = "*"
+mdformat-gfm = "*"
+mdformat-frontmatter = "*"
+mdformat-footnote = "*"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
+pytest-rerunfailures = "*"
+pytest-random-order = "*"
+hypothesis = "*"
 
 [tool.poetry.group.doc.dependencies]
 sphinx = "*"
 sphinx_rtd_theme = "*"
 sphinx_copybutton = "*"
 
+[tool.pytest.ini_options]
+addopts = "--random-order-bucket=global"
+
 [tool.black]
 line-length = 119
 target-version = ["py38", "py39", "py310", "py311"]
 
 [tool.ruff]
-select = [
-  "E",  # pycodestyle - https://beta.ruff.rs/docs/rules/#pycodestyle-e-w
-  "F",  # pyflakes - https://beta.ruff.rs/docs/rules/#pyflakes-f
-  "I",  # isort - https://beta.ruff.rs/docs/rules/#isort-i
-  "D",  # pydocstyle - https://beta.ruff.rs/docs/rules/#pydocstyle-d
-  "PL",  # Pylint - https://beta.ruff.rs/docs/rules/#pylint-pl
-  "YTT",  # flake8-2020 - https://beta.ruff.rs/docs/rules/#flake8-2020-ytt
-  # "ANN",
-  "ASYNC",  # flake8-async - https://beta.ruff.rs/docs/rules/#flake8-async-async
-  "S",  # flake8-bandit - https://beta.ruff.rs/docs/rules/#flake8-bandit-s
-  "BLE",  # flake8-blind-except - https://beta.ruff.rs/docs/rules/#flake8-blind-except-ble
-  # "FBT",
-  "B",  # flake8-bugbear - https://beta.ruff.rs/docs/rules/#flake8-bugbear-b
-  "A",  # flake8-builtins - https://beta.ruff.rs/docs/rules/#flake8-builtins-a
-  "COM",  # flake8-commas - https://beta.ruff.rs/docs/rules/#flake8-commas-com
-  "CPY001",  # flake8-copyright - https://beta.ruff.rs/docs/rules/#flake8-copyright-cpy
-  "C4",  # flake8-comprehensions - https://beta.ruff.rs/docs/rules/#flake8-comprehensions-c4
-  "DTZ",  # flake8-datetimez - https://beta.ruff.rs/docs/rules/#flake8-datetimez-dtz
-  "T10",  # flake8-debugger - https://beta.ruff.rs/docs/rules/#flake8-debugger-t10
-  # "EM",
-  "EXE",  # flake8-executable - https://beta.ruff.rs/docs/rules/#flake8-executable-exe
-]
 line-length = 119
-fixable = ["I"]
 target-version = "py38"
+
+
+[tool.ruff.lint]
+select = ["ALL"]
+fixable = ["I"]
 ignore = [
+  "DJ",  # flake8-django - https://docs.astral.sh/ruff/rules/#flake8-django-dj
+  "ERA",  # eradicate - https://docs.astral.sh/ruff/rules/#eradicate-era
+  "ANN",  # flake8-annotations - https://docs.astral.sh/ruff/rules/#flake8-annotations-ann
+  "FA",  # flake8-future-annotations - https://docs.astral.sh/ruff/rules/#flake8-future-annotations-fa
+  "EM",  # flake8-errmsg - https://docs.astral.sh/ruff/rules/#flake8-errmsg-em
+  "PTH",  # flake8-use-pathlib - https://docs.astral.sh/ruff/rules/#flake8-use-pathlib-pth
+  "FBT",  # flake8-boolean-trap - https://docs.astral.sh/ruff/rules/#flake8-boolean-trap-fbt
+  "TD", # flake8-todos - https://docs.astral.sh/ruff/rules/#flake8-todos-td
+  "SLF",  # flake8-self - https://docs.astral.sh/ruff/rules/#flake8-self-slf
   "D107",  # Missing docstring in __init__
   "D410",  # Missing blank line after section ("{name}")
   "D411",  # Missing blank line before section ("{name}")
   "PLR0913",  # Too many arguments to function call ({c_args} > {max_args})
   "S106",  # Possible hardcoded password assigned to argument: "{}"
   "COM812",  # Trailing comma missing
   "S101",  # Use of `assert` detected
   "PLR2004",  # Magic value used in comparison
   "B011",  # Do not `assert False`
+  "RET505",  # Unnecessary `else` after `return` statement
+  "TRY003",  # Avoid specifying long messages outside the exception class
+  "RET504",  # Unnecessary assignment before `return` statement
+  "T201",  # `print` found
+  "RET507",  # Unnecessary `else` after `continue` statement
+  "PT015",  # Assertion always fails, replace with `pytest.fail()`
+  "UP015",  # Unnecessary open mode parameters
+  "FIX002",  # Line contains TODO, consider resolving the issue
+  "PT011",  # `pytest.raises(ValueError)` is too broad, set the `match` parameter or use a more specific exception
+  "PT001",  # Use `@pytest.fixture()` over `@pytest.fixture`
+  "RUF015",  # Prefer `next(iter(sentences))` over single element slice
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**/test_*.py" = [
   "D100",  # Missing docstring in public module
   "D103",  # Missing docstring in public function
   "PLR2004",  # Magic value used in comparison, consider replacing {value} with a constant variable
   "S101",  # Use of assert detected
+  "N802",  # Function name should be lowercase
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.flake8-copyright]
-notice-rgx = "(# Copyright \\(c\\) \\d{4} .*\\n)+# This software is distributed under the terms of the MIT license\\n# which is available at https://opensource.org/licenses/MIT\\n\\n"
+[tool.ruff.lint.flake8-copyright]
+notice-rgx = "(# Copyright \\(c\\) \\d{4}.*\\n)+# This software is distributed under the terms of the MIT license\\n# which is available at https://opensource.org/licenses/MIT\\n\\n"
 
 [tool.mypy]
 ignore_missing_imports = true
+warn_unused_ignores = true
+enable_error_code=["ignore-without-code"]
```

### Comparing `mltb2-0.9.1rc1/PKG-INFO` & `mltb2-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.9.1rc1
+Version: 1.0.0
 Summary: Machine Learning Toolbox 2
 Home-page: https://github.com/telekom/mltb2
 Keywords: optuna,deep learning,ml,ai,machine learning,hyperparameter optimization,hyperparameter tuning,nlp,natural language processing,transformers,llm,large-language-models,openai,plot
 Author: PhilipMay
 Author-email: philip@may.la
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,43 +21,46 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: arangodb
+Provides-Extra: bs
 Provides-Extra: data
 Provides-Extra: fasttext
 Provides-Extra: files
 Provides-Extra: md
 Provides-Extra: openai
 Provides-Extra: optuna
 Provides-Extra: plot
 Provides-Extra: somajo
 Provides-Extra: somajo-transformers
 Provides-Extra: transformers
-Requires-Dist: SoMaJo (>=2.3.1) ; extra == "somajo" or extra == "somajo-transformers"
-Requires-Dist: beautifulsoup4 ; extra == "data"
+Requires-Dist: SoMaJo (>=2.4.1) ; extra == "somajo" or extra == "somajo-transformers"
+Requires-Dist: beautifulsoup4 ; extra == "data" or extra == "bs"
 Requires-Dist: fasttext-wheel ; extra == "fasttext"
-Requires-Dist: joblib ; extra == "data"
+Requires-Dist: joblib ; extra == "files" or extra == "data"
 Requires-Dist: jsonlines ; extra == "arangodb"
+Requires-Dist: markdownify ; extra == "bs"
 Requires-Dist: matplotlib ; extra == "plot"
+Requires-Dist: mdformat ; extra == "bs"
 Requires-Dist: numpy
-Requires-Dist: openai (>=0,<1) ; extra == "openai"
+Requires-Dist: openai (>=1,<2) ; extra == "openai"
 Requires-Dist: optuna ; extra == "optuna"
 Requires-Dist: pandas ; extra == "data"
 Requires-Dist: platformdirs ; extra == "files" or extra == "fasttext" or extra == "data"
 Requires-Dist: python-arango ; extra == "arangodb"
 Requires-Dist: python-dotenv ; extra == "arangodb"
 Requires-Dist: pyyaml ; extra == "openai"
 Requires-Dist: safetensors (!=0.3.2) ; extra == "transformers" or extra == "md" or extra == "somajo-transformers"
 Requires-Dist: scikit-learn ; extra == "files" or extra == "fasttext" or extra == "data" or extra == "transformers" or extra == "md" or extra == "somajo-transformers"
 Requires-Dist: scipy
 Requires-Dist: tiktoken ; extra == "openai"
-Requires-Dist: torch (!=2.0.1,!=2.1.0) ; extra == "transformers" or extra == "md" or extra == "somajo-transformers"
+Requires-Dist: torch (!=2.0.1,!=2.1.0,!=2.3.0) ; extra == "transformers" or extra == "md" or extra == "somajo-transformers"
 Requires-Dist: tqdm
 Requires-Dist: transformers ; extra == "transformers" or extra == "md" or extra == "somajo-transformers"
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
 Description-Content-Type: text/markdown
 
 # Machine Learning Toolbox 2 - MLTB2
@@ -68,39 +71,35 @@
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://github.com/telekom/mltb2/blob/main/pyproject.toml)
 <br/>
 [![pytest](https://github.com/telekom/mltb2/actions/workflows/pytest.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/pytest.yml)
 [![Static Code Checks](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml)
 [![Build & Deploy Doc](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml)
 [![GitHub issues](https://img.shields.io/github/issues-raw/telekom/mltb2)](https://github.com/telekom/mltb2/issues)
 
-📦 A box of machine learning tools. 📦
+📦 A box full of machine learning tools. 📦
 
 - [Documentation Page](https://telekom.github.io/mltb2/)
 - [How to contribute](https://github.com/telekom/mltb2/blob/main/CONTRIBUTING.md)
 
 ## Installation
 
 MLTB2 is available at [the Python Package Index (PyPI)](https://pypi.org/project/mltb2/).
 It can be installed with pip:
 
 ```bash
 pip install mltb2
 ```
 
-Some optional dependencies might be necessary. You can install all of them with:
-
-```bash
-pip install mltb2[files,fasttext,optuna,plot,somajo,transformers,somajo_transformers,openai]
-```
-
-If you don't want to install all dependencies, see
+For many modules optional dependencies are necessary.
+Those optional dependencies must be installed when you want to use the module.
+To install those module specific dependencies see
 [the description of the individual modules](https://telekom.github.io/mltb2/api-reference.html).
 
 ## Licensing
 
-Copyright (c) 2023 Philip May\
-Copyright (c) 2023 Philip May, Deutsche Telekom AG
+Copyright (c) 2023-2024 [Philip May](https://philipmay.org)\
+Copyright (c) 2023-2024 [Philip May](https://philipmay.org), [Deutsche Telekom AG](https://www.telekom.de/)
 
 Licensed under the **MIT License** (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License by reviewing the file
 [LICENSE](https://github.com/telekom/mltb2/blob/main/LICENSE) in the repository.
```

