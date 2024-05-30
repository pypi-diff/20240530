# Comparing `tmp/graphe-0.0.2.tar.gz` & `tmp/graphe-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphe-0.0.2.tar", last modified: Wed Jun 28 11:35:05 2023, max compression
+gzip compressed data, was "graphe-0.1.0.tar", last modified: Thu May 30 10:48:17 2024, max compression
```

## Comparing `graphe-0.0.2.tar` & `graphe-0.1.0.tar`

### file list

```diff
@@ -1,95 +1,98 @@
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.137782 graphe-0.0.2/
--rw-r--r--   0 mortenchristensen (640641318) 14964212       66 2023-01-05 15:40:14.000000 graphe-0.0.2/.gitignore
--rw-r--r--   0 mortenchristensen (640641318) 14964212      742 2023-01-14 14:12:06.000000 graphe-0.0.2/.readthedocs.yaml
--rw-r--r--   0 mortenchristensen (640641318) 14964212     1316 2022-12-31 07:26:15.000000 graphe-0.0.2/LICENSE
--rw-r--r--   0 mortenchristensen (640641318) 14964212      934 2023-06-28 11:35:05.137102 graphe-0.0.2/PKG-INFO
--rw-r--r--   0 mortenchristensen (640641318) 14964212      325 2023-01-14 14:07:05.000000 graphe-0.0.2/README.md
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.071722 graphe-0.0.2/data/
--rw-r--r--   0 mortenchristensen (640641318) 14964212      407 2023-01-11 15:22:52.000000 graphe-0.0.2/data/jobs.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212     9107 2022-12-26 21:16:26.000000 graphe-0.0.2/data/mediumG.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212       29 2023-06-28 10:06:18.000000 graphe-0.0.2/data/rosalind_tree.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212      144 2023-01-01 21:07:05.000000 graphe-0.0.2/data/routes.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212       97 2023-01-08 12:50:20.000000 graphe-0.0.2/data/scc.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212      326 2023-01-09 11:02:29.000000 graphe-0.0.2/data/test.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212       71 2023-01-08 19:42:36.000000 graphe-0.0.2/data/tinyDAG.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212      138 2023-01-02 21:07:13.000000 graphe-0.0.2/data/tinyDG.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212       63 2022-12-26 20:07:32.000000 graphe-0.0.2/data/tinyG.txt
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.072638 graphe-0.0.2/docs/
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.073767 graphe-0.0.2/docs/docs/
--rw-r--r--   0 mortenchristensen (640641318) 14964212      638 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/Makefile
--rw-r--r--   0 mortenchristensen (640641318) 14964212      804 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/make.bat
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.080395 graphe-0.0.2/docs/docs/source/
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.081162 graphe-0.0.2/docs/docs/source/_static/
--rw-r--r--   0 mortenchristensen (640641318) 14964212       64 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/_static/custom.css
--rw-r--r--   0 mortenchristensen (640641318) 14964212     1115 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/conf.py
--rw-r--r--   0 mortenchristensen (640641318) 14964212     3192 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/digraph.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212     1394 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/digraphappl.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212     1634 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/files.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212     2150 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/graph.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212      117 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/graphappl.rst
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.094368 graphe-0.0.2/docs/docs/source/images/
--rw-r--r--   0 mortenchristensen (640641318) 14964212   157842 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/digraph_dfs.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212   117680 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/digraph_loop.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212   163006 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/graph.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212   167961 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/long.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212    29510 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/node_names.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212   164521 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/short.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212    29454 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/symbol_graph_bfs.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212    51917 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/images/symbolg.png
--rw-r--r--   0 mortenchristensen (640641318) 14964212      910 2023-01-14 14:16:12.000000 graphe-0.0.2/docs/docs/source/index.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212      252 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/install.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212     3112 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/usage.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212      985 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/docs/source/utils.rst
--rw-r--r--   0 mortenchristensen (640641318) 14964212      227 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/pyproject.toml
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.095839 graphe-0.0.2/docs/scripts/
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212       63 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/scripts/localbuild
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212       45 2023-01-14 14:04:31.000000 graphe-0.0.2/docs/scripts/view
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.107444 graphe-0.0.2/examples/
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      293 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/bfs.py
--rw-r--r--   0 mortenchristensen (640641318) 14964212      256 2023-06-28 10:36:24.000000 graphe-0.0.2/examples/cc.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      359 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/dfs.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      250 2023-01-13 22:56:03.000000 graphe-0.0.2/examples/digraph.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      494 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/directeddfs.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      225 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/graph.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      325 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/node_names.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      993 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/regex.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      349 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/symbol_graph.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      467 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/symbol_graph_bfs.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      343 2023-01-13 22:46:32.000000 graphe-0.0.2/examples/topological_sort.py
--rw-r--r--   0 mortenchristensen (640641318) 14964212      767 2023-06-28 09:43:09.000000 graphe-0.0.2/pyproject.toml
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.108888 graphe-0.0.2/scripts/
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      118 2023-01-13 22:46:32.000000 graphe-0.0.2/scripts/coverage
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      134 2023-06-28 11:31:29.000000 graphe-0.0.2/scripts/publish
--rw-r--r--   0 mortenchristensen (640641318) 14964212       38 2023-06-28 11:35:05.138019 graphe-0.0.2/setup.cfg
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.061450 graphe-0.0.2/src/
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.110126 graphe-0.0.2/src/graphe/
--rw-r--r--   0 mortenchristensen (640641318) 14964212        0 2022-12-31 07:15:14.000000 graphe-0.0.2/src/graphe/__init__.py
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.124498 graphe-0.0.2/src/graphe/digraph/
--rw-r--r--   0 mortenchristensen (640641318) 14964212        0 2023-01-11 14:39:13.000000 graphe-0.0.2/src/graphe/digraph/__init__.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212     1132 2023-01-13 22:46:32.000000 graphe-0.0.2/src/graphe/digraph/cycle.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212     2044 2023-01-13 22:46:32.000000 graphe-0.0.2/src/graphe/digraph/ddfo.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212     1078 2023-01-11 22:19:37.000000 graphe-0.0.2/src/graphe/digraph/digraph.py
--rw-r--r--   0 mortenchristensen (640641318) 14964212     1296 2023-01-13 22:46:32.000000 graphe-0.0.2/src/graphe/digraph/digraphdfs.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212     1078 2023-01-13 22:46:32.000000 graphe-0.0.2/src/graphe/digraph/ksscc.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212     3140 2023-01-13 22:46:32.000000 graphe-0.0.2/src/graphe/digraph/regex.py
--rw-r--r--   0 mortenchristensen (640641318) 14964212     1149 2023-01-13 22:46:32.000000 graphe-0.0.2/src/graphe/digraph/symboldigraph.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      901 2023-01-13 22:46:32.000000 graphe-0.0.2/src/graphe/digraph/topological.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212     1639 2023-01-13 22:52:41.000000 graphe-0.0.2/src/graphe/draw.py
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.128613 graphe-0.0.2/src/graphe/graph/
--rw-r--r--   0 mortenchristensen (640641318) 14964212        0 2023-01-11 14:39:18.000000 graphe-0.0.2/src/graphe/graph/__init__.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      988 2023-01-05 11:11:11.000000 graphe-0.0.2/src/graphe/graph/bfs.py
--rw-r--r--   0 mortenchristensen (640641318) 14964212      681 2023-06-28 10:30:58.000000 graphe-0.0.2/src/graphe/graph/cc.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      822 2023-01-11 14:56:38.000000 graphe-0.0.2/src/graphe/graph/dfs.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      923 2023-01-11 16:02:31.000000 graphe-0.0.2/src/graphe/graph/graph.py
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.116058 graphe-0.0.2/src/graphe.egg-info/
--rw-r--r--   0 mortenchristensen (640641318) 14964212      934 2023-06-28 11:35:04.000000 graphe-0.0.2/src/graphe.egg-info/PKG-INFO
--rw-r--r--   0 mortenchristensen (640641318) 14964212     1894 2023-06-28 11:35:05.000000 graphe-0.0.2/src/graphe.egg-info/SOURCES.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212        1 2023-06-28 11:35:04.000000 graphe-0.0.2/src/graphe.egg-info/dependency_links.txt
--rw-r--r--   0 mortenchristensen (640641318) 14964212        7 2023-06-28 11:35:04.000000 graphe-0.0.2/src/graphe.egg-info/top_level.txt
-drwxr-xr-x   0 mortenchristensen (640641318) 14964212        0 2023-06-28 11:35:05.136245 graphe-0.0.2/tests/
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      857 2023-01-13 22:46:32.000000 graphe-0.0.2/tests/test_bfs.py
--rw-r--r--   0 mortenchristensen (640641318) 14964212      634 2023-01-13 22:46:32.000000 graphe-0.0.2/tests/test_cycle.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      858 2023-01-13 22:46:32.000000 graphe-0.0.2/tests/test_dfs.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      966 2023-01-13 22:46:32.000000 graphe-0.0.2/tests/test_digraph.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      710 2023-01-13 22:46:32.000000 graphe-0.0.2/tests/test_digraphdfs.py
--rwxr-xr-x   0 mortenchristensen (640641318) 14964212      362 2023-01-13 22:46:32.000000 graphe-0.0.2/tests/test_graph.py
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.973187 graphe-0.1.0/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       66 2023-01-05 15:40:14.000000 graphe-0.1.0/.gitignore
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      742 2023-01-14 14:12:06.000000 graphe-0.1.0/.readthedocs.yaml
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1316 2022-12-31 07:26:15.000000 graphe-0.1.0/LICENSE
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      934 2024-05-30 10:48:17.972207 graphe-0.1.0/PKG-INFO
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      325 2023-01-14 14:07:05.000000 graphe-0.1.0/README.md
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.911299 graphe-0.1.0/data/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      407 2023-01-11 15:22:52.000000 graphe-0.1.0/data/jobs.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     9107 2022-12-26 21:16:26.000000 graphe-0.1.0/data/mediumG.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       29 2023-06-28 10:06:18.000000 graphe-0.1.0/data/rosalind_tree.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      144 2023-01-01 21:07:05.000000 graphe-0.1.0/data/routes.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       97 2023-01-08 12:50:20.000000 graphe-0.1.0/data/scc.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      326 2023-01-09 11:02:29.000000 graphe-0.1.0/data/test.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       71 2023-01-08 19:42:36.000000 graphe-0.1.0/data/tinyDAG.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      138 2023-01-02 21:07:13.000000 graphe-0.1.0/data/tinyDG.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       63 2022-12-26 20:07:32.000000 graphe-0.1.0/data/tinyG.txt
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.912017 graphe-0.1.0/docs/
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.913511 graphe-0.1.0/docs/docs/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      638 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/Makefile
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      804 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/make.bat
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.920658 graphe-0.1.0/docs/docs/source/
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.921360 graphe-0.1.0/docs/docs/source/_static/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       64 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/_static/custom.css
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1115 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/conf.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     3192 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/digraph.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1394 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/digraphappl.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1634 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/files.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     2150 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/graph.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      117 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/graphappl.rst
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.930469 graphe-0.1.0/docs/docs/source/images/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)   157842 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/digraph_dfs.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)   117680 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/digraph_loop.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)   163006 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/graph.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)   167961 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/long.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)    29510 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/node_names.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)   164521 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/short.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)    29454 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/symbol_graph_bfs.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)    51917 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/images/symbolg.png
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      910 2023-01-14 14:16:12.000000 graphe-0.1.0/docs/docs/source/index.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      252 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/install.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     3112 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/usage.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      985 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/docs/source/utils.rst
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      227 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/pyproject.toml
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.932453 graphe-0.1.0/docs/scripts/
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       63 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/scripts/localbuild
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       45 2023-01-14 14:04:31.000000 graphe-0.1.0/docs/scripts/view
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.942090 graphe-0.1.0/examples/
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      293 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/bfs.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      256 2023-06-28 10:36:24.000000 graphe-0.1.0/examples/cc.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      359 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/dfs.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      250 2023-01-13 22:56:03.000000 graphe-0.1.0/examples/digraph.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      494 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/directeddfs.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      225 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/graph.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      325 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/node_names.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      993 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/regex.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      349 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/symbol_graph.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      467 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/symbol_graph_bfs.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      343 2023-01-13 22:46:32.000000 graphe-0.1.0/examples/topological_sort.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      767 2024-05-30 10:48:02.000000 graphe-0.1.0/pyproject.toml
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.945007 graphe-0.1.0/scripts/
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      107 2024-05-30 10:29:54.000000 graphe-0.1.0/scripts/blackcheck
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       77 2024-05-30 10:26:57.000000 graphe-0.1.0/scripts/blackrun
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      118 2023-01-13 22:46:32.000000 graphe-0.1.0/scripts/coverage
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      206 2023-06-28 11:35:48.000000 graphe-0.1.0/scripts/publish
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)       38 2024-05-30 10:48:17.973386 graphe-0.1.0/setup.cfg
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.900971 graphe-0.1.0/src/
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.946459 graphe-0.1.0/src/graphe/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2022-12-31 07:15:14.000000 graphe-0.1.0/src/graphe/__init__.py
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.958734 graphe-0.1.0/src/graphe/digraph/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2023-01-11 14:39:13.000000 graphe-0.1.0/src/graphe/digraph/__init__.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1128 2024-05-29 11:57:11.000000 graphe-0.1.0/src/graphe/digraph/cycle.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     2033 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/digraph/ddfo.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1073 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/digraph/digraph.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1288 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/digraph/digraphdfs.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1071 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/digraph/ksscc.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     3150 2024-05-30 10:43:38.000000 graphe-0.1.0/src/graphe/digraph/regex.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1148 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/digraph/symboldigraph.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      898 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/digraph/topological.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1783 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/draw.py
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.962917 graphe-0.1.0/src/graphe/graph/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2023-01-11 14:39:18.000000 graphe-0.1.0/src/graphe/graph/__init__.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      983 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/graph/bfs.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      729 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/graph/cc.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      817 2024-05-30 10:30:10.000000 graphe-0.1.0/src/graphe/graph/dfs.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      920 2024-05-29 10:33:04.000000 graphe-0.1.0/src/graphe/graph/graph.py
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.970950 graphe-0.1.0/src/graphe.egg-info/
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      934 2024-05-30 10:48:17.000000 graphe-0.1.0/src/graphe.egg-info/PKG-INFO
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)     1950 2024-05-30 10:48:17.000000 graphe-0.1.0/src/graphe.egg-info/SOURCES.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        1 2024-05-30 10:48:17.000000 graphe-0.1.0/src/graphe.egg-info/dependency_links.txt
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        7 2024-05-30 10:48:17.000000 graphe-0.1.0/src/graphe.egg-info/top_level.txt
+drwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)        0 2024-05-30 10:48:17.969694 graphe-0.1.0/tests/
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      857 2023-01-13 22:46:32.000000 graphe-0.1.0/tests/test_bfs.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      634 2023-01-13 22:46:32.000000 graphe-0.1.0/tests/test_cycle.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      858 2023-01-13 22:46:32.000000 graphe-0.1.0/tests/test_dfs.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      966 2023-01-13 22:46:32.000000 graphe-0.1.0/tests/test_digraph.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      710 2023-01-13 22:46:32.000000 graphe-0.1.0/tests/test_digraphdfs.py
+-rwxr-xr-x   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      362 2023-01-13 22:46:32.000000 graphe-0.1.0/tests/test_graph.py
+-rw-r--r--   0 mortenchristensen (640641318) ESSS\Domain Users (14964212)      509 2024-05-30 10:45:20.000000 graphe-0.1.0/tests/test_regex.py
```

### Comparing `graphe-0.0.2/.readthedocs.yaml` & `graphe-0.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/LICENSE` & `graphe-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/PKG-INFO` & `graphe-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphe
-Version: 0.0.2
+Version: 0.1.0
 Summary: Collection of graph algorithms, applications and visualisations
 Author-email: Morten Jagd Christensen <mortenjc@jcaps.com>
 Project-URL: Homepage, https://github.com/mortenjc/graphe
 Project-URL: Documentation, https://graphe.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/mortenjc/graphe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `graphe-0.0.2/data/mediumG.txt` & `graphe-0.1.0/data/mediumG.txt`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/Makefile` & `graphe-0.1.0/docs/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/make.bat` & `graphe-0.1.0/docs/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/conf.py` & `graphe-0.1.0/docs/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/digraph.rst` & `graphe-0.1.0/docs/docs/source/digraph.rst`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/digraphappl.rst` & `graphe-0.1.0/docs/docs/source/digraphappl.rst`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/files.rst` & `graphe-0.1.0/docs/docs/source/files.rst`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/graph.rst` & `graphe-0.1.0/docs/docs/source/graph.rst`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/digraph_dfs.png` & `graphe-0.1.0/docs/docs/source/images/digraph_dfs.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/digraph_loop.png` & `graphe-0.1.0/docs/docs/source/images/digraph_loop.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/graph.png` & `graphe-0.1.0/docs/docs/source/images/graph.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/long.png` & `graphe-0.1.0/docs/docs/source/images/long.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/node_names.png` & `graphe-0.1.0/docs/docs/source/images/node_names.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/short.png` & `graphe-0.1.0/docs/docs/source/images/short.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/symbol_graph_bfs.png` & `graphe-0.1.0/docs/docs/source/images/symbol_graph_bfs.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/images/symbolg.png` & `graphe-0.1.0/docs/docs/source/images/symbolg.png`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/index.rst` & `graphe-0.1.0/docs/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/usage.rst` & `graphe-0.1.0/docs/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/docs/docs/source/utils.rst` & `graphe-0.1.0/docs/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/examples/regex.py` & `graphe-0.1.0/examples/regex.py`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/pyproject.toml` & `graphe-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphe"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Morten Jagd Christensen", email="mortenjc@jcaps.com" },
 ]
 description = "Collection of graph algorithms, applications and visualisations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `graphe-0.0.2/src/graphe/digraph/cycle.py` & `graphe-0.1.0/src/graphe/digraph/cycle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 
 from graphe.digraph import digraph
 from collections import deque
 
-class DirectedCycle():
+
+class DirectedCycle:
 
     def __init__(self, DG):
         assert isinstance(DG, digraph.Digraph)
         self.marked = [False for i in range(DG.V)]
         self.onstack = [False for i in range(DG.V)]
         self.edgeto = [-1 for i in range(DG.V)]
         self.cycle = deque()
 
         for v in range(DG.V):
             if not self.marked[v]:
                 self.dfs(DG, v)
 
-
     def dfs(self, DG, v):
         self.onstack[v] = True
         self.marked[v] = True
         for w in DG.adj(v):
             if self.has_cycle():
                 return
             elif not self.marked[w]:
@@ -31,14 +31,12 @@
                 while x != w:
                     self.cycle.append(x)
                     x = self.edgeto[x]
                 self.cycle.append(w)
                 self.cycle.append(v)
         self.onstack[v] = False
 
-
     def has_cycle(self):
         return len(self.cycle) != 0
 
-
     def get_cycle(self):
         return self.cycle
```

### Comparing `graphe-0.0.2/src/graphe/digraph/ddfo.py` & `graphe-0.1.0/src/graphe/digraph/ddfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/local/bin/python3
 
 import sys
 from graphe.digraph import digraph
 from collections import deque
 
 
-class DepthFirstOrder():
+class DepthFirstOrder:
     def __init__(self, DG):
         assert isinstance(DG, digraph.Digraph)
         self.marked = [False for i in range(DG.V)]
         self.pre = [-1 for i in range(DG.V)]
         self.post = [-1 for i in range(DG.V)]
         self.postorder = []
         self.preorder = []
@@ -17,28 +17,26 @@
         self.postCounter = 0
         for v in range(DG.V):
             if not self.marked[v]:
                 self.dfs(DG, v)
 
         assert self.check() == True
 
-
     def dfs(self, DG, v):
-        self.marked[v] = True;
+        self.marked[v] = True
         self.pre[v] = self.preCounter
         self.preCounter += 1
-        self.preorder.append(v);
+        self.preorder.append(v)
         for w in DG.adj(v):
             if not self.marked[w]:
                 self.dfs(DG, w)
         self.postorder.append(v)
         self.post[v] = self.postCounter
         self.postCounter += 1
 
-
     def check(self):
         # check that post(v) is consistent with post()
         r = 0
         for v in self.get_post():
             if self.get_postv(v) != r:
                 print(f'r === {r}: post(v) and post() inconsistent')
                 return False
@@ -48,31 +46,26 @@
         for v in self.get_pre():
             if self.get_prev(v) != r:
                 print('pre(v) and pre() inconsistent')
                 return False
             r += 1
         return True
 
-
     def get_prev(self, v):
         return self.pre[v]
 
-
     def get_postv(self, v):
         return self.post[v]
 
-
     def get_pre(self):
         return self.preorder
 
-
     def get_post(self):
         return self.postorder
 
-
     def get_reverse_post(self):
         new_lst = self.postorder[::-1]
         return new_lst
 
 
 if __name__ == '__main__':
```

### Comparing `graphe-0.0.2/src/graphe/digraph/digraph.py` & `graphe-0.1.0/src/graphe/digraph/digraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 #!/usr/local/bin/python3
 
 import sys
 
-class Digraph():
+
+class Digraph:
     def __init__(self, arg):
         self.E = 0
         if type(arg) is int:
             self.V = arg
             self.G = [[] for i in range(self.V)]
             return
 
-        infile = arg # assume string
+        infile = arg  # assume string
         with open(infile) as f:
             self.V = int(f.readline())
             E = int(f.readline())
             self.G = [[] for i in range(self.V)]
             for line in f:
                 From, To = line.strip().split()
                 self.add_edge(int(From), int(To))
         assert self.E == E
         f.close()
 
-
     def add_edge(self, v, w):
         assert v < self.V
         assert w < self.V
         self.G[v].append(w)
         self.E += 1
         return
 
-
     def adj(self, v):
         assert v < self.V
         return self.G[v]
 
-
     def reverse(self):
         DG = Digraph(self.V)
         for v in range(self.V):
             for w in self.adj(v):
                 DG.add_edge(w, v)
-        return  DG
-
+        return DG
 
     def to_string(self):
         s = f'G: {self.V} vertices, {self.E} edges'
         return s
```

### Comparing `graphe-0.0.2/src/graphe/digraph/digraphdfs.py` & `graphe-0.1.0/src/graphe/digraph/digraphdfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 #!/usr/local/bin/python3
 
 from graphe.digraph import digraph
 
-class DirectedDFSearch():
+
+class DirectedDFSearch:
     def __init__(self, DG, s):
         assert isinstance(DG, digraph.Digraph)
         self.marked = [False for i in range(DG.V)]
         self.edgeTo = [-1 for i in range(DG.V)]
         self.s = s
         self.V = DG.V
         if type(s) is int:
             self.validate_vertex(s)
             self.dfs(DG, s)
         else:
             for v in s:
                 self.validate_vertex(v)
             for v in s:
                 if not self.marked[v]:
-                    self.dfs(DG, v);
-
+                    self.dfs(DG, v)
 
     def validate_vertex(self, v):
         assert v >= 0 and v < self.V
 
-
     def dfs(self, DG, v):
         self.marked[v] = True
         for w in DG.adj(v):
             if not self.marked[w]:
                 self.edgeTo[w] = v
                 self.dfs(DG, w)
 
-
     def is_marked(self, v):
         return self.marked[v]
 
-
     def has_path_to(self, v):
         return self.marked[v]
 
-
     def path_to(self, v):
         path = []
         if not self.has_path_to(v):
             return path
         x = v
         while x != self.s:
             path.append(x)
             x = self.edgeTo[x]
         path.append(self.s)
         return path
 
-
     def count(self):
         return sum([1 for x in self.marked if x == True]) - 1
```

### Comparing `graphe-0.0.2/src/graphe/digraph/ksscc.py` & `graphe-0.1.0/src/graphe/digraph/ksscc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,50 +2,45 @@
 
 import sys
 from graphe.digraph import digraph
 from graphe.digraph import ddfo
 from collections import deque
 
 
-class KnSSCC():
+class KnSSCC:
     def __init__(self, Digraph):
         self.count = 0
         self.marked = [False for i in range(Digraph.V)]
         self.id = [0 for i in range(Digraph.V)]
 
         ddfs = ddfo.DepthFirstOrder(Digraph)
         print(ddfs.get_post())
 
         for v in ddfs.get_reverse_post():
             if not self.marked[v]:
                 self.dfs(Digraph, v)
                 self.count += 1
 
-
     def dfs(self, Digraph, v):
         self.marked[v] = True
         self.id[v] = self.count
         for w in Digraph.adj(v):
             if not self.marked[w]:
                 self.dfs(Digraph, w)
 
-
     def strongly_connected(self, v, w):
         return self.id[v] == self.id[w]
 
-
     def get_id(self, v):
         return self.id[v]
 
-
     def get_count(self):
         return self.count
 
 
-
 if __name__ == '__main__':
 
     DG = digraph.Digraph('../../data/tinyDG.txt')
 
     SCC = KnSSCC(DG)
 
     print(f'DG has {SCC.get_count()} components')
```

### Comparing `graphe-0.0.2/src/graphe/digraph/regex.py` & `graphe-0.1.0/src/graphe/digraph/regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,45 +2,44 @@
 
 import sys
 from graphe.digraph import digraph
 from graphe.digraph import digraphdfs
 from collections import deque
 
 
-class Regex():
+class Regex:
     def __init__(self, regexp):
         self.re = regexp.strip()
         self.M = len(self.re)
         ops = deque()
         self.DG = digraph.Digraph(self.M + 1)
 
         for i in range(self.M):
             lp = i
             if self.re[i] == '(' or self.re[i] == '|':
                 ops.append(i)
             elif self.re[i] == ')':
                 opr = ops.pop()
                 if self.re[opr] == '|':
                     lp = ops.pop()
-                    self.G.add_edge(lp, opr+1)
-                    self.G.add_edge(opr, i)
+                    self.DG.add_edge(lp, opr + 1)
+                    self.DG.add_edge(opr, i)
                 elif self.re[opr] == '(':
                     lp = opr
                 else:
                     assert False
 
-            if i < self.M-1 and self.re[i+1] == '*':
-                self.DG.add_edge(lp, i+1)
-                self.DG.add_edge(i+1, lp)
+            if i < self.M - 1 and self.re[i + 1] == '*':
+                self.DG.add_edge(lp, i + 1)
+                self.DG.add_edge(i + 1, lp)
             if self.re[i] == '(' or self.re[i] == '*' or self.re[i] == ')':
-                self.DG.add_edge(i, i+1)
+                self.DG.add_edge(i, i + 1)
         if len(ops) != 0:
             raise Exception('invalid regular expression {}'.format(regexp))
 
-
     def match(self, text):
         dfs = digraphdfs.DirectedDFSearch(self.DG, 0)
         pc = set()
         invalid = set(['*', '|', '(', ')'])
         for v in range(self.DG.V):
             if dfs.is_marked(v):
                 pc.add(v)
@@ -50,27 +49,27 @@
                 raise Exception('text has metacharacter: {}'.format(text[i]))
 
             match = []
             for v in pc:
                 if v == self.M:
                     continue
                 if self.re[v] == text[i] or self.re[v] == '.':
-                    match.append(v+1)
+                    match.append(v + 1)
 
                 if len(match) == 0:
                     continue
 
-                dfs = digraphdfs.DirectedDFSearch(self.DG, match);
+                dfs = digraphdfs.DirectedDFSearch(self.DG, match)
                 pc = set()
                 for v in range(self.DG.V):
-                    if (dfs.is_marked(v)):
+                    if dfs.is_marked(v):
                         pc.add(v)
 
                 if len(pc) == 0:
-                    return False # if no reacable states, finish early
+                    return False  # if no reacable states, finish early
 
             for v in pc:
                 if v == self.M:
                     return True
         return False
 
 
@@ -100,9 +99,8 @@
     assert re.match('ABABAB') == True
 
     re = Regex('(0|(1(01*(00)*0)*1)*)*')
     matches = ['11', '011', '110', '1001', '1100', '1111', '10010']
     for m in matches:
         assert re.match(m) == True
 
-
     print('passed')
```

### Comparing `graphe-0.0.2/src/graphe/digraph/symboldigraph.py` & `graphe-0.1.0/src/graphe/digraph/symboldigraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 
 import sys
 
 from graphe.digraph import digraph
 
-class SymbolDigraph():
+
+class SymbolDigraph:
     def __init__(self, infile, sc=' '):
-        self.keys = [] # vertice index to name
-        self.ST = {} # vertice name to index
+        self.keys = []  # vertice index to name
+        self.ST = {}  # vertice name to index
 
         lines = open(infile).read().splitlines()
         for line in lines:
             res = line.split(sc)
             assert len(res) >= 2
             for i in res:
                 if not i in self.ST:
@@ -28,19 +29,17 @@
             assert len(res) >= 2
 
             v = self.ST[res[0]]
             for i in res[1:]:
                 w = self.ST[i]
                 self.DG.add_edge(v, w)
 
-
     def graph(self):
         return self.DG
 
-
     def node_names(self):
         return self.keys
 
 
 if __name__ == '__main__':
     sg = SymbolDigraph('../../../data/routes.txt')
     assert sg.G.V == 10
```

### Comparing `graphe-0.0.2/src/graphe/digraph/topological.py` & `graphe-0.1.0/src/graphe/digraph/topological.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 from graphe.digraph import symboldigraph
 from graphe.digraph import cycle
 from graphe.digraph import ddfo
 
 
-class Topological():
+class Topological:
     def __init__(self, G):
         assert isinstance(G, digraph.Digraph)
         self.G = G
         self.rank = [-1 for i in range(self.G.V)]
 
         cycle = cycle.DirectedCycle(G)
         if cycle.has_cycle():
@@ -19,15 +19,14 @@
 
         dfo = ddfo.DepthFirstOrder(self.G)
         self.order = dfo.get_reverse_post()
 
         for i, v in enumerate(self.order):
             self.rank[v] = i
 
-
     def get_order(self):
         return self.order
 
 
 if __name__ == '__main__':
 
     SG = symboldigraph.SymbolDigraph('../../../data/jobs.txt', '/')
```

### Comparing `graphe-0.0.2/src/graphe/draw.py` & `graphe-0.1.0/src/graphe/draw.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 #!/usr/local/bin/python3
 
 import sys
 import graphviz
 
+
 class Draw:
     def __init__(self, digraph=False):
         if digraph:
             self.g = graphviz.Digraph()
         else:
             self.g = graphviz.Graph()
         self.g.engine = 'neato'
-        self.g.attr('node', margin='0', fontsize='4',
-                    fontcolor='white', color='black', shape='circle',
-                    style='filled', width='0.1')
+        self.g.attr(
+            'node',
+            margin='0',
+            fontsize='4',
+            fontcolor='white',
+            color='black',
+            shape='circle',
+            style='filled',
+            width='0.1',
+        )
         self.g.attr('edge', color='grey', penwidth='0.75')
 
         self.names = []
 
-
     def set_names(self, names):
         self.names = names
 
-
     def get_name(self, v):
         if len(self.names) != 0:
             return self.names[v]
         else:
             return str(v)
 
-
     def node_attr(self, **kwargs):
         self.g.attr('node', **kwargs)
 
-
     def edge_attr(self, **kwargs):
         self.g.attr('edge', **kwargs)
 
-
     def draw(self, Graph, path=[]):
         for v in range(Graph.V):
             self.g.node(self.get_name(v))
 
         pset = set()
         if len(path) >= 2:
             for i in range(len(path) - 1):
-                pset.add((path[i], path[i+1]))
-                pset.add((path[i+1], path[i]))
+                pset.add((path[i], path[i + 1]))
+                pset.add((path[i + 1], path[i]))
 
         seen = set()
         for v, e in enumerate(Graph.G):
             for w in e:
                 vname = self.get_name(v)
                 wname = self.get_name(w)
                 if not (w, v) in seen:
                     if (w, v) in pset:
-                        self.g.edge(vname, wname, color='black', penwidth='2.5', rank=f'{v}')
+                        self.g.edge(
+                            vname, wname, color='black', penwidth='2.5', rank=f'{v}'
+                        )
                     else:
                         self.g.edge(vname, wname, rank=f'{v}')
-                    seen.add((v,w))
+                    seen.add((v, w))
 
-        self.g.view()
+        self.g.view(tempfile.mktemp('.gv'))
```

### Comparing `graphe-0.0.2/src/graphe/graph/bfs.py` & `graphe-0.1.0/src/graphe/graph/bfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 #!/usr/local/bin/python3
 
 import sys
 from collections import deque
 
-class BFSearch():
+
+class BFSearch:
     def __init__(self, G, s):
         self.marked = [False for i in range(G.V)]
         self.edgeTo = [-1 for i in range(G.V)]
         self.s = s
         self.bfs(G, s)
 
-
     def bfs(self, Graph, s):
         Q = deque()
         self.marked[s] = True
         Q.append(s)
         while Q:
             v = Q.popleft()
             for w in Graph.adj(v):
                 if not self.marked[w]:
                     self.edgeTo[w] = v
                     self.marked[w] = True
                     Q.append(w)
 
-
     def has_path_to(self, v):
         return self.marked[v]
 
-
     def path_to(self, v):
         path = []
         if not self.has_path_to(v):
             return path
         x = v
         while x != self.s:
             path.append(x)
             x = self.edgeTo[x]
         path.append(self.s)
         return path
 
-
     def count(self):
         return sum([1 for x in self.marked if x == True]) - 1
```

### Comparing `graphe-0.0.2/src/graphe/graph/cc.py` & `graphe-0.1.0/src/graphe/graph/cc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/local/bin/python3
 
 import sys
 from graphe.graph import graph
 
+
 class CC:
-   def __init__(self, Graph):
-      self.G = Graph
-      self.cc = []
-
-   #todo should use dfs.py instead
-   def DFS(self, temp, v, visited):
-      visited[v] = True
-      temp.append(v)
-
-      for i in self.G.adj(v):
-         if visited[i] == False:
-            temp = self.DFS(temp, i, visited)
-      return temp
-
-
-   def ccomps(self):
-      visited = []
-      self.cc = []
-      for i in range(self.G.V):
-         visited.append(False)
-      for v in range(self.G.V):
-         if visited[v] == False:
-            temp = []
-            self.cc.append(self.DFS(temp, v, visited))
-      return self.cc
+    def __init__(self, Graph):
+        self.G = Graph
+        self.cc = []
+
+    # todo should use dfs.py instead
+    def DFS(self, temp, v, visited):
+        visited[v] = True
+        temp.append(v)
+
+        for i in self.G.adj(v):
+            if visited[i] == False:
+                temp = self.DFS(temp, i, visited)
+        return temp
+
+    def ccomps(self):
+        visited = []
+        self.cc = []
+        for i in range(self.G.V):
+            visited.append(False)
+        for v in range(self.G.V):
+            if visited[v] == False:
+                temp = []
+                self.cc.append(self.DFS(temp, v, visited))
+        return self.cc
```

### Comparing `graphe-0.0.2/src/graphe/graph/dfs.py` & `graphe-0.1.0/src/graphe/graph/dfs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 #!/usr/local/bin/python3
 
 import sys
 
-class DFSearch():
+
+class DFSearch:
     def __init__(self, G, s):
         self.marked = [False for i in range(G.V)]
         self.edgeTo = [-1 for i in range(G.V)]
         self.s = s
         self.dfs(G, s)
 
-
     def dfs(self, Graph, v):
         self.marked[v] = True
         for w in Graph.adj(v):
             if not self.marked[w]:
                 self.edgeTo[w] = v
                 self.dfs(Graph, w)
 
-
     def has_path_to(self, v):
         return self.marked[v]
 
-
     def path_to(self, v):
         path = []
         if not self.has_path_to(v):
             return path
         x = v
         while x != self.s:
             path.append(x)
             x = self.edgeTo[x]
         path.append(self.s)
         return path
 
-
     def count(self):
         return sum([1 for x in self.marked if x == True]) - 1
```

### Comparing `graphe-0.0.2/src/graphe/graph/graph.py` & `graphe-0.1.0/src/graphe/graph/graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 #!/usr/local/bin/python3
 
 import sys
 
-class Graph():
+
+class Graph:
     def __init__(self, arg):
         self.E = 0
         if type(arg) is int:
             self.V = arg
             self.G = [[] for i in range(self.V)]
             return
 
-        infile = arg # assume string
+        infile = arg  # assume string
         with open(infile) as f:
             self.V = int(f.readline())
             E = int(f.readline())
             self.G = [[] for i in range(self.V)]
             for line in f:
                 From, To = line.split()
                 self.add_edge(int(From), int(To))
         assert self.E == E
         f.close()
 
-
     def add_edge(self, v, w):
         assert v < self.V
         assert w < self.V
         self.G[v].append(w)
         self.G[w].append(v)
         self.E += 1
         return
 
-
     def adj(self, v):
         assert v < self.V
         return self.G[v]
 
-
     def to_string(self):
-        s = f'G: {self.V} vertices, {self.E} edges'
+        s = f"G: {self.V} vertices, {self.E} edges"
         return s
```

### Comparing `graphe-0.0.2/src/graphe.egg-info/PKG-INFO` & `graphe-0.1.0/src/graphe.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphe
-Version: 0.0.2
+Version: 0.1.0
 Summary: Collection of graph algorithms, applications and visualisations
 Author-email: Morten Jagd Christensen <mortenjc@jcaps.com>
 Project-URL: Homepage, https://github.com/mortenjc/graphe
 Project-URL: Documentation, https://graphe.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/mortenjc/graphe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `graphe-0.0.2/src/graphe.egg-info/SOURCES.txt` & `graphe-0.1.0/src/graphe.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 examples/directeddfs.py
 examples/graph.py
 examples/node_names.py
 examples/regex.py
 examples/symbol_graph.py
 examples/symbol_graph_bfs.py
 examples/topological_sort.py
+scripts/blackcheck
+scripts/blackrun
 scripts/coverage
 scripts/publish
 src/graphe/__init__.py
 src/graphe/draw.py
 src/graphe.egg-info/PKG-INFO
 src/graphe.egg-info/SOURCES.txt
 src/graphe.egg-info/dependency_links.txt
@@ -70,8 +72,9 @@
 src/graphe/graph/dfs.py
 src/graphe/graph/graph.py
 tests/test_bfs.py
 tests/test_cycle.py
 tests/test_dfs.py
 tests/test_digraph.py
 tests/test_digraphdfs.py
-tests/test_graph.py
+tests/test_graph.py
+tests/test_regex.py
```

### Comparing `graphe-0.0.2/tests/test_bfs.py` & `graphe-0.1.0/tests/test_bfs.py`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/tests/test_cycle.py` & `graphe-0.1.0/tests/test_cycle.py`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/tests/test_dfs.py` & `graphe-0.1.0/tests/test_dfs.py`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/tests/test_digraph.py` & `graphe-0.1.0/tests/test_digraph.py`

 * *Files identical despite different names*

### Comparing `graphe-0.0.2/tests/test_digraphdfs.py` & `graphe-0.1.0/tests/test_digraphdfs.py`

 * *Files identical despite different names*

