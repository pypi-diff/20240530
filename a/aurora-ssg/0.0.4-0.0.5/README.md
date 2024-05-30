# Comparing `tmp/aurora_ssg-0.0.4.tar.gz` & `tmp/aurora_ssg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora_ssg-0.0.4.tar", last modified: Tue May 28 18:37:13 2024, max compression
+gzip compressed data, was "aurora_ssg-0.0.5.tar", last modified: Thu May 30 19:24:32 2024, max compression
```

## Comparing `aurora_ssg-0.0.4.tar` & `aurora_ssg-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 18:37:13.278304 aurora_ssg-0.0.4/
--rw-r--r--   0 james      (501) staff       (20)     2238 2024-05-28 09:57:50.000000 aurora_ssg-0.0.4/.gitignore
--rw-r--r--   0 james      (501) staff       (20)      544 2024-05-28 10:09:29.000000 aurora_ssg-0.0.4/CHANGELOG.md
--rw-r--r--   0 james      (501) staff       (20)     1061 2024-05-28 08:11:52.000000 aurora_ssg-0.0.4/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 18:37:13.277990 aurora_ssg-0.0.4/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5787 2024-05-28 08:11:52.000000 aurora_ssg-0.0.4/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 18:37:13.275308 aurora_ssg-0.0.4/aurora/
--rw-r--r--   0 james      (501) staff       (20)       22 2024-05-28 18:37:09.000000 aurora_ssg-0.0.4/aurora/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1517 2024-05-28 18:35:22.000000 aurora_ssg-0.0.4/aurora/cli.py
--rw-r--r--   0 james      (501) staff       (20)      728 2024-05-28 08:11:52.000000 aurora_ssg-0.0.4/aurora/date_helpers.py
--rw-r--r--   0 james      (501) staff       (20)    20923 2024-05-28 18:35:47.000000 aurora_ssg-0.0.4/aurora/graph.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 18:37:13.277137 aurora_ssg-0.0.4/aurora_ssg.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 18:37:13.000000 aurora_ssg-0.0.4/aurora_ssg.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      339 2024-05-28 18:37:13.000000 aurora_ssg-0.0.4/aurora_ssg.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-05-28 18:37:13.000000 aurora_ssg-0.0.4/aurora_ssg.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       43 2024-05-28 18:37:13.000000 aurora_ssg-0.0.4/aurora_ssg.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)      153 2024-05-28 18:37:13.000000 aurora_ssg-0.0.4/aurora_ssg.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        7 2024-05-28 18:37:13.000000 aurora_ssg-0.0.4/aurora_ssg.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)   923054 2024-05-28 08:11:52.000000 aurora_ssg-0.0.4/banner.png
--rw-r--r--   0 james      (501) staff       (20)       38 2024-05-28 18:37:13.278366 aurora_ssg-0.0.4/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1563 2024-05-28 09:57:24.000000 aurora_ssg-0.0.4/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-30 19:24:32.196680 aurora_ssg-0.0.5/
+-rw-r--r--   0 james      (501) staff       (20)     1061 2024-05-27 15:17:29.000000 aurora_ssg-0.0.5/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     9046 2024-05-30 19:24:32.196207 aurora_ssg-0.0.5/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     8054 2024-05-29 18:01:58.000000 aurora_ssg-0.0.5/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-30 19:24:32.192921 aurora_ssg-0.0.5/aurora/
+-rw-r--r--   0 james      (501) staff       (20)       22 2024-05-30 19:24:22.000000 aurora_ssg-0.0.5/aurora/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1517 2024-05-29 18:01:58.000000 aurora_ssg-0.0.5/aurora/cli.py
+-rw-r--r--   0 james      (501) staff       (20)      728 2024-05-27 15:43:42.000000 aurora_ssg-0.0.5/aurora/date_helpers.py
+-rw-r--r--   0 james      (501) staff       (20)    21386 2024-05-30 19:20:46.000000 aurora_ssg-0.0.5/aurora/graph.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-30 19:24:32.195164 aurora_ssg-0.0.5/aurora_ssg.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     9046 2024-05-30 19:24:32.000000 aurora_ssg-0.0.5/aurora_ssg.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      304 2024-05-30 19:24:32.000000 aurora_ssg-0.0.5/aurora_ssg.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-30 19:24:32.000000 aurora_ssg-0.0.5/aurora_ssg.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       43 2024-05-30 19:24:32.000000 aurora_ssg-0.0.5/aurora_ssg.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      153 2024-05-30 19:24:32.000000 aurora_ssg-0.0.5/aurora_ssg.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        7 2024-05-30 19:24:32.000000 aurora_ssg-0.0.5/aurora_ssg.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-05-30 19:24:32.196757 aurora_ssg-0.0.5/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1563 2024-05-29 18:01:58.000000 aurora_ssg-0.0.5/setup.py
```

### Comparing `aurora_ssg-0.0.4/LICENSE` & `aurora_ssg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.4/PKG-INFO` & `aurora_ssg-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: aurora-ssg
-Version: 0.0.4
-Summary: A fast static site generator implemented in Python.
-Home-page: https://github.com/capjamesg/aurora
-Author: capjamesg
-Author-email: readers@jamesg.blog
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: jinja2
-Requires-Dist: watchdog
-Requires-Dist: toposort
-Requires-Dist: pyromark
-Requires-Dist: python-frontmatter
-Requires-Dist: requests
-Requires-Dist: progress
-Requires-Dist: click
-Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: black==22.3.0; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: wheel; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
-
 ![Banner](banner.png)
 
 <div align="center">
 
 [![version](https://badge.fury.io/py/aurora-ssg.svg)](https://badge.fury.io/py/aurora-ssg)
 [![downloads](https://img.shields.io/pypi/dm/aurora-ssg)](https://pypistats.org/packages/aurora-ssg)
 [![license](https://img.shields.io/pypi/l/aurora-ssg)](https://github.com/capjamesg/aurora-ssg/blob/main/LICENSE.md)
@@ -118,14 +87,25 @@
 git clone https://github.com/capjamesg/aurora
 cd aurora
 pip3 install -e .
 ```
 
 This will install Aurora in editable mode. In editable mode, you can make changes to the code and see them reflected in your local installation.
 
+## Aurora Site Structure
+
+By default, an Aurora site has the following structure in the root directory:
+
+- `pages`: Where all pages used to generate your site are stored.
+- `pages/_layouts`: Where you can store layouts for use in generating your website.
+- `pages/_data`: Where you can store JSON data files for use in generating pages. See the "Render Collections of Data" section later in this document for information on how to use this directory to generate pages from data files.
+- `pages/posts`: Where you can store all of your blog posts, if you use your site as a blog. The posts directory is processed with additional logic to automatically generate date archive and category archive pages, if applicable.
+
+Any file in `pages` or a folder you make in `pages` (not including `_layouts` and `_data`) will be rendered on your website. For example, if you create a `pages/interests/coffee.html` file, this will generate a page called `_site/pages/interests/coffee/index.html`.
+
 ## Configuration
 
 You need a `config.py` file in the directory in which you will build your Aurora site. This file is automatically generated when you run `aurora new [site-name]`.
 
 This configuration file defines a few values that Aurora will use when processing your website.
 
 Here is the default `config.py` file, with accompanying comments:
@@ -153,14 +133,34 @@
 BASE_URLS = {
     "production": "https://jamesg.blog",
     "staging": "https://staging.jamesg.blog",
     "local": os.getcwd(),
 }
 ```
 
+## Render Collections of Data 
+
+You can render data from JSON files as web pages with Aurora. This is useful if you have a JSON collection of data, such as a list of coffee shop reviews, that you want to turn into posts without creating corresponding markdown files.
+
+To create a collection, add a new file to your site's `pages/_data` directory. This file should have a `.json` extension.
+
+Within the file, create a list that contains JSON objects, like this:
+
+```json
+[
+    {"slug": "rosslyn-coffee", "layout": "coffee", "title": "Rosslyn Coffee in London is terrific."}
+]
+```
+
+This file is called `pages/_data/coffee.json`.
+
+Every entry must have a `layout` key. This corresponds with the name of the template that will be used to render the page. For example, the `coffee` layout will be rendered using the `pages/_layouts/coffee.html` template.
+
+Every entry must also have a `slug` key. This corresponds with the name of the page that will be generated. In the case above, one file will be created in the `_site` output directory: `_site/coffee/rosslyn-coffee/index.html`.
+
 ## Build Hooks (Advanced)
 
 You can define custom functions that are run before a file is processed by Aurora. You can use this feature to save metadata about a page that can then be consumed by a template.
 
 These functions are called "hooks".
 
 To define a hook, you need to:
@@ -203,17 +203,17 @@
 REGISTERED_HOOKS = {
     "hook_file_name": ["hook1", "hook2", "hook3"],
 }
 ```
 
 ## Performance
 
-In a test on a website with 1763 files, Aurora built the website in `0:00:04.23`.
+In a test on a website with 1,763 files and multiple layers of inheritance, Aurora built the website in under two seconds. The files in this test were a combination of blog posts, static pages, and programmatic archives for blog posts (date pages, category pages).
 
-The files were a combination of blog posts, static pages, and programmatic archives for blog posts (date pages, category pages).
+In a test rendering 4,000 markdown files with a single layer of inheritance in each template, Aurora built the website in between 0.9 and 1.2 seconds.
 
 ## Users
 
 The following sites are built with Aurora:
 
 - [James' Coffee Blog](https://jamesg.blog) (1,500+ pages)
```

### Comparing `aurora_ssg-0.0.4/aurora/cli.py` & `aurora_ssg-0.0.5/aurora/cli.py`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.4/aurora/date_helpers.py` & `aurora_ssg-0.0.5/aurora/date_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.4/aurora/graph.py` & `aurora_ssg-0.0.5/aurora/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,20 +66,20 @@
     """
     return value.lower().replace(" ", "-")
 
 
 class Watcher(FileSystemEventHandler):
     def on_modified(self, event):
         print(f"Detected change in {event.src_path}. Rebuilding.")
-        file_name = event.src_path
-        file_name = file_name.replace(os.getcwd() + "/", "")
-        file_dependencies = all_dependencies[file_name]
-        file_dependencies.add(file_name)
+        # file_name = event.src_path
+        # file_name = file_name.replace(os.getcwd() + "/", "")
+        # file_dependencies = all_dependencies[file_name]
+        # file_dependencies.add(file_name)
 
-        main(deps=file_dependencies)
+        main() #deps=file_dependencies)
 
 
 class VariableVisitor(NodeVisitor):
     """
     Find all variables in a jinja2 template.
     """
 
@@ -254,14 +254,22 @@
         dependencies.add(
             f"{ROOT_DIR}/{LAYOUTS_BASE_DIR}/{parsed_content['layout']}.html"
         )
         if not state.get(parsed_content["layout"] + "s"):
             state[parsed_content["layout"] + "s"] = []
 
         state[parsed_content["layout"] + "s"].append(parsed_content)
+
+    if "collection" in parsed_content:
+        collection_normalized = parsed_content["collection"].lower()
+        if not state.get(collection_normalized):
+            state[collection_normalized] = []
+
+        state[collection_normalized].append(parsed_content)
+        
     return dependencies, parsed_content
 
 
 for page, contents in all_opened_pages.items():
     dependencies, parsed_page = get_file_dependencies_and_evaluated_contents(
         page, contents
     )
@@ -464,15 +472,18 @@
                 page_state["page"].permalink.strip("/"), "index.html"
             )
         else:
             permalink = file.replace("templates/", "")
     else:
         permalink = file.replace("templates/", "")
 
-    make_any_nonexistent_directories(os.path.dirname(os.path.join(SITE_DIR, permalink)))
+    if permalink.endswith(".html"):
+        make_any_nonexistent_directories(os.path.dirname(os.path.join(SITE_DIR, permalink)))
+    else:
+        make_any_nonexistent_directories(os.path.join(SITE_DIR))
 
     permalink = os.path.join(SITE_DIR, permalink)
 
     state_to_write[permalink] = rendered
 
     state["pages"].append({"url": f"{BASE_URL}/{permalink}", "file": file})
 
@@ -634,14 +645,16 @@
     for file in state_to_write:
         with open(file, "wb", buffering=1000) as f:
             f.write(state_to_write[file].encode())
 
     process_date_archives()
     process_category_archives()
 
+    print(f"Built site in {datetime.datetime.now() - start}")
+
     if watch:
         observer = Observer()
         observer.schedule(Watcher(), path="pages", recursive=True)
         observer.start()
 
         print("Watching for changes...")
         print("View your site at ", os.path.join(os.getcwd(), SITE_DIR, "index.html"))
```

### Comparing `aurora_ssg-0.0.4/setup.py` & `aurora_ssg-0.0.5/setup.py`

 * *Files identical despite different names*

