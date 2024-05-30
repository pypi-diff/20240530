# Comparing `tmp/hextools-0.1.3.tar.gz` & `tmp/hextools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hextools-0.1.3.tar", last modified: Thu Mar 14 00:02:07 2024, max compression
+gzip compressed data, was "hextools-0.2.0.tar", last modified: Thu May 30 16:42:39 2024, max compression
```

## Comparing `hextools-0.1.3.tar` & `hextools-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.213822 hextools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-14 00:01:46.000000 hextools-0.1.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 00:01:46.000000 hextools-0.1.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-14 00:01:46.000000 hextools-0.1.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.209822 hextools-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-14 00:01:46.000000 hextools-0.1.3/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-14 00:01:46.000000 hextools-0.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.209822 hextools-0.1.3/.github/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-14 00:01:46.000000 hextools-0.1.3/.github/matchers/pylint.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.209822 hextools-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-14 00:01:46.000000 hextools-0.1.3/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-14 00:01:46.000000 hextools-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-14 00:01:46.000000 hextools-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-14 00:01:46.000000 hextools-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-14 00:01:46.000000 hextools-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-14 00:02:07.213822 hextools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-14 00:01:46.000000 hextools-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.209822 hextools-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-14 00:01:46.000000 hextools-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-14 00:01:46.000000 hextools-0.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-03-14 00:01:46.000000 hextools-0.1.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-14 00:01:46.000000 hextools-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 00:02:07.213822 hextools-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.205822 hextools-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.209822 hextools-0.1.3/src/hextools/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-14 00:02:07.000000 hextools-0.1.3/src/hextools/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/_version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.213822 hextools-0.1.3/src/hextools/germ/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/germ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/germ/caproto_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/germ/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/germ/ophyd.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-14 00:01:46.000000 hextools-0.1.3/src/hextools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.213822 hextools-0.1.3/src/hextools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-14 00:02:07.000000 hextools-0.1.3/src/hextools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-14 00:02:07.000000 hextools-0.1.3/src/hextools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 00:02:07.000000 hextools-0.1.3/src/hextools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-14 00:02:07.000000 hextools-0.1.3/src/hextools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-14 00:02:07.000000 hextools-0.1.3/src/hextools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 00:02:07.000000 hextools-0.1.3/src/hextools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:02:07.213822 hextools-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-14 00:01:46.000000 hextools-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-14 00:01:46.000000 hextools-0.1.3/tests/test_data_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-14 00:01:46.000000 hextools-0.1.3/tests/test_germ.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-14 00:01:46.000000 hextools-0.1.3/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.975440 hextools-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 16:42:36.000000 hextools-0.2.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 16:42:36.000000 hextools-0.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 16:42:36.000000 hextools-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.967440 hextools-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-30 16:42:36.000000 hextools-0.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-30 16:42:36.000000 hextools-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.967440 hextools-0.2.0/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 16:42:36.000000 hextools-0.2.0/.github/matchers/pylint.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.967440 hextools-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 16:42:36.000000 hextools-0.2.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-30 16:42:36.000000 hextools-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-30 16:42:36.000000 hextools-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-30 16:42:36.000000 hextools-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-30 16:42:36.000000 hextools-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-30 16:42:39.975440 hextools-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-30 16:42:36.000000 hextools-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.967440 hextools-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-30 16:42:36.000000 hextools-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 16:42:36.000000 hextools-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-30 16:42:36.000000 hextools-0.2.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-30 16:42:36.000000 hextools-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:42:39.975440 hextools-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.963439 hextools-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.967440 hextools-0.2.0/src/hextools/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 16:42:39.000000 hextools-0.2.0/src/hextools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/_version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.971440 hextools-0.2.0/src/hextools/germ/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/germ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/germ/caproto_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/germ/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/germ/ophyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 16:42:36.000000 hextools-0.2.0/src/hextools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.971440 hextools-0.2.0/src/hextools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-30 16:42:39.000000 hextools-0.2.0/src/hextools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-30 16:42:39.000000 hextools-0.2.0/src/hextools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:42:39.000000 hextools-0.2.0/src/hextools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 16:42:39.000000 hextools-0.2.0/src/hextools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-30 16:42:39.000000 hextools-0.2.0/src/hextools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 16:42:39.000000 hextools-0.2.0/src/hextools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:42:39.971440 hextools-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-30 16:42:36.000000 hextools-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-30 16:42:36.000000 hextools-0.2.0/tests/test_data_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-30 16:42:36.000000 hextools-0.2.0/tests/test_germ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:42:36.000000 hextools-0.2.0/tests/test_package.py
```

### Comparing `hextools-0.1.3/.github/CONTRIBUTING.md` & `hextools-0.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/.github/matchers/pylint.json` & `hextools-0.2.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/.github/workflows/cd.yml` & `hextools-0.2.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/.github/workflows/ci.yml` & `hextools-0.2.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -63,8 +63,8 @@
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20 -m "(not hardware) and (not tiled)"
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.4.1
```

### Comparing `hextools-0.1.3/.gitignore` & `hextools-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/.pre-commit-config.yaml` & `hextools-0.2.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.*]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -32,49 +32,49 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.1.0"
+    rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.9"
+    rev: "v0.4.4"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: "v0.9.0.6"
+    rev: "v0.10.0.1"
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.18
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.27.0
+    rev: 0.28.4
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
```

### Comparing `hextools-0.1.3/LICENSE` & `hextools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/PKG-INFO` & `hextools-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hextools
-Version: 0.1.3
+Version: 0.2.0
 Summary: Tools for NSLS-II HEX beamline
 Author-email: Brookhaven National Laboratory <mrakitin@bnl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Brookhaven National Laboratory.
         All rights reserved.
         
@@ -53,15 +53,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: area-detector-handlers
 Requires-Dist: caproto
-Requires-Dist: event-model
+Requires-Dist: event-model>=1.21.0
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: ophyd
 Requires-Dist: pillow
 Requires-Dist: pyepics
 Requires-Dist: tifffile
 Provides-Extra: test
```

### Comparing `hextools-0.1.3/README.md` & `hextools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/docs/conf.py` & `hextools-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/noxfile.py` & `hextools-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/pyproject.toml` & `hextools-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   "area-detector-handlers",
   "caproto",
-  "event-model",
+  "event-model>=1.21.0",
   "h5py",
   "numpy",
   "ophyd",
   "pillow",
   "pyepics",
   "tifffile",
 ]
```

### Comparing `hextools-0.1.3/src/hextools/germ/caproto_ioc.py` & `hextools-0.2.0/src/hextools/germ/caproto_ioc.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,36 +100,18 @@
     count = pvproperty_with_rbv(
         value=AcqStatuses.IDLE.value,
         enum_strings=[x.value for x in AcqStatuses],
         dtype=ChannelType.ENUM,
         doc="Trigger the detector via a mirrored PV and save the data",
     )
 
-    _already_counting = None
-    _already_done = None
-
     async def callback_count(self, pv, response):
         """A callback method for the 'count' PV."""
         # pylint: disable=unused-argument
-
-        # The conditions below are needed to account for doubled
-        # Count(=1)/Done(=0)responses from the libCA IOC to process such events
-        # only once.
-        if response.data[0] == 1:
-            if self._already_counting in (None, False):
-                self._already_counting = True
-                await self.count.readback.write(response.data)
-            else:
-                self._already_counting = False
-        elif response.data[0] == 0:
-            if self._already_done in (None, False):
-                self._already_done = True
-                await self.count.readback.write(response.data)
-            else:
-                self._already_done = False
+        await self.count.readback.write(response.data)
 
     @count.setpoint.startup
     async def count(obj, instance, async_lib):
         # pylint: disable=[function-redefined, no-self-argument, unused-argument, protected-access]
         """Startup behavior of count."""
         await obj.parent._add_subscription("count")
```

### Comparing `hextools-0.1.3/src/hextools/germ/export.py` & `hextools-0.2.0/src/hextools/germ/export.py`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/src/hextools/germ/ophyd.py` & `hextools-0.2.0/src/hextools/germ/ophyd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from __future__ import annotations
 
 import datetime
+import logging
 import uuid
 from collections import deque
 from pathlib import Path
+from pprint import pformat
 
 import numpy as np
-from event_model import compose_resource
+from event_model import StreamRange, compose_resource, compose_stream_resource
 from ophyd import Component as Cpt
 from ophyd import Device, EpicsSignal, Kind, Signal
 from ophyd.sim import new_uid
 from ophyd.status import SubscriptionStatus
 from PIL import Image
 
+from hextools.utils import get_ioc_hostname
+
 from . import AcqStatuses, StageStates
 
+logger = logging.getLogger(__name__)
+
 
 class ExternalFileReference(Signal):
     """
     A pure software Signal that describe()s an image in an external file.
     """
 
     def describe(self):
         resource_document_data = super().describe()
         resource_document_data[self.name].update(
             {
-                "external": "FILESTORE:",
+                "external": "STREAM:",
                 "dtype": "array",
             }
         )
         return resource_document_data
 
 
 class GeRMMiniClassForCaprotoIOC(Device):
@@ -104,27 +110,27 @@
 
     def __init__(self, *args, root_dir=None, **kwargs):
         super().__init__(*args, **kwargs)
         if root_dir is None:
             msg = "The 'root_dir' kwarg cannot be None"
             raise RuntimeError(msg)
         self._root_dir = root_dir
-        self._resource_document, self._datum_factory = None, None
+        self._stream_resource_document, self._stream_datum_factory = None, None
         self._asset_docs_cache = deque()
 
     def collect_asset_docs(self):
         """The method to collect resource/datum documents."""
         items = list(self._asset_docs_cache)
         self._asset_docs_cache.clear()
         yield from items
 
     def unstage(self):
         super().unstage()
-        self._resource_document = None
-        self._datum_factory = None
+        self._stream_resource_document = None
+        self._stream_datum_factory = None
 
     def get_current_image(self):
         """The function to return a current image from detector's MCA."""
         # This is the reshaping we want
         # This doesn't trigger the detector
         raw_data = self.mca.get()
         return np.reshape(raw_data, self.frame_shape)
@@ -137,14 +143,18 @@
         return True
     return False
 
 
 class GeRMDetectorTIFF(GeRMDetectorBase):
     """The ophyd class for GeRM detector producing TIFF files."""
 
+    def __init__(self, *args, root_dir=None, **kwargs):
+        super().__init__(*args, root_dir=root_dir, **kwargs)
+        self._resource_document, self._datum_factory = None, None
+
     def trigger(self):
         "The trigger method to acquire a single frame."
 
         status = SubscriptionStatus(self.count, run=False, callback=done_callback)
 
         self.count.put(AcqStatuses.ACQUIRING.value)
         status.wait()
@@ -213,25 +223,37 @@
         self._asset_docs_cache.clear()
 
         date = datetime.datetime.now()
         assets_dir = date.strftime("%Y/%m/%d")
         data_file_no_ext = f"{new_uid()}"
         data_file_with_ext = f"{data_file_no_ext}.h5"
 
-        self._resource_document, self._datum_factory, _ = compose_resource(
-            start={"uid": "needed for compose_resource() but will be discarded"},
-            spec="AD_HDF5_GERM",
-            root=self._root_dir,
-            resource_path=str(Path(assets_dir) / Path(data_file_with_ext)),
-            resource_kwargs={},
+        full_path = Path(self._root_dir) / Path(assets_dir) / Path(data_file_with_ext)
+
+        hostname = get_ioc_hostname(self.count.pvname)
+        uri = f"file://{hostname}/{str(full_path).strip('/')}"
+
+        (
+            self._stream_resource_document,
+            self._stream_datum_factory,
+        ) = compose_stream_resource(
+            mimetype="application/x-hdf5",
+            uri=uri,
+            data_key=self.image.name,
+            parameters={"chunk_size": 1, "path": "/entry/data/data"},
         )
 
-        # now discard the start uid, a real one will be added later
-        self._resource_document.pop("run_start")
-        self._asset_docs_cache.append(("resource", self._resource_document))
+        logger.debug(
+            "stream_resource_doc:\n %s", {pformat(self._stream_resource_document)}
+        )
+
+        # self._stream_resource_document.pop("run_start")
+        self._asset_docs_cache.append(
+            ("stream_resource", self._stream_resource_document)
+        )
 
         # Update caproto IOC parameters:
         self.write_dir.put(self._root_dir)
         self.file_name_prefix.put(data_file_no_ext)
         self.ioc_stage.put(StageStates.STAGED.value)
 
     def describe(self):
@@ -242,19 +264,22 @@
         return res
 
     def trigger(self):
         status = SubscriptionStatus(self.count, run=False, callback=done_callback)
 
         # Reuse the counter from the caproto IOC
         current_frame = self.frame_num.get()
+        stream_datum_document = self._stream_datum_factory(
+            StreamRange(start=current_frame, stop=current_frame + 1),
+        )
+
         self.count.put(AcqStatuses.ACQUIRING.value)
 
-        datum_document = self._datum_factory(datum_kwargs={"frame": current_frame})
-        self._asset_docs_cache.append(("datum", datum_document))
+        logger.debug("stream_datum_document:\n%s", pformat(stream_datum_document))
 
-        self.image.put(datum_document["datum_id"])
+        self._asset_docs_cache.append(("stream_datum", stream_datum_document))
 
         return status
 
     def unstage(self):
         self.ioc_stage.put(StageStates.UNSTAGED.value)
         super().unstage()
```

### Comparing `hextools-0.1.3/src/hextools/handlers.py` & `hextools-0.2.0/src/hextools/handlers.py`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/src/hextools.egg-info/PKG-INFO` & `hextools-0.2.0/src/hextools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hextools
-Version: 0.1.3
+Version: 0.2.0
 Summary: Tools for NSLS-II HEX beamline
 Author-email: Brookhaven National Laboratory <mrakitin@bnl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Brookhaven National Laboratory.
         All rights reserved.
         
@@ -53,15 +53,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: area-detector-handlers
 Requires-Dist: caproto
-Requires-Dist: event-model
+Requires-Dist: event-model>=1.21.0
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: ophyd
 Requires-Dist: pillow
 Requires-Dist: pyepics
 Requires-Dist: tifffile
 Provides-Extra: test
```

### Comparing `hextools-0.1.3/src/hextools.egg-info/SOURCES.txt` & `hextools-0.2.0/src/hextools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/tests/conftest.py` & `hextools-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/tests/test_data_access.py` & `hextools-0.2.0/tests/test_data_access.py`

 * *Files identical despite different names*

### Comparing `hextools-0.1.3/tests/test_germ.py` & `hextools-0.2.0/tests/test_germ.py`

 * *Files identical despite different names*

