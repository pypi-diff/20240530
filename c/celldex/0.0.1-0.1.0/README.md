# Comparing `tmp/celldex-0.0.1.tar.gz` & `tmp/celldex-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celldex-0.0.1.tar", last modified: Tue May 28 20:37:14 2024, max compression
+gzip compressed data, was "celldex-0.1.0.tar", last modified: Wed May 29 20:31:26 2024, max compression
```

## Comparing `celldex-0.0.1.tar` & `celldex-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.314721 celldex-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-28 20:36:34.000000 celldex-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.306721 celldex-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.310721 celldex-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-28 20:36:34.000000 celldex-0.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-28 20:36:34.000000 celldex-0.0.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 20:36:34.000000 celldex-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-28 20:36:34.000000 celldex-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 20:36:34.000000 celldex-0.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 20:36:34.000000 celldex-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 20:36:34.000000 celldex-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-05-28 20:36:34.000000 celldex-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 20:36:34.000000 celldex-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-28 20:37:14.314721 celldex-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-28 20:36:34.000000 celldex-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.310721 celldex-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.310721 celldex-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 20:36:34.000000 celldex-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 20:36:34.000000 celldex-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-28 20:37:14.314721 celldex-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-28 20:36:34.000000 celldex-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.306721 celldex-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.310721 celldex-0.0.1/src/celldex/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 20:36:34.000000 celldex-0.0.1/src/celldex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-28 20:36:34.000000 celldex-0.0.1/src/celldex/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.314721 celldex-0.0.1/src/celldex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-28 20:37:14.000000 celldex-0.0.1/src/celldex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-28 20:37:14.000000 celldex-0.0.1/src/celldex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:37:14.000000 celldex-0.0.1/src/celldex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:37:14.000000 celldex-0.0.1/src/celldex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 20:37:14.000000 celldex-0.0.1/src/celldex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 20:37:14.000000 celldex-0.0.1/src/celldex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:37:14.314721 celldex-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:36:34.000000 celldex-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-28 20:36:34.000000 celldex-0.0.1/tests/test_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 20:36:34.000000 celldex-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.112904 celldex-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-29 20:27:51.000000 celldex-0.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.100904 celldex-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.104904 celldex-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-29 20:27:51.000000 celldex-0.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-29 20:27:51.000000 celldex-0.1.0/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 20:27:51.000000 celldex-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-29 20:27:51.000000 celldex-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-29 20:27:51.000000 celldex-0.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 20:27:51.000000 celldex-0.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-29 20:27:51.000000 celldex-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-05-29 20:27:51.000000 celldex-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 20:27:51.000000 celldex-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-29 20:31:26.112904 celldex-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-29 20:27:51.000000 celldex-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.108904 celldex-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.108904 celldex-0.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-29 20:27:51.000000 celldex-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 20:27:51.000000 celldex-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-29 20:31:26.112904 celldex-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-29 20:27:51.000000 celldex-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.100904 celldex-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.108904 celldex-0.1.0/src/celldex/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/fetch_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/list_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/list_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/save_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/search_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/upload_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-29 20:27:51.000000 celldex-0.1.0/src/celldex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.112904 celldex-0.1.0/src/celldex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-29 20:31:26.000000 celldex-0.1.0/src/celldex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-29 20:31:26.000000 celldex-0.1.0/src/celldex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:31:26.000000 celldex-0.1.0/src/celldex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:31:25.000000 celldex-0.1.0/src/celldex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 20:31:26.000000 celldex-0.1.0/src/celldex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 20:31:26.000000 celldex-0.1.0/src/celldex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:31:26.112904 celldex-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-29 20:27:51.000000 celldex-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-29 20:27:51.000000 celldex-0.1.0/tests/test_fetch_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-29 20:27:51.000000 celldex-0.1.0/tests/test_list_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 20:27:51.000000 celldex-0.1.0/tests/test_save_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-29 20:27:51.000000 celldex-0.1.0/tests/test_search_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-29 20:27:51.000000 celldex-0.1.0/tox.ini
```

### Comparing `celldex-0.0.1/.coveragerc` & `celldex-0.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `celldex-0.0.1/.github/workflows/pypi-publish.yml` & `celldex-0.1.0/.github/workflows/pypi-publish.yml`

 * *Files 23% similar despite different names*

```diff
@@ -5,47 +5,76 @@
 
 on:
   push:
     tags: "*"
 
 jobs:
   build:
-
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python 3.9
-      uses: actions/setup-python@v2
-      with:
-        python-version: 3.9
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install flake8 pytest tox
-    # - name: Lint with flake8
-    #   run: |
-    #     # stop the build if there are Python syntax errors or undefined names
-    #     flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-    #     # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-    #     # flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-    - name: Test with tox
-      run: |
-        tox
-    - name: Build docs
-      run: |
-        tox -e docs
-    - run: touch ./docs/_build/html/.nojekyll
-    - name: GH Pages Deployment
-      uses: JamesIves/github-pages-deploy-action@4.1.3
-      with:
-        branch: gh-pages # The branch the action should deploy to.
-        folder: ./docs/_build/html
-        clean: true # Automatically remove deleted files from the deploy branch
-    - name: Build Project and Publish
-      run: |
-        python -m tox -e clean,build
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_PASSWORD }}
+      - uses: actions/checkout@v2
+
+      - name: Set up Python 3.9
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.9
+
+      # build SQLite from source, because I need 3.35<=
+      - name: Download SQLite3
+        run: |
+          wget https://www.sqlite.org/2024/sqlite-autoconf-3450300.tar.gz
+          tar -xvf sqlite-autoconf-3450300.tar.gz
+
+      - name: Install SQLite3
+        run: |
+          ./configure
+          make
+          sudo make install
+          export PATH="/usr/local/lib:$PATH"
+        working-directory: sqlite-autoconf-3450300
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install flake8 pytest tox
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+      # - name: Lint with flake8
+      #   run: |
+      #     # stop the build if there are Python syntax errors or undefined names
+      #     flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+      #     # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
+      #     # flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+
+      - name: Test with tox
+        run: |
+          tox
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+
+      - name: Build docs
+        run: |
+          tox -e docs
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+
+      - run: touch ./docs/_build/html/.nojekyll
+
+      - name: GH Pages Deployment
+        uses: JamesIves/github-pages-deploy-action@4.1.3
+        with:
+          branch: gh-pages # The branch the action should deploy to.
+          folder: ./docs/_build/html
+          clean: true # Automatically remove deleted files from the deploy branch
+
+      - name: Build Project and Publish
+        run: |
+          python -m tox -e clean,build
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+
+      - name: Publish package
+        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `celldex-0.0.1/.gitignore` & `celldex-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `celldex-0.0.1/.pre-commit-config.yaml` & `celldex-0.1.0/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 #   - id: blacken-docs
 #     additional_dependencies: [black]
 
 ## Check for misspells in documentation files:
 # - repo: https://github.com/codespell-project/codespell
 #   rev: v2.2.5
 #   hooks:
-#   - id: codespell
+#   - id: codespell
```

### Comparing `celldex-0.0.1/.readthedocs.yml` & `celldex-0.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `celldex-0.0.1/CONTRIBUTING.md` & `celldex-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `celldex-0.0.1/LICENSE.txt` & `celldex-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `celldex-0.0.1/docs/Makefile` & `celldex-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `celldex-0.0.1/docs/conf.py` & `celldex-0.1.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "sidebar_width": "300px",
     "page_width": "1200px"
@@ -245,14 +245,25 @@
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "celldex-doc"
 
+autodoc_default_options = {
+    # 'members': 'var1, var2',
+    # 'member-order': 'bysource',
+    "special-members": True,
+    "undoc-members": True,
+    "exclude-members": "__weakref__, __dict__, __str__, __module__",
+}
+
+autosummary_generate = True
+autosummary_imported_members = True
+
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ("letterpaper" or "a4paper").
     # "papersize": "letterpaper",
     # The font size ("10pt", "11pt" or "12pt").
@@ -295,10 +306,18 @@
     "matplotlib": ("https://matplotlib.org", None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "sklearn": ("https://scikit-learn.org/stable", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
+    "biocframe": ("https://biocpy.github.io/BiocFrame", None),
+    "genomicranges": ("https://biocpy.github.io/GenomicRanges", None),
+    "singlecellexperiment": ("https://biocpy.github.io/SingleCellExperiment", None),
+    "summarizedexperiment": ("https://biocpy.github.io/SummarizedExperiment", None),
+    "gypsum_client": ("https://artifactdb.github.io/gypsum-py", None),
+    "delayedarray": ("https://biocpy.github.io/DelayedArray", None),
+    "dolomite_base": ("https://artifactdb.github.io/dolomite-base", None),
+    "anndata": ("https://anndata.readthedocs.io/en/latest/", None),
 }
 
 print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `celldex-0.0.1/pyproject.toml` & `celldex-0.1.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 
 [tool.black]
-force-exclude = "__init__.py"
+force-exclude = "__init__.py"
```

### Comparing `celldex-0.0.1/setup.cfg` & `celldex-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
+	dolomite_base
+	dolomite_matrix
+	dolomite_sce>=0.1.2
+	gypsum_client>=0.1.3
+	delayedarray>=0.5.1
+	summarizedexperiment
+	singlecellexperiment
+	pandas
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `celldex-0.0.1/setup.py` & `celldex-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-"""
-    Setup file for celldex.
-    Use setup.cfg to configure your project.
+"""Setup file for celldex. Use setup.cfg to configure your project.
 
-    This file was generated with PyScaffold 4.5.
-    PyScaffold helps you to put up the scaffold of your new Python project.
-    Learn more under: https://pyscaffold.org/
+This file was generated with PyScaffold 4.5.
+PyScaffold helps you to put up the scaffold of your new Python project.
+Learn more under: https://pyscaffold.org/
 """
+
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(use_scm_version={"version_scheme": "no-guess-dev"})
     except:  # noqa
         print(
```

### Comparing `celldex-0.0.1/tox.ini` & `celldex-0.1.0/tox.ini`

 * *Files identical despite different names*

