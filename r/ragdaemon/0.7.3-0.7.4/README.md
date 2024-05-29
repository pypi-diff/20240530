# Comparing `tmp/ragdaemon-0.7.3.tar.gz` & `tmp/ragdaemon-0.7.4.tar.gz`

## Comparing `ragdaemon-0.7.3.tar` & `ragdaemon-0.7.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/app.py
--rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/context.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/graph.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/utils.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/chunker/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/chunker/chunk_astroid.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/chunker/chunk_line.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/chunker/chunk_llm.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/annotators/chunker/utils.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/database/pg_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/chunk_llm.toml
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/test_sample.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/data/context_message.txt
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragdaemon-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/app.py
+-rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/context.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/graph.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/locate.py
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/utils.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/chunker/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/chunker/chunk_astroid.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/chunker/chunk_line.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/chunker/chunk_llm.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/annotators/chunker/utils.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/database/pg_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/chunk_llm.toml
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/test_sample.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/data/context_message.txt
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragdaemon-0.7.4/PKG-INFO
```

### Comparing `ragdaemon-0.7.3/scratch.ipynb` & `ragdaemon-0.7.4/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tutorial.ipynb` & `ragdaemon-0.7.4/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/.github/workflows/run-tests.yml` & `ragdaemon-0.7.4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/app.py` & `ragdaemon-0.7.4/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/context.py` & `ragdaemon-0.7.4/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/daemon.py` & `ragdaemon-0.7.4/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/get_paths.py` & `ragdaemon-0.7.4/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/graph.py` & `ragdaemon-0.7.4/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/locate.py` & `ragdaemon-0.7.4/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/utils.py` & `ragdaemon-0.7.4/ragdaemon/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,17 @@
         diff_ref, path_ref = id.split(":", 1)
         path, lines = parse_path_ref(path_ref)
     else:
         diff_ref, path, lines = id, None, None
     return diff_ref, path, lines
 
 
-def get_document(ref: str, cwd: Path, type: str = "file") -> str:
+def get_document(
+    ref: str, cwd: Path, type: str = "file", ignore_patterns: set[Path] = set()
+) -> str:
     if type == "diff":
         if ":" in ref:
             diff_ref, lines_ref = ref.split(":", 1)
             lines = parse_lines_ref(lines_ref)
         else:
             diff_ref, lines = ref, None
         diff = get_git_diff(diff_ref, str(cwd))
@@ -109,15 +111,20 @@
             )
         else:
             text = diff
         ref = f"git diff{'' if diff_ref == 'DEFAULT' else f' {diff_ref}'}"
 
     elif type == "directory":
         path = cwd if ref == "ROOT" else cwd / ref
-        paths = sorted([p.as_posix() for p in get_paths_for_directory(path)])
+        paths = sorted(
+            [
+                p.as_posix()
+                for p in get_paths_for_directory(path, exclude_patterns=ignore_patterns)
+            ]
+        )
         text = "\n".join(paths)
 
     elif type in {"file", "chunk"}:
         path, lines = parse_path_ref(ref)
         if lines:
             text = ""
             with open(cwd / path, "r") as f:
```

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/__init__.py` & `ragdaemon-0.7.4/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.7.4/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.7.4/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/diff.py` & `ragdaemon-0.7.4/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.7.4/ragdaemon/annotators/hierarchy.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,18 +69,20 @@
                 directories.add(parent)
                 edges.add((parent.as_posix(), _last.as_posix()))
                 _last = parent
 
         for dir in directories:
             dir_str = dir.as_posix()
             dir_path = dir if dir != Path("ROOT") else Path(".")
-            document = get_document(dir_str, cwd, type="directory")
+            document = get_document(
+                dir_str, cwd, type="directory", ignore_patterns=self.ignore_patterns
+            )
             checksum = hash_str(
                 "".join(
-                    checksums[dir_path / subpath]
+                    checksums.get(dir_path / subpath, "")
                     for subpath in document.split("\n")[1:]
                 )
             )
             data = {
                 "id": dir_str,
                 "type": "directory",
                 "ref": dir_str,
```

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.7.4/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.7.4/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/chunker/__init__.py` & `ragdaemon-0.7.4/ragdaemon/annotators/chunker/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/chunker/chunk_astroid.py` & `ragdaemon-0.7.4/ragdaemon/annotators/chunker/chunk_astroid.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/chunker/chunk_line.py` & `ragdaemon-0.7.4/ragdaemon/annotators/chunker/chunk_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/chunker/chunk_llm.py` & `ragdaemon-0.7.4/ragdaemon/annotators/chunker/chunk_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/annotators/chunker/utils.py` & `ragdaemon-0.7.4/ragdaemon/annotators/chunker/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/database/__init__.py` & `ragdaemon-0.7.4/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/database/chroma_database.py` & `ragdaemon-0.7.4/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/database/database.py` & `ragdaemon-0.7.4/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/database/lite_database.py` & `ragdaemon-0.7.4/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/database/pg_database.py` & `ragdaemon-0.7.4/ragdaemon/database/pg_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.7.4/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/chunk_llm.toml` & `ragdaemon-0.7.4/ragdaemon/prompts/chunk_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/locate.toml` & `ragdaemon-0.7.4/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.7.4/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.7.4/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.7.4/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.7.4/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.7.4/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/static/favicon.ico` & `ragdaemon-0.7.4/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.7.4/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/static/js/main.js` & `ragdaemon-0.7.4/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.7.4/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/static/js/three/node.js` & `ragdaemon-0.7.4/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.7.4/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/ragdaemon/templates/index.html` & `ragdaemon-0.7.4/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/conftest.py` & `ragdaemon-0.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/test_comments.py` & `ragdaemon-0.7.4/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/test_context.py` & `ragdaemon-0.7.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/test_daemon.py` & `ragdaemon-0.7.4/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/test_get_paths.py` & `ragdaemon-0.7.4/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/test_sample.py` & `ragdaemon-0.7.4/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/annotators/test_chunker.py` & `ragdaemon-0.7.4/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/annotators/test_diff.py` & `ragdaemon-0.7.4/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/annotators/test_hierarchy.py` & `ragdaemon-0.7.4/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.7.4/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/annotators/test_summarizer.py` & `ragdaemon-0.7.4/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/data/chunker_graph.json` & `ragdaemon-0.7.4/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/data/context_message.txt` & `ragdaemon-0.7.4/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/data/diff_graph.json` & `ragdaemon-0.7.4/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/data/hard_to_chunk.txt` & `ragdaemon-0.7.4/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/data/hierarchy_graph.json` & `ragdaemon-0.7.4/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.7.4/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/data/summarizer_graph.json` & `ragdaemon-0.7.4/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/tests/sample/src/interface.py` & `ragdaemon-0.7.4/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/LICENSE` & `ragdaemon-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/README.md` & `ragdaemon-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.3/pyproject.toml` & `ragdaemon-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.7.3"
+version = "0.7.4"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "astroid==3.2.2",
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
```

### Comparing `ragdaemon-0.7.3/PKG-INFO` & `ragdaemon-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.7.3
+Version: 0.7.4
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

