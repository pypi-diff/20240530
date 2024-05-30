# Comparing `tmp/geneweaver_db-0.5.0a0.tar.gz` & `tmp/geneweaver_db-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.5.0a0.tar", max compression
+gzip compressed data, was "geneweaver_db-0.5.0a1.tar", max compression
```

## Comparing `geneweaver_db-0.5.0a0.tar` & `geneweaver_db-0.5.0a1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-05-29 14:33:54.663021 geneweaver_db-0.5.0a0/LICENSE
--rw-r--r--   0        0        0     2162 2024-05-29 14:33:54.663021 geneweaver_db-0.5.0a0/README.md
--rw-r--r--   0        0        0      955 2024-05-29 14:33:54.663021 geneweaver_db-0.5.0a0/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0      132 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     5163 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/geneset.py
--rw-r--r--   0        0        0     4062 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1310 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0      809 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/threshold.py
--rw-r--r--   0        0        0       56 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      845 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/cursor.py
--rw-r--r--   0        0        0      145 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1769 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      438 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10316 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8981 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7887 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     3913 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     5410 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0      364 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/__init__.py
--rw-r--r--   0        0        0     1351 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/const.py
--rw-r--r--   0        0        0     5492 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/read.py
--rw-r--r--   0        0        0     4824 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/utils.py
--rw-r--r--   0        0        0     4014 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/write.py
--rw-r--r--   0        0        0      982 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/project.py
--rw-r--r--   0        0        0     6984 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0       60 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/__init__.py
--rw-r--r--   0        0        0       50 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/search.py
--rw-r--r--   0        0        0     1572 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/utils.py
--rw-r--r--   0        0        0     1603 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     2900 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/threshold.py
--rw-r--r--   0        0        0     1782 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/utils.py
--rw-r--r--   0        0        0     1249 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/species.py
--rw-r--r--   0        0        0      775 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/threshold.py
--rw-r--r--   0        0        0     6887 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3201 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.5.0a0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/LICENSE
+-rw-r--r--   0        0        0     2162 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/README.md
+-rw-r--r--   0        0        0      957 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     9259 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     4062 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      809 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0    12901 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     3913 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     5410 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      407 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     5492 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     5543 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     5058 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     6984 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1572 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     2900 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1782 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      775 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3201 2024-05-29 20:48:27.816048 geneweaver_db-0.5.0a1/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 geneweaver_db-0.5.0a1/PKG-INFO
```

### Comparing `geneweaver_db-0.5.0a0/LICENSE` & `geneweaver_db-0.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/README.md` & `geneweaver_db-0.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/pyproject.toml` & `geneweaver_db-0.5.0a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.5.0a0"
+version = "0.5.0a1"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
     { include = "geneweaver/db", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-geneweaver-core = ">=0.9.1,<1.0.0"
-psycopg = {extras = ["binary"], version = "^3.1.13"}
+geneweaver-core = ">=0.10.0a0,<1.0.0"
+psycopg = {version = "3.1.18", extras = ["binary"]}
 
 [tool.poetry.group.dev.dependencies]
 geneweaver-testing = ">=0.1.2,<1.0.0"
 pytest-asyncio = "^0.23.5"
 
 [tool.ruff]
 select = ['F', 'E', 'W', 'A', 'C90', 'N', 'B', 'ANN', 'D', 'I', 'ERA', 'PD', 'NPY', 'PT']
```

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/aio/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/geneset.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/read.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,149 +1,148 @@
-"""Async database interaction code relating to Genesets."""
+"""SQL query generation code for reading genesets."""
 
-from typing import List, Optional
+from typing import Optional, Tuple
 
 from geneweaver.core.enum import GeneIdentifier, ScoreType, Species
-from geneweaver.db.query import geneset as geneset_query
-from geneweaver.db.utils import GenesetTierOrTiers
-from psycopg import AsyncCursor
-from psycopg.rows import Row
+from geneweaver.db.query.geneset.utils import (
+    add_ontology_parameter,
+    add_ontology_query,
+    format_select_query,
+    is_readable,
+    restrict_tier,
+    search,
+)
+from geneweaver.db.query.utils import construct_filters
+from geneweaver.db.utils import GenesetTierOrTiers, limit_and_offset
+from psycopg.sql import SQL, Composed
 
 
-async def get(
-    cursor: AsyncCursor,
+def get(
     gs_id: Optional[int] = None,
     owner_id: Optional[int] = None,
     curation_tier: Optional[GenesetTierOrTiers] = None,
     species: Optional[Species] = None,
     name: Optional[str] = None,
     abbreviation: Optional[str] = None,
     publication_id: Optional[int] = None,
     pubmed_id: Optional[int] = None,
     gene_id_type: Optional[GeneIdentifier] = None,
     search_text: Optional[str] = None,
+    status: Optional[str] = "normal",
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
     ontology_term: Optional[str] = None,
     score_type: Optional[ScoreType] = None,
-) -> List[Row]:
-    """Get genesets from the database.
+) -> Tuple[Composed, dict]:
+    """Get genesets.
 
-    :param cursor: An async database cursor.
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
     :param curation_tier: Show only results of this curation tier.
     :param species: Show only results associated with this species.
     :param name: Show only results with this name.
     :param abbreviation: Show only results with this abbreviation.
     :param publication_id: Show only results with this publication ID (internal).
     :param pubmed_id: Show only results with this PubMed ID.
     :param gene_id_type: Show only results with this gene ID type.
     :param search_text: Return genesets that match this search text (using PostgreSQL
                         full-text search).
+    :param status: Show only results with this status. Default is "normal".
     :param limit: Limit the number of results.
     :param offset: Offset the results.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
     :param ontology_term: Show only results associated with this ontology term.
     :param score_type: Show only results with given score type.
-
-    :return: list of results using `.fetchall()`
     """
-    await cursor.execute(
-        *geneset_query.get(
-            is_readable_by=is_readable_by,
-            gs_id=gs_id,
-            owner_id=owner_id,
-            curation_tier=curation_tier,
-            species=species,
-            name=name,
-            abbreviation=abbreviation,
-            publication_id=publication_id,
-            pubmed_id=pubmed_id,
-            gene_id_type=gene_id_type,
-            search_text=search_text,
-            limit=limit,
-            offset=offset,
-            with_publication_info=with_publication_info,
+    params = {}
+    filtering = []
+    query = format_select_query(
+        with_publication_info=with_publication_info,
+        with_publication_join=pubmed_id is not None,
+    )
+
+    # expand query to include ontology term if needed
+    if ontology_term:
+        query = add_ontology_query(query=query)
+        filtering, params = add_ontology_parameter(
+            existing_filters=filtering,
+            existing_params=params,
             ontology_term=ontology_term,
-            score_type=score_type,
         )
-    )
 
-    return await cursor.fetchall()
+    filtering, params = is_readable(filtering, params, is_readable_by)
+    filtering, params = search(filtering, params, search_text)
+    filtering, params = restrict_tier(filtering, params, curation_tier)
+
+    filtering, params = construct_filters(
+        filtering,
+        params,
+        {
+            "gs_id": gs_id,
+            "usr_id": owner_id,
+            "sp_id": int(species) if species is not None else None,
+            "gs_name": name,
+            "gs_abbreviation": abbreviation,
+            "pub_id": publication_id,
+            "pub_pubmed": str(pubmed_id) if pubmed_id is not None else None,
+            "gs_gene_id_type": int(gene_id_type) if gene_id_type is not None else None,
+            "gs_status": status,
+            "gs_threshold_type": int(score_type) if score_type is not None else None,
+        },
+    )
 
+    if len(filtering) > 0:
+        query += SQL("WHERE") + SQL("AND").join(filtering)
 
-async def by_id(
-    cursor: AsyncCursor,
-    gs_id: int,
-    is_readable_by: Optional[int] = None,
-    with_publication_info: bool = True,
-) -> Optional[Row]:
-    """Get a geneset by its ID.
-
-    :param cursor: An async database cursor.
-    :param gs_id: The geneset ID to search for.
-    :param is_readable_by: A user ID to check if the user can read the results.
-    :param with_publication_info: Include publication info in the return.
-    """
-    await cursor.execute(
-        *geneset_query.get(
-            gs_id=gs_id,
-            is_readable_by=is_readable_by,
-            with_publication_info=with_publication_info,
-        )
-    )
+    query = limit_and_offset(query, limit, offset).join(" ")
 
-    return await cursor.fetchone()
+    return query, params
 
 
-async def by_owner_id(
-    cursor: AsyncCursor,
-    owner_id: int,
-    is_readable_by: Optional[int] = None,
+def shared_with_user(
+    user_id: int,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     with_publication_info: bool = True,
-) -> List[Row]:
-    """Get genesets by owner ID.
+) -> Tuple[Composed, dict]:
+    """Get Genesets that are shared with a user.
 
-    :param cursor: An async database cursor.
-    :param owner_id: The owner ID to search for.
-    :param is_readable_by: A user ID to check if the user can read the results.
-    :param with_publication_info: Include publication info in the return.
-
-    :return: list of results using `.fetchall()`
+    NOTE: NOT IMPLEMENTED
     """
-    await cursor.execute(
-        *geneset_query.get(
-            owner_id=owner_id,
-            is_readable_by=is_readable_by,
-            with_publication_info=with_publication_info,
-        )
-    )
-    return await cursor.fetchall()
+    raise NotImplementedError()
 
 
-async def by_project_id(
-    cursor: AsyncCursor,
+def by_project_id(
     project_id: int,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
-) -> List[Row]:
-    """Get a list of genesets by their membership in a project.
+) -> Tuple[Composed, dict]:
+    """Create a psycopg query to get genesets by project ID.
 
-    :param cursor: An async database cursor.
     :param project_id: The project ID to search for.
+    :param limit: The limit of results to return.
+    :param offset: The offset of results to return.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
 
-    :return: list of results using `.fetchall()`
+    :return: A query (and params) that can be executed on a cursor.
     """
-    await cursor.execute(
-        *geneset_query.by_project_id(
-            project_id=project_id,
-            is_readable_by=is_readable_by,
-            with_publication_info=with_publication_info,
-        )
+    query = (
+        format_select_query(with_publication_info=with_publication_info)
+        + SQL("JOIN project_geneset ON geneset.gs_id = project_geneset.gs_id")
+        + SQL("INNER JOIN production.project2geneset")
+        + SQL("ON geneset.gs_id=project2geneset.gs_id")
+        + SQL("WHERE project2geneset.pj_id=%(project_id)s")
     )
-    return await cursor.fetchall()
+    params = {"project_id": project_id}
+    filtering, params = is_readable([], params, is_readable_by)
+
+    if len(filtering) > 0:
+        query += SQL("WHERE") + SQL("AND").join(filtering)
+    query = limit_and_offset(query, limit, offset).join(" ")
+
+    return query, params
```

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/publication.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/aio/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/aio/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/threshold.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/aio/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/core/cursor.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/core/cursor.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/core/settings_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/gene.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/geneset.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/aio/geneset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,65 @@
-"""Geneset database functions."""
+"""Async database interaction code relating to Genesets."""
 
 from typing import List, Optional
 
-from geneweaver.core.enum import GeneIdentifier, ScoreType, Species
+from geneweaver.core.enum import GeneIdentifier, GenesetTier, ScoreType, Species
+from geneweaver.core.schema.gene import GeneValue
+from geneweaver.core.schema.geneset import GenesetUpload
+from geneweaver.core.schema.score import GenesetScoreType
 from geneweaver.db.query import geneset as geneset_query
-from geneweaver.db.utils import GenesetTierOrTiers, temp_override_row_factory
-from psycopg import Cursor, rows
+from geneweaver.db.query.geneset.utils import geneset_upload_to_kwargs
+from geneweaver.db.utils import GenesetTierOrTiers
+from psycopg import AsyncCursor
 from psycopg.rows import Row
 
 
-def get(
-    cursor: Cursor,
-    is_readable_by: Optional[int] = None,
+async def get(
+    cursor: AsyncCursor,
     gs_id: Optional[int] = None,
     owner_id: Optional[int] = None,
     curation_tier: Optional[GenesetTierOrTiers] = None,
     species: Optional[Species] = None,
     name: Optional[str] = None,
     abbreviation: Optional[str] = None,
     publication_id: Optional[int] = None,
     pubmed_id: Optional[int] = None,
     gene_id_type: Optional[GeneIdentifier] = None,
     search_text: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
+    is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
     ontology_term: Optional[str] = None,
     score_type: Optional[ScoreType] = None,
 ) -> List[Row]:
     """Get genesets from the database.
 
     :param cursor: An async database cursor.
-    :param is_readable_by: A user ID to check if the user can read the results.
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
     :param curation_tier: Show only results of this curation tier.
     :param species: Show only results associated with this species.
     :param name: Show only results with this name.
     :param abbreviation: Show only results with this abbreviation.
     :param publication_id: Show only results with this publication ID (internal).
     :param pubmed_id: Show only results with this PubMed ID.
     :param gene_id_type: Show only results with this gene ID type.
     :param search_text: Return genesets that match this search text (using PostgreSQL
                         full-text search).
     :param limit: Limit the number of results.
     :param offset: Offset the results.
+    :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
     :param ontology_term: Show only results associated with this ontology term.
     :param score_type: Show only results with given score type.
 
     :return: list of results using `.fetchall()`
     """
-    cursor.execute(
+    await cursor.execute(
         *geneset_query.get(
             is_readable_by=is_readable_by,
             gs_id=gs_id,
             owner_id=owner_id,
             curation_tier=curation_tier,
             species=species,
             name=name,
@@ -68,214 +72,197 @@
             offset=offset,
             with_publication_info=with_publication_info,
             ontology_term=ontology_term,
             score_type=score_type,
         )
     )
 
-    return cursor.fetchall()
+    return await cursor.fetchall()
 
 
-def by_id(
-    cursor: Cursor,
+async def by_id(
+    cursor: AsyncCursor,
     gs_id: int,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
 ) -> Optional[Row]:
     """Get a geneset by its ID.
 
-    :param cursor: A database cursor.
+    :param cursor: An async database cursor.
     :param gs_id: The geneset ID to search for.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
     """
-    cursor.execute(
+    await cursor.execute(
         *geneset_query.get(
             gs_id=gs_id,
             is_readable_by=is_readable_by,
             with_publication_info=with_publication_info,
         )
     )
 
-    return cursor.fetchone()
+    return await cursor.fetchone()
 
 
-def by_owner_id(
-    cursor: Cursor,
+async def by_owner_id(
+    cursor: AsyncCursor,
     owner_id: int,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
 ) -> List[Row]:
     """Get genesets by owner ID.
 
-    :param cursor: A database cursor.
+    :param cursor: An async database cursor.
     :param owner_id: The owner ID to search for.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
 
     :return: list of results using `.fetchall()`
     """
-    cursor.execute(
+    await cursor.execute(
         *geneset_query.get(
             owner_id=owner_id,
             is_readable_by=is_readable_by,
             with_publication_info=with_publication_info,
         )
     )
-    return cursor.fetchall()
+    return await cursor.fetchall()
 
 
-def by_project_id(
-    cursor: Cursor,
+async def by_project_id(
+    cursor: AsyncCursor,
     project_id: int,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
 ) -> List[Row]:
     """Get a list of genesets by their membership in a project.
 
     :param cursor: An async database cursor.
     :param project_id: The project ID to search for.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
 
     :return: list of results using `.fetchall()`
     """
-    cursor.execute(
+    await cursor.execute(
         *geneset_query.by_project_id(
             project_id=project_id,
             is_readable_by=is_readable_by,
             with_publication_info=with_publication_info,
         )
     )
-    return cursor.fetchall()
-
-
-# --------------------------------------------------------------------------------------
-# The following functions are not yet implemented in the aio/concurrent paradigm.
-# They are subject to change and may be deprecated in the future.
-
-
-@temp_override_row_factory(rows.tuple_row)
-def is_readable(cursor: Cursor, user_id: int, geneset_id: int) -> bool:
-    """Check if a geneset is readable by a user.
-
-    :param cursor: The database cursor.
-    :param user_id: The user id (internal) to check.
-    :param geneset_id: The geneset id to check.
+    return await cursor.fetchall()
 
-    :return: True if the geneset is readable by the user, False otherwise.
-    """
-    cursor.execute(
-        """
-        SELECT production.geneset_is_readable2(%(user_id)s, %(geneset_id)s);
-        """,
-        {"user_id": user_id, "geneset_id": geneset_id},
-    )
-    return cursor.fetchone()[0] is True
 
+async def add_geneset(
+    cursor: AsyncCursor,
+    user_id: int,
+    file_id: int,
+    name: str,
+    abbreviation: str,
+    tier: GenesetTier,
+    species: Species,
+    count: int,
+    score: GenesetScoreType,
+    gene_id_type: GeneIdentifier,
+    description: str = "",
+    publication_id: Optional[int] = None,
+    attribution: Optional[str] = None,
+) -> Optional[Row]:
+    """Add a geneset to the database.
 
-@temp_override_row_factory(rows.tuple_row)
-def user_is_owner(cursor: Cursor, user_id: int, geneset_id: int) -> bool:
-    """Check if a user is the owner of a geneset.
+    NOTE: This function _only_ adds the geneset instance to the database, and does not
+    perform any of the required related tasks for new genesets. You most likely *do not*
+    want to use this function.
 
-    :param cursor: The database cursor.
-    :param user_id: The user id (internal) to check.
-    :param geneset_id: The geneset id to check.
+    If you are adding a new geneset, you should use the `add` function instead.
 
-    :return: True if the user is the owner of the geneset, False otherwise.
+    :param cursor: An async database cursor.
+    :param user_id: The owner of the geneset.
+    :param file_id: The file ID of the geneset's values.
+    :param name: The name of the geneset.
+    :param abbreviation: The abbreviation of the geneset.
+    :param tier: The curation tier of the geneset.
+    :param species: The species of the geneset.
+    :param count: The number of genes in the geneset.
+    :param score: The score of the geneset (GenesetScoreType includes threshold info).
+    :param gene_id_type: The gene ID type of the geneset.
+    :param description: The description of the geneset.
+    :param publication_id: The publication ID of the geneset (not the PubMed ID).
+    :param attribution: The attribution of the geneset.
+    :return: The ID of the added Geneset using fetchone().
     """
-    cursor.execute(
-        """
-        SELECT COUNT(gs_id) FROM geneset
-        WHERE usr_id=%(user_id)s AND gs_id=%(geneset_id)s;
-        """,
-        {"user_id": user_id, "geneset_id": geneset_id},
+    await cursor.execute(
+        *geneset_query.add(
+            user_id=user_id,
+            file_id=file_id,
+            name=name,
+            abbreviation=abbreviation,
+            tier=tier,
+            species=species,
+            count=count,
+            score=score,
+            gene_id_type=gene_id_type,
+            description=description,
+            publication_id=publication_id,
+            attribution=attribution,
+        )
     )
-    result = cursor.fetchone()[0]
-    return result == 1 and not isinstance(result, bool)
+    return await cursor.fetchone()
 
 
-@temp_override_row_factory(rows.tuple_row)
-def update_date(cursor: Cursor, geneset_id: int) -> str:
-    """Update the date of a geneset.
-
-    :param cursor: The database cursor.
-    :param geneset_id: The geneset id to update.
-
-    :return: The updated date.
-    """
-    cursor.execute(
-        """
-        UPDATE geneset SET gs_updated = NOW()
-        WHERE gs_id = %(geneset_id)s
-        RETURNING gs_updated
-        """,
-        {"geneset_id": geneset_id},
-    )
-    cursor.connection.commit()
-    return cursor.fetchone()[0]
-
+async def add_geneset_file(
+    cursor: AsyncCursor,
+    values: List[GeneValue],
+    comments: str = "",
+) -> Optional[Row]:
+    """Add a geneset file to the database.
 
-@temp_override_row_factory(rows.tuple_row)
-def tier(cursor: Cursor, geneset_id: int) -> Optional[int]:
-    """Get the tier of a geneset.
+    NOTE: This function _only_ adds the geneset file to the database, and does not
+    perform any of the required related tasks for new genesets. You most likely *do not*
+    want to use this function.
 
-    :param cursor: The database cursor.
-    :param geneset_id: The geneset id to get the tier of.
+    If you are adding a new geneset, you should use the `add` function instead.
 
-    :return: The tier of the geneset, or None if the geneset does not have a tier,
-    or does not exist.
+    :param cursor: An async database cursor.
+    :param values: A list of GeneValues to render into a file.
+    :param comments: Comments to include with the file.
+    :return: The ID of the added file using fetchone().
     """
-    cursor.execute(
-        """
-        SELECT cur_id FROM geneset WHERE gs_id = %(geneset_id)s;
-        """,
-        {"geneset_id": geneset_id},
+    await cursor.execute(
+        *geneset_query.add_geneset_file(
+            values=values,
+            comments=comments,
+        )
     )
-    result = cursor.fetchone()
-
-    if not result:
-        return None
 
-    return result[0]
+    return await cursor.fetchone()
 
 
-def homology_ids(cursor: Cursor, geneset_id: int) -> List:
-    """Get all homology_ids that are associated with a geneset ID.
-
-    :param cursor: The database cursor.
-    :param geneset_id: The geneset ID to search for.
+async def add(
+    cursor: AsyncCursor,
+    geneset: GenesetUpload,
+    owner_id: Optional[int] = None,
+    publication_id: Optional[int] = None,
+) -> int:
+    """Add a geneset to the database with all necessary components.
 
-    :return: list of results using `.fetchall()`
+    :param cursor: An async database cursor.
+    :param geneset: An instance of a GenesetUpload schema.
+    :param owner_id: The owner of the geneset.
+    :param publication_id: The (internal) publication ID associated with the Geneset.
+    :return: The geneset ID.
     """
-    cursor.execute(
-        """
-        SELECT DISTINCT hom_id FROM extsrc.homology h
-        INNER JOIN extsrc.geneset_value gsv
-            ON h.ode_gene_id=gsv.ode_gene_id
-        INNER JOIN production.geneset g
-            ON gsv.gs_id=g.gs_id
-        WHERE gs_status not like 'de%%' AND g.gs_id=%(geneset_id)s""",
-        {"geneset_id": geneset_id},
+    file_id = await add_geneset_file(
+        cursor=cursor,
+        values=geneset.gene_list,
     )
-    return cursor.fetchall()
-
-
-# TODO: reimplement `get_all_geneset_values`
-
-
-@temp_override_row_factory(rows.tuple_row)
-def num_genes(cursor: Cursor, geneset_id: int) -> int:
-    """Get the number of genes associated with a geneset ID.
-
-    :param cursor: The database cursor.
-    :param geneset_id: The geneset ID to search for.
-
-    :return: The number of genes associated with the geneset ID.
-    """
-    cursor.execute(
-        """
-        SELECT COUNT(*) FROM extsrc.geneset_value WHERE gs_id = %(geneset_id)s;
-        """,
-        {"geneset_id": geneset_id},
+    geneset_id = await add_geneset(
+        cursor=cursor,
+        user_id=owner_id,
+        file_id=file_id,
+        publication_id=publication_id,
+        **geneset_upload_to_kwargs(geneset)
     )
-    return cursor.fetchone()[0]
+    await cursor.execute(*geneset_query.reparse_geneset_file(geneset_id=geneset_id))
+    await cursor.execute(*geneset_query.process_thresholds(geneset_id=geneset_id))
+    return geneset_id
```

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/geneset_value.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/publication.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/const.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/const.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/utils.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility functions for the geneset query."""
 
 from typing import Optional, Tuple
 
 from geneweaver.core.enum import GenesetTier
+from geneweaver.core.schema.geneset import GenesetUpload
 from geneweaver.db.query.geneset.const import (
     GENESET_FIELDS,
     GENESET_TSVECTOR,
     PUB_FIELDS,
 )
 from geneweaver.db.query.search import utils
 from geneweaver.db.query.utils import (
@@ -136,7 +137,26 @@
     """
     if isinstance(curation_tier, GenesetTier):
         curation_tier = {curation_tier}
     if curation_tier is not None:
         existing_filters.append(SQL("geneset.cur_id = ANY(%(curation_tier)s)"))
         existing_params["curation_tier"] = [int(tier) for tier in curation_tier]
     return existing_filters, existing_params
+
+
+def geneset_upload_to_kwargs(geneset: GenesetUpload) -> dict:
+    """Turn a GenesetUpload into a dict to be used as kwargs for SQL functions.
+
+    :param geneset: The geneset to process.
+    :return: A dict of the SQL function kwargs for adding a geneset.
+    """
+    tier = GenesetTier.TIER4 if geneset.private is not True else GenesetTier.TIER5
+    return {
+        "name": geneset.name,
+        "abbreviation": geneset.abbreviation,
+        "tier": tier,
+        "species": geneset.species,
+        "count": len(geneset.values),
+        "score": geneset.score,
+        "gene_id_type": geneset.gene_id_type,
+        "description": geneset.description,
+    }
```

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/write.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/geneset/write.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 """SQL query generation code for writing genesets."""
 
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 from geneweaver.core.enum import GeneIdentifier, GenesetTier, Species
 from geneweaver.core.schema.gene import GeneValue
+from geneweaver.core.schema.score import GenesetScoreType
 from psycopg.sql import SQL, Composed
 
 
 def add(
     user_id: int,
     file_id: int,
     name: str,
     abbreviation: str,
-    publication_id: int,
     tier: GenesetTier,
-    description: str,
     species: Species,
     count: int,
-    threshold_type: str,
-    threshold: float,
+    score: GenesetScoreType,
     gene_id_type: GeneIdentifier,
-    attribution: str,
+    description: str = "",
+    publication_id: Optional[int] = None,
+    attribution: Optional[str] = None,
 ) -> Tuple[Composed, dict]:
     """Add a geneset to the database.
 
     :param user_id: The user ID of the geneset owner.
     :param file_id: The file ID of the geneset file.
     :param name: The name of the geneset.
     :param abbreviation: The abbreviation of the geneset.
     :param publication_id: The publication ID of the geneset.
     :param tier: The curation tier of the geneset.
     :param description: The description of the geneset.
     :param species: The species of the geneset.
     :param count: The count of the geneset.
-    :param threshold_type: The threshold type of the geneset.
-    :param threshold: The threshold of the geneset.
+    :param score: The threshold type and amount of the geneset.
     :param gene_id_type: The gene ID type of the geneset.
     :param attribution: The attribution of the geneset.
 
     :return: A query (and params) that can be executed on a cursor.
     """
     query_cols = SQL(
         """
@@ -69,44 +68,44 @@
         "gs_name": name,
         "gs_abbreviation": abbreviation,
         "pub_id": publication_id,
         "cur_id": int(tier),
         "gs_description": description,
         "sp_id": int(species),
         "gs_count": count,
-        "gs_threshold_type": threshold_type,
-        "gs_threshold": threshold,
+        "gs_threshold_type": int(score.score_type),
+        "gs_threshold": score.threshold_as_db_string(),
         "gs_groups": "",
         "gs_gene_id_type": int(gene_id_type),
         "gs_created": "NOW()",
         "gs_attribution": attribution,
     }
 
     return query, params
 
 
-def render_and_add_geneset_file(
+def add_geneset_file(
     values: List[GeneValue],
     comments: str = "",
 ) -> Tuple[Composed, dict]:
     """Render and add a geneset file to the database.
 
     This function takes a list of gene values and renders them into a string
     that can be added to the database as a geneset file.
 
     :param values: The gene values to render.
     :param comments: The comments for the file.
     :return: A query (and params) that can be executed on a cursor.
     """
     contents = "\n".join(f"{value.symbol}\t{value.value}" for value in values)
     size = len(contents)
-    return add_geneset_file(size, contents, comments)
+    return add_geneset_file_raw(size, contents, comments)
 
 
-def add_geneset_file(
+def add_geneset_file_raw(
     size: int,
     contents: str,
     comments: str,
 ) -> Tuple[Composed, dict]:
     """Add a geneset file to the database.
 
     :param size: The size of the file.
@@ -118,7 +117,35 @@
         SQL("INSERT INTO file")
         + SQL("(file_size, file_contents, file_comments, file_created)")
         + SQL("VALUES (%(file_size)s, %(file_contents)s, %(file_comments)s, NOW())")
         + SQL("RETURNING file_id")
     ).join(" ")
     params = {"file_size": size, "file_contents": contents, "file_comments": comments}
     return query, params
+
+
+def reparse_geneset_file(geneset_id: int) -> Tuple[Composed, dict]:
+    """Call the `reparse_geneset_file` function in the database.
+
+    :param geneset_id: The ID of the geneset to reparse.
+    :return: A query (and params) that can be executed on a cursor.
+    """
+    query = (
+        SQL("SELECT")
+        + SQL("production.reparse_geneset_file($(reparse_geneset_file__geneset_id));")
+    ).join(" ")
+    params = {"reparse_geneset_file__geneset_id": geneset_id}
+    return query, params
+
+
+def process_thresholds(geneset_id: int) -> Tuple[Composed, dict]:
+    """Call the `process_thresholds` function in the database.
+
+    :param geneset_id: The ID of the geneset to process.
+    :return: A query (and params) that can be executed on a cursor.
+    """
+    query = (
+        SQL("SELECT")
+        + SQL("production.process_thresholds($(process_thresholds__geneset_id));")
+    ).join(" ")
+    params = {"process_thresholds__geneset_id": geneset_id}
+    return query, params
```

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/project.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/project.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/publication.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/utils.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/search/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/species.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/threshold.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/query/utils.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/query/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/species.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/threshold.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/user.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/src/geneweaver/db/utils.py` & `geneweaver_db-0.5.0a1/src/geneweaver/db/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.5.0a0/PKG-INFO` & `geneweaver_db-0.5.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: geneweaver-db
-Version: 0.5.0a0
+Version: 0.5.0a1
 Summary: Database Interaction Services for GeneWeaver
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: geneweaver-core (>=0.9.1,<1.0.0)
-Requires-Dist: psycopg[binary] (>=3.1.13,<4.0.0)
+Requires-Dist: geneweaver-core (>=0.10.0a0,<1.0.0)
+Requires-Dist: psycopg[binary] (==3.1.18)
 Project-URL: Repository, https://github.com/TheJacksonLaboratory/geneweaver-db
 Description-Content-Type: text/markdown
 
 # Geneweaver DB
 
 [![Tests](https://github.com/TheJacksonLaboratory/geneweaver-db/actions/workflows/tests.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-db/actions/workflows/tests.yml)
 [![Style](https://github.com/TheJacksonLaboratory/geneweaver-db/actions/workflows/style.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-db/actions/workflows/style.yml)
```

