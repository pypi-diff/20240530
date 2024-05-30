# Comparing `tmp/nbnorm-0.3.2.tar.gz` & `tmp/nbnorm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbnorm-0.3.2.tar", last modified: Fri Jul 28 15:41:07 2023, max compression
+gzip compressed data, was "nbnorm-0.4.0.tar", last modified: Thu May 30 11:42:47 2024, max compression
```

## Comparing `nbnorm-0.3.2.tar` & `nbnorm-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-07-28 15:41:07.995734 nbnorm-0.3.2/
--rw-r--r--   0 tparment (15010) diana    (200036)      506 2023-07-28 15:41:07.995346 nbnorm-0.3.2/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      226 2022-07-21 09:34:26.000000 nbnorm-0.3.2/README.md
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-07-28 15:41:07.991735 nbnorm-0.3.2/nbnorm/
--rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-07-21 09:27:30.000000 nbnorm-0.3.2/nbnorm/__init__.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)    18570 2023-07-28 15:07:09.000000 nbnorm-0.3.2/nbnorm/nbnorm.py
--rw-r--r--   0 tparment (15010) diana    (200036)       22 2023-07-28 15:40:47.000000 nbnorm-0.3.2/nbnorm/version.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1482 2022-07-21 09:28:39.000000 nbnorm-0.3.2/nbnorm/xpath.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-07-28 15:41:07.994862 nbnorm-0.3.2/nbnorm.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)      506 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      299 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       46 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/entry_points.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-07-21 09:47:04.000000 nbnorm-0.3.2/nbnorm.egg-info/not-zip-safe
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/requires.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        7 2023-07-28 15:41:07.000000 nbnorm-0.3.2/nbnorm.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-07-28 15:41:07.995835 nbnorm-0.3.2/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1442 2022-07-21 09:35:19.000000 nbnorm-0.3.2/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-30 11:42:47.470228 nbnorm-0.4.0/
+-rw-r--r--   0 tparment (15010) diana    (200036)      530 2024-05-30 11:42:47.469678 nbnorm-0.4.0/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      226 2022-07-21 09:34:26.000000 nbnorm-0.4.0/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-30 11:42:47.464930 nbnorm-0.4.0/nbnorm/
+-rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-07-21 09:27:30.000000 nbnorm-0.4.0/nbnorm/__init__.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)    17651 2024-05-30 11:37:55.000000 nbnorm-0.4.0/nbnorm/nbnorm.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       22 2024-05-30 11:42:20.000000 nbnorm-0.4.0/nbnorm/version.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1482 2022-07-21 09:28:39.000000 nbnorm-0.4.0/nbnorm/xpath.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-30 11:42:47.469089 nbnorm-0.4.0/nbnorm.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)      530 2024-05-30 11:42:47.000000 nbnorm-0.4.0/nbnorm.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      299 2024-05-30 11:42:47.000000 nbnorm-0.4.0/nbnorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-05-30 11:42:47.000000 nbnorm-0.4.0/nbnorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       46 2024-05-30 11:42:47.000000 nbnorm-0.4.0/nbnorm.egg-info/entry_points.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-07-21 09:47:04.000000 nbnorm-0.4.0/nbnorm.egg-info/not-zip-safe
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-05-30 11:42:47.000000 nbnorm-0.4.0/nbnorm.egg-info/requires.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        7 2024-05-30 11:42:47.000000 nbnorm-0.4.0/nbnorm.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-05-30 11:42:47.470351 nbnorm-0.4.0/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1442 2022-07-21 09:35:19.000000 nbnorm-0.4.0/setup.py
```

### Comparing `nbnorm-0.3.2/nbnorm/nbnorm.py` & `nbnorm-0.4.0/nbnorm/nbnorm.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,44 +15,26 @@
 import IPython
 from nbformat.notebooknode import NotebookNode
 import jupytext
 
 
 from nbnorm.xpath import xpath, xpath_create
 
+from jupytext.config import find_jupytext_configuration_file, load_jupytext_configuration_file
 
-# we drop older versions, requires IPython v4
-assert IPython.version_info[0] >= 4
+def jupytext_config():
+    config_file = find_jupytext_configuration_file('.')
+    config = load_jupytext_configuration_file(config_file)
+    return config
 
 
-# not customizable yet
-# at the notebook level
-
-
-RISE_METADATA_PADDING = {
-    'rise': {
-        "autolaunch" : True,
-        "theme": "sky",
-        "start_slideshow_at": "selected",
-        "slideNumber": "c/t",
-        "transition": "cube",
-    },
-}
-
-# this was for the video slides, it's bad on regular notebooks
-RISE_METADATA_CLEAR = {
-#    'celltoolbar': 'Slideshow',
-}
-
-EXTENSIONS_METADATA_CELL_PADDING = {
-    "deletable": True,
-    "editable": True,
-    "run_control": {
-        "frozen": False,
-        "read_only": False
+LANG_INFO_PADDING = {
+    'language_info': {
+        'name': 'python',
+        'nbconvert_exporter': 'python',
     }
 }
 
 ####################
 # padding is a set of keys/subkeys
 # that we want to make sure are defined
 # this will never alter a key already present
@@ -101,15 +83,15 @@
         self.filename = self.name
         self.verbose = verbose
         self.notebook = None
 
 
     def parse(self):
         try:
-            self.notebook = jupytext.read(self.filename)
+            self.notebook = jupytext.read(self.filename, config=jupytext_config())
         except Exception:       # pylint: disable=broad-except
             print(f"Could not parse {self.filename}")
             traceback.print_exc()
 
     # def debug(self, message):
     #     print(f"-- {message} - we have {len(self.notebook.cells)} cells")
     #     for index, cell in enumerate(self.notebook.cells[:3]):
@@ -163,37 +145,21 @@
                       f"     not changed to `{new_title}`")
                 print(f"  use -f to override") # pylint: disable=f-string-without-interpolation
             return
         self.xpath('metadata.nbhosting')['title'] = new_title
         if self.verbose:
             print(f"{self.filename} title -> {self.xpath('metadata.nbhosting.title')}")
 
-
-    def fill_rise_metadata(self, rise):
-        """
-        if rise is set:
-        if metadata is missing the 'rise' key,
-        fill it with a set of hard-wired settings
-        """
-        if not rise:
-            return
-        metadata = self.notebook['metadata']
-        pad_metadata(metadata, RISE_METADATA_PADDING)
-        clear_metadata(metadata, RISE_METADATA_CLEAR)
-
-    def fill_extensions_metadata(self, extensions):
+    def fill_language_info(self, language_info):
         """
-        if extensions is set, fill each cell metadata's with a hard-wired
-        set of defaults for extensions; this is to minimize git diffs
+        make sure the language_info section is defined
         """
-        if not extensions:
+        if not language_info:
             return
-        for cell in self.cells():
-            pad_metadata(cell['metadata'], EXTENSIONS_METADATA_CELL_PADDING)
-
+        pad_metadata(self.notebook['metadata'], LANG_INFO_PADDING)
 
     def _ensure_item(self, name, cell_type, rank, crumb, template_filename):
         path = Path(template_filename)
 
         if not path.exists():
             raise FileNotFoundError(f"the {name} feature requires a {template_filename} file")
 
@@ -393,28 +359,28 @@
                     continue
                 match3 = re.search(rf'<.*{url}.*>', line)
                 if not match3:
                     print(f"DIRURL: {self.name}:{index} -> {line}")
 
 
     def save(self):
-        jupytext.write(self.notebook, self.filename)
+        jupytext.write(self.notebook, self.filename, config=jupytext_config())
         print(f"{self.filename} saved")
 
 
     def full_monty(self, *, title, force_title,
                    style_rank, style_crumb,
                    license_rank, license_crumb,
-                   rise, extensions, backquotes, urls):
+                   language_info,
+                   backquotes, urls):
         self.parse()
         self.clear_all_outputs()
         self.remove_empty_cells()
         self.set_title_from_heading1(title=title, force_title=force_title)
-        self.fill_rise_metadata(rise)
-        self.fill_extensions_metadata(extensions)
+        self.fill_language_info(language_info)
         if style_rank is not None:
             self.ensure_style(style_rank, style_crumb)
         if license_rank is not None:
             self.ensure_license(license_rank, license_crumb)
         self.fix_ill_formed_markdown_bullets()
         self.spot_long_code_cells()
         if backquotes:
@@ -431,17 +397,18 @@
 
 
 USAGE = """normalize notebooks
  * Metadata
    * checks for nbhosting.title (from first heading1 if missing, or from forced name on the command line)
  * Contents
    * makes sure a correct license cell is inserted - defined in .license
+   * same for a style cell - defined in .style
+* Miscell
    * clears all outputs
    * removes empty code cells
-* Miscell
   * also notify of miscell common markdown errors
 """
 
 def main():
     parser = ArgumentParser(usage=USAGE, formatter_class=ArgumentDefaultsHelpFormatter)
     parser.add_argument(
         "-t", "--title", action="store", dest="title", default=None,
@@ -466,19 +433,16 @@
         help="""make sure the license cell is up-to-date with .license;
                 provide the license cell rank, used only for inserting a missing cell;
                 default is to not manage license""")
     parser.add_argument(
         "-L", "--license-crumb", default="license",
         help="a cell that contains that string is considered a license cell")
     parser.add_argument(
-        "-r", "--rise", dest='rise', default=False, action='store_true',
-        help="fill in RISE/livereveal metadata with hard-wired settings")
-    parser.add_argument(
-        "-e", "--extensions", dest='extensions', action='store_true', default=False,
-        help="fill cell metadata for extensions, if missing")
+        "-i", "--language-info", default=False, action='store_true',
+        help="make sure the language_info section is defined")
     parser.add_argument(
         "-b", "--backquotes", default=False, action='store_true',
         help="check for use of ``` rather than 4 preceding spaces")
     parser.add_argument(
         "-u", "--urls", default=False, action='store_true',
         help="tries to spot direct URLs, i.e. used outside of markdown []()")
     parser.add_argument(
@@ -497,16 +461,15 @@
     if args.summary:
         print(f"nbhosting.title: {args.title}")
         print(f"force title: {args.force_title}")
         print(f"style rank: {args.style_rank}")
         print(f"style crumb: {args.style_crumb}")
         print(f"license rank: {args.license_rank}")
         print(f"license crumb: {args.license_crumb}")
-        print(f"rise: {args.rise}")
-        print(f"extensions: {args.extensions}")
+        print(f"language info: {args.language_info}")
         print(f"backquotes: {args.backquotes}")
         print(f"urls: {args.urls}")
         exit(0)
 
     if not args.notebooks:
         parser.print_help()
         sys.exit(1)
@@ -514,13 +477,13 @@
     for notebook in args.notebooks:
         if args.verbose:
             print(f"{sys.argv[0]} is opening notebook {notebook}")
         full_monty(
             notebook, title=args.title, force_title=args.force_title,
             license_rank=args.license_rank, license_crumb=args.license_crumb,
             style_rank=args.style_rank, style_crumb=args.style_crumb,
-            rise=args.rise,
-            extensions=args.extensions, backquotes=args.backquotes,
+            language_info=args.language_info,
+            backquotes=args.backquotes,
             urls=args.urls, verbose=args.verbose)
 
 if __name__ == '__main__':
     main()
```

### Comparing `nbnorm-0.3.2/nbnorm/xpath.py` & `nbnorm-0.4.0/nbnorm/xpath.py`

 * *Files identical despite different names*

### Comparing `nbnorm-0.3.2/setup.py` & `nbnorm-0.4.0/setup.py`

 * *Files identical despite different names*

