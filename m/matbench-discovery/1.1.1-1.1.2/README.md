# Comparing `tmp/matbench-discovery-1.1.1.tar.gz` & `tmp/matbench_discovery-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matbench-discovery-1.1.1.tar", last modified: Sun Jan 28 14:19:15 2024, max compression
+gzip compressed data, was "matbench_discovery-1.1.2.tar", last modified: Thu May 30 18:23:00 2024, max compression
```

## Comparing `matbench-discovery-1.1.1.tar` & `matbench_discovery-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-01-28 14:19:15.966043 matbench-discovery-1.1.1/
--rw-r--r--   0 janosh     (501) staff       (20)     6143 2024-01-28 14:19:15.965816 matbench-discovery-1.1.1/PKG-INFO
--rw-r--r--   0 janosh     (501) staff       (20)     1073 2023-08-11 01:47:47.000000 matbench-discovery-1.1.1/license
-drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-01-28 14:19:15.961728 matbench-discovery-1.1.1/matbench_discovery/
--rw-r--r--   0 janosh     (501) staff       (20)     7348 2024-01-28 13:42:29.000000 matbench-discovery-1.1.1/matbench_discovery/__init__.py
--rw-r--r--   0 janosh     (501) staff       (20)    10588 2024-01-25 10:21:28.000000 matbench-discovery-1.1.1/matbench_discovery/data.py
--rw-r--r--   0 janosh     (501) staff       (20)     4588 2024-01-18 19:11:24.000000 matbench-discovery-1.1.1/matbench_discovery/energy.py
-drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-01-28 14:19:15.963093 matbench-discovery-1.1.1/matbench_discovery/figshare/
--rw-r--r--   0 janosh     (501) staff       (20)     1807 2024-01-28 13:42:29.000000 matbench-discovery-1.1.1/matbench_discovery/figshare/1.0.0.json
--rw-r--r--   0 janosh     (501) staff       (20)      140 2024-01-28 13:42:29.000000 matbench-discovery-1.1.1/matbench_discovery/figshare/readme.md
--rw-r--r--   0 janosh     (501) staff       (20)     4795 2024-01-20 16:55:08.000000 matbench-discovery-1.1.1/matbench_discovery/metrics.py
--rw-r--r--   0 janosh     (501) staff       (20)      935 2023-12-24 04:04:45.000000 matbench-discovery-1.1.1/matbench_discovery/models.py
--rw-r--r--   0 janosh     (501) staff       (20)    34950 2024-01-06 16:09:09.000000 matbench-discovery-1.1.1/matbench_discovery/plots.py
--rw-r--r--   0 janosh     (501) staff       (20)    10603 2024-01-28 13:42:29.000000 matbench-discovery-1.1.1/matbench_discovery/preds.py
--rw-r--r--   0 janosh     (501) staff       (20)     4443 2023-12-24 04:04:45.000000 matbench-discovery-1.1.1/matbench_discovery/slurm.py
--rw-r--r--   0 janosh     (501) staff       (20)     1816 2023-12-28 10:28:38.000000 matbench-discovery-1.1.1/matbench_discovery/structure.py
-drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-01-28 14:19:15.965015 matbench-discovery-1.1.1/matbench_discovery.egg-info/
--rw-r--r--   0 janosh     (501) staff       (20)     6143 2024-01-28 14:19:15.000000 matbench-discovery-1.1.1/matbench_discovery.egg-info/PKG-INFO
--rw-r--r--   0 janosh     (501) staff       (20)      766 2024-01-28 14:19:15.000000 matbench-discovery-1.1.1/matbench_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 janosh     (501) staff       (20)        1 2024-01-28 14:19:15.000000 matbench-discovery-1.1.1/matbench_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 janosh     (501) staff       (20)      298 2024-01-28 14:19:15.000000 matbench-discovery-1.1.1/matbench_discovery.egg-info/requires.txt
--rw-r--r--   0 janosh     (501) staff       (20)       19 2024-01-28 14:19:15.000000 matbench-discovery-1.1.1/matbench_discovery.egg-info/top_level.txt
--rw-r--r--   0 janosh     (501) staff       (20)     3734 2024-01-28 13:42:36.000000 matbench-discovery-1.1.1/pyproject.toml
--rw-r--r--   0 janosh     (501) staff       (20)     2853 2024-01-25 10:21:28.000000 matbench-discovery-1.1.1/readme.md
--rw-r--r--   0 janosh     (501) staff       (20)       38 2024-01-28 14:19:15.966097 matbench-discovery-1.1.1/setup.cfg
-drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-01-28 14:19:15.964813 matbench-discovery-1.1.1/tests/
--rw-r--r--   0 janosh     (501) staff       (20)     6605 2024-01-25 10:25:01.000000 matbench-discovery-1.1.1/tests/test_data.py
--rw-r--r--   0 janosh     (501) staff       (20)     2182 2023-11-28 01:02:54.000000 matbench-discovery-1.1.1/tests/test_energy.py
--rw-r--r--   0 janosh     (501) staff       (20)      292 2023-09-21 00:24:14.000000 matbench-discovery-1.1.1/tests/test_init.py
--rw-r--r--   0 janosh     (501) staff       (20)     3189 2024-01-21 11:54:41.000000 matbench-discovery-1.1.1/tests/test_metrics.py
--rw-r--r--   0 janosh     (501) staff       (20)     2720 2023-12-24 04:04:45.000000 matbench-discovery-1.1.1/tests/test_models.py
--rw-r--r--   0 janosh     (501) staff       (20)     5336 2024-01-21 11:53:08.000000 matbench-discovery-1.1.1/tests/test_plots.py
--rw-r--r--   0 janosh     (501) staff       (20)     2269 2024-01-21 11:53:08.000000 matbench-discovery-1.1.1/tests/test_preds.py
--rw-r--r--   0 janosh     (501) staff       (20)     2040 2023-09-21 00:24:14.000000 matbench-discovery-1.1.1/tests/test_slurm.py
--rw-r--r--   0 janosh     (501) staff       (20)      613 2023-12-28 10:24:35.000000 matbench-discovery-1.1.1/tests/test_structure.py
+drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-05-30 18:23:00.601391 matbench_discovery-1.1.2/
+-rw-r--r--   0 janosh     (501) staff       (20)     6160 2024-05-30 18:23:00.601182 matbench_discovery-1.1.2/PKG-INFO
+-rw-r--r--   0 janosh     (501) staff       (20)     1073 2023-08-11 01:47:47.000000 matbench_discovery-1.1.2/license
+drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-05-30 18:23:00.597828 matbench_discovery-1.1.2/matbench_discovery/
+-rw-r--r--   0 janosh     (501) staff       (20)     3346 2024-05-15 19:13:00.000000 matbench_discovery-1.1.2/matbench_discovery/__init__.py
+-rw-r--r--   0 janosh     (501) staff       (20)    10936 2024-05-15 19:18:58.000000 matbench_discovery-1.1.2/matbench_discovery/data.py
+-rw-r--r--   0 janosh     (501) staff       (20)     4689 2024-05-15 19:18:41.000000 matbench_discovery-1.1.2/matbench_discovery/energy.py
+-rw-r--r--   0 janosh     (501) staff       (20)     8006 2024-05-15 14:50:50.000000 matbench_discovery-1.1.2/matbench_discovery/enums.py
+drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-05-30 18:23:00.598918 matbench_discovery-1.1.2/matbench_discovery/figshare/
+-rw-r--r--   0 janosh     (501) staff       (20)     1807 2024-01-28 13:42:29.000000 matbench_discovery-1.1.2/matbench_discovery/figshare/1.0.0.json
+-rw-r--r--   0 janosh     (501) staff       (20)      140 2024-01-28 13:42:29.000000 matbench_discovery-1.1.2/matbench_discovery/figshare/readme.md
+-rw-r--r--   0 janosh     (501) staff       (20)     5606 2024-05-30 18:18:36.000000 matbench_discovery-1.1.2/matbench_discovery/metrics.py
+-rw-r--r--   0 janosh     (501) staff       (20)      872 2024-04-26 00:03:31.000000 matbench_discovery-1.1.2/matbench_discovery/models.py
+-rw-r--r--   0 janosh     (501) staff       (20)    35674 2024-05-15 19:25:04.000000 matbench_discovery-1.1.2/matbench_discovery/plots.py
+-rw-r--r--   0 janosh     (501) staff       (20)    10738 2024-05-15 19:20:21.000000 matbench_discovery-1.1.2/matbench_discovery/preds.py
+-rw-r--r--   0 janosh     (501) staff       (20)     4396 2024-04-25 23:57:52.000000 matbench_discovery-1.1.2/matbench_discovery/slurm.py
+-rw-r--r--   0 janosh     (501) staff       (20)     1826 2024-04-25 23:57:36.000000 matbench_discovery-1.1.2/matbench_discovery/structure.py
+drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-05-30 18:23:00.600455 matbench_discovery-1.1.2/matbench_discovery.egg-info/
+-rw-r--r--   0 janosh     (501) staff       (20)     6160 2024-05-30 18:23:00.000000 matbench_discovery-1.1.2/matbench_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 janosh     (501) staff       (20)      814 2024-05-30 18:23:00.000000 matbench_discovery-1.1.2/matbench_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 janosh     (501) staff       (20)        1 2024-05-30 18:23:00.000000 matbench_discovery-1.1.2/matbench_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 janosh     (501) staff       (20)      313 2024-05-30 18:23:00.000000 matbench_discovery-1.1.2/matbench_discovery.egg-info/requires.txt
+-rw-r--r--   0 janosh     (501) staff       (20)       19 2024-05-30 18:23:00.000000 matbench_discovery-1.1.2/matbench_discovery.egg-info/top_level.txt
+-rw-r--r--   0 janosh     (501) staff       (20)     3940 2024-05-30 18:20:02.000000 matbench_discovery-1.1.2/pyproject.toml
+-rw-r--r--   0 janosh     (501) staff       (20)     2840 2024-04-26 00:10:21.000000 matbench_discovery-1.1.2/readme.md
+-rw-r--r--   0 janosh     (501) staff       (20)       38 2024-05-30 18:23:00.601427 matbench_discovery-1.1.2/setup.cfg
+drwxr-xr-x   0 janosh     (501) staff       (20)        0 2024-05-30 18:23:00.600299 matbench_discovery-1.1.2/tests/
+-rw-r--r--   0 janosh     (501) staff       (20)     6566 2024-03-30 17:20:12.000000 matbench_discovery-1.1.2/tests/test_data.py
+-rw-r--r--   0 janosh     (501) staff       (20)     2173 2024-03-30 17:19:22.000000 matbench_discovery-1.1.2/tests/test_energy.py
+-rw-r--r--   0 janosh     (501) staff       (20)      690 2024-02-29 15:08:53.000000 matbench_discovery-1.1.2/tests/test_enums.py
+-rw-r--r--   0 janosh     (501) staff       (20)      256 2024-03-30 17:19:22.000000 matbench_discovery-1.1.2/tests/test_init.py
+-rw-r--r--   0 janosh     (501) staff       (20)     3779 2024-03-30 17:22:09.000000 matbench_discovery-1.1.2/tests/test_metrics.py
+-rw-r--r--   0 janosh     (501) staff       (20)     2720 2024-02-29 15:08:53.000000 matbench_discovery-1.1.2/tests/test_models.py
+-rw-r--r--   0 janosh     (501) staff       (20)     5257 2024-05-30 18:18:52.000000 matbench_discovery-1.1.2/tests/test_plots.py
+-rw-r--r--   0 janosh     (501) staff       (20)     2284 2024-05-30 18:18:58.000000 matbench_discovery-1.1.2/tests/test_preds.py
+-rw-r--r--   0 janosh     (501) staff       (20)     2078 2024-04-16 08:50:40.000000 matbench_discovery-1.1.2/tests/test_slurm.py
+-rw-r--r--   0 janosh     (501) staff       (20)      534 2024-03-30 17:23:50.000000 matbench_discovery-1.1.2/tests/test_structure.py
```

### Comparing `matbench-discovery-1.1.1/PKG-INFO` & `matbench_discovery-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matbench-discovery
-Version: 1.1.1
+Version: 1.1.2
 Summary: A benchmark for machine learning energy models on inorganic crystal stability prediction from unrelaxed structures
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,59 +42,60 @@
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: plotly
 Requires-Dist: pymatgen
 Requires-Dist: pymatviz[df-pdf-export,export-figs]
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
+Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: wandb
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: running-models
 Requires-Dist: alignn; extra == "running-models"
-Requires-Dist: chgnet; extra == "running-models"
+Requires-Dist: chgnet>=0.3.0; extra == "running-models"
 Requires-Dist: jarvis-tools; extra == "running-models"
 Requires-Dist: m3gnet; extra == "running-models"
 Requires-Dist: mace-torch; extra == "running-models"
 Requires-Dist: maml; extra == "running-models"
 Requires-Dist: megnet; extra == "running-models"
 Provides-Extra: 3d-structures
 Requires-Dist: crystaltoolkit; extra == "3d-structures"
 Provides-Extra: fetch-wbm-data
 Requires-Dist: gdown; extra == "fetch-wbm-data"
 Provides-Extra: make-wbm-umap
 Requires-Dist: umap-learn; extra == "make-wbm-umap"
 
-<h1 align="center">
+<h1 align="center" style="line-height: 0; margin: 0 auto 1em;">
   <img src="https://github.com/janosh/matbench-discovery/raw/main/site/static/favicon.svg" alt="Logo" width="60px"><br>
   Matbench Discovery
 </h1>
 
-<h4 align="center" class="toc-exclude">
+<h4 align="center" class="toc-exclude" style="display: none;">
 
 [![arXiv](https://img.shields.io/badge/arXiv-2308.14920-blue?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.14920)
 [![Tests](https://github.com/janosh/matbench-discovery/actions/workflows/test.yml/badge.svg)](https://github.com/janosh/matbench-discovery/actions/workflows/test.yml)
 [![GitHub Pages](https://github.com/janosh/matbench-discovery/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/janosh/matbench-discovery/actions/workflows/gh-pages.yml)
 [![Requires Python 3.11+](https://img.shields.io/badge/Python-3.11+-blue.svg?logo=python&logoColor=white)](https://python.org/downloads)
 [![PyPI](https://img.shields.io/pypi/v/matbench-discovery?logo=pypi&logoColor=white)](https://pypi.org/project/matbench-discovery?logo=pypi&logoColor=white)
 
 </h4>
 
-> TL;DR: We benchmark ML models on crystal stability prediction from unrelaxed structures finding universal interatomic potentials (UIP) like [CHGNet](https://github.com/CederGroupHub/chgnet), [MACE](https://github.com/ACEsuit/mace) and [M3GNet](https://github.com/materialsvirtuallab/m3gnet) to be highly accurate, robust across chemistries and ready for production use in high-throughput materials discovery.
+> Disclaimer: We evaluate how accurately ML models predict solid-state thermodynamic stability. Although this is an important aspect of high-throughput materials discovery, the ranking cannot give a complete picture of a model's general applicability to materials. A high ranking does not constitute endorsement by the Materials Project.
 
 Matbench Discovery is an [interactive leaderboard](https://janosh.github.io/matbench-discovery/models) and associated [PyPI package](https://pypi.org/project/matbench-discovery) which together make it easy to rank ML energy models on a task designed to simulate a high-throughput discovery campaign for new stable inorganic crystals.
 
 We've tested <slot name="model-count" />models covering multiple methodologies ranging from random forests with structure fingerprints to graph neural networks, from one-shot predictors to iterative Bayesian optimizers and interatomic potential relaxers.
 
 <slot name="best-report" />
 
 Our results show that ML models have become robust enough to deploy them as triaging steps to more effectively allocate compute in high-throughput DFT relaxations. This work provides valuable insights for anyone looking to build large-scale materials databases.
 
 <slot name="metrics-table" />
 
 We welcome contributions that add new models to the leaderboard through GitHub PRs. See the [contributing guide](https://janosh.github.io/matbench-discovery/contribute) for details.
 
-If you're interested in joining this work, feel free to [open a GitHub discussion](https://github.com/janosh/matbench-discovery/discussions) or [send an email](mailto:janosh.riebesell@gmail.gov?subject=Collaborate%20on%20Matbench%20Discovery).
+If you're interested in joining this work, please reach out via [GitHub discussion](https://github.com/janosh/matbench-discovery/discussions) or [email](mailto:janosh.riebesell@gmail.com?subject=Collaborate%20on%20Matbench%20Discovery).
 
 For detailed results and analysis, check out the [preprint](https://janosh.github.io/matbench-discovery/preprint).
```

### Comparing `matbench-discovery-1.1.1/license` & `matbench_discovery-1.1.2/license`

 * *Files identical despite different names*

### Comparing `matbench-discovery-1.1.1/matbench_discovery/data.py` & `matbench_discovery-1.1.2/matbench_discovery/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from __future__ import annotations
+"""Download, cache and hydrate data files from the Matbench Discovery Figshare article.
+
+https://figshare.com/articles/dataset/22715158
+"""
 
 import gzip
 import json
 import os
 import pickle
 import sys
 import urllib.error
 import urllib.request
+from collections.abc import Callable
 from glob import glob
-from typing import TYPE_CHECKING, Any, Callable
+from pathlib import Path
+from typing import Any
 
 import pandas as pd
 from monty.json import MontyDecoder
+from pymatgen.analysis.phase_diagram import PatchedPhaseDiagram
 from tqdm import tqdm
 
-from matbench_discovery import FIGSHARE_DIR, Key
-
-if TYPE_CHECKING:
-    from pathlib import Path
-
-    from pymatgen.analysis.phase_diagram import PatchedPhaseDiagram
+from matbench_discovery import FIGSHARE_DIR
+from matbench_discovery.enums import Key
 
 # ruff: noqa: T201
 
 # repo URL to raw files on GitHub
 RAW_REPO_URL = "https://github.com/janosh/matbench-discovery/raw"
 figshare_versions = sorted(
     x.split(os.path.sep)[-1].split(".json")[0] for x in glob(f"{FIGSHARE_DIR}/*.json")
@@ -45,14 +47,15 @@
     except AttributeError:
         return None  # replace unhandled objects with None in serialized data
         # removes e.g. non-serializable AseAtoms from M3GNet relaxation trajectories
 
 
 def load(
     key: str,
+    *,
     version: str = figshare_versions[-1],
     cache_dir: str | Path = default_cache_dir,
     hydrate: bool = False,
     **kwargs: Any,
 ) -> pd.DataFrame | PatchedPhaseDiagram:
     """Download parts of or the full MP training data and WBM test data as pandas
     DataFrames. The full training and test sets are each about ~500 MB as compressed
@@ -111,14 +114,16 @@
             print(f"\n\nvariable dump:\n{file_path=},\n{url=}")
             raise
 
     print(f"Loading {key!r} from cached file at {cache_path!r}")
     if ".pkl" in file_path:  # handle key='mp_patched_phase_diagram' separately
         with gzip.open(cache_path, "rb") as zip_file:
             return pickle.load(zip_file)
+    if ".pth" in file_path:  # handle model checkpoints (e.g. key='alignn_checkpoint')
+        return cache_path
 
     csv_ext = (".csv", ".csv.gz", ".csv.bz2")
     reader = pd.read_csv if file_path.endswith(csv_ext) else pd.read_json
     try:
         df = reader(cache_path, **kwargs)
     except Exception:
         print(f"\n\nvariable dump:\n{file_path=},\n{reader=}\n{kwargs=}")
@@ -141,14 +146,15 @@
                 raise
 
     return df
 
 
 def glob_to_df(
     pattern: str,
+    *,
     reader: Callable[[Any], pd.DataFrame] | None = None,
     pbar: bool = True,
     **kwargs: Any,
 ) -> pd.DataFrame:
     """Combine data files matching a glob pattern into a single dataframe.
 
     Args:
@@ -263,8 +269,9 @@
 
 
 # data files can be downloaded and cached with matbench_discovery.data.load()
 DATA_FILES = DataFiles()
 
 
 df_wbm = load("wbm_summary")
-df_wbm[Key.mat_id] = df_wbm.index
+# str() around Key.mat_id added for https://github.com/janosh/matbench-discovery/issues/81
+df_wbm[str(Key.mat_id)] = df_wbm.index
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery/energy.py` & `matbench_discovery-1.1.2/matbench_discovery/energy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+"""Functions to compute formation and elemental reference energies from
+pymatgen EntryLikes.
+"""
+
 import itertools
 from collections.abc import Sequence
 
 import pandas as pd
 from pymatgen.analysis.phase_diagram import Entry, PDEntry
 from pymatgen.core import Composition
 from pymatgen.entries.computed_entries import ComputedEntry
 from pymatgen.util.typing import EntryLike
 from tqdm import tqdm
 
 from matbench_discovery.data import DATA_FILES
 
 
 def get_elemental_ref_entries(
-    entries: Sequence[EntryLike], verbose: bool = True
+    entries: Sequence[EntryLike], *, verbose: bool = True
 ) -> dict[str, Entry]:
     """Get the lowest energy pymatgen Entry for each element in a list of entries.
 
     Args:
         entries (Sequence[Entry]): pymatgen Entries (PDEntry, ComputedEntry or
             ComputedStructureEntry) to find elemental reference entries of.
         verbose (bool, optional): Whether to show a progress bar. Defaults to False.
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery/figshare/1.0.0.json` & `matbench_discovery-1.1.2/matbench_discovery/figshare/1.0.0.json`

 * *Files identical despite different names*

### Comparing `matbench-discovery-1.1.1/matbench_discovery/metrics.py` & `matbench_discovery-1.1.2/matbench_discovery/metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,135 @@
 """Functions to classify energy above convex hull predictions as true/false
 positive/negative and compute performance metrics.
 """
 
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
+from collections.abc import Sequence
 
 import numpy as np
+import pandas as pd
 from sklearn.metrics import r2_score
 
 from matbench_discovery import STABILITY_THRESHOLD
 
-if TYPE_CHECKING:
-    from collections.abc import Sequence
-
-    import pandas as pd
-
-
 __author__ = "Janosh Riebesell"
 __date__ = "2023-02-01"
 
 
 def classify_stable(
     e_above_hull_true: pd.Series,
     e_above_hull_pred: pd.Series,
+    *,
     stability_threshold: float | None = 0,
+    fillna: bool = True,
 ) -> tuple[pd.Series, pd.Series, pd.Series, pd.Series]:
     """Classify model stability predictions as true/false positive/negatives (usually
     w.r.t DFT-ground truth labels). All energies are assumed to be in eV/atom
     (but shouldn't really matter as long as they're consistent).
 
     Args:
         e_above_hull_true (pd.Series): Ground truth energy above convex hull values.
         e_above_hull_pred (pd.Series): Model predicted energy above convex hull values.
         stability_threshold (float | None, optional): Maximum energy above convex hull
             for a material to still be considered stable. Usually 0, 0.05 or 0.1.
             Defaults to 0, meaning a material has to be directly on the hull to be
             called stable. Negative values mean a material has to pull the known hull
             down by that amount to count as stable. Few materials lie below the known
             hull, so only negative values very close to 0 make sense.
+        fillna (bool): Whether to fill NaNs as the model predicting unstable. Defaults
+            to True.
 
     Returns:
         tuple[TP, FN, FP, TN]: Indices as pd.Series for true positives,
             false negatives, false positives and true negatives (in this order).
     """
     actual_pos = e_above_hull_true <= (stability_threshold or 0)  # guard against None
     actual_neg = e_above_hull_true > (stability_threshold or 0)
+
     model_pos = e_above_hull_pred <= (stability_threshold or 0)
     model_neg = e_above_hull_pred > (stability_threshold or 0)
 
+    if fillna:
+        nan_mask = np.isnan(e_above_hull_pred)
+        model_pos[nan_mask] = False  # fill NaNs as unstable
+        model_neg[nan_mask] = True  # fill NaNs as unstable
+
+        n_pos, n_neg, total = model_pos.sum(), model_neg.sum(), len(e_above_hull_pred)
+        if n_pos + n_neg != total:
+            raise ValueError(
+                f"after filling NaNs, the sum of positive ({n_pos}) and negative "
+                f"({n_neg}) predictions should add up to {total=}"
+            )
+
     true_pos = actual_pos & model_pos
     false_neg = actual_pos & model_neg
     false_pos = actual_neg & model_pos
     true_neg = actual_neg & model_neg
 
     return true_pos, false_neg, false_pos, true_neg
 
 
 def stable_metrics(
     each_true: Sequence[float],
     each_pred: Sequence[float],
+    *,
     stability_threshold: float = STABILITY_THRESHOLD,
+    fillna: bool = True,
 ) -> dict[str, float]:
     """Get a dictionary of stability prediction metrics. Mostly binary classification
     metrics, but also MAE, RMSE and R2.
 
     Args:
         each_true (list[float]): true energy above convex hull
         each_pred (list[float]): predicted energy above convex hull
         stability_threshold (float): Where to place stability threshold relative to
             convex hull in eV/atom, usually 0 or 0.1 eV. Defaults to 0.
+        fillna (bool): Whether to fill NaNs as the model predicting unstable. Defaults
+            to True.
 
     Note: Should give equivalent classification metrics to
         sklearn.metrics.classification_report(
             each_true > STABILITY_THRESHOLD,
             each_pred > STABILITY_THRESHOLD,
             output_dict=True,
         )
 
     Returns:
         dict[str, float]: dictionary of classification metrics with keys DAF, Precision,
             Recall, Accuracy, F1, TPR, FPR, TNR, FNR, MAE, RMSE, R2.
     """
     n_true_pos, n_false_neg, n_false_pos, n_true_neg = map(
-        sum, classify_stable(each_true, each_pred, stability_threshold)
+        sum,
+        classify_stable(
+            each_true, each_pred, stability_threshold=stability_threshold, fillna=fillna
+        ),
     )
 
     n_total_pos = n_true_pos + n_false_neg
     n_total_neg = n_true_neg + n_false_pos
     # prevalence: dummy discovery rate of stable crystals by selecting randomly from
     # all materials
-    prevalence = n_total_pos / len(each_true)
+    prevalence = n_total_pos / (n_total_pos + n_total_neg)
     precision = n_true_pos / (n_true_pos + n_false_pos)  # model's discovery rate
     recall = n_true_pos / n_total_pos
 
-    is_nan = np.isnan(each_true) | np.isnan(each_pred)
-    each_true, each_pred = np.array(each_true)[~is_nan], np.array(each_pred)[~is_nan]
-
     TPR = recall
     FPR = n_false_pos / n_total_neg
     TNR = n_true_neg / n_total_neg
     FNR = n_false_neg / n_total_pos
 
     if FPR + TNR != 1:  # sanity check: false positives + true negatives = all negatives
         raise ValueError(f"{FPR=} {TNR=} don't add up to 1")
 
     if TPR + FNR != 1:  # sanity check: true positives + false negatives = all positives
         raise ValueError(f"{TPR=} {FNR=} don't add up to 1")
 
+    # Drop NaNs to calculate regression metrics
+    is_nan = np.isnan(each_true) | np.isnan(each_pred)
+    each_true, each_pred = np.array(each_true)[~is_nan], np.array(each_pred)[~is_nan]
+
     return dict(
         F1=2 * (precision * recall) / (precision + recall),
         DAF=precision / prevalence,
         Precision=precision,
         Recall=recall,
         Accuracy=(n_true_pos + n_true_neg) / len(each_true),
         **dict(TPR=TPR, FPR=FPR, TNR=TNR, FNR=FNR),
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery/models.py` & `matbench_discovery-1.1.2/matbench_discovery/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
+"""Initializes global variable MODEL_METADATA."""
+
 from glob import glob
 from typing import Any
 
 import yaml
 
 from matbench_discovery import ROOT
 
 MODEL_DIRS = glob(f"{ROOT}/models/*/")
 MODEL_METADATA: dict[str, dict[str, Any]] = {}
 
 for model_dir in MODEL_DIRS:
     # skip directories without python files
     if glob(f"{model_dir}*.py") == []:
         continue
-    md_files = glob(f"{model_dir}metadata*.yml")
-    if len(md_files) != 1:
+    md_files = glob(f"{model_dir}*.yml")
+    if not 1 <= len(md_files) <= 2:
         raise RuntimeError(f"expected 1 metadata file, got {md_files=} in {model_dir=}")
-    md_file = md_files[0]
-    if md_file.endswith("aborted.yml"):
-        continue
-    # make sure all required keys are non-empty
-    with open(md_file) as yml_file:
-        models = yaml.full_load(yml_file)
-
-    # some metadata files contain a single model, some have multiple
-    if not isinstance(models, list):
-        models = [models]
-    for model in models:
-        model["model_dir"] = model_dir
-        MODEL_METADATA[model["model_name"]] = model
+    for md_file in md_files:
+        if md_file.endswith("aborted.yml"):
+            continue
+        # make sure all required keys are non-empty
+        with open(md_file) as yml_file:
+            model_data = yaml.full_load(yml_file)
+
+        model_data["model_dir"] = model_dir
+        MODEL_METADATA[model_data["model_name"]] = model_data
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery/plots.py` & `matbench_discovery-1.1.2/matbench_discovery/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Plotting functions for analyzing model performance on materials discovery."""
 
-from __future__ import annotations
-
 import functools
 import math
 from collections import defaultdict
-from typing import TYPE_CHECKING, Any, Literal
+from collections.abc import Sequence
+from typing import Any, Literal
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objs as go
 import scipy.interpolate
@@ -19,17 +18,14 @@
 from plotly.validators.scatter.line import DashValidator
 from plotly.validators.scatter.marker import SymbolValidator
 from tqdm import tqdm
 
 from matbench_discovery import STABILITY_THRESHOLD
 from matbench_discovery.metrics import classify_stable
 
-if TYPE_CHECKING:
-    from collections.abc import Sequence
-
 __author__ = "Janosh Riebesell"
 __date__ = "2022-08-05"
 
 Backend = Literal["matplotlib", "plotly"]
 
 plotly_markers = SymbolValidator().values[2::3]  # noqa: PD011
 plotly_line_styles = DashValidator().values[:-1]  # noqa: PD011
@@ -39,15 +35,15 @@
 plotly_colors *= len(plotly_markers) // len(plotly_colors)
 
 
 # color list https://plotly.com/python-api-reference/generated/plotly.graph_objects.layout
 colorway = ("lightseagreen", "orange", "lightsalmon", "dodgerblue")
 clf_labels = ("True Positive", "False Negative", "False Positive", "True Negative")
 clf_colors = ("lightseagreen", "orange", "lightsalmon", "dodgerblue")
-clf_color_map = dict(zip(clf_labels, clf_colors))
+clf_color_map = dict(zip(clf_labels, clf_colors, strict=True))
 
 
 def hist_classified_stable_vs_hull_dist(
     df: pd.DataFrame,
     each_true_col: str,
     each_pred_col: str,
     ax: plt.Axes | None = None,
@@ -99,34 +95,39 @@
     Returns:
         tuple[plt.Axes, dict[str, float]]: plot axes and classification metrics
 
     NOTE this figure plots hist bars separately which causes aliasing in pdf. Can be
     fixed in Inkscape or similar by merging regions by color.
     """
     x_col = dict(true=each_true_col, pred=each_pred_col)[which_energy]
+    clf_col, value_name = "classified", "count"
 
     df_plot = pd.DataFrame()
+    each_true_pos = each_true_neg = each_false_neg = each_false_pos = None
+
     for facet, df_group in (
         df.groupby(kwargs["facet_col"]) if "facet_col" in kwargs else [(None, df)]
     ):
         true_pos, false_neg, false_pos, true_neg = classify_stable(
-            df_group[each_true_col], df_group[each_pred_col], stability_threshold
+            df_group[each_true_col],
+            df_group[each_pred_col],
+            stability_threshold=stability_threshold,
         )
 
         # switch between hist of DFT-computed and model-predicted convex hull distance
-        e_above_hull = df_group[x_col]
-        each_true_pos = e_above_hull[true_pos]
-        each_true_neg = e_above_hull[true_neg]
-        each_false_neg = e_above_hull[false_neg]
-        each_false_pos = e_above_hull[false_pos]
+        srs_each = df_group[x_col]
+        each_true_pos = srs_each[true_pos]
+        each_true_neg = srs_each[true_neg]
+        each_false_neg = srs_each[false_neg]
+        each_false_pos = srs_each[false_pos]
         # n_true_pos, n_false_pos, n_true_neg, n_false_neg = map(
         #     sum, (true_pos, false_pos, true_neg, false_neg)
         # )
 
-        df_group[(clf_col := "classified")] = np.array(clf_labels)[
+        df_group[clf_col] = np.array(clf_labels)[
             true_pos * 0 + false_neg * 1 + false_pos * 2 + true_neg * 3
         ]
 
         # calculate histograms for each category
         hist_true_pos, bin_edges = np.histogram(
             each_true_pos - 0.001, bins=n_bins, range=x_lim
         )
@@ -140,15 +141,14 @@
 
         # combine histograms into a single dataframe
         df_hist = pd.DataFrame(
             (hist_true_pos, hist_false_neg, hist_false_pos, hist_true_neg),
             index=clf_labels,
         ).T
         df_hist[x_col] = bin_edges[:-1]
-        value_name = "count"
         df_melt = df_hist.melt(
             id_vars=x_col,
             value_vars=clf_labels,
             var_name=clf_col,
             value_name=value_name,
         ).assign(**{kwargs.get("facet_col", ""): facet})
         df_plot = pd.concat([df_plot, df_melt])
@@ -261,55 +261,59 @@
             )
 
     return fig
 
 
 def rolling_mae_vs_hull_dist(
     e_above_hull_true: pd.Series,
-    e_above_hull_errors: pd.DataFrame | dict[str, pd.Series],
+    e_above_hull_preds: pd.DataFrame | dict[str, pd.Series],
+    *,
     df_rolling_err: pd.DataFrame | None = None,
     df_err_std: pd.DataFrame | None = None,
-    window: float = 0.02,
+    window: float = 0.04,
     bin_width: float = 0.005,
     x_lim: tuple[float, float] = (-0.2, 0.2),
     y_lim: tuple[float, float] = (0, 0.2),
     backend: Backend = "plotly",
-    y_label: str = "rolling MAE (eV/atom)",
+    x_label: str | None = None,
+    y_label: str = "Rolling MAE (eV/atom)",
     just_plot_lines: bool = False,
     with_sem: bool = True,
     show_dft_acc: bool = False,
     show_dummy_mae: bool = False,
     pbar: bool = True,
     **kwargs: Any,
 ) -> plt.Axes | go.Figure:
-    """Rolling mean absolute error as the energy to the convex hull is varied. A scale
+    r"""Rolling mean absolute error as the energy to the convex hull is varied. A scale
     bar is shown for the windowing period of 40 meV per atom used when calculating the
     rolling MAE. The standard error in the mean is shaded around each curve. The
     highlighted V-shaped region shows the area in which the average absolute error is
     greater than the energy to the known convex hull. This is where models are most at
     risk of misclassifying structures.
 
     Args:
         e_above_hull_true (pd.Series): Distance to convex hull according to DFT
             ground truth (in eV / atom).
-        e_above_hull_errors (pd.DataFrame | dict[str, pd.Series]): Error in
-            model-predicted distance to convex hull, i.e. actual hull distance minus
-            predicted hull distance (in eV / atom).
+        e_above_hull_preds (pd.DataFrame | dict[str, pd.Series]): Predicted distance to
+            convex hull by models, one column per model (in eV / atom).
         df_rolling_err (pd.DataFrame, optional): Cached rolling MAE(s) as returned by
             previous call to this function. Defaults to None.
         df_err_std (pd.DataFrame, optional): Cached standard error in the mean of the
             rolling MAE(s) as returned by prev. call to this function. Defaults to None.
         window (float, optional): Rolling MAE averaging window. Defaults to 0.02 (20
             meV/atom)
         bin_width (float, optional): Density of line points (more points the
             smaller). Defaults to 0.002.
         x_lim (tuple[float, float], optional): x-axis range. Defaults to (-0.2, 0.3).
         y_lim (tuple[float, float], optional): y-axis range. Defaults to (0.0, 0.14).
         backend ('matplotlib' | 'plotly'], optional): Which plotting engine to use.
             Changes the return type. Defaults to 'plotly'.
+        x_label (str, optional): x-axis label. Defaults to "$E_\mathrm{above\ MP\ hull}$
+            (eV/atom)" for matplotlib and "E<sub>above MP hull</sub> (eV/atom)" for
+            plotly.
         y_label (str, optional): y-axis label. Defaults to "rolling MAE (eV/atom)".
         just_plot_line (bool, optional): If True, plot only the rolling MAE, no shapes
             and annotations. Also won't plot the standard error in the mean. Defaults
             to False.
         just_plot_lines (bool, optional): If True, plot only the rolling MAE, no shapes
             and annotations. Also won't plot the standard error in the mean. Defaults
             to False.
@@ -328,38 +332,41 @@
         tuple[plt.Axes | go.Figure, pd.DataFrame, pd.DataFrame]: matplotlib Axes or
         plotly
             Figure depending on backend, followed by two dataframes containing the
             rolling error for each column in e_above_hull_errors and the rolling
             standard error in the mean.
     """
     bins = np.arange(*x_lim, bin_width)
-    models = list(e_above_hull_errors)
+    models = list(e_above_hull_preds)
 
     if df_rolling_err is None or df_err_std is None:
         df_rolling_err = pd.DataFrame(columns=models, index=bins)
         df_err_std = df_rolling_err.copy()
 
         for model in (
             prog_bar := tqdm(models, desc="Calculating rolling MAE", disable=not pbar)
         ):
             prog_bar.set_postfix_str(model)
-            for idx, bin_center in enumerate(bins):
-                low = bin_center - window
-                high = bin_center + window
+            e_above_hull_pred = e_above_hull_preds[model].dropna()
+            e_above_hull_ref = e_above_hull_true.loc[e_above_hull_pred.index]
 
-                mask = (e_above_hull_true <= high) & (e_above_hull_true > low)
+            for bin_center in bins:
+                low = bin_center - window / 2
+                high = bin_center + window / 2
 
-                bin_mae = e_above_hull_errors[model].loc[mask].abs().mean()
-                df_rolling_err[model].iloc[idx] = bin_mae
+                mask = (e_above_hull_ref <= high) & (e_above_hull_ref > low)
+
+                bin_mae = (e_above_hull_pred - e_above_hull_ref).loc[mask].abs().mean()
+                df_rolling_err.loc[bin_center, model] = bin_mae
 
                 # drop NaNs to avoid error, scipy doesn't ignore NaNs
                 each_std = scipy.stats.sem(
-                    e_above_hull_errors[model].loc[mask].dropna().abs()
+                    (e_above_hull_pred - e_above_hull_ref).loc[mask].dropna().abs()
                 )
-                df_err_std[model].iloc[idx] = each_std
+                df_err_std.loc[bin_center, model] = each_std
     else:
         print("Using pre-calculated rolling MAE")
 
     fig = df_rolling_err.plot(backend=backend, **kwargs)
 
     if just_plot_lines:
         # return earlier if all plot objects besides the line were already drawn by a
@@ -368,15 +375,15 @@
 
     # DFT accuracy at 25 meV/atom for relative difference of e_above_hull for chemically
     # similar systems which is lower than formation energy error due to systematic error
     # cancellation among similar chemistries, supporting ref:
     href = "https://doi.org/10.1103/PhysRevB.85.155208"
     dft_acc = 0.025
 
-    window_bar_anno = f"rolling window={2 * window * 1000:.0f} meV"
+    window_bar_anno = f"rolling window={window * 1000:.0f} meV"
     dummy_mae = (e_above_hull_true - e_above_hull_true.mean()).abs().mean()
     dummy_mae_text = f"dummy MAE = {dummy_mae:.2f} eV/atom"
 
     if backend == "matplotlib":
         # assert df_rolling_err.isna().sum().sum() == 0, "NaNs in df_rolling_err"
         # assert df_err_std.isna().sum().sum() == 0, "NaNs in df_err_std"
         # for model in df_rolling_err if with_sem else []:
@@ -430,15 +437,17 @@
 
         fig.axhline(dummy_mae, color="tab:blue", linestyle="--", linewidth=0.5)
         fig.text(dummy_mae, 0.1, dummy_mae_text)
 
         fig.text(
             0, 0.13, r"MAE > $|E_\mathrm{above\ hull}|$", horizontalalignment="center"
         )
-        fig.set(xlabel=r"$E_\mathrm{above\ hull}$ (eV/atom)", ylabel=y_label)
+        fig.set(
+            xlabel=x_label or r"$E_\mathrm{above\ MP\ hull}$ (eV/atom)", ylabel=y_label
+        )
         fig.set(xlim=x_lim, ylim=y_lim)
         plt_line_styles = "- -- -. :".split() * 10
         plt_markers = "o s ^ v D * p X".split() * 10
 
         for idx, line in enumerate(fig.lines):
             line_label = line.get_label()
             if line_label.startswith("_"):
@@ -465,16 +474,16 @@
                 opacity=0.4,
                 showlegend=False,
             )
 
         fig.layout.legend.update(title="", x=0, y=0, yanchor="bottom")
         # change tooltip precision to 2 decimal places
         fig.update_traces(hovertemplate="x = %{x:.2f} eV/atom<br>y = %{y:.2f} eV/atom")
-        fig.layout.xaxis.title.text = "E<sub>above MP hull</sub> (eV/atom)"
-        fig.layout.yaxis.title.text = "rolling MAE (eV/atom)"
+        fig.layout.xaxis.title.text = x_label or "E<sub>above MP hull</sub> (eV/atom)"
+        fig.layout.yaxis.title.text = y_label
         fig.update_xaxes(range=x_lim)
         fig.update_yaxes(range=y_lim)
         # exclude from hover tooltip
         scatter_kwds = dict(
             fill="toself", opacity=0.2, hoverinfo="skip", showlegend=False
         )
         triangle_anno = "MAE > |E<sub>hull dist</sub>|"
@@ -528,23 +537,28 @@
             y=y0,
             text=window_bar_anno,
             showarrow=False,
             xshift=-4,
             yshift=-6,
             yanchor="bottom",
             xanchor="right",
+            xref="x",
         )
-        fig.add_shape(type="rect", x0=x0, y0=y0, x1=x0 - window, y1=y0 + window / 5)
+        fig.add_shape(type="rect", x0=x0, y0=y0, x1=x0 - window, y1=y0 + 0.006)
 
         from matbench_discovery.preds import model_styles
 
-        for trace in fig.data:
+        for idx, trace in enumerate(fig.data):
             if style := model_styles.get(trace.name):
                 ls, _marker, color = style
                 trace.line = dict(color=color, dash=ls, width=2)
+            else:  # pick from default colors, line styles, markers
+                trace.line = dict(
+                    color=plotly_colors[idx], dash=plotly_line_styles[idx], width=2
+                )
             # marker_spacing = 2
             # fig.add_scatter(
             #     x=trace.x[::marker_spacing],
             #     y=trace.y[::marker_spacing],
             #     mode="markers",
             #     marker=dict(symbol=marker, color=trace.line.color, size=8),
             #     showlegend=False,
@@ -552,14 +566,15 @@
             # )
     return fig, df_rolling_err, df_err_std
 
 
 def cumulative_metrics(
     e_above_hull_true: pd.Series,
     df_preds: pd.DataFrame,
+    *,
     metrics: Sequence[str] = ("Precision", "Recall"),
     stability_threshold: float = 0,  # set stability threshold as distance to convex
     # hull in eV / atom, usually 0 or 0.1 eV
     project_end_point: Literal["x", "y", "xy", ""] = "xy",
     optimal_recall: str | None = "Optimal Recall",
     show_n_stable: bool = True,
     backend: Backend = "plotly",
@@ -619,16 +634,19 @@
         )
 
     for model_name in df_preds:
         each_pred = df_preds[model_name].sort_values()
         # sort targets by model ranking
         each_true = e_above_hull_true.loc[each_pred.index]
 
-        true_pos_cum, false_neg_cum, false_pos_cum, true_neg_cum = map(
-            np.cumsum, classify_stable(each_true, each_pred, stability_threshold)
+        true_pos_cum, false_neg_cum, false_pos_cum, _true_neg_cum = map(
+            np.cumsum,
+            classify_stable(
+                each_true, each_pred, stability_threshold=stability_threshold
+            ),
         )
 
         # precision aka positive predictive value (PPV)
         n_total_pos = true_pos_cum.iloc[-1] + false_neg_cum.iloc[-1]
         precision_cum = true_pos_cum / (true_pos_cum + false_pos_cum)
         recall_cum = true_pos_cum / n_total_pos  # aka true_pos_rate aka sensitivity
 
@@ -697,23 +715,23 @@
                 legend=False,
                 backend=backend,
                 **line_kwargs | kwargs,
                 ylabel=metric,
             )
             df = dfs[metric]
             ax.set(ylim=(0, 1), xlim=(0, None), ylabel=metric)
+            bbox = dict(facecolor="white", alpha=0.5, edgecolor="none")
             for model in df_preds:
                 # TODO is this really necessary?
                 if len(df[model].dropna()) == 0:
                     continue
                 x_end = df[model].dropna().index[-1]
                 y_end = df[model].dropna().iloc[-1]
                 # add some visual guidelines to the plot
                 intersect_kwargs = dict(linestyle=":", alpha=0.4, linewidth=2)
-                bbox = dict(facecolor="white", alpha=0.5, edgecolor="none")
                 # place model name at the end of every line
                 ax.text(x_end, y_end, model, va="bottom", rotation=30, bbox=bbox)
                 if "x" in project_end_point:
                     ax.plot((x_end, x_end), (0, y_end), **intersect_kwargs)
                 if "y" in project_end_point:
                     ax.plot((0, x_end), (y_end, y_end), **intersect_kwargs)
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery/preds.py` & `matbench_discovery-1.1.2/matbench_discovery/preds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,25 @@
-from __future__ import annotations
+"""Centralize data-loading and computing metrics for plotting scripts."""
 
-from typing import TYPE_CHECKING, Any, Literal
+from collections.abc import Sequence
+from typing import Any, Literal
 
 import pandas as pd
 from tqdm import tqdm
 
-from matbench_discovery import (
-    ROOT,
-    STABILITY_THRESHOLD,
-    Key,
-    ev_per_atom,
-    model_labels,
-    quantity_labels,
-)
+from matbench_discovery import ROOT, STABILITY_THRESHOLD, Model
 from matbench_discovery.data import Files, df_wbm, glob_to_df
+from matbench_discovery.enums import Key
 from matbench_discovery.metrics import stable_metrics
 from matbench_discovery.plots import plotly_colors, plotly_line_styles, plotly_markers
 
-if TYPE_CHECKING:
-    from collections.abc import Sequence
-
-"""Centralize data-loading and computing metrics for plotting scripts"""
-
 __author__ = "Janosh Riebesell"
 __date__ = "2023-02-04"
 
 
-for col in (Key.model_mean_each, Key.model_mean_err, Key.model_std_each):
-    quantity_labels[col] = f"{col} {ev_per_atom}"
-
-
 class PredFiles(Files):
     """Data files provided by Matbench Discovery.
     See https://janosh.github.io/matbench-discovery/contribute for data descriptions.
     """
 
     # BOWSR optimizer coupled with original megnet
     bowsr_megnet = "bowsr/2023-01-23-bowsr-megnet-wbm-IS2RE.csv.gz"
@@ -59,29 +45,32 @@
     # # CHGNet-relaxed structures fed into MEGNet for formation energy prediction
     # chgnet_megnet = "chgnet/2023-03-06-chgnet-0.2.0-wbm-IS2RE.csv.gz"
     # # M3GNet-relaxed structures fed into MEGNet for formation energy prediction
     # m3gnet_megnet = "m3gnet/2022-10-31-m3gnet-wbm-IS2RE.csv.gz"
     # megnet_rs2re = "megnet/2023-08-23-megnet-wbm-RS2RE.csv.gz"
 
     # Magpie composition+Voronoi tessellation structure features + sklearn random forest
-    voronoi_rf = "voronoi/2022-11-27-train-test/e-form-preds-IS2RE.csv.gz"
+    voronoi_rf = "voronoi_rf/2022-11-27-train-test/e-form-preds-IS2RE.csv.gz"
 
     # wrenformer 10-member ensemble
     wrenformer = "wrenformer/2022-11-15-wrenformer-ens=10-IS2RE-preds.csv.gz"
 
     alignn = "alignn/2023-06-02-alignn-wbm-IS2RE.csv.gz"
     # alignn_pretrained = "alignn/2023-06-03-mp-e-form-alignn-wbm-IS2RE.csv.gz"
     # alignn_ff = "alignn_ff/2023-07-11-alignn-ff-wbm-IS2RE.csv.gz"
 
+    gnome = "gnome/2023-11-01-gnome-preds-50076332.csv.gz"
+
 
-# model_labels remaps model keys to pretty plot labels (see Files)
-PRED_FILES = PredFiles(root=f"{ROOT}/models", key_map=model_labels)
+# key_map maps model keys to pretty labels
+PRED_FILES = PredFiles(root=f"{ROOT}/models", key_map=Model.key_val_dict())
 
 
 def load_df_wbm_with_preds(
+    *,
     models: Sequence[str] = (*PRED_FILES,),
     pbar: bool = True,
     id_col: str = Key.mat_id,
     subset: pd.Index | Sequence[str] | Literal["uniq_protos"] | None = None,
     **kwargs: Any,
 ) -> pd.DataFrame:
     """Load WBM summary dataframe with model predictions from disk.
@@ -106,31 +95,34 @@
     """
     if mismatch := ", ".join(set(models) - set(PRED_FILES)):
         raise ValueError(
             f"Unknown models: {mismatch}, expected subset of {set(PRED_FILES)}"
         )
 
     dfs: dict[str, pd.DataFrame] = {}
-
     try:
         for model_name in (bar := tqdm(models, disable=not pbar, desc="Loading preds")):
             bar.set_postfix_str(model_name)
             df = glob_to_df(PRED_FILES[model_name], pbar=False, **kwargs)
             df = df.set_index(id_col)
             dfs[model_name] = df
     except Exception as exc:
-        raise RuntimeError(f"Failed to load {model_name=}") from exc
+        raise RuntimeError(f"Failed to load {locals().get('model_name')=}") from exc
 
     from matbench_discovery.data import df_wbm
 
     df_out = df_wbm.copy()
     for model_name, df in dfs.items():
         model_key = model_name.lower().replace("→", "_").replace(" ", "_")
 
-        cols = [col for col in df if col.startswith(f"e_form_per_atom_{model_key}")]
+        cols = [
+            col
+            for col in df
+            if col.startswith((f"e_form_per_atom_{model_key}", f"e_{model_key}_"))
+        ]
         if cols:
             if len(cols) > 1:
                 print(
                     f"Warning: multiple pred cols for {model_name=}, using {cols[0]!r} "
                     f"out of {cols=}"
                 )
             df_out[model_name] = df[cols[0]]
@@ -176,35 +168,43 @@
 df_metrics_10k.attrs["title"] = "Metrics for 10k Most Stable Predictions"
 df_metrics_uniq_protos = pd.DataFrame(index=df_metrics.index)
 df_metrics_uniq_protos.attrs["title"] = "Metrics for unique non-MP prototypes"
 
 for df in (df_metrics, df_metrics_10k, df_metrics_uniq_protos):
     df.index.name = "model"
 
-prevalence = (df_wbm[Key.each_true] <= STABILITY_THRESHOLD).mean()
+full_prevalence = (df_wbm[Key.each_true] <= STABILITY_THRESHOLD).mean()
+uniq_proto_prevalence = (
+    df_wbm.query(Key.uniq_proto)[Key.each_true] <= STABILITY_THRESHOLD
+).mean()
+
 for model in PRED_FILES:
     each_pred = df_preds[Key.each_true] + df_preds[model] - df_preds[Key.e_form]
-    df_metrics[model] = stable_metrics(df_preds[Key.each_true], each_pred)
-    most_stable_10k = each_pred.nsmallest(10_000)
-    df_metrics_10k[model] = stable_metrics(
-        df_preds[Key.each_true].loc[most_stable_10k.index], most_stable_10k
-    )
-    # DAF is only defined w.r.t. whole test set stability prevalence, stable_metrics()
-    # uses the stable prevalence of just the subset of predictions used to calculate the
-    # metrics
-    df_metrics_10k.loc["DAF", model] = df_metrics_10k[model]["Precision"] / prevalence
+    df_metrics[model] = stable_metrics(df_preds[Key.each_true], each_pred, fillna=True)
 
     df_uniq_proto_preds = df_preds[df_wbm[Key.uniq_proto]]
     each_pred_uniq_proto = (
         df_uniq_proto_preds[Key.each_true]
         + df_uniq_proto_preds[model]
         - df_uniq_proto_preds[Key.e_form]
     )
     df_metrics_uniq_protos[model] = stable_metrics(
-        df_uniq_proto_preds[Key.each_true], each_pred_uniq_proto
+        df_uniq_proto_preds[Key.each_true], each_pred_uniq_proto, fillna=True
+    )
+    df_metrics_uniq_protos.loc[Key.daf, model] = (
+        df_metrics_uniq_protos[model]["Precision"] / uniq_proto_prevalence
+    )
+
+    # look only at each model's 10k most stable predictions in the unique prototype set
+    most_stable_10k = each_pred_uniq_proto.nsmallest(10_000)
+    df_metrics_10k[model] = stable_metrics(
+        df_preds[Key.each_true].loc[most_stable_10k.index], most_stable_10k, fillna=True
+    )
+    df_metrics_10k.loc[Key.daf, model] = (
+        df_metrics_10k[model]["Precision"] / uniq_proto_prevalence
     )
 
 
 # pick F1 as primary metric to sort by
 df_metrics = df_metrics.round(3).sort_values("F1", axis=1, ascending=False)
 df_metrics_10k = df_metrics_10k.round(3).sort_values("F1", axis=1, ascending=False)
 df_metrics_uniq_protos = df_metrics_uniq_protos.round(3).sort_values(
@@ -235,19 +235,19 @@
 for model in models:
     df_each_pred[model] = (
         df_preds[Key.each_true] + df_preds[model] - df_preds[Key.e_form]
     )
 
 # important: do df_each_pred.std(axis=1) before inserting Key.model_mean_each into df
 df_preds[Key.model_std_each] = df_each_pred.std(axis=1)
-df_each_pred[Key.model_mean_each] = df_preds[Key.model_mean_each] = df_each_pred.mean(
+df_each_pred[Key.each_mean_models] = df_preds[Key.each_mean_models] = df_each_pred.mean(
     axis=1
 )
 
 # dataframe of all models' errors in their EACH predictions (eV/atom)
 df_each_err = pd.DataFrame()
 for model in models:
     df_each_err[model] = df_preds[model] - df_preds[Key.e_form]
 
-df_each_err[Key.model_mean_err] = df_preds[Key.model_mean_err] = df_each_err.abs().mean(
-    axis=1
+df_each_err[Key.each_err_models] = df_preds[Key.each_err_models] = (
+    df_each_err.abs().mean(axis=1)
 )
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery/slurm.py` & `matbench_discovery-1.1.2/matbench_discovery/slurm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from __future__ import annotations
+"""Slurm job submission helper function."""
 
 import os
 import subprocess
 import sys
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from collections.abc import Sequence
+from collections.abc import Sequence
 
 # taken from https://slurm.schedmd.com/job_array.html#env_vars, lower-cased and
 # and removed the SLURM_ prefix
 SLURM_KEYS = (
     "job_id array_job_id array_task_id array_task_count mem_per_node nodelist"
     "submit_host job_partition job_user job_account tasks_per_node job_qos"
 ).split()
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery/structure.py` & `matbench_discovery-1.1.2/matbench_discovery/structure.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import annotations
+"""Perturb atomic coordinates of a pymatgen structure.
 
-from typing import TYPE_CHECKING
+Used for CGCNN+P training set augmentation.
+"""
 
 import numpy as np
-
-if TYPE_CHECKING:
-    from pymatgen.core import Structure
+from pymatgen.core import Structure
 
 __author__ = "Janosh Riebesell"
 __date__ = "2022-12-02"
 
 rng = np.random.default_rng(0)  # ensure reproducible structure perturbations
 
 
@@ -47,15 +46,15 @@
 
     # reproduces the dist in https://www.nature.com/articles/s41524-022-00891-8#Fig5
     ax = plt.hist(samples, bins=100)
     # add vertical line at the mean
     plt.axvline(mean, color="gray", linestyle="dashed", linewidth=1)
     # annotate the mean line
     plt.annotate(
-        f"{mean = :.2f}",
+        f"{mean=:.2f}",
         xy=(mean, 1),
         # use ax coords for y
         xycoords=("data", "axes fraction"),
         # add text offset
         xytext=(10, -20),
         textcoords="offset points",
     )
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery.egg-info/PKG-INFO` & `matbench_discovery-1.1.2/matbench_discovery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matbench-discovery
-Version: 1.1.1
+Version: 1.1.2
 Summary: A benchmark for machine learning energy models on inorganic crystal stability prediction from unrelaxed structures
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,59 +42,60 @@
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: plotly
 Requires-Dist: pymatgen
 Requires-Dist: pymatviz[df-pdf-export,export-figs]
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
+Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: wandb
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: running-models
 Requires-Dist: alignn; extra == "running-models"
-Requires-Dist: chgnet; extra == "running-models"
+Requires-Dist: chgnet>=0.3.0; extra == "running-models"
 Requires-Dist: jarvis-tools; extra == "running-models"
 Requires-Dist: m3gnet; extra == "running-models"
 Requires-Dist: mace-torch; extra == "running-models"
 Requires-Dist: maml; extra == "running-models"
 Requires-Dist: megnet; extra == "running-models"
 Provides-Extra: 3d-structures
 Requires-Dist: crystaltoolkit; extra == "3d-structures"
 Provides-Extra: fetch-wbm-data
 Requires-Dist: gdown; extra == "fetch-wbm-data"
 Provides-Extra: make-wbm-umap
 Requires-Dist: umap-learn; extra == "make-wbm-umap"
 
-<h1 align="center">
+<h1 align="center" style="line-height: 0; margin: 0 auto 1em;">
   <img src="https://github.com/janosh/matbench-discovery/raw/main/site/static/favicon.svg" alt="Logo" width="60px"><br>
   Matbench Discovery
 </h1>
 
-<h4 align="center" class="toc-exclude">
+<h4 align="center" class="toc-exclude" style="display: none;">
 
 [![arXiv](https://img.shields.io/badge/arXiv-2308.14920-blue?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.14920)
 [![Tests](https://github.com/janosh/matbench-discovery/actions/workflows/test.yml/badge.svg)](https://github.com/janosh/matbench-discovery/actions/workflows/test.yml)
 [![GitHub Pages](https://github.com/janosh/matbench-discovery/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/janosh/matbench-discovery/actions/workflows/gh-pages.yml)
 [![Requires Python 3.11+](https://img.shields.io/badge/Python-3.11+-blue.svg?logo=python&logoColor=white)](https://python.org/downloads)
 [![PyPI](https://img.shields.io/pypi/v/matbench-discovery?logo=pypi&logoColor=white)](https://pypi.org/project/matbench-discovery?logo=pypi&logoColor=white)
 
 </h4>
 
-> TL;DR: We benchmark ML models on crystal stability prediction from unrelaxed structures finding universal interatomic potentials (UIP) like [CHGNet](https://github.com/CederGroupHub/chgnet), [MACE](https://github.com/ACEsuit/mace) and [M3GNet](https://github.com/materialsvirtuallab/m3gnet) to be highly accurate, robust across chemistries and ready for production use in high-throughput materials discovery.
+> Disclaimer: We evaluate how accurately ML models predict solid-state thermodynamic stability. Although this is an important aspect of high-throughput materials discovery, the ranking cannot give a complete picture of a model's general applicability to materials. A high ranking does not constitute endorsement by the Materials Project.
 
 Matbench Discovery is an [interactive leaderboard](https://janosh.github.io/matbench-discovery/models) and associated [PyPI package](https://pypi.org/project/matbench-discovery) which together make it easy to rank ML energy models on a task designed to simulate a high-throughput discovery campaign for new stable inorganic crystals.
 
 We've tested <slot name="model-count" />models covering multiple methodologies ranging from random forests with structure fingerprints to graph neural networks, from one-shot predictors to iterative Bayesian optimizers and interatomic potential relaxers.
 
 <slot name="best-report" />
 
 Our results show that ML models have become robust enough to deploy them as triaging steps to more effectively allocate compute in high-throughput DFT relaxations. This work provides valuable insights for anyone looking to build large-scale materials databases.
 
 <slot name="metrics-table" />
 
 We welcome contributions that add new models to the leaderboard through GitHub PRs. See the [contributing guide](https://janosh.github.io/matbench-discovery/contribute) for details.
 
-If you're interested in joining this work, feel free to [open a GitHub discussion](https://github.com/janosh/matbench-discovery/discussions) or [send an email](mailto:janosh.riebesell@gmail.gov?subject=Collaborate%20on%20Matbench%20Discovery).
+If you're interested in joining this work, please reach out via [GitHub discussion](https://github.com/janosh/matbench-discovery/discussions) or [email](mailto:janosh.riebesell@gmail.com?subject=Collaborate%20on%20Matbench%20Discovery).
 
 For detailed results and analysis, check out the [preprint](https://janosh.github.io/matbench-discovery/preprint).
```

### Comparing `matbench-discovery-1.1.1/matbench_discovery.egg-info/SOURCES.txt` & `matbench_discovery-1.1.2/matbench_discovery.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 license
 pyproject.toml
 readme.md
 matbench_discovery/__init__.py
 matbench_discovery/data.py
 matbench_discovery/energy.py
+matbench_discovery/enums.py
 matbench_discovery/metrics.py
 matbench_discovery/models.py
 matbench_discovery/plots.py
 matbench_discovery/preds.py
 matbench_discovery/slurm.py
 matbench_discovery/structure.py
 matbench_discovery.egg-info/PKG-INFO
@@ -15,14 +16,15 @@
 matbench_discovery.egg-info/dependency_links.txt
 matbench_discovery.egg-info/requires.txt
 matbench_discovery.egg-info/top_level.txt
 matbench_discovery/figshare/1.0.0.json
 matbench_discovery/figshare/readme.md
 tests/test_data.py
 tests/test_energy.py
+tests/test_enums.py
 tests/test_init.py
 tests/test_metrics.py
 tests/test_models.py
 tests/test_plots.py
 tests/test_preds.py
 tests/test_slurm.py
 tests/test_structure.py
```

### Comparing `matbench-discovery-1.1.1/pyproject.toml` & `matbench_discovery-1.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "matbench-discovery"
-version = "1.1.1"
+version = "1.1.2"
 description = "A benchmark for machine learning energy models on inorganic crystal stability prediction from unrelaxed structures"
 authors = [{ name = "Janosh Riebesell", email = "janosh.riebesell@gmail.com" }]
 readme = "readme.md"
 license = { file = "license" }
 keywords = [
   "Bayesian optimization",
   "convex hull",
@@ -33,14 +33,15 @@
   "numpy",
   "pandas>=2.0.0",
   "plotly",
   "pymatgen",
   "pymatviz[export-figs,df-pdf-export]",
   "scikit-learn",
   "scipy",
+  "seaborn",
   "tqdm",
   "wandb",
 ]
 
 [project.urls]
 Homepage = "https://janosh.github.io/matbench-discovery"
 Repo = "https://github.com/janosh/matbench-discovery"
@@ -50,15 +51,15 @@
 test = ["pytest", "pytest-cov"]
 # how to specify git deps: https://stackoverflow.com/a/73572379
 running-models = [
   # aviary commented-out since dep on git repo raises "Invalid value for requires_dist"
   # when attempting PyPI publish
   # "aviary@git+https://github.com/CompRhys/aviary",
   "alignn",
-  "chgnet",
+  "chgnet>=0.3.0",
   "jarvis-tools",
   "m3gnet",
   "mace-torch",
   "maml",
   "megnet",
 ]
 3d-structures = ["crystaltoolkit"]
@@ -72,32 +73,34 @@
 [tool.setuptools.package-data]
 matbench_discovery = ["figshare/*"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.ruff]
-target-version = "py39"
+target-version = "py311"
+
+[tool.ruff.lint]
 select = ["ALL"]
 ignore = [
   "ANN101",
+  "ANN102",
   "ANN401",
+  "B905",    # zip without explicit strict
   "BLE001",
   "C408",    # unnecessary-collection-call
   "C901",
   "COM812",
-  "D100",    # undocumented-public-module
   "D205",    # blank-line-after-summary
-  "DTZ005",
   "E731",    # lambda-assignment
+  "EM101",
   "EM102",
-  "FBT001",
-  "FBT002",
   "FIX002",
   "INP001",
+  "ISC001",
   "N806",    # non-lowercase-variable-in-function
   "PD901",   # pandas-df-variable-name
   "PERF203", # try-except-in-loop
   "PLC0414", # useless-import-alias
   "PLR",     # pylint refactor
   "PLW2901", # redefined-loop-name
   "PT006",   # pytest-parametrize-names-wrong-type
@@ -113,18 +116,18 @@
   "TRY003",
   "TRY301",
 ]
 pydocstyle.convention = "google"
 isort.known-third-party = ["wandb"]
 isort.split-on-trailing-comma = false
 
-[tool.ruff.per-file-ignores]
-"tests/*" = ["D", "S101"]
-"matbench_discovery/plots.py" = ["ERA001"] # allow commented out code
-"matbench_discovery/preds.py" = ["ERA001"] # allow commented out code
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = ["D", "FBT001", "FBT002", "S101"]
+"matbench_discovery/plots.py" = ["ERA001"]    # allow commented out code
+"matbench_discovery/preds.py" = ["ERA001"]    # allow commented out code
 "scripts/*" = ["D", "ERA001", "S101"]
 "models/*" = ["D", "ERA001", "S101"]
 "data/*" = ["ERA001", "S101"]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_untyped_defs = true
@@ -139,7 +142,13 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-p no:warnings -m 'not slow and not very_slow'"
 markers = [
   "slow: deselect slow tests with -m 'not slow'",
   "very_slow: select with -m 'very_slow'",
 ]
+
+[tool.pyright]
+typeCheckingMode = "off"
+reportPossiblyUnboundVariable = true
+reportUnboundVariable = true
+reportMissingImports = false
```

### Comparing `matbench-discovery-1.1.1/readme.md` & `matbench_discovery-1.1.2/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-<h1 align="center">
+<h1 align="center" style="line-height: 0; margin: 0 auto 1em;">
   <img src="https://github.com/janosh/matbench-discovery/raw/main/site/static/favicon.svg" alt="Logo" width="60px"><br>
   Matbench Discovery
 </h1>
 
-<h4 align="center" class="toc-exclude">
+<h4 align="center" class="toc-exclude" style="display: none;">
 
 [![arXiv](https://img.shields.io/badge/arXiv-2308.14920-blue?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.14920)
 [![Tests](https://github.com/janosh/matbench-discovery/actions/workflows/test.yml/badge.svg)](https://github.com/janosh/matbench-discovery/actions/workflows/test.yml)
 [![GitHub Pages](https://github.com/janosh/matbench-discovery/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/janosh/matbench-discovery/actions/workflows/gh-pages.yml)
 [![Requires Python 3.11+](https://img.shields.io/badge/Python-3.11+-blue.svg?logo=python&logoColor=white)](https://python.org/downloads)
 [![PyPI](https://img.shields.io/pypi/v/matbench-discovery?logo=pypi&logoColor=white)](https://pypi.org/project/matbench-discovery?logo=pypi&logoColor=white)
 
 </h4>
 
-> TL;DR: We benchmark ML models on crystal stability prediction from unrelaxed structures finding universal interatomic potentials (UIP) like [CHGNet](https://github.com/CederGroupHub/chgnet), [MACE](https://github.com/ACEsuit/mace) and [M3GNet](https://github.com/materialsvirtuallab/m3gnet) to be highly accurate, robust across chemistries and ready for production use in high-throughput materials discovery.
+> Disclaimer: We evaluate how accurately ML models predict solid-state thermodynamic stability. Although this is an important aspect of high-throughput materials discovery, the ranking cannot give a complete picture of a model's general applicability to materials. A high ranking does not constitute endorsement by the Materials Project.
 
 Matbench Discovery is an [interactive leaderboard](https://janosh.github.io/matbench-discovery/models) and associated [PyPI package](https://pypi.org/project/matbench-discovery) which together make it easy to rank ML energy models on a task designed to simulate a high-throughput discovery campaign for new stable inorganic crystals.
 
 We've tested <slot name="model-count" />models covering multiple methodologies ranging from random forests with structure fingerprints to graph neural networks, from one-shot predictors to iterative Bayesian optimizers and interatomic potential relaxers.
 
 <slot name="best-report" />
 
 Our results show that ML models have become robust enough to deploy them as triaging steps to more effectively allocate compute in high-throughput DFT relaxations. This work provides valuable insights for anyone looking to build large-scale materials databases.
 
 <slot name="metrics-table" />
 
 We welcome contributions that add new models to the leaderboard through GitHub PRs. See the [contributing guide](https://janosh.github.io/matbench-discovery/contribute) for details.
 
-If you're interested in joining this work, feel free to [open a GitHub discussion](https://github.com/janosh/matbench-discovery/discussions) or [send an email](mailto:janosh.riebesell@gmail.gov?subject=Collaborate%20on%20Matbench%20Discovery).
+If you're interested in joining this work, please reach out via [GitHub discussion](https://github.com/janosh/matbench-discovery/discussions) or [email](mailto:janosh.riebesell@gmail.com?subject=Collaborate%20on%20Matbench%20Discovery).
 
 For detailed results and analysis, check out the [preprint](https://janosh.github.io/matbench-discovery/preprint).
```

### Comparing `matbench-discovery-1.1.1/tests/test_data.py` & `matbench_discovery-1.1.2/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-from __future__ import annotations
-
 import json
 import os
+from pathlib import Path
 from random import random
-from typing import TYPE_CHECKING, Any
+from typing import Any
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
 from pymatgen.core import Lattice, Structure
 from pytest import CaptureFixture
 
-from matbench_discovery import FIGSHARE_DIR, ROOT, Key
+from matbench_discovery import FIGSHARE_DIR, ROOT
 from matbench_discovery.data import (
     DATA_FILES,
     as_dict_handler,
     df_wbm,
     figshare_versions,
     glob_to_df,
     load,
 )
-
-if TYPE_CHECKING:
-    from pathlib import Path
-
+from matbench_discovery.enums import Key
 
 with open(f"{FIGSHARE_DIR}/{figshare_versions[-1]}.json") as file:
     figshare_urls = json.load(file)["files"]
 
 structure = Structure(
     lattice=Lattice.cubic(5),
     species=("Fe", "O"),
```

### Comparing `matbench-discovery-1.1.1/tests/test_energy.py` & `matbench_discovery-1.1.2/tests/test_energy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from __future__ import annotations
-
-from typing import Any, Callable
+from collections.abc import Callable
+from typing import Any
 
 import pytest
 from pymatgen.analysis.phase_diagram import PDEntry
 from pymatgen.core import Lattice, Structure
 from pymatgen.entries.computed_entries import ComputedEntry, Entry
 from pytest import approx
```

### Comparing `matbench-discovery-1.1.1/tests/test_metrics.py` & `matbench_discovery-1.1.2/tests/test_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from __future__ import annotations
-
 import math
-from typing import TYPE_CHECKING
 
 import numpy as np
+import pandas as pd
 import pytest
 from pytest import approx
 
+from matbench_discovery.enums import Key
 from matbench_discovery.metrics import classify_stable, stable_metrics
 
-if TYPE_CHECKING:
-    import pandas as pd
-
 
 @pytest.mark.parametrize(
     "stability_threshold, expected",
     [(-0.1, (2, 4, 3, 1)), (0, (2, 4, 3, 1)), (0.1, (4, 3, 2, 1))],
 )
 def test_classify_stable(
     stability_threshold: float,
@@ -34,15 +30,15 @@
     assert (n_true_pos, n_false_neg, n_false_pos, n_true_neg) == expected
     assert n_true_pos + n_false_neg + n_false_pos + n_true_neg == len(df_float)
     assert n_true_neg + n_false_pos == sum(stability_threshold < df_float.A)
     assert n_true_pos + n_false_neg == sum(stability_threshold >= df_float.A)
 
 
 def test_stable_metrics() -> None:
-    metrics = stable_metrics(np.arange(-1, 1, 0.1), np.arange(1, -1, -0.1))
+    metrics = stable_metrics(np.arange(-1, 1, 0.1), np.arange(1, -1, -0.1), fillna=True)
     for key, val in dict(
         DAF=0,
         Precision=0,
         Recall=0,
         Accuracy=0,
         TPR=0,
         FPR=1,
@@ -52,19 +48,37 @@
         RMSE=1.157,
         R2=-3.030,
     ).items():
         assert metrics[key] == approx(val, abs=1e-3), f"{key=}"
 
     assert math.isnan(metrics["F1"])
 
+    metrics = stable_metrics(
+        np.array((-1, 1, 0.1, -0.5, 0.5)),
+        np.array((-1, 1, -0.1, np.nan, np.nan)),
+        fillna=False,
+    )
+    fillna_metrics = stable_metrics(
+        np.array((-1, 1, 0.1, -0.5, 0.5)),
+        np.array((-1, 1, -0.1, np.nan, np.nan)),
+        fillna=True,
+    )
+
+    assert metrics["Precision"] == fillna_metrics["Precision"]
+    assert metrics["DAF"] > fillna_metrics["DAF"]  # nan's dropped in prevalence
+    assert metrics["TNR"] == 0.5
+    assert metrics["FNR"] == 0
+    assert fillna_metrics["TNR"] == 2 / 3
+    assert fillna_metrics["FNR"] == 1 / 2
+
     # test stable_metrics gives the same result as sklearn.metrics.classification_report
     # for random numpy data
     rng = np.random.default_rng(0)
     y_true, y_pred = rng.normal(size=(2, 100))
-    metrics = stable_metrics(y_true, y_pred)
+    metrics = stable_metrics(y_true, y_pred, fillna=True)
 
     from sklearn.metrics import classification_report
 
     skl_report = classification_report(y_true > 0, y_pred > 0, output_dict=True)
 
     assert metrics["Precision"] == pytest.approx(skl_report["False"]["precision"])
     assert metrics["Recall"] == pytest.approx(skl_report["False"]["recall"])
@@ -80,15 +94,15 @@
 
     # test stable_metrics docstring is up to date, all returned metrics should be listed
     assert stable_metrics.__doc__  # for mypy
     assert all(key in stable_metrics.__doc__ for key in metrics)
 
     # test discovery acceleration factor (DAF)
     n_true_pos, n_false_neg, n_false_pos, n_true_neg = map(
-        sum, classify_stable(y_true, y_pred)
+        sum, classify_stable(y_true, y_pred, fillna=True)
     )
 
     dummy_hit_rate = (n_true_pos + n_false_neg) / (
         n_true_pos + n_false_pos + n_false_neg + n_true_neg
     )
     precision = n_true_pos / (n_true_pos + n_false_pos)
-    assert metrics["DAF"] == precision / dummy_hit_rate
+    assert metrics[Key.daf] == precision / dummy_hit_rate
```

### Comparing `matbench-discovery-1.1.1/tests/test_models.py` & `matbench_discovery-1.1.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `matbench-discovery-1.1.1/tests/test_plots.py` & `matbench_discovery-1.1.2/tests/test_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from __future__ import annotations
-
 from typing import Literal
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import plotly.graph_objects as go
 import pytest
 
-from matbench_discovery import Key
+from matbench_discovery.enums import Key
 from matbench_discovery.plots import (
     Backend,
     cumulative_metrics,
     hist_classified_stable_vs_hull_dist,
     plotly_line_styles,
     plotly_markers,
     rolling_mae_vs_hull_dist,
 )
 from matbench_discovery.preds import load_df_wbm_with_preds
 
 AxLine = Literal["x", "y", "xy", ""]
 models = ["MEGNet", "CGCNN", "Voronoi RF"]
-df_wbm = load_df_wbm_with_preds(models, nrows=100)
+df_wbm = load_df_wbm_with_preds(models=models, nrows=100)
 
 
 @pytest.mark.parametrize(
     "project_end_point,stability_threshold",
     [("", 0), ("x", 0), ("x", -0.05), ("xy", 0.1)],
 )
 @pytest.mark.parametrize("backend", ["matplotlib", "plotly"])
@@ -85,35 +83,34 @@
     show_dft_acc: bool,
 ) -> None:
     kwargs = dict(window=window, bin_width=bin_width, backend=backend)
     if backend == "matplotlib":
         ax = plt.figure().gca()  # new figure ensures test functions use different axes
         kwargs["ax"] = ax
 
-    for model_name in models:
-        ax, df_err, df_std = rolling_mae_vs_hull_dist(
-            e_above_hull_true=df_wbm[model_name],
-            e_above_hull_errors=df_wbm[models],
-            x_lim=x_lim,
-            show_dft_acc=show_dft_acc,
-            **kwargs,  # type: ignore[arg-type]
-        )
+    ax, df_err, df_std = rolling_mae_vs_hull_dist(
+        e_above_hull_true=df_wbm[models[0]],
+        e_above_hull_preds=df_wbm[models],
+        x_lim=x_lim,
+        show_dft_acc=show_dft_acc,
+        **kwargs,  # type: ignore[arg-type]
+    )
 
     assert isinstance(df_err, pd.DataFrame)
     assert isinstance(df_std, pd.DataFrame)
     assert (
         list(df_err) == list(df_std) == models
     ), f"expected {list(df_err)} == {list(df_std)} == {models}"
 
-    expected_ylabel = "rolling MAE (eV/atom)"
+    expected_ylabel = "Rolling MAE (eV/atom)"
     if backend == "matplotlib":
         assert isinstance(ax, plt.Axes)
         assert ax.get_ylim()[0] == 0
         assert ax.get_ylabel() == expected_ylabel
-        assert ax.get_xlabel() == r"$E_\mathrm{above\ hull}$ (eV/atom)"
+        assert ax.get_xlabel() == r"$E_\mathrm{above\ MP\ hull}$ (eV/atom)"
     elif backend == "plotly":
         assert isinstance(ax, go.Figure)
         assert ax.layout.yaxis.title.text == expected_ylabel
         assert ax.layout.xaxis.title.text == "E<sub>above MP hull</sub> (eV/atom)"
 
 
 @pytest.mark.parametrize("stability_threshold", [0.1, 0.01])
```

### Comparing `matbench-discovery-1.1.1/tests/test_preds.py` & `matbench_discovery-1.1.2/tests/test_preds.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import pytest
 
-from matbench_discovery import Key
 from matbench_discovery.data import df_wbm
+from matbench_discovery.enums import Key
 from matbench_discovery.preds import (
     PRED_FILES,
     df_each_err,
     df_each_pred,
     df_metrics,
     load_df_wbm_with_preds,
 )
@@ -26,31 +26,31 @@
     assert df_metrics.isna().sum().sum() == 0, "NaNs in metrics"
 
 
 def test_df_each_pred() -> None:
     assert len(df_each_pred) == len(df_wbm)
     assert {*df_each_pred} == {
         *df_metrics,
-        Key.model_mean_each,
+        Key.each_mean_models,
     }, "df_each_pred has wrong columns"
     assert all(df_each_pred.isna().mean() < 0.05), "too many NaNs in df_each_pred"
 
 
 def test_df_each_err() -> None:
     assert len(df_each_err) == len(df_wbm)
     assert {*df_each_err} == {
         *df_metrics,
-        Key.model_mean_err,
+        Key.each_err_models,
     }, "df_each_err has wrong columns"
     assert all(df_each_err.isna().mean() < 0.05), "too many NaNs in df_each_err"
 
 
 @pytest.mark.parametrize("models", [[], ["Wrenformer"]])
 def test_load_df_wbm_with_preds(models: list[str]) -> None:
-    df = load_df_wbm_with_preds(models)
+    df = load_df_wbm_with_preds(models=models)
     assert len(df) == len(df_wbm)
     assert list(df) == list(df_wbm) + models + [f"{model}_std" for model in models]
     assert df.index.name == Key.mat_id
 
     for model_name in models:
         assert model_name in df
         assert df[model_name].isna().sum() == 0
```

### Comparing `matbench-discovery-1.1.1/tests/test_slurm.py` & `matbench_discovery-1.1.2/tests/test_slurm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import os
 from unittest.mock import patch
 
 import pytest
 from pytest import CaptureFixture
 
 from matbench_discovery.slurm import _get_calling_file_path, slurm_submit
@@ -16,39 +14,41 @@
     capsys: CaptureFixture[str], py_file_path: str | None, partition: str | None
 ) -> None:
     job_name = "test_job"
     out_dir = "tmp"
     time = "0:0:1"
     account = "fake-account"
 
-    func_call = lambda: slurm_submit(
+    kwargs = dict(
         job_name=job_name,
         out_dir=out_dir,
         time=time,
         partition=partition,
         account=account,
         py_file_path=py_file_path,
         slurm_flags="--foo",
     )
 
-    slurm_vars = func_call()
+    slurm_vars = slurm_submit(**kwargs)  # type: ignore[arg-type]
 
     assert slurm_vars == dict(
         slurm_job_id="1234", slurm_timelimit="0:0:1", slurm_flags="--foo"
     )
 
     stdout, stderr = capsys.readouterr()
     # check slurm_submit() did nothing in normal mode
     assert stderr == stderr == ""
 
     # check slurm_submit() prints cmd and calls subprocess.run() in submit mode
-    with pytest.raises(SystemExit), patch("sys.argv", ["slurm-submit"]), patch(
-        "matbench_discovery.slurm.subprocess.run"
-    ) as mock_subprocess_run:
-        func_call()
+    with (
+        pytest.raises(SystemExit),
+        patch("sys.argv", ["slurm-submit"]),
+        patch("matbench_discovery.slurm.subprocess.run") as mock_subprocess_run,
+    ):
+        slurm_submit(**kwargs)  # type: ignore[arg-type]
 
     assert mock_subprocess_run.call_count == 1
 
     sbatch_cmd = (
         f"sbatch --account={account} --time={time} "
         f"--job-name {job_name} --output {out_dir}/slurm-%A.log --foo "
         f"--wrap python {py_file_path or __file__}"
```

### Comparing `matbench-discovery-1.1.1/tests/test_structure.py` & `matbench_discovery-1.1.2/tests/test_structure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
+from pymatgen.core import Structure
 
 from matbench_discovery.structure import perturb_structure
 
-if TYPE_CHECKING:
-    from pymatgen.core import Structure
-
 
 def test_perturb_structure(dummy_struct: Structure) -> None:
     perturbed = perturb_structure(dummy_struct)
     assert len(perturbed) == len(dummy_struct)
 
-    for site, new in zip(dummy_struct, perturbed):
+    for site, new in zip(dummy_struct, perturbed, strict=True):
         assert site.specie == new.specie
         assert tuple(site.coords) != tuple(new.coords)
 
     # but different on subsequent calls
     assert perturb_structure(dummy_struct) != perturb_structure(dummy_struct)
```

