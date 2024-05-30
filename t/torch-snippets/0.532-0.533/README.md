# Comparing `tmp/torch_snippets-0.532.tar.gz` & `tmp/torch_snippets-0.533.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.532.tar", last modified: Thu May 23 10:47:04 2024, max compression
+gzip compressed data, was "torch_snippets-0.533.tar", last modified: Thu May 30 06:24:55 2024, max compression
```

## Comparing `torch_snippets-0.532.tar` & `torch_snippets-0.533.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.065409 torch_snippets-0.532/
--rw-r--r--   0 apple      (501) staff       (20)    11357 2024-05-16 14:23:49.000000 torch_snippets-0.532/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)     1062 2024-05-16 14:23:49.000000 torch_snippets-0.532/LICENSE.txt
--rw-r--r--   0 apple      (501) staff       (20)      111 2024-05-16 14:23:49.000000 torch_snippets-0.532/MANIFEST.in
--rw-r--r--   0 apple      (501) staff       (20)     6437 2024-05-23 10:47:04.065328 torch_snippets-0.532/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     4999 2024-05-16 14:23:49.000000 torch_snippets-0.532/README.md
--rw-r--r--   0 apple      (501) staff       (20)      871 2024-05-23 10:33:02.000000 torch_snippets-0.532/settings.ini
--rw-r--r--   0 apple      (501) staff       (20)       79 2024-05-23 10:47:04.065621 torch_snippets-0.532/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     2001 2024-05-16 14:23:49.000000 torch_snippets-0.532/setup.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.062721 torch_snippets-0.532/torch_snippets/
--rw-r--r--   0 apple      (501) staff       (20)      401 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    57057 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/_modidx.py
--rw-r--r--   0 apple      (501) staff       (20)     4482 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/_nbdev.py
--rw-r--r--   0 apple      (501) staff       (20)     8846 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/adapters.py
--rw-r--r--   0 apple      (501) staff       (20)    17079 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/bb_utils.py
--rw-r--r--   0 apple      (501) staff       (20)     2026 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/bokeh_loader.py
--rw-r--r--   0 apple      (501) staff       (20)    19042 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/charts.py
--rw-r--r--   0 apple      (501) staff       (20)     1866 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/dates.py
--rw-r--r--   0 apple      (501) staff       (20)     2056 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/decorators.py
--rw-r--r--   0 apple      (501) staff       (20)       73 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/fastcores.py
--rw-r--r--   0 apple      (501) staff       (20)    11427 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/icecream.py
--rw-r--r--   0 apple      (501) staff       (20)     8479 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/imgaug_loader.py
--rw-r--r--   0 apple      (501) staff       (20)     3429 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/inspector.py
--rw-r--r--   0 apple      (501) staff       (20)     8386 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/interactive_show.py
--rw-r--r--   0 apple      (501) staff       (20)     5727 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/ipython.py
--rw-r--r--   0 apple      (501) staff       (20)      597 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/load_defaults.py
--rwxr-xr-x   0 apple      (501) staff       (20)    23434 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/loader.py
--rw-r--r--   0 apple      (501) staff       (20)     8480 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/logger.py
--rw-r--r--   0 apple      (501) staff       (20)    15588 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/markup.py
--rw-r--r--   0 apple      (501) staff       (20)    17741 2024-05-23 10:32:45.000000 torch_snippets-0.532/torch_snippets/markup2.py
--rw-r--r--   0 apple      (501) staff       (20)     2054 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/misc.py
--rw-r--r--   0 apple      (501) staff       (20)    11039 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/paths.py
--rw-r--r--   0 apple      (501) staff       (20)     1465 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/pdf_loader.py
--rw-r--r--   0 apple      (501) staff       (20)      822 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/registry.py
--rw-r--r--   0 apple      (501) staff       (20)     3234 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/scp.py
--rw-r--r--   0 apple      (501) staff       (20)     6144 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/sklegos.py
--rw-r--r--   0 apple      (501) staff       (20)    14202 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/text_utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.063714 torch_snippets-0.532/torch_snippets/thinc_parser/
--rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1082 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 apple      (501) staff       (20)    31250 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/torch_loader.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.064574 torch_snippets-0.532/torch_snippets/trainer/
--rw-r--r--   0 apple      (501) staff       (20)       23 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/trainer/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     6882 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/trainer/capsule.py
--rw-r--r--   0 apple      (501) staff       (20)     2432 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/trainer/config.py
--rw-r--r--   0 apple      (501) staff       (20)     5801 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/trainer/hooks.py
--rw-r--r--   0 apple      (501) staff       (20)     2137 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/video.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.064933 torch_snippets-0.532/torch_snippets.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     6437 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     1296 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 apple      (501) staff       (20)      281 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)       15 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-30 06:24:55.818865 torch_snippets-0.533/
+-rw-r--r--   0 apple      (501) staff       (20)    11357 2024-05-16 14:23:49.000000 torch_snippets-0.533/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)     1062 2024-05-16 14:23:49.000000 torch_snippets-0.533/LICENSE.txt
+-rw-r--r--   0 apple      (501) staff       (20)      111 2024-05-16 14:23:49.000000 torch_snippets-0.533/MANIFEST.in
+-rw-r--r--   0 apple      (501) staff       (20)     6437 2024-05-30 06:24:55.818783 torch_snippets-0.533/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     4999 2024-05-16 14:23:49.000000 torch_snippets-0.533/README.md
+-rw-r--r--   0 apple      (501) staff       (20)      871 2024-05-30 06:23:51.000000 torch_snippets-0.533/settings.ini
+-rw-r--r--   0 apple      (501) staff       (20)       79 2024-05-30 06:24:55.819085 torch_snippets-0.533/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)     2001 2024-05-16 14:23:49.000000 torch_snippets-0.533/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-30 06:24:55.816799 torch_snippets-0.533/torch_snippets/
+-rw-r--r--   0 apple      (501) staff       (20)      401 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    57320 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/_modidx.py
+-rw-r--r--   0 apple      (501) staff       (20)     4482 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/_nbdev.py
+-rw-r--r--   0 apple      (501) staff       (20)     8846 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/adapters.py
+-rw-r--r--   0 apple      (501) staff       (20)    17079 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/bb_utils.py
+-rw-r--r--   0 apple      (501) staff       (20)     2026 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 apple      (501) staff       (20)    19042 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/charts.py
+-rw-r--r--   0 apple      (501) staff       (20)     1866 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/dates.py
+-rw-r--r--   0 apple      (501) staff       (20)     2056 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/decorators.py
+-rw-r--r--   0 apple      (501) staff       (20)       73 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/fastcores.py
+-rw-r--r--   0 apple      (501) staff       (20)    11427 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/icecream.py
+-rw-r--r--   0 apple      (501) staff       (20)     8479 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 apple      (501) staff       (20)     3429 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/inspector.py
+-rw-r--r--   0 apple      (501) staff       (20)     8386 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/interactive_show.py
+-rw-r--r--   0 apple      (501) staff       (20)     5727 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/ipython.py
+-rw-r--r--   0 apple      (501) staff       (20)      597 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 apple      (501) staff       (20)    23434 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/loader.py
+-rw-r--r--   0 apple      (501) staff       (20)     8480 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/logger.py
+-rw-r--r--   0 apple      (501) staff       (20)    15874 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/markup.py
+-rw-r--r--   0 apple      (501) staff       (20)    17904 2024-05-24 04:38:00.000000 torch_snippets-0.533/torch_snippets/markup2.py
+-rw-r--r--   0 apple      (501) staff       (20)     2054 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/misc.py
+-rw-r--r--   0 apple      (501) staff       (20)    11039 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/paths.py
+-rw-r--r--   0 apple      (501) staff       (20)     1465 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/pdf_loader.py
+-rw-r--r--   0 apple      (501) staff       (20)      822 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/registry.py
+-rw-r--r--   0 apple      (501) staff       (20)     3234 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/scp.py
+-rw-r--r--   0 apple      (501) staff       (20)     6144 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/sklegos.py
+-rw-r--r--   0 apple      (501) staff       (20)    14202 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/text_utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-30 06:24:55.817723 torch_snippets-0.533/torch_snippets/thinc_parser/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1082 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 apple      (501) staff       (20)    31250 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/torch_loader.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-30 06:24:55.818240 torch_snippets-0.533/torch_snippets/trainer/
+-rw-r--r--   0 apple      (501) staff       (20)       23 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     6882 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 apple      (501) staff       (20)     2432 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets/trainer/config.py
+-rw-r--r--   0 apple      (501) staff       (20)     5934 2024-05-30 06:23:08.000000 torch_snippets-0.533/torch_snippets/trainer/hooks.py
+-rw-r--r--   0 apple      (501) staff       (20)     2137 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets/video.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-30 06:24:55.818453 torch_snippets-0.533/torch_snippets.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     6437 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     1296 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-16 14:23:49.000000 torch_snippets-0.533/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 apple      (501) staff       (20)      281 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)       15 2024-05-30 06:24:55.000000 torch_snippets-0.533/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.532/LICENSE` & `torch_snippets-0.533/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/LICENSE.txt` & `torch_snippets-0.533/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/PKG-INFO` & `torch_snippets-0.533/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_snippets
-Version: 0.532
+Version: 0.533
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.532/README.md` & `torch_snippets-0.533/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/settings.ini` & `torch_snippets-0.533/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.532
+version = 0.533
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = fastcore matplotlib Pillow altair dill ipython loguru numpy pandas tqdm rich PyYAML catalogue confection pydantic typing srsly typing_extensions wasabi jsonlines imgaug>=0.4.0 xmltodict fuzzywuzzy scikit-learn nltk python-Levenshtein pre-commit pymupdf nbconvert nbformat icecream
```

### Comparing `torch_snippets-0.532/setup.py` & `torch_snippets-0.533/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/_modidx.py` & `torch_snippets-0.533/torch_snippets/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,15 @@
                                        'torch_snippets.markup.AttrDict.update': ( 'markups.html#attrdict.update',
                                                                                   'torch_snippets/markup.py'),
                                        'torch_snippets.markup.AttrDict.values': ( 'markups.html#attrdict.values',
                                                                                   'torch_snippets/markup.py'),
                                        'torch_snippets.markup.AttrDict.write_summary': ( 'markups.html#attrdict.write_summary',
                                                                                          'torch_snippets/markup.py'),
                                        'torch_snippets.markup._default': ('markups.html#_default', 'torch_snippets/markup.py'),
+                                       'torch_snippets.markup.decompose': ('markups.html#decompose', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.isnamedtupleinstance': ( 'markups.html#isnamedtupleinstance',
                                                                                        'torch_snippets/markup.py'),
                                        'torch_snippets.markup.pretty_json': ('markups.html#pretty_json', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.read_json': ('markups.html#read_json', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.read_jsonl': ('markups.html#read_jsonl', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.read_xml': ('markups.html#read_xml', 'torch_snippets/markup.py'),
                                        'torch_snippets.markup.read_yaml': ('markups.html#read_yaml', 'torch_snippets/markup.py'),
@@ -264,14 +265,15 @@
                                         'torch_snippets.markup2.AttrDict.update': ( 'markups.html#attrdict.update',
                                                                                     'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2.AttrDict.values': ( 'markups.html#attrdict.values',
                                                                                     'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2.AttrDict.write_summary': ( 'markups.html#attrdict.write_summary',
                                                                                            'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2._default': ('markups.html#_default', 'torch_snippets/markup2.py'),
+                                        'torch_snippets.markup2.decompose': ('markups.html#decompose', 'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2.hash_pandas_dataframe': ( 'markups.html#hash_pandas_dataframe',
                                                                                           'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2.hash_tensor': ('markups.html#hash_tensor', 'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2.isnamedtupleinstance': ( 'markups.html#isnamedtupleinstance',
                                                                                          'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2.pretty_json': ('markups.html#pretty_json', 'torch_snippets/markup2.py'),
                                         'torch_snippets.markup2.read_json': ('markups.html#read_json', 'torch_snippets/markup2.py'),
```

### Comparing `torch_snippets-0.532/torch_snippets/_nbdev.py` & `torch_snippets-0.533/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/adapters.py` & `torch_snippets-0.533/torch_snippets/adapters.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/bb_utils.py` & `torch_snippets-0.533/torch_snippets/bb_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/bokeh_loader.py` & `torch_snippets-0.533/torch_snippets/bokeh_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/charts.py` & `torch_snippets-0.533/torch_snippets/charts.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/dates.py` & `torch_snippets-0.533/torch_snippets/dates.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/decorators.py` & `torch_snippets-0.533/torch_snippets/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/icecream.py` & `torch_snippets-0.533/torch_snippets/icecream.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/imgaug_loader.py` & `torch_snippets-0.533/torch_snippets/imgaug_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/inspector.py` & `torch_snippets-0.533/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/interactive_show.py` & `torch_snippets-0.533/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/ipython.py` & `torch_snippets-0.533/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/load_defaults.py` & `torch_snippets-0.533/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/loader.py` & `torch_snippets-0.533/torch_snippets/loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/logger.py` & `torch_snippets-0.533/torch_snippets/logger.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/markup.py` & `torch_snippets-0.533/torch_snippets/markup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/markups.ipynb.
 
 # %% auto 0
-__all__ = ['AD', 'Config', 'isnamedtupleinstance', 'unpack', 'AttrDict', 'pretty_json', 'read_json', 'write_json', 'write_jsonl',
-           'read_jsonl', 'read_yaml', 'write_yaml', 'read_xml', 'write_xml']
+__all__ = ['AD', 'Config', 'isnamedtupleinstance', 'unpack', 'AttrDict', 'decompose', 'pretty_json', 'read_json', 'write_json',
+           'write_jsonl', 'read_jsonl', 'read_yaml', 'write_yaml', 'read_xml', 'write_xml']
 
 # %% ../nbs/markups.ipynb 2
 import json, os
 from json import JSONEncoder
 import jsonlines
 import yaml
 
@@ -267,14 +267,16 @@
             elif isinstance(item, (torch.Tensor, np.ndarray)):
                 is_np = False
                 if isinstance(item, np.ndarray):
                     is_np = True
                     item = torch.tensor(item)
                 is_np = "🔦" if not is_np else "np."
                 return f"{sep * depth}{key} - {is_np}{item} - {hash_tensor(item)}\n"
+            elif isinstance(item, type):
+                raise NotImplementedError("Implement for type object")
 
             else:
                 if isinstance(item, (int, float, complex, str)):
                     is_multiline = False
                     if isinstance(item, str):
                         is_multiline = "\n" in item
                         _sep = (
@@ -329,14 +331,21 @@
             except:
                 o = o[p]
         return o
 
 
 AD = AttrDict
 
+def decompose(i):
+    print(
+        AD(
+            {k: getattr(i, k) for k in dir(i) if not k.startswith("_")},
+            type=str(type(i)),
+        )
+    )
 
 def pretty_json(
     i, fpath=None, indent=4, print_with_logger=True, return_as_string=False
 ):
     def set_default(obj):
         if isinstance(obj, (set, BB, L)):
             return list(obj)
```

### Comparing `torch_snippets-0.532/torch_snippets/markup2.py` & `torch_snippets-0.533/torch_snippets/markup2.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,14 +490,23 @@
     with open(file_path, "w") as xml_file:
         data = data.to_dict() if isinstance(data, AttrDict) else data
         assert isinstance(data, dict), "Function only supports dicts for now"
         data = xmltodict.unparse(data, pretty=True)
         xml_file.write(data)
 
 
+def decompose(i):
+    print(
+        AD(
+            {k: getattr(i, k) for k in dir(i) if not k.startswith("_")},
+            type=str(type(i)),
+        )
+    )
+
+
 # %% ../nbs/markups.ipynb 13
 Config = Config
 
 if __name__ == "__main__":
     assert AD({}) == {}
 
     p = 1
```

### Comparing `torch_snippets-0.532/torch_snippets/misc.py` & `torch_snippets-0.533/torch_snippets/misc.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/paths.py` & `torch_snippets-0.533/torch_snippets/paths.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/pdf_loader.py` & `torch_snippets-0.533/torch_snippets/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/registry.py` & `torch_snippets-0.533/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/scp.py` & `torch_snippets-0.533/torch_snippets/scp.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/sklegos.py` & `torch_snippets-0.533/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/text_utils.py` & `torch_snippets-0.533/torch_snippets/text_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.533/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/torch_loader.py` & `torch_snippets-0.533/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/trainer/capsule.py` & `torch_snippets-0.533/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/trainer/config.py` & `torch_snippets-0.533/torch_snippets/trainer/config.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets/trainer/hooks.py` & `torch_snippets-0.533/torch_snippets/trainer/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,28 +105,33 @@
     parent_name="",
 ):
     """Function to attach the hooks and return handles"""
     # handles = [model.register_forward_hook(hook, with_kwargs=True)]
     handles = []
     for child_name, layer in model.named_children():
         _child_name = f"{parent_name}.{child_name}" if parent_name != "" else child_name
-        if required_children is not None and _child_name in required_children:
+        if (
+            required_children is not None and _child_name in required_children
+        ) or (
+            layer.__class__.__name__ in print_only
+        ):
             _hook = partial(
                 print_shapes_hook,
                 keep={layer.__class__.__name__},
                 child_name=_child_name,
             )
             handle = layer.register_forward_hook(_hook, with_kwargs=True)
             handles.append(handle)
         if len(list(layer.children())) > 0:
             handles.extend(
                 attach_hooks(
                     layer,
                     hook=hook,
                     required_children=required_children,
+                    print_only=print_only,
                     parent_name=_child_name,
                 )
             )
     return handles
 
 
 def detach_hooks(handles):
```

### Comparing `torch_snippets-0.532/torch_snippets/video.py` & `torch_snippets-0.533/torch_snippets/video.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.532/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.533/torch_snippets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_snippets
-Version: 0.532
+Version: 0.533
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.532/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.533/torch_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

