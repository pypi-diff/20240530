# Comparing `tmp/ourchester-0.1.3.tar.gz` & `tmp/ourchester-0.1.4.tar.gz`

## Comparing `ourchester-0.1.3.tar` & `ourchester-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ourchester-0.1.3/.bumpversion.cfg
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ourchester-0.1.3/Makefile
--rwxr-xr-x   0        0        0     1736 2020-02-02 00:00:00.000000 ourchester-0.1.3/make_txtar.sh
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ourchester-0.1.3/ourchester.code-workspace
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ourchester-0.1.3/requirements-dev.lock
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 ourchester-0.1.3/requirements.lock
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 ourchester-0.1.3/src/ourchester/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 ourchester-0.1.3/src/ourchester/cli.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ourchester-0.1.3/src/ourchester/indexer.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ourchester-0.1.3/src/ourchester/log.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ourchester-0.1.3/src/ourchester/searcher.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file1.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file10.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file2.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file3.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file4.md
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file5.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file6.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file7.md
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file8.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ourchester-0.1.3/testdata/file9.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ourchester-0.1.3/.gitignore
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.3/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ourchester-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 ourchester-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ourchester-0.1.4/.bumpversion.cfg
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ourchester-0.1.4/Makefile
+-rwxr-xr-x   0        0        0     1736 2020-02-02 00:00:00.000000 ourchester-0.1.4/make_txtar.sh
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ourchester-0.1.4/ourchester.code-workspace
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ourchester-0.1.4/requirements-dev.lock
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 ourchester-0.1.4/requirements.lock
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ourchester-0.1.4/src/ourchester/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 ourchester-0.1.4/src/ourchester/cli.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 ourchester-0.1.4/src/ourchester/indexer.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ourchester-0.1.4/src/ourchester/log.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ourchester-0.1.4/src/ourchester/searcher.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file1.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file10.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file2.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file3.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file4.md
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file5.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file6.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file7.md
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file8.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ourchester-0.1.4/testdata/file9.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ourchester-0.1.4/.gitignore
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.4/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ourchester-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 ourchester-0.1.4/PKG-INFO
```

### Comparing `ourchester-0.1.3/make_txtar.sh` & `ourchester-0.1.4/make_txtar.sh`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.3/requirements-dev.lock` & `ourchester-0.1.4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.3/requirements.lock` & `ourchester-0.1.4/requirements.lock`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.3/src/ourchester/__init__.py` & `ourchester-0.1.4/src/ourchester/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import typing
 
 import fishhoof.find_files
 import platformdirs
 import whoosh.index
 
 from . import cli, indexer, log, searcher
 
@@ -14,23 +15,28 @@
     log.configure_logging(args.verbose)
 
     cache_dir = _get_cache_dir()
     index_dir = cache_dir / args.index
 
     if args.command == "index":
         directories = [pathlib.Path(dir) for dir in args.directories]
-        fps = fishhoof.find_files.build_path_list(
-            directories,
-            excludes=args.exclude,
-            extensions=args.extensions,
-            newer=args.newer,
+        file_paths: typing.List[fishhoof.FileWithTimestamp] = (
+            fishhoof.find_files.build_path_list(
+                directories,
+                excludes=args.exclude,
+                extensions=args.extensions,
+                newer=args.newer,
+            )
         )
-
-        file_paths = [str(p.file) for p in fps]
+        file_paths = [item.file for item in file_paths]
         indexer.index_files(file_paths, index_dir)
+
+    elif args.command == "listindex":
+        indexer.get_index_files(index_dir)
+
     elif args.command == "search":
         try:
             index = indexer.load_index(index_dir)
             results = searcher.perform_proximity_search(index, args.query)
             _print_search_results(results)
         except whoosh.index.EmptyIndexError:
             print(f"Index does not exist in {index_dir}")
```

### Comparing `ourchester-0.1.3/src/ourchester/cli.py` & `ourchester-0.1.4/src/ourchester/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 def parse_args():
     parser = argparse.ArgumentParser(
         description="Perform proximity search on text files."
     )
 
     subparsers = parser.add_subparsers(dest="command", required=True)
 
+    listindex_parser = subparsers.add_parser(
+        "listindex", help="List files in index for debug"
+    )
+    listindex_parser.add_argument(
+        "-i", "--index", type=str, default="index", help="Directory to store the index"
+    )
+    listindex_parser.add_argument(
+        "-v", "--verbose", action="store_true", help="Enable verbose output"
+    )
+
     index_parser = subparsers.add_parser("index", help="Index text files")
     index_parser.add_argument(
         "directories", type=str, nargs="+", help="Directories containing text files"
     )
     index_parser.add_argument(
         "-i", "--index", type=str, default="index", help="Directory to store the index"
     )
```

### Comparing `ourchester-0.1.3/src/ourchester/indexer.py` & `ourchester-0.1.4/src/ourchester/indexer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import pathlib
 import time
+import typing
 
 import whoosh.fields
 import whoosh.index
 
 logger = logging.getLogger(__name__)
 
 
@@ -15,34 +16,52 @@
         return whoosh.index.create_in(index_home_path, schema)
 
 
 def _index_files(file_paths, writer):
     indexed_paths = set()
     for file_path in file_paths:
         logging.debug(f"deleting from whoosh index {file_path}")
-        writer.delete_by_term("path", file_path)
+        writer.delete_by_term("path", str(file_path))
         with open(file_path, "r") as file:
             content = file.read()
             logging.debug(f"indexing {file_path}")
-            writer.add_document(path=file_path, content=content)
+            writer.add_document(
+                path=str(file_path),
+                title=file_path.with_suffix("").name,
+                content=content,
+            )
             indexed_paths.add(file_path)
     return indexed_paths
 
 
 def _remove_deleted_files(ix, indexed_paths, writer):
     for doc in ix.searcher().documents():
         if pathlib.Path(doc["path"]).exists():
             continue
         if doc["path"] not in indexed_paths:
             logging.debug(f"deleting from whoosh index {doc['path']}")
             writer.delete_by_term("path", doc["path"])
 
 
-def index_files(file_paths, index_home_path):
+def get_index_files(index_home_path):
+    ix = whoosh.index.open_dir(index_home_path)
+
+    with ix.reader() as reader:
+        for stored_fields in reader.all_stored_fields():
+            doc_title = stored_fields["title"]
+            doc_path = stored_fields["path"]
+
+            print(f"Title: {doc_title}")
+            print(f"Path: {doc_path}")
+            print("---")
+
+
+def index_files(file_paths: typing.List[pathlib.Path], index_home_path):
     schema = whoosh.fields.Schema(
+        title=whoosh.fields.TEXT(stored=True),
         path=whoosh.fields.ID(unique=True, stored=True),
         content=whoosh.fields.TEXT(stored=True),
     )
     start_time = time.time()
     ix = _create_or_open_index(index_home_path, schema)
     writer = ix.writer()
     indexed_paths = _index_files(file_paths, writer)
```

### Comparing `ourchester-0.1.3/pyproject.toml` & `ourchester-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ourchester"
-version = "0.1.3"
+version = "0.1.4"
 description = "Add your description here"
 authors = [
     { name = "Taylor Monacelli", email = "taylormonacelli@gmail.com" }
 ]
 dependencies = [
     "jinja2>=3.1.3",
     "whoosh>=2.7.4",
```

### Comparing `ourchester-0.1.3/PKG-INFO` & `ourchester-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ourchester
-Version: 0.1.3
+Version: 0.1.4
 Summary: Add your description here
 Author-email: Taylor Monacelli <taylormonacelli@gmail.com>
 Requires-Python: >=3.12
 Requires-Dist: fishhoof>=0.0.2
 Requires-Dist: ivylantern>=0.1.0
 Requires-Dist: jinja2>=3.1.3
 Requires-Dist: platformdirs>=4.2.2
```

