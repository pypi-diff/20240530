# Comparing `tmp/jupyter_nebulagraph-0.13.0.tar.gz` & `tmp/jupyter_nebulagraph-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_nebulagraph-0.13.0.tar", last modified: Thu May 30 03:41:29 2024, max compression
+gzip compressed data, was "jupyter_nebulagraph-0.9.1.tar", last modified: Thu Apr  4 03:35:06 2024, max compression
```

## Comparing `jupyter_nebulagraph-0.13.0.tar` & `jupyter_nebulagraph-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:41:29.985752 jupyter_nebulagraph-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 03:41:22.000000 jupyter_nebulagraph-0.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-30 03:41:29.985752 jupyter_nebulagraph-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-30 03:41:22.000000 jupyter_nebulagraph-0.13.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:41:29.985752 jupyter_nebulagraph-0.13.0/jupyter_nebulagraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-30 03:41:29.000000 jupyter_nebulagraph-0.13.0/jupyter_nebulagraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 03:41:29.000000 jupyter_nebulagraph-0.13.0/jupyter_nebulagraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:41:29.000000 jupyter_nebulagraph-0.13.0/jupyter_nebulagraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 03:41:29.000000 jupyter_nebulagraph-0.13.0/jupyter_nebulagraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 03:41:29.000000 jupyter_nebulagraph-0.13.0/jupyter_nebulagraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:41:29.985752 jupyter_nebulagraph-0.13.0/ngql/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 03:41:22.000000 jupyter_nebulagraph-0.13.0/ngql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30470 2024-05-30 03:41:22.000000 jupyter_nebulagraph-0.13.0/ngql/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-05-30 03:41:22.000000 jupyter_nebulagraph-0.13.0/ngql/ng_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 03:41:22.000000 jupyter_nebulagraph-0.13.0/ngql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:41:29.985752 jupyter_nebulagraph-0.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-30 03:41:22.000000 jupyter_nebulagraph-0.13.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/ngql/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/ngql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36253 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/ngql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/setup.py
```

### Comparing `jupyter_nebulagraph-0.13.0/LICENSE` & `jupyter_nebulagraph-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_nebulagraph-0.13.0/PKG-INFO` & `jupyter_nebulagraph-0.9.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,29 @@
-Metadata-Version: 2.1
-Name: jupyter_nebulagraph
-Version: 0.13.0
-Summary: Jupyter extension for NebulaGraph
-Home-page: https://github.com/wey-gu/jupyter_nebulagraph
-Author: Wey Gu
-Author-email: weyl.gu@gmail.com
-Project-URL: Bug Tracker, https://github.com/wey-gu/jupyter_nebulagraph/issues
-Project-URL: Documentation, https://jupyter-nebulagraph.readthedocs.io/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Jinja2
-Requires-Dist: nebula3-python>=3.8.0
-Requires-Dist: pandas
-Requires-Dist: tqdm
-Requires-Dist: pyvis
-Requires-Dist: requests
-Requires-Dist: pydantic
-Requires-Dist: scipy
-
-![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/61fccff2-c9be-43a0-a26f-6f5a00b1c198)
-
 
 [![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
 [![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
-[![Documentation](https://img.shields.io/badge/docs-Read%20The%20Docs-blue)](https://jupyter-nebulagraph.readthedocs.io/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
 
 https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
+`jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
-`jupyter_nebulagraph`, formerly `ipython-ngql`, is a Python package that simplifies the process of connecting to NebulaGraph from Jupyter Notebooks or iPython environments. It enhances the user experience by streamlining the creation, debugging, and sharing of Jupyter Notebooks. With `jupyter_nebulagraph`, users can effortlessly connect to NebulaGraph, load data, execute queries, visualize results, and fine-tune query outputs, thereby boosting collaborative efforts and productivity.
+Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
-![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
 
-## Getting Started
+![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
-```bash
-pip install jupyter_nebulagraph
-```
+![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
-Load the extension in Jupyter Notebook or iPython:
 
-```python
-%load_ext ngql
-%ngql --address 127.0.0.1 --port 9669 --user root --password nebula
-```
-
-Make queries:
+## Get Started
 
-```python
-%ngql USE basketballplayer;
-%ngql MATCH p=(v:player)-->(v2:player) WHERE id(v) == "player100" RETURN p;
-```
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
-Draw the graph:
-
-```python
-%ng_draw
-```
-
-Discover the features of `jupyter_nebulagraph` by experimenting with it on [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb). You can also access a similar Jupyter Notebook in the documentation [here](https://jupyter-nebulagraph.readthedocs.io/en/stable/get_started_docs/).
-
-For a detailed guide, refer to the [official documentation](https://jupyter-nebulagraph.readthedocs.io/en/stable).
-
-| Feature | Cheat Sheet | Example | Command Documentation |
-| ------- | ----------- | --------- | ---------------------- |
-| Connect | `%ngql --address 127.0.0.1 --port 9669 --user user --password password` | [Connect](https://jupyter-nebulagraph.readthedocs.io/en/stable/get_started_docs/#connect-to-nebulagraph) | [`%ngql`](https://jupyter-nebulagraph.readthedocs.io/en/stable/magic_words/ngql/#connect-to-nebulagraph) |
-| Load Data from CSV | `%ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer` | [Load Data](https://jupyter-nebulagraph.readthedocs.io/en/stable/get_started_docs/#load-data-from-csv) | [`%ng_load`](https://jupyter-nebulagraph.readthedocs.io/en/stable/magic_words/ng_load/) |
-| Query Execution | `%ngql MATCH p=(v:player{name:"Tim Duncan"})-->(v2:player) RETURN p;`| [Query Execution](https://jupyter-nebulagraph.readthedocs.io/en/stable/get_started_docs/#query) | [`%ngql` or `%%ngql`(multi-line)](https://jupyter-nebulagraph.readthedocs.io/en/stable/magic_words/ngql/#make-queries) |
-| Result Visualization | `%ng_draw` | [Draw Graph](https://jupyter-nebulagraph.readthedocs.io/en/stable/magic_words/ng_draw/) | [`%ng_draw`](https://jupyter-nebulagraph.readthedocs.io/en/stable/magic_words/ng_draw/) |
-| Draw Schema | `%ng_draw_schema` | [Draw Schema](https://jupyter-nebulagraph.readthedocs.io/en/stable/magic_words/ng_draw_schema/) | [`%ng_draw_schema`](https://jupyter-nebulagraph.readthedocs.io/en/stable/magic_words/ng_draw_schema/) |
-| Tweak Query Result | `df = _` to get last query result as `pd.dataframe` or [`ResultSet`](https://github.com/vesoft-inc/nebula-python/blob/master/nebula3/data/ResultSet.py) | [Tweak Result](https://jupyter-nebulagraph.readthedocs.io/en/stable/get_started_docs/#result-handling) | [Configure `ngql_result_style`](https://jupyter-nebulagraph.readthedocs.io/en/stable/configurations/#configure-ngql_result_style) |
-
-
-<details>
-<summary>Click to see more!</summary>
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
 `jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
@@ -136,14 +77,16 @@
 
 ```python
 %%ngql
 SHOW TAGS;
 SHOW HOSTS;
 ```
 
+> There will be other options in future, i.e. from a `.ngql` file.
+
 ### Query String with Variables
 
 `jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
@@ -158,50 +101,28 @@
 0	LaMarcus Aldridge	Trail Blazers
 1	LaMarcus Aldridge	Spurs
 2	Marco Belinelli	Warriors
 ```
 
 ### Draw query results
 
-**Draw Last Query**
-
 Just call `%ng_draw` after queries with graph data.
 
 ```python
 # one query
 %ngql GET SUBGRAPH 2 STEPS FROM "player101" YIELD VERTICES AS nodes, EDGES AS relationships;
 %ng_draw
 
 # another query
 %ngql match p=(:player)-[]->() return p LIMIT 5
 %ng_draw
 ```
 
 ![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
 
-**Draw a Query**
-
-Or `%ng_draw <one_line_query>`, `%%ng_draw <multiline_query>` instead of drawing the result of the last query.
-
-<img width="1142" alt="ng_draw_demo_1" src="https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/a6e3b2d4-0320-4287-bd2f-537cff77c1de">
-
-One line query:
-
-```python
-%ng_draw GET SUBGRAPH 2 STEPS FROM "player101" YIELD VERTICES AS nodes, EDGES AS relationships;
-```
-
-Multiple lines query:
-
-```python
-%%ng_draw
-MATCH path_0=(n)--() WHERE id(n) == "p_0"
-OPTIONAL MATCH path_1=(n)--()--()
-RETURN path_0, path_1
-```
 ### Draw Graph Schema
 
 ```python
 %ng_draw_schema
 ```
 
 ![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
@@ -231,36 +152,101 @@
 %ng_load --source https://github.com/wey-gu/jupyter_nebulagraph/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer
 # with rank column
 %ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
 # without rank column
 %ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
 ```
 
-### Tweak Query Result
+### Configure `ngql_result_style`
 
-By default, the query result is a Pandas Dataframe, and we could access that by read from variable `_`.
+By default, `jupyter_nebulagraph` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
+
+This can be done ad-hoc with below one line:
 
 ```python
-In [1]: %ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
+%config IPythonNGQL.ngql_result_style="raw"
+```
+
+After the above line is executed, the output will be like this:
 
-In [2]: df = _
+```python
+ResultSet(ExecutionResponse(
+    error_code=0,
+    latency_in_us=2844,
+    data=DataSet(
+        column_names=[b'Trainer_Name'],
+        rows=[Row(
+            values=[Value(
+                sVal=b'Tom')]),
+...
+        Row(
+            values=[Value(
+                sVal=b'Wey')])]),
+    space_name=b'pokemon_club'))
 ```
 
-It's also configurable to have the result in raw ResultSet, to enable handy NebulaGraph Python App Development.
+The result are always stored in variable `_` in Jupyter Notebook, thus, to tweak the result, just refer a new var to it like:
+
+```python
+In [1] : %config IPythonNGQL.ngql_result_style="raw"
+
+In [2] : %%ngql USE pokemon_club;
+    ...: GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id
+    ...: | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
+    ...:
+    ...:
+Out[3]:
+ResultSet(ExecutionResponse(
+    error_code=0,
+    latency_in_us=3270,
+    data=DataSet(
+        column_names=[b'Trainer_Name'],
+        rows=[Row(
+            values=[Value(
+                sVal=b'Tom')]),
+...
+        Row(
+            values=[Value(
+                sVal=b'Wey')])]),
+    space_name=b'pokemon_club'))
+
+In [4]: r = _
 
-See more via [Docs: Result Handling](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started_docs/#result-handling)
+In [5]: r.column_values(key='Trainer_Name')[0].cast()
+Out[5]: 'Tom'
+```
 
-### CheatSheet
+### Get Help
 
-If you find yourself forgetting commands or not wanting to rely solely on the cheat sheet, remember this one thing: seek help through the help command!
+Don't remember anything or even relying on the cheatsheet here, oen takeaway for you: the help!
 
 ```python
-%ngql help
+In [1]: %ngql help
 ```
 
-</details>
+### Examples
 
-## Acknowledgments ♥️
+#### Jupyter Notebook
 
-- Inspiration for this project comes from [ipython-sql](https://github.com/catherinedevlin/ipython-sql), courtesy of [Catherine Devlin](https://catherinedevlin.blogspot.com/).
-- Graph visualization features are enabled by [pyvis](https://github.com/WestHealth/pyvis), a project by [WestHealth](https://github.com/WestHealth).
-- Generous sponsorship and support provided by [Vesoft Inc.](https://www.vesoft.com/) and the [NebulaGraph community](https://github.com/vesoft-inc/nebula).
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
+
+#### iPython
+
+```python
+In [1]: %load_ext ngql
+
+In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
+Connection Pool Created
+Out[2]: 
+                        Name
+0           basketballplayer
+1  demo_movie_recommendation
+2                        k8s
+3                       test
+
+In [3]: %ngql USE basketballplayer;
+   ...: %ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
+Out[3]: 
+            Name
+0    Tony Parker
+1  Manu Ginobili
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jupyter_nebulagraph-0.13.0/ngql/magic.py` & `jupyter_nebulagraph-0.9.1/ngql/magic.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,33 @@
 from IPython.core.magic import (
     Magics,
     magics_class,
     line_cell_magic,
     needs_local_scope,
 )
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
+from tqdm.notebook import tqdm
 
-from typing import Dict, List, Optional, Any
+from typing import Dict, List
 import networkx as nx
 
 
 from jinja2 import Template, Environment, meta
 from traitlets.config.configurable import Configurable
 from traitlets import Bool, Int, Unicode
 
 from nebula3.data.DataObject import Node, Relationship, PathWrapper
 from nebula3.gclient.net import ConnectionPool as NebulaConnectionPool
 from nebula3.Config import Config as NebulaConfig
-from nebula3.Config import SSL_config
-
-from ngql.ng_load import ng_load
-from ngql.types import LoadDataArgsModel
 
 
 rel_query_sample_edge = Template(
     """
 MATCH ()-[e:`{{ edge_type }}`]->()
-RETURN [src(e), dst(e)] AS sample_edge LIMIT 10
+RETURN [src(e), dst(e)] AS sample_edge LIMIT 1
 """
 )
 
 
 rel_query_edge_type = Template(
     """
 MATCH (m)-[:`{{ edge_type }}`]->(n)
@@ -77,18 +74,14 @@
 def get_color(input_str):
     hash_val = 0
     for char in input_str:
         hash_val = (hash_val * 31 + ord(char)) & 0xFFFFFFFF
     return COLORS[hash_val % len(COLORS)]
 
 
-def is_human_readable(field):
-    return any(c.isalpha() for c in field) and len(field) < 20
-
-
 @magics_class
 class IPythonNGQL(Magics, Configurable):
     ngql_verbose = Bool(False, config=True, help="Set verbose mode")
     max_connection_pool_size = Int(
         None,
         config=True,
         allow_none=True,
@@ -152,58 +145,43 @@
             query = (
                 line.replace(ESCAPE_ARROW_STRING, "->") + "\n" + (cell if cell else "")
             )
             return self._stylized(self._execute(query))
         else:  # We shouldn't reach here
             return f"Nothing triggerred, Connection State: { connection_state }"
 
-    def _init_connection_pool(self, args: Optional[Any] = None):
-        if args is None:
-            return (
-                CONNECTION_POOL_EXISTED
-                if self.connection_pool is not None
-                else CONNECTION_POOL_NONE
-            )
-
+    def _init_connection_pool(self, args):
         connection_info = (args.address, args.port, args.user, args.password)
         if any(connection_info):
             if not all(connection_info):
                 raise ValueError(
                     "One or more arguments missing: address, port, user, "
                     "password should None or all be provided."
                 )
-            # all connection information ready
-            connection_pool = NebulaConnectionPool()
-            config = NebulaConfig()
-            if self.max_connection_pool_size:
-                config.max_connection_pool_size = self.max_connection_pool_size
+            else:  # all connection information ready
+                connection_pool = NebulaConnectionPool()
+                config = NebulaConfig()
+                if self.max_connection_pool_size:
+                    config.max_connection_pool_size = self.max_connection_pool_size
 
-            self.credential = args.user, args.password
-            try:
+                self.credential = args.user, args.password
                 connect_init_result = connection_pool.init(
                     [(args.address, args.port)], config
                 )
-            except RuntimeError:
-                # When GraphD is over TLS
-                print("Got RuntimeError, trying to connect assuming GraphD is over TLS")
-                ssl_config = SSL_config()
-                connect_init_result = connection_pool.init(
-                    [(args.address, args.port)], config, ssl_config
-                )
-            if not connect_init_result:
-                return CONNECTION_POOL_INIT_FAILURE
-            else:
-                self.connection_pool = connection_pool
-                return CONNECTION_POOL_CREATED
+                if not connect_init_result:
+                    return CONNECTION_POOL_INIT_FAILURE
+                else:
+                    self.connection_pool = connection_pool
+                    return CONNECTION_POOL_CREATED
+
+        # else a.k.a not any(connection_info)
+        if self.connection_pool is not None:
+            return CONNECTION_POOL_EXISTED
         else:
-            return (
-                CONNECTION_POOL_EXISTED
-                if self.connection_pool is not None
-                else CONNECTION_POOL_NONE
-            )
+            return CONNECTION_POOL_NONE
 
     def _render_cell_vars(self, cell, local_ns):
         if cell is not None:
             env = Environment()
             cell_vars = meta.find_undeclared_variables(env.parse(cell))
             cell_params = {}
             for variable in cell_vars:
@@ -262,42 +240,32 @@
         return result
 
     def _remember_space(self, result):
         last_space_used = result.space_name()
         if last_space_used != "":
             self.space = last_space_used
 
-    def _stylized(self, result, style=None):
-        style = style or self.ngql_result_style
-        if style == STYLE_PANDAS:
+    def _stylized(self, result):
+        if self.ngql_result_style == STYLE_PANDAS:
             try:
                 import pandas as pd
             except ImportError:
                 raise ImportError("Please install pandas to use STYLE_PANDAS")
 
-            pd.set_option("display.max_columns", None)
-            pd.set_option("display.max_colwidth", None)
-            pd.set_option("display.max_rows", 300)
-            pd.set_option("display.expand_frame_repr", False)
-
             columns = result.keys()
             d: Dict[str, list] = {}
             for col_num in range(result.col_size()):
                 col_name = columns[col_num]
                 col_list = result.column_values(col_name)
                 d[col_name] = [x.cast() for x in col_list]
-            df = pd.DataFrame(d)
-            df.style.set_table_styles(
-                [{"selector": "table", "props": [("overflow-x", "scroll")]}]
-            )
-            return df
-        elif style == STYLE_RAW:
+            return pd.DataFrame(d)
+        elif self.ngql_result_style == STYLE_RAW:
             return result
         else:
-            raise ValueError(f"Unknown ngql_result_style: { style }")
+            raise ValueError("Unknown ngql_result_style")
 
     @staticmethod
     def _help_info():
         help_info = """
 
         Supported Configurations:
         ------------------------
@@ -332,24 +300,20 @@
         Reload ngql Magic
         %reload_ext ngql
 
         > Variables in query, we are using Jinja2 here
         name = "nba"
         %ngql USE "{{ name }}"
 
-        > Query and draw the graph of last executed query.
+        > Query and draw the graph
 
-        %ngql GET SUBGRAPH WITH PROP 2 STEPS FROM "player101" YIELD VERTICES AS nodes, EDGES AS relationships;
+        %ngql GET SUBGRAPH 2 STEPS FROM "player101" YIELD VERTICES AS nodes, EDGES AS relationships;
 
         %ng_draw
 
-        Or draw a Query
-
-        %ng_draw GET SUBGRAPH WITH PROP 2 STEPS FROM "player101" YIELD VERTICES AS nodes, EDGES AS relationships;
-
         > Query and draw the graph schema
 
         %ng_draw_schema
 
         > Load data from CSV file into NebulaGraph as vertices or edges
         %ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer
 
@@ -388,56 +352,23 @@
             from IPython.display import display, IFrame, HTML
 
             # import get_ipython
             from IPython import get_ipython
 
         except ImportError:
             raise ImportError("Please install pyvis to draw the graph")
-        # when `%ng_draw foo`, varible_name is "foo", else it's "_"
-        arguments_line = line.strip()
-
-        if not arguments_line and not cell:
-            # No arguments and no cell content, draw the graph with the last execution result
-
-            variable_name = arguments_line or "_"
-            # Check if the last execution result is available in the local namespace
-            if variable_name not in local_ns:
-                return "No result found, please execute a query first."
-            result_df = local_ns[variable_name]
-
-            if not isinstance(result_df, pd.DataFrame):
-                try:
-                    result_df = self._stylized(result_df, style=STYLE_PANDAS)
-                except Exception as e:
-                    print(
-                        f"[ERROR]: the last execution result is not a %ngql query, make a query first "
-                        f"or use %ng_draw <some query> instead, please. Something wrong with the result "
-                        f"parsing: \n { e }"
-                    )
-
-        else:
-            # Arguments provided, execute the query and draw the graph
-
-            if line == "help":
-                return self._help_info()
-
-            cell = self._render_cell_vars(cell, local_ns)
-
-            # Replace "->" with ESCAPE_ARROW_STRING to avoid argument parsing issues
-            modified_line = line.replace("->", ESCAPE_ARROW_STRING)
-
-            connection_state = self._init_connection_pool()
-            if connection_state == CONNECTION_POOL_EXISTED:
-                # Restore "->" in the query before executing it
-                query = (
-                    modified_line.replace(ESCAPE_ARROW_STRING, "->")
-                    + "\n"
-                    + (cell if cell else "")
-                )
-                result_df = self._stylized(self._execute(query), style=STYLE_PANDAS)
+        # when `%ngql foo`, varible_name is "foo", else it's "_"
+        variable_name = line.strip() or "_"
+        # Check if the last execution result is available in the local namespace
+        if variable_name not in local_ns:
+            return "No result found, please execute a query first."
+        result_df = local_ns[variable_name]
+        assert isinstance(
+            result_df, pd.DataFrame
+        ), "Result is not in Pandas DataFrame Style"
 
         # Create a graph
         g = Network(
             notebook=True,
             directed=True,
             cdn_resources="in_line",
             height="500px",
@@ -447,52 +378,36 @@
             neighborhood_highlight=True,
         )
         g_nx = nx.MultiDiGraph()
         for _, row in result_df.iterrows():
             for item in row:
                 self.render_pd_item(g, g_nx, item)
 
-        try:
-            # Calculate PageRank
-            pagerank_scores = nx.pagerank(g_nx)
-
-            # Update node sizes based on PageRank scores
-            for node_id, score in pagerank_scores.items():
-                g.get_node(node_id)["size"] = (
-                    10 + score * 130
-                )  # Normalized size for visibility
-        except Exception as e:
-            print(
-                f"[WARN]: failed to calculate PageRank, left graph node unsized. Reason:\n { e }"
-            )
-
         g.repulsion(
             node_distance=90,
             central_gravity=0.2,
             spring_length=200,
             spring_strength=0.05,
             damping=0.09,
         )
         # g.show_buttons(filter_='physics')
-        # return g.show("nebulagraph.html", notebook=True)
-        cell_num = get_ipython().execution_count
-        graph_render_filename = f"nebulagraph_cell_{cell_num}.html"
-        g_html_string = g.generate_html(graph_render_filename)
-        with open(graph_render_filename, "w", encoding="utf-8") as f:
+        # return g.show("nebulagraph_draw.html", notebook=True)
+        g_html_string = g.generate_html("nebulagraph.html")
+        with open("nebulagraph.html", "w", encoding="utf-8") as f:
             f.write(g_html_string)
         # detect if we are in colab or not
         try:
             if "google.colab" in str(get_ipython()):
                 display(HTML(g_html_string))
             else:
-                display(IFrame(src=graph_render_filename, width="100%", height="500px"))
+                display(IFrame(src="nebulagraph.html", width="100%", height="500px"))
         except Exception as e:
             print(f"[WARN]: failed to display the graph\n { e }")
             try:
-                display(IFrame(src=graph_render_filename, width="100%", height="500px"))
+                display(IFrame(src="nebulagraph.html", width="100%", height="500px"))
             except Exception as e:
                 print(f"[WARN]: failed to display the graph\n { e }")
 
         return g
 
     @line_cell_magic
     @magic_arguments()
@@ -608,171 +523,114 @@
 
         for edge_schema in relationship_samples:
             src_tag, dst_tag, edge_type = (
                 edge_schema["src_tag"],
                 edge_schema["dst_tag"],
                 edge_schema["edge_type"],
             )
-            title = (
-                "{\n  "
-                + "\n  ".join([f"{k}: {v}" for k, v in edge_schema.items()])
-                + "\n}"
-            )
-            g.add_edge(src_tag, dst_tag, label=edge_type, title=title)
+            g.add_edge(src_tag, dst_tag, label=edge_type, title=str(edge_schema))
             g_nx.add_edge(src_tag, dst_tag, **edge_schema)
 
-        try:
-            # Calculate PageRank
-            pagerank_scores = nx.pagerank(g_nx)
-
-            # Update node sizes based on PageRank scores
-            for node_id, score in pagerank_scores.items():
-                g.get_node(node_id)["size"] = (
-                    10 + score * 130
-                )  # Normalized size for visibility
-        except Exception as e:
-            print(
-                f"[WARN]: failed to calculate PageRank, left graph node unsized. Reason:\n { e }"
-            )
-
         g.repulsion(
             node_distance=90,
             central_gravity=0.2,
             spring_length=200,
             spring_strength=0.05,
             damping=0.09,
         )
         # g.show_buttons(filter_='physics')
         # return g.show("nebulagraph_draw.html", notebook=True)
-        cell_num = get_ipython().execution_count
-        schema_html_filename = f"nebulagraph_schema_cell_{cell_num}_{space}.html"
-        g_html_string = g.generate_html(schema_html_filename)
-        with open(schema_html_filename, "w", encoding="utf-8") as f:
+        g_html_string = g.generate_html("nebulagraph_schema.html")
+        with open("nebulagraph_schema.html", "w", encoding="utf-8") as f:
             f.write(g_html_string)
         # detect if we are in colab or not
         try:
             if "google.colab" in str(get_ipython()):
                 display(HTML(g_html_string))
             else:
-                display(IFrame(src=schema_html_filename, width="100%", height="500px"))
+                display(
+                    IFrame(src="nebulagraph_schema.html", width="100%", height="500px")
+                )
         except Exception as e:
             print(f"[WARN]: failed to display the graph\n { e }")
             try:
-                display(IFrame(src=schema_html_filename, width="100%", height="500px"))
+                display(
+                    IFrame(src="nebulagraph_schema.html", width="100%", height="500px")
+                )
             except Exception as e:
                 print(f"[WARN]: failed to display the graph\n { e }")
 
         return g
 
     def render_pd_item(self, g, g_nx, item):
         # g is pyvis graph
         # g_nx is networkx graph
 
         if isinstance(item, Node):
             node_id = str(item.get_id().cast())
             tags = item.tags()  # list of strings
-            tags_str = tags[0] if len(tags) == 1 else ",".join(tags)
             props_raw = dict()
             for tag in tags:
                 props_raw.update(item.properties(tag))
             props = {
                 k: str(v.cast()) if hasattr(v, "cast") else str(v)
                 for k, v in props_raw.items()
             }
-            # populating empty and null properties
-            props = {
-                k: v for k, v in props.items() if v not in ["__NULL__", "__EMPTY__"]
-            }
 
             if "name" in props:
                 label = props["name"]
             else:
-                if is_human_readable(node_id):
-                    label = f"tag: {tags_str},\nid: {node_id}"
-                else:
-                    label = f"tag: {tags_str},\nid: {node_id[:3]}..{node_id[-3:]}"
+                label = f"tag: {tags}, id: {node_id}"
                 for k in props:
                     if "name" in str(k).lower():
                         label = props[k]
                         break
-
             if "id" not in props:
                 props["id"] = node_id
-            title = "\n".join([f"{k}: {v}" for k, v in props.items()])
 
-            g.add_node(node_id, label=label, title=title, color=get_color(node_id))
+            g.add_node(node_id, label=label, title=str(props), color=get_color(node_id))
 
             # networkx
             if len(tags) > 1:
-                props["__tags__"] = ",".join(tags)
-            g_nx.add_node(node_id, **props)
+                g_nx.add_node(node_id, type=tags[0], **props)
+            else:
+                g_nx.add_node(node_id, **props)
         elif isinstance(item, Relationship):
             src_id = str(item.start_vertex_id().cast())
             dst_id = str(item.end_vertex_id().cast())
             edge_name = item.edge_name()
             props_raw = item.properties()
-            rank = item.ranking()
             props = {
                 k: str(v.cast()) if hasattr(v, "cast") else str(v)
                 for k, v in props_raw.items()
             }
-            if rank != 0:
-                props.update({"rank": rank})
-            # populating empty and null properties
-            props = {
-                k: v for k, v in props.items() if v not in ["__NULL__", "__EMPTY__"]
-            }
             # ensure start and end vertex exist in graph
             if not src_id in g.node_ids:
-                label = (
-                    f"tag: {src_id[:3]}..{src_id[-3:]}"
-                    if not is_human_readable(src_id)
-                    else src_id
-                )
                 g.add_node(
                     src_id,
-                    label=label,
-                    title=src_id,
+                    label=str(src_id),
+                    title=str(src_id),
                     color=get_color(src_id),
                 )
             if not dst_id in g.node_ids:
-                label = (
-                    f"tag: {dst_id[:3]}..{dst_id[-3:]}"
-                    if not is_human_readable(dst_id)
-                    else dst_id
-                )
                 g.add_node(
                     dst_id,
-                    label=label,
-                    title=dst_id,
+                    label=str(dst_id),
+                    title=str(dst_id),
                     color=get_color(dst_id),
                 )
             props_str_list: List[str] = []
             for k in props:
                 if len(props_str_list) >= 1:
                     break
                 props_str_list.append(f"{truncate(k, 7)}: {truncate(str(props[k]), 8)}")
             props_str = "\n".join(props_str_list)
 
             label = f"{props_str}\n{edge_name}" if props else edge_name
-            if props:
-                title = (
-                    "{\n  "
-                    + "\n  ".join([f"{k}: {v}" for k, v in props.items()])
-                    + "\n}"
-                )
-            else:
-                title = edge_name
-            g.add_edge(
-                src_id,
-                dst_id,
-                label=label,
-                title=title,
-                weight=props.get("rank", 0),
-            )
+            g.add_edge(src_id, dst_id, label=label, title=str(props))
             # networkx
             props["edge_type"] = edge_name
             g_nx.add_edge(src_id, dst_id, **props)
 
         elif isinstance(item, PathWrapper):
             for node in item.nodes():
                 self.render_pd_item(g, g_nx, node)
@@ -795,21 +653,14 @@
     @argument("-t", "--tag", type=str, help="Tag name for vertices")
     @argument("--vid", type=int, help="Vertex ID column index")
     @argument("-e", "--edge", type=str, help="Edge type name")
     @argument("--src", type=int, help="Source vertex ID column index")
     @argument("--dst", type=int, help="Destination vertex ID column index")
     @argument("--rank", type=int, help="Rank column index", default=None)
     @argument(
-        "-l",
-        "--limit",
-        type=int,
-        help="Sample maximum n lines of the CSV file",
-        default=-1,
-    )
-    @argument(
         "--props",
         type=str,
         help="Property mapping, comma-separated column indexes",
         default=None,
     )
     @argument(
         "-b", "--batch", type=int, help="Batch size for data loading", default=256
@@ -833,11 +684,262 @@
         if self.connection_pool is None:
             print(
                 "Please connect to NebulaGraph first using %ngql magic before using ng_load"
                 "\nExample: %ngql --address 127.0.0.1 --port 9669 --user root --password nebula"
             )
             return
 
+        try:
+            import requests
+            import pandas as pd
+            from io import StringIO
+        except ImportError:
+            raise ImportError(
+                "Please install requests and pandas to use ng_load"
+                " magic: %pip3 install requests pandas"
+            )
+
         args = parse_argstring(self.ng_load, line)
-        ng_load(
-            self._execute, LoadDataArgsModel.model_validate(args, from_attributes=True)
+
+        # Check if space is specified
+        if args.space is None:
+            print("Please specify the space name using --space")
+            return
+        space = args.space
+
+        # Inspect space to get Vid Type
+        r = self._execute(f"DESC SPACE `{space}`")
+        try:
+            assert len(r.column_values("Vid Type")) == 1, "Space may not exist"
+            vid_type = r.column_values("Vid Type")[0].cast()
+        except Exception as e:
+            raise ValueError(
+                f"Failed to get Vid Type from space '{self.space}', error: {e}"
+            )
+
+        vid_length = 0
+        if "FIXED_STRING" in vid_type:
+            vid_length = int(vid_type.split("(")[1].split(")")[0])
+        is_vid_int = vid_length == 0
+
+        # Validate required arguments
+        if not args.tag and not args.edge:
+            print(
+                "Missing required argument: --tag tag_name for vertex loading or --edge edge_type for edge loading"
+            )
+            return
+
+        # If with header
+        with_header = args.header
+
+        # Load CSV from file or URL
+        if args.source.startswith("http://") or args.source.startswith("https://"):
+            response = requests.get(args.source)
+            csv_string = response.content.decode("utf-8")
+            df = pd.read_csv(StringIO(csv_string), header=0 if with_header else None)
+        else:
+            df = pd.read_csv(args.source, header=0 if with_header else None)
+
+        # Build schema type map for tag or edge type
+        prop_schema_map = {}
+        DESC_TYPE = "TAG" if args.tag else "EDGE"
+        DESC_TARGET = args.tag if args.tag else args.edge
+        r = self._execute(f"USE {space}; DESCRIBE {DESC_TYPE} `{DESC_TARGET}`")
+        props, types, nullable = (
+            r.column_values("Field"),
+            r.column_values("Type"),
+            r.column_values("Null"),
+        )
+        for i in range(r.row_size()):
+            # back compatible with old version of nebula-python
+            prop_schema_map[props[i].cast()] = {
+                "type": types[i].cast(),
+                "nullable": nullable[i].cast() == "YES",
+            }
+
+        # Process properties mapping
+        props_mapping = (
+            {int(k): v for k, v in (prop.split(":") for prop in args.props.split(","))}
+            if args.props
+            else {}
         )
+        # Values of props_mapping are property names they should be strings
+        # Keys of props_mapping are column indexes they should be integers
+        for k, v in props_mapping.items():
+            if not isinstance(k, int):
+                print(
+                    f"ERROR during prop mapping validation: Key '{k}' in property mapping is not an integer"
+                )
+                return
+            if not isinstance(v, str):
+                print(
+                    f"ERROR during prop mapping validation: Value '{v}' in property mapping is not a string"
+                )
+                return
+            if k >= len(df.columns) or k < 0:
+                print(
+                    f"ERROR during prop mapping validation: Key '{k}' in property mapping is out of range: 0-{len(df.columns)-1}"
+                )
+                return
+
+        with_props = True if props_mapping else False
+
+        # Validate props_mapping against schema
+        matched = True
+        for i, prop in props_mapping.items():
+            if prop not in prop_schema_map:
+                print(
+                    f"Error: Property '{prop}' not found in schema for {DESC_TYPE} '{args.tag}'"
+                )
+                matched = False
+        for prop in prop_schema_map:
+            # For not nullable properties, check if they are in props_mapping
+            if (
+                not prop_schema_map[prop]["nullable"]
+                and prop not in props_mapping.values()
+            ):
+                print(
+                    f"Error: Property '{prop}' is not nullable and not found in property mapping"
+                )
+                matched = False
+
+        if not matched:
+            print("Error: Property mapping does not match schema")
+            return
+
+        if args.rank is not None:
+            with_rank = True
+        else:
+            with_rank = False
+
+        # Prepare data for loading
+        if args.tag and not args.edge:
+            if args.vid is None:
+                raise ValueError("Missing required argument: --vid for vertex ID")
+            # Process properties mapping
+            vertex_data_columns = ["___vid"] + [
+                props_mapping[i] for i in range(len(df.columns)) if i in props_mapping
+            ]
+            vertex_data = df.iloc[:, [args.vid] + list(props_mapping.keys())]
+            vertex_data.columns = vertex_data_columns
+            # Here you would load vertex_data into NebulaGraph under the specified tag and space
+            print(
+                f"Parsed {len(vertex_data)} vertices '{args.space}' for tag '{args.tag}' in memory"
+            )
+        elif args.edge and not args.tag:
+            if args.src is None or args.dst is None:
+                raise ValueError(
+                    "Missing required arguments: --src and/or --dst for edge source and destination IDs"
+                )
+            # Process properties mapping
+            edge_data_columns = ["___src", "___dst"] + [
+                props_mapping[i] for i in range(len(df.columns)) if i in props_mapping
+            ]
+            edge_data_indices = [args.src, args.dst] + list(props_mapping.keys())
+            if with_rank:
+                edge_data_columns += ["___rank"]
+                edge_data_indices += [args.rank]
+            edge_data = df.iloc[:, edge_data_indices]
+            edge_data.columns = edge_data_columns
+            # Here you would load edge_data into NebulaGraph under the specified edge type and space
+            print(
+                f"Parsed {len(edge_data)} edges '{args.space}' for edge type '{args.edge}' in memory"
+            )
+        else:
+            raise ValueError(
+                "Specify either --tag for vertex loading or --edge for edge loading, not both"
+            )
+
+        # Load data into NebulaGraph
+        batch_size = args.batch
+
+        QUOTE_VID = "" if is_vid_int else '"'
+        QUOTE = '"'
+
+        if args.tag:
+            # Load vertex_data into NebulaGraph under the specified tag and space
+            # Now prepare INSERT query for vertices in batches
+            # Example of QUERY: INSERT VERTEX t2 (name, age) VALUES "13":("n3", 12), "14":("n4", 8);
+
+            for i in tqdm(
+                range(0, len(vertex_data), batch_size), desc="Loading Vertices"
+            ):
+                batch = vertex_data.iloc[i : i + batch_size]
+                query = f"INSERT VERTEX {args.tag} ({', '.join([col for col in vertex_data.columns if col != '___vid'])}) VALUES "
+                for index, row in batch.iterrows():
+                    vid_str = f'{QUOTE_VID}{row["___vid"]}{QUOTE_VID}'
+                    prop_str = ""
+                    if with_props:
+                        for prop_name in props_mapping.values():
+                            prop_value = row[prop_name]
+                            if pd.isnull(prop_value):
+                                if not prop_schema_map[prop_name]["nullable"]:
+                                    raise ValueError(
+                                        f"Error: Property '{prop_name}' is not nullable but received NULL value, "
+                                        f"data: {row}, column: {prop_name}"
+                                    )
+                                prop_str += "NULL, "
+                            elif prop_schema_map[prop_name]["type"] == "string":
+                                prop_str += f"{QUOTE}{prop_value}{QUOTE}, "
+                            else:
+                                prop_str += f"{prop_value}, "
+                        prop_str = prop_str[:-2]
+                    query += f"{vid_str}:({prop_str}), "
+                query = query[:-2] + ";"
+                try:
+                    result = self._execute(query)
+                except Exception as e:
+                    print(
+                        f"INSERT Failed on row {i + index}, data: {row}, error: {result.error_msg()}"
+                    )
+                    return
+                tqdm.write(f"Loaded {i + len(batch)} of {len(vertex_data)} vertices")
+
+            print(
+                f"Successfully loaded {len(vertex_data)} vertices '{args.space}' for tag '{args.tag}'"
+            )
+        elif args.edge:
+            # Load edge_data into NebulaGraph under the specified edge type and space
+            # Now prepare INSERT query for edges in batches
+            # Example of QUERY:
+            # with_rank INSERT EDGE e1 (name, age) VALUES "13" -> "14"@1:("n3", 12), "14" -> "15"@132:("n4", 8);
+            # without_rank INSERT EDGE e1 (name, age) VALUES "13" -> "14":("n3", 12), "14" -> "15":("n4", 8);
+
+            for i in tqdm(range(0, len(edge_data), batch_size), desc="Loading Edges"):
+                batch = edge_data.iloc[i : i + batch_size]
+                query = f"INSERT EDGE {args.edge} ({', '.join([col for col in edge_data.columns if col not in ['___src', '___dst', '___rank']])}) VALUES "
+                for index, row in batch.iterrows():
+                    src_str = f'{QUOTE_VID}{row["___src"]}{QUOTE_VID}'
+                    dst_str = f'{QUOTE_VID}{row["___dst"]}{QUOTE_VID}'
+                    prop_str = ""
+                    if with_props:
+                        for prop_name in props_mapping.values():
+                            prop_value = row[prop_name]
+                            if pd.isnull(prop_value):
+                                if not prop_schema_map[prop_name]["nullable"]:
+                                    raise ValueError(
+                                        f"Error: Property '{prop_name}' is not nullable but received NULL value, "
+                                        f"data: {row}, column: {prop_name}"
+                                    )
+                                prop_str += "NULL, "
+                            elif prop_schema_map[prop_name]["type"] == "string":
+                                prop_str += f"{QUOTE}{prop_value}{QUOTE}, "
+                            else:
+                                prop_str += f"{prop_value}, "
+                        prop_str = prop_str[:-2]
+                    if with_rank:
+                        rank_str = f"@{row['___rank']}"
+                    else:
+                        rank_str = ""
+                    query += f"{src_str} -> {dst_str}{rank_str}:({prop_str}), "
+                query = query[:-2] + ";"
+                try:
+                    result = self._execute(query)
+                except Exception as e:
+                    print(
+                        f"INSERT Failed on row {i + index}, data: {row}, error: {result.error_msg()}"
+                    )
+                    return
+                tqdm.write(f"Loaded {i + len(batch)} of {len(edge_data)} edges")
+            print(
+                f"Successfully loaded {len(edge_data)} edges '{args.space}' for edge type '{args.edge}'"
+            )
```

### Comparing `jupyter_nebulagraph-0.13.0/setup.py` & `jupyter_nebulagraph-0.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jupyter_nebulagraph",
-    version="0.13.0",
+    version="0.9.1",
     author="Wey Gu",
     author_email="weyl.gu@gmail.com",
     description="Jupyter extension for NebulaGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wey-gu/jupyter_nebulagraph",
     project_urls={
         "Bug Tracker": "https://github.com/wey-gu/jupyter_nebulagraph/issues",
-        "Documentation": "https://jupyter-nebulagraph.readthedocs.io/",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     install_requires=[
         "Jinja2",
-        "nebula3-python>=3.8.0",
+        "nebula3-python>=3.5.0",
         "pandas",
         "tqdm",
         "pyvis",
-        "requests",
-        "pydantic",
-        "scipy",
     ],
 )
```

