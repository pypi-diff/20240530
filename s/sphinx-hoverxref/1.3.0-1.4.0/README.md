# Comparing `tmp/sphinx-hoverxref-1.3.0.tar.gz` & `tmp/sphinx_hoverxref-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-hoverxref-1.3.0.tar", last modified: Tue Oct 25 12:06:05 2022, max compression
+gzip compressed data, was "sphinx_hoverxref-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx-hoverxref-1.3.0.tar` & `sphinx_hoverxref-1.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     2359 2022-10-25 12:05:26.751551 sphinx-hoverxref-1.3.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1072 2019-06-02 14:00:27.460165 sphinx-hoverxref-1.3.0/LICENSE
--rw-r--r--   0        0        0     1556 2022-07-20 15:47:11.914364 sphinx-hoverxref-1.3.0/README.rst
--rw-r--r--   0        0        0      865 2020-04-16 18:46:59.115081 sphinx-hoverxref-1.3.0/docs/Makefile
--rw-r--r--   0        0        0      115 2020-04-10 13:06:28.670806 sphinx-hoverxref-1.3.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0     7576 2022-09-14 11:37:22.990275 sphinx-hoverxref-1.3.0/docs/conf.py
--rw-r--r--   0        0        0     6673 2022-10-24 16:30:53.967503 sphinx-hoverxref-1.3.0/docs/configuration.rst
--rw-r--r--   0        0        0   310173 2022-09-14 11:37:22.993608 sphinx-hoverxref-1.3.0/docs/crest-usage.gif
--rw-r--r--   0        0        0     4591 2022-06-23 16:26:15.745873 sphinx-hoverxref-1.3.0/docs/development.rst
--rw-r--r--   0        0        0   180935 2022-09-14 11:37:22.993608 sphinx-hoverxref-1.3.0/docs/disnake-usage.gif
--rw-r--r--   0        0        0      215 2021-09-27 12:18:58.052423 sphinx-hoverxref-1.3.0/docs/hoverxref.rst
--rw-r--r--   0        0        0   242658 2022-09-14 11:37:22.993608 sphinx-hoverxref-1.3.0/docs/hypothesis-usage.gif
--rw-r--r--   0        0        0     3333 2022-09-14 11:37:22.993608 sphinx-hoverxref-1.3.0/docs/index.rst
--rw-r--r--   0        0        0     1407 2022-06-01 11:28:54.114241 sphinx-hoverxref-1.3.0/docs/installation.rst
--rw-r--r--   0        0        0      258 2019-08-20 21:34:10.848065 sphinx-hoverxref-1.3.0/docs/mathjax.rst
--rw-r--r--   0        0        0   135780 2022-07-21 17:04:22.518043 sphinx-hoverxref-1.3.0/docs/poliastro-usage.gif
--rw-r--r--   0        0        0      162 2021-09-28 17:00:36.542182 sphinx-hoverxref-1.3.0/docs/refs.bib
--rw-r--r--   0        0        0      709 2022-06-01 11:42:04.763347 sphinx-hoverxref-1.3.0/docs/releasing.rst
--rw-r--r--   0        0        0     2843 2022-10-25 11:40:12.941243 sphinx-hoverxref-1.3.0/docs/requirements.txt
--rw-r--r--   0        0        0   218000 2022-09-14 11:37:22.996941 sphinx-hoverxref-1.3.0/docs/returns-usage.gif
--rw-r--r--   0        0        0   194090 2022-09-14 11:37:22.996941 sphinx-hoverxref-1.3.0/docs/scrapy-usage.gif
--rw-r--r--   0        0        0   217166 2022-09-14 11:37:22.996941 sphinx-hoverxref-1.3.0/docs/setuptools-usage.gif
--rw-r--r--   0        0        0    79717 2019-08-17 14:57:07.081432 sphinx-hoverxref-1.3.0/docs/sphinx-hoverxref-example.png
--rw-r--r--   0        0        0   125982 2022-09-14 11:37:22.996941 sphinx-hoverxref-1.3.0/docs/tweepy-usage.gif
--rw-r--r--   0        0        0     7314 2022-09-14 11:37:20.710291 sphinx-hoverxref-1.3.0/docs/usage.rst
--rw-r--r--   0        0        0     1346 2022-09-14 11:37:22.996941 sphinx-hoverxref-1.3.0/docs/who-is-using-it.rst
--rw-r--r--   0        0        0      109 2022-10-25 12:05:54.004659 sphinx-hoverxref-1.3.0/hoverxref/__init__.py
--rw-r--r--   0        0        0       38 2020-04-10 13:06:28.680806 sphinx-hoverxref-1.3.0/hoverxref/_static/css/alabaster.css
--rw-r--r--   0        0        0     2998 2020-04-10 13:06:28.680806 sphinx-hoverxref-1.3.0/hoverxref/_static/css/micromodal.css
--rw-r--r--   0        0        0       82 2020-04-10 13:06:28.680806 sphinx-hoverxref-1.3.0/hoverxref/_static/css/sphinx_material.css
--rw-r--r--   0        0        0      115 2020-04-10 13:06:28.680806 sphinx-hoverxref-1.3.0/hoverxref/_static/css/sphinx_rtd_theme.css
--rw-r--r--   0        0        0     1806 2020-04-06 19:13:00.239347 sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-borderless.min.css
--rw-r--r--   0        0        0     1782 2020-04-06 19:13:00.239347 sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-light.min.css
--rw-r--r--   0        0        0     1324 2020-04-06 19:13:00.239347 sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-noir.min.css
--rw-r--r--   0        0        0      825 2020-04-06 19:13:00.239347 sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-punk.min.css
--rw-r--r--   0        0        0     1684 2019-06-03 15:53:47.423280 sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-shadow.min.css
--rw-r--r--   0        0        0     6495 2018-01-29 21:02:23.000000 sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster.bundle.min.css
--rw-r--r--   0        0        0      552 2022-07-07 15:07:01.001626 sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster.custom.css_t
--rw-r--r--   0        0        0    11376 2022-10-24 16:30:53.967503 sphinx-hoverxref-1.3.0/hoverxref/_static/js/hoverxref.js_t
--rw-r--r--   0        0        0     6928 2020-04-10 13:06:28.680806 sphinx-hoverxref-1.3.0/hoverxref/_static/js/micromodal.min.js
--rw-r--r--   0        0        0    39900 2018-01-29 21:02:23.000000 sphinx-hoverxref-1.3.0/hoverxref/_static/js/tooltipster.bundle.min.js
--rw-r--r--   0        0        0     6574 2022-08-23 10:04:57.525244 sphinx-hoverxref-1.3.0/hoverxref/domains.py
--rw-r--r--   0        0        0    15744 2022-10-25 12:04:36.095304 sphinx-hoverxref-1.3.0/hoverxref/extension.py
--rw-r--r--   0        0        0     1954 2022-10-25 12:05:54.004659 sphinx-hoverxref-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 sphinx-hoverxref-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2727 2024-05-30 20:32:26.246672 sphinx_hoverxref-1.4.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1072 2024-05-30 20:25:24.992917 sphinx_hoverxref-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1556 2024-05-30 20:25:24.992917 sphinx_hoverxref-1.4.0/README.rst
+-rw-r--r--   0        0        0      724 2024-05-30 20:25:24.993917 sphinx_hoverxref-1.4.0/docs/Makefile
+-rw-r--r--   0        0        0      115 2024-05-30 20:25:24.994917 sphinx_hoverxref-1.4.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     7409 2024-05-30 20:25:24.994917 sphinx_hoverxref-1.4.0/docs/conf.py
+-rw-r--r--   0        0        0     6661 2024-05-30 20:25:24.995917 sphinx_hoverxref-1.4.0/docs/configuration.rst
+-rw-r--r--   0        0        0   310173 2024-05-30 20:25:25.000917 sphinx_hoverxref-1.4.0/docs/crest-usage.gif
+-rw-r--r--   0        0        0     3915 2024-05-30 20:25:25.001917 sphinx_hoverxref-1.4.0/docs/development.rst
+-rw-r--r--   0        0        0   180935 2024-05-30 20:25:25.004917 sphinx_hoverxref-1.4.0/docs/disnake-usage.gif
+-rw-r--r--   0        0        0      215 2024-05-30 20:25:25.004917 sphinx_hoverxref-1.4.0/docs/hoverxref.rst
+-rw-r--r--   0        0        0   242658 2024-05-30 20:25:25.008917 sphinx_hoverxref-1.4.0/docs/hypothesis-usage.gif
+-rw-r--r--   0        0        0     3333 2024-05-30 20:25:25.008917 sphinx_hoverxref-1.4.0/docs/index.rst
+-rw-r--r--   0        0        0     1407 2024-05-30 20:25:25.009917 sphinx_hoverxref-1.4.0/docs/installation.rst
+-rw-r--r--   0        0        0      258 2024-05-30 20:25:25.009917 sphinx_hoverxref-1.4.0/docs/mathjax.rst
+-rw-r--r--   0        0        0   135780 2024-05-30 20:25:25.011917 sphinx_hoverxref-1.4.0/docs/poliastro-usage.gif
+-rw-r--r--   0        0        0      162 2024-05-30 20:25:25.012917 sphinx_hoverxref-1.4.0/docs/refs.bib
+-rw-r--r--   0        0        0      709 2024-05-30 20:25:25.012917 sphinx_hoverxref-1.4.0/docs/releasing.rst
+-rw-r--r--   0        0        0     2974 2024-05-30 20:25:25.012917 sphinx_hoverxref-1.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0   218000 2024-05-30 20:25:25.016917 sphinx_hoverxref-1.4.0/docs/returns-usage.gif
+-rw-r--r--   0        0        0   194090 2024-05-30 20:25:25.019917 sphinx_hoverxref-1.4.0/docs/scrapy-usage.gif
+-rw-r--r--   0        0        0   217166 2024-05-30 20:25:25.023917 sphinx_hoverxref-1.4.0/docs/setuptools-usage.gif
+-rw-r--r--   0        0        0    79717 2024-05-30 20:25:25.024917 sphinx_hoverxref-1.4.0/docs/sphinx-hoverxref-example.png
+-rw-r--r--   0        0        0   125982 2024-05-30 20:25:25.026917 sphinx_hoverxref-1.4.0/docs/tweepy-usage.gif
+-rw-r--r--   0        0        0     7314 2024-05-30 20:25:25.027917 sphinx_hoverxref-1.4.0/docs/usage.rst
+-rw-r--r--   0        0        0     1346 2024-05-30 20:25:25.027917 sphinx_hoverxref-1.4.0/docs/who-is-using-it.rst
+-rw-r--r--   0        0        0      109 2024-05-30 20:34:14.362380 sphinx_hoverxref-1.4.0/hoverxref/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-30 20:25:25.028917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/alabaster.css
+-rw-r--r--   0        0        0     2998 2024-05-30 20:25:25.028917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/micromodal.css
+-rw-r--r--   0        0        0       82 2024-05-30 20:25:25.028917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/sphinx_material.css
+-rw-r--r--   0        0        0      115 2024-05-30 20:25:25.028917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/sphinx_rtd_theme.css
+-rw-r--r--   0        0        0     1806 2024-05-30 20:25:25.029917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-borderless.min.css
+-rw-r--r--   0        0        0     1782 2024-05-30 20:25:25.029917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-light.min.css
+-rw-r--r--   0        0        0     1324 2024-05-30 20:25:25.029917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-noir.min.css
+-rw-r--r--   0        0        0      825 2024-05-30 20:25:25.029917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-punk.min.css
+-rw-r--r--   0        0        0     1684 2024-05-30 20:25:25.030917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-shadow.min.css
+-rw-r--r--   0        0        0     6495 2024-05-30 20:25:25.030917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster.bundle.min.css
+-rw-r--r--   0        0        0      552 2024-05-30 20:25:25.030917 sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster.custom.css_t
+-rw-r--r--   0        0        0    11376 2024-05-30 20:25:25.031917 sphinx_hoverxref-1.4.0/hoverxref/_static/js/hoverxref.js_t
+-rw-r--r--   0        0        0     6928 2024-05-30 20:25:25.031917 sphinx_hoverxref-1.4.0/hoverxref/_static/js/micromodal.min.js
+-rw-r--r--   0        0        0    39900 2024-05-30 20:25:25.032917 sphinx_hoverxref-1.4.0/hoverxref/_static/js/tooltipster.bundle.min.js
+-rw-r--r--   0        0        0     6574 2024-05-30 20:25:25.032917 sphinx_hoverxref-1.4.0/hoverxref/domains.py
+-rw-r--r--   0        0        0    15209 2024-05-30 20:25:25.032917 sphinx_hoverxref-1.4.0/hoverxref/extension.py
+-rw-r--r--   0        0        0     2078 2024-05-30 20:34:14.360380 sphinx_hoverxref-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 sphinx_hoverxref-1.4.0/PKG-INFO
```

### Comparing `sphinx-hoverxref-1.3.0/CHANGELOG.rst` & `sphinx_hoverxref-1.4.0/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 Changelog
 =========
 
 This page shows all the changes done on each version.
 
+Version 1.4.0
+-------------
+
+* Require ``sphinxcontrib-bibtex>=2.6.0`` (https://github.com/readthedocs/sphinx-hoverxref/pull/281) 
+* Sphinx 5 is the minimum supported version (https://github.com/readthedocs/sphinx-hoverxref/pull/282)
+* Default ``hoverxref_api_host`` to ``/_`` to make use of our proxied API (https://github.com/readthedocs/sphinx-hoverxref/pull/134)
+
 Version 1.3.0
 -------------
 
 * Handle explicit intersphinx inventory names in all domains --not just ``std`` (https://github.com/readthedocs/sphinx-hoverxref/pull/236)
 
 Version 1.2.0
 -------------
```

### Comparing `sphinx-hoverxref-1.3.0/LICENSE` & `sphinx_hoverxref-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/README.rst` & `sphinx_hoverxref-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/Makefile` & `sphinx_hoverxref-1.4.0/docs/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 SOURCEDIR     = .
 BUILDDIR      = _build
 
-# sphinx-hoverxref expected variables
-export READTHEDOCS=True
-export READTHEDOCS_PROJECT=sphinx-hoverxref
-export READTHEDOCS_VERSION=latest
-
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
```

### Comparing `sphinx-hoverxref-1.3.0/docs/conf.py` & `sphinx_hoverxref-1.4.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
 # -- Path setup --------------------------------------------------------------
@@ -71,20 +69,16 @@
     'python',
 ]
 hoverxref_intersphinx_types = {
     'readthedocs': 'modal',
     'sphinx': 'tooltip',
 }
 
-# Used when building the documentation from the terminal and using a local Read
-# the Docs instance as backend
-hoverxref_api_host = 'http://localhost:8000'
-
-if os.environ.get('READTHEDOCS') == 'True':
-    # Building on Read the Docs
+# Used when building the documentation locally.
+if os.environ.get('READTHEDOCS') != 'True':
     hoverxref_api_host = 'https://readthedocs.org'
 
     if os.environ.get('PROXIED_API_ENDPOINT') == 'True':
         # Use the proxied API endpoint
         hoverxref_api_host = '/_'
 
 if os.environ.get('LOCAL_READTHEDOCS') == 'True':
@@ -135,15 +129,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `sphinx-hoverxref-1.3.0/docs/configuration.rst` & `sphinx_hoverxref-1.4.0/docs/configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -147,22 +147,22 @@
    Type: bool
 
 .. _Mathjax: http://www.sphinx-doc.org/es/master/usage/extensions/math.html#module-sphinx.ext.mathjax
 
 
 .. confval:: hoverxref_api_host
 
-   Description: Host URL for the API to retrieve the content of the floating window
+   Description: Host or root URL for the API to retrieve the content of the floating window
 
    .. warning::
 
      You shouldn't modify this setting unless you know what you are doing.
      Its default should be fine to build the documentation and make it work in Read the Docs.
 
-   Default: ``https://readthedocs.org``
+   Default: ``/_``
 
    Type: string
 
 
 Tooltipster
 -----------
 
@@ -174,14 +174,15 @@
 
    Default: ``rst-content``
 
    Type: string
 
 
 .. confval:: hoverxref_tooltip_lazy
+
    Description: Whether to lazily generate tooltips (insert the HTML for the tooltip on hover, rather than on page load).
    This is known to be slower, but prevents the browser from stalling on load for very big doc pages.
    We recommend you keeping it as `False` unless you are experiencing page load issues.
 
    Default ``False``
 
    Type: bool
```

### Comparing `sphinx-hoverxref-1.3.0/docs/crest-usage.gif` & `sphinx_hoverxref-1.4.0/docs/crest-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/development.rst` & `sphinx_hoverxref-1.4.0/docs/development.rst`

 * *Files 15% similar despite different names*

```diff
@@ -50,32 +50,14 @@
 
 .. prompt:: bash
 
    python -m http.server --directory _build/html 9000
 
 Now, you can hit http://localhost:9000/ and you should see your documentation here.
 
-
-Avoid CORS on local backend
-+++++++++++++++++++++++++++
-
-When building the documentation locally,
-the API calls will be blocked by the browser because of :abbr:`CORS (Cross Origin Resource Sharing)`
-(you are hitting the URL http://localhost:9000/ and the API calls are to https://readthedocs.org/).
-
-You can disable this while developing our extension.
-To do this, you can open Google Chrome with these arguments:
-
-.. prompt:: bash
-
-   google-chrome-stable --disable-web-security --user-data-dir='/tmp/testing'
-
-If Firefox, you can install this add-ons: `Allow CORS: Access-Control-Allow-Origin <https://addons.mozilla.org/es/firefox/addon/access-control-allow-origin/>`_.
-
-
 Using a local Read the Docs instance
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You can `install Read the Docs locally following these instructions`_.
 Although, it may be too complicated just to retrieve the same content that you could have in https://readthedocs.org.
 
 To make the extension to work, you will need to define this setting in your ``conf.py`` file:
```

### Comparing `sphinx-hoverxref-1.3.0/docs/disnake-usage.gif` & `sphinx_hoverxref-1.4.0/docs/disnake-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/hypothesis-usage.gif` & `sphinx_hoverxref-1.4.0/docs/hypothesis-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/index.rst` & `sphinx_hoverxref-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/installation.rst` & `sphinx_hoverxref-1.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/poliastro-usage.gif` & `sphinx_hoverxref-1.4.0/docs/poliastro-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/releasing.rst` & `sphinx_hoverxref-1.4.0/docs/releasing.rst`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/requirements.txt` & `sphinx_hoverxref-1.4.0/docs/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,126 +1,135 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --extra=doc --output-file=docs/requirements.txt pyproject.toml
 #
-alabaster==0.7.12
+alabaster==0.7.16
     # via sphinx
-astroid==2.12.12
+anyascii==0.3.2
     # via sphinx-autoapi
-babel==2.10.3
+anyio==4.3.0
+    # via starlette
+astroid==3.1.0
+    # via sphinx-autoapi
+babel==2.14.0
     # via sphinx
-certifi==2022.9.24
+certifi==2024.2.2
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.3.2
     # via requests
-colorama==0.4.5
+click==8.1.7
+    # via uvicorn
+colorama==0.4.6
     # via sphinx-autobuild
-docutils==0.17.1
+docutils==0.20.1
     # via
     #   pybtex-docutils
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-rtd-theme
     #   sphinx-tabs
     #   sphinxcontrib-bibtex
-idna==3.4
-    # via requests
+exceptiongroup==1.2.0
+    # via anyio
+h11==0.14.0
+    # via uvicorn
+idna==3.7
+    # via
+    #   anyio
+    #   requests
 imagesize==1.4.1
     # via sphinx
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   sphinx
     #   sphinx-autoapi
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-lazy-object-proxy==1.7.1
-    # via astroid
-livereload==2.6.3
-    # via sphinx-autobuild
-markupsafe==2.1.1
+markupsafe==2.1.5
     # via jinja2
-packaging==21.3
+packaging==24.0
     # via sphinx
 pybtex==0.24.0
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
-pybtex-docutils==1.0.2
+pybtex-docutils==1.0.3
     # via sphinxcontrib-bibtex
-pygments==2.13.0
+pygments==2.17.2
     # via
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.0.9
-    # via packaging
-pytz==2022.5
-    # via babel
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   pybtex
     #   sphinx-autoapi
-requests==2.28.1
+requests==2.31.0
     # via sphinx
 six==1.16.0
-    # via
-    #   latexcodec
-    #   livereload
-    #   pybtex
+    # via pybtex
+sniffio==1.3.1
+    # via anyio
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==4.5.0
+sphinx==7.2.6
     # via
     #   sphinx-autoapi
     #   sphinx-autobuild
     #   sphinx-hoverxref (pyproject.toml)
     #   sphinx-notfound-page
     #   sphinx-prompt
     #   sphinx-rtd-theme
     #   sphinx-tabs
     #   sphinx-version-warning
     #   sphinxcontrib-bibtex
+    #   sphinxcontrib-jquery
     #   sphinxemoji
-sphinx-autoapi==2.0.0
+sphinx-autoapi==3.0.0
     # via sphinx-hoverxref (pyproject.toml)
-sphinx-autobuild==2021.3.14
+sphinx-autobuild==2024.4.13
     # via sphinx-hoverxref (pyproject.toml)
-sphinx-notfound-page==0.8.3
+sphinx-notfound-page==1.0.0
     # via sphinx-hoverxref (pyproject.toml)
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-hoverxref (pyproject.toml)
-sphinx-rtd-theme==1.0.0
+sphinx-rtd-theme==2.0.0
     # via sphinx-hoverxref (pyproject.toml)
-sphinx-tabs==3.3.1
+sphinx-tabs==3.4.5
     # via sphinx-hoverxref (pyproject.toml)
 sphinx-version-warning==1.1.2
     # via sphinx-hoverxref (pyproject.toml)
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-bibtex==2.5.0
+sphinxcontrib-bibtex==2.6.2
     # via sphinx-hoverxref (pyproject.toml)
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
-sphinxcontrib-jquery==2.0.0
-    # via sphinx-hoverxref (pyproject.toml)
+sphinxcontrib-jquery==4.1
+    # via
+    #   sphinx-hoverxref (pyproject.toml)
+    #   sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sphinxemoji==0.2.0
+sphinxemoji==0.3.1
     # via sphinx-hoverxref (pyproject.toml)
-tornado==6.2
-    # via livereload
-unidecode==1.3.6
-    # via sphinx-autoapi
-urllib3==1.26.12
+starlette==0.37.2
+    # via sphinx-autobuild
+typing-extensions==4.11.0
+    # via
+    #   anyio
+    #   astroid
+    #   uvicorn
+urllib3==2.2.1
     # via requests
-wrapt==1.14.1
-    # via astroid
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+uvicorn==0.29.0
+    # via sphinx-autobuild
+websockets==12.0
+    # via sphinx-autobuild
```

### Comparing `sphinx-hoverxref-1.3.0/docs/returns-usage.gif` & `sphinx_hoverxref-1.4.0/docs/returns-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/scrapy-usage.gif` & `sphinx_hoverxref-1.4.0/docs/scrapy-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/setuptools-usage.gif` & `sphinx_hoverxref-1.4.0/docs/setuptools-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/sphinx-hoverxref-example.png` & `sphinx_hoverxref-1.4.0/docs/sphinx-hoverxref-example.png`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/tweepy-usage.gif` & `sphinx_hoverxref-1.4.0/docs/tweepy-usage.gif`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/usage.rst` & `sphinx_hoverxref-1.4.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/docs/who-is-using-it.rst` & `sphinx_hoverxref-1.4.0/docs/who-is-using-it.rst`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/micromodal.css` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/micromodal.css`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-borderless.min.css` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-borderless.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-light.min.css` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-light.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-noir.min.css` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-noir.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-punk.min.css` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-punk.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster-sideTip-shadow.min.css` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster-sideTip-shadow.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster.bundle.min.css` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster.bundle.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/css/tooltipster.custom.css_t` & `sphinx_hoverxref-1.4.0/hoverxref/_static/css/tooltipster.custom.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/js/hoverxref.js_t` & `sphinx_hoverxref-1.4.0/hoverxref/_static/js/hoverxref.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/js/micromodal.min.js` & `sphinx_hoverxref-1.4.0/hoverxref/_static/js/micromodal.min.js`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/_static/js/tooltipster.bundle.min.js` & `sphinx_hoverxref-1.4.0/hoverxref/_static/js/tooltipster.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/domains.py` & `sphinx_hoverxref-1.4.0/hoverxref/domains.py`

 * *Files identical despite different names*

### Comparing `sphinx-hoverxref-1.3.0/hoverxref/extension.py` & `sphinx_hoverxref-1.4.0/hoverxref/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,25 +147,18 @@
 def setup_sphinx_tabs(app, config):
     """
     Disconnect ``update_context`` function from ``sphinx-tabs``.
 
     Sphinx Tabs removes the CSS/JS from pages that does not use the directive.
     Although, we need them to use inside the tooltip.
     """
-    if sphinx.version_info < (3, 0, 0):
-        listeners = list(app.events.listeners.get('html-page-context').items())
-    else:
-        listeners = [
-            (listener.id, listener.handler)
-            for listener in app.events.listeners.get('html-page-context')
-        ]
-    for listener_id, function in listeners:
-        module_name = inspect.getmodule(function).__name__
+    for listener in app.events.listeners.get('html-page-context'):
+        module_name = inspect.getmodule(listener.handler).__name__
         if module_name == 'sphinx_tabs.tabs':
-            app.disconnect(listener_id)
+            app.disconnect(listener.id)
 
 
 def setup_intersphinx(app, config):
     """
     Disconnect ``missing-reference`` from ``sphinx.ext.intershinx``.
 
     As there is no way to hook into the ``missing_referece`` function to add
@@ -175,25 +168,18 @@
     https://github.com/sphinx-doc/sphinx/blob/53c1dff/sphinx/ext/intersphinx.py
     """
     if not app.config.hoverxref_intersphinx:
         # Do not disconnect original intersphinx missing-reference if the user
         # does not have hoverxref intersphinx enabled
         return
 
-    if sphinx.version_info < (3, 0, 0):
-        listeners = list(app.events.listeners.get('missing-reference').items())
-    else:
-        listeners = [
-            (listener.id, listener.handler)
-            for listener in app.events.listeners.get('missing-reference')
-        ]
-    for listener_id, function in listeners:
-        module_name = inspect.getmodule(function).__name__
+    for listener in app.events.listeners.get('missing-reference'):
+        module_name = inspect.getmodule(listener.handler).__name__
         if module_name == 'sphinx.ext.intersphinx':
-            app.disconnect(listener_id)
+            app.disconnect(listener.id)
 
 
 def missing_reference(app, env, node, contnode):
     """
     Override original ``missing_referece`` to add data into the node.
 
     We call the original intersphinx extension and add hoverxref CSS classes
@@ -331,34 +317,34 @@
         app.config.hoverxref_api_host = app.config.hoverxref_tooltip_api_host
 
 
 
 def setup(app):
     """Setup ``hoverxref`` Sphinx extension."""
 
-    # ``override`` was introduced in 1.8
-    app.require_sphinx('1.8')
+    # Matches requirement from pyproject.toml
+    app.require_sphinx('5.0')
 
     app.add_config_value('hoverxref_auto_ref', False, 'env')
     app.add_config_value('hoverxref_mathjax', False, 'env')
     app.add_config_value('hoverxref_sphinxtabs', False, 'env')
     app.add_config_value('hoverxref_roles', [], 'env')
     app.add_config_value('hoverxref_domains', [], 'env')
     app.add_config_value('hoverxref_ignore_refs', ['genindex', 'modindex', 'search'], 'env')
     app.add_config_value('hoverxref_role_types', {}, 'env')
     app.add_config_value('hoverxref_default_type', 'tooltip', 'env')
     app.add_config_value('hoverxref_intersphinx', [], 'env')
     app.add_config_value('hoverxref_intersphinx_types', {}, 'env')
-    app.add_config_value('hoverxref_api_host', 'https://readthedocs.org', 'env')
+    app.add_config_value('hoverxref_api_host', '/_', 'env')
     app.add_config_value('hoverxref_sphinx_version', sphinx.__version__, 'env')
     app.add_config_value('hoverxref_tooltip_lazy', False, 'env')
 
     # Tooltipster settings
     # Deprecated in favor of ``hoverxref_api_host``
-    app.add_config_value('hoverxref_tooltip_api_host', 'https://readthedocs.org', 'env')
+    app.add_config_value('hoverxref_tooltip_api_host', '/_', 'env')
     app.add_config_value('hoverxref_tooltip_theme', ['tooltipster-shadow', 'tooltipster-shadow-custom'], 'env')
     app.add_config_value('hoverxref_tooltip_interactive', True, 'env')
     app.add_config_value('hoverxref_tooltip_maxwidth', 450, 'env')
     app.add_config_value('hoverxref_tooltip_side', 'right', 'env')
     app.add_config_value('hoverxref_tooltip_animation', 'fade', 'env')
     app.add_config_value('hoverxref_tooltip_animation_duration', 0, 'env')
     app.add_config_value('hoverxref_tooltip_content', 'Loading...', 'env')
```

### Comparing `sphinx-hoverxref-1.3.0/pyproject.toml` & `sphinx_hoverxref-1.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     "modal",
     "hover",
     "hoverxref",
     "sphinx",
     "documentation",
 ]
 dependencies = [
-    "sphinx >=1.8",
+    "sphinx >=5.0",
     "sphinxcontrib-jquery",
 ]
-version = "1.3.0"
+version = "1.4.0"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Sphinx",
     "Framework :: Sphinx :: Extension",
     "License :: OSI Approved :: MIT License",
@@ -40,20 +40,23 @@
     "tox",
 ]
 
 doc = [
     "sphinx",
     "sphinx-autoapi",
     "sphinx-rtd-theme",
-    "sphinx-tabs==3.3.1",
+    "sphinx-tabs",
     "sphinx-prompt",
     "sphinx-version-warning",
     "sphinx-notfound-page",
     "sphinx-autobuild",
-    "sphinxcontrib-bibtex",
+    # versions older than this don't pin
+    # docutils which is necessary for
+    # bibtex html rendering to work properly
+    "sphinxcontrib-bibtex>=2.6.0",
     "sphinxemoji",
 ]
 
 [project.urls]
 Documentation = "https://sphinx-hoverxref.readthedocs.io/"
 Source = "https://github.com/readthedocs/sphinx-hoverxref"
 Tracker = "https://github.com/readthedocs/sphinx-hoverxref/issues"
@@ -71,15 +74,15 @@
   ".readthedocs.yml",
   "pytest.ini",
   "conftest.py",
   "tox.ini",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0"
+current_version = "1.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Release {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `sphinx-hoverxref-1.3.0/PKG-INFO` & `sphinx_hoverxref-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: sphinx-hoverxref
-Version: 1.3.0
+Version: 1.4.0
 Summary: Sphinx extension to show tooltips with content embedded when hover a reference.
 Keywords: tooltip,modal,hover,hoverxref,sphinx,documentation
 Author-email: Manuel Kaufmann <humitos@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Requires-Dist: sphinx >=1.8
+Requires-Dist: sphinx >=5.0
 Requires-Dist: sphinxcontrib-jquery
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx-autoapi ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme ; extra == "doc"
-Requires-Dist: sphinx-tabs==3.3.1 ; extra == "doc"
+Requires-Dist: sphinx-tabs ; extra == "doc"
 Requires-Dist: sphinx-prompt ; extra == "doc"
 Requires-Dist: sphinx-version-warning ; extra == "doc"
 Requires-Dist: sphinx-notfound-page ; extra == "doc"
 Requires-Dist: sphinx-autobuild ; extra == "doc"
-Requires-Dist: sphinxcontrib-bibtex ; extra == "doc"
+Requires-Dist: sphinxcontrib-bibtex>=2.6.0 ; extra == "doc"
 Requires-Dist: sphinxemoji ; extra == "doc"
 Requires-Dist: tox ; extra == "test"
 Project-URL: Documentation, https://sphinx-hoverxref.readthedocs.io/
 Project-URL: Source, https://github.com/readthedocs/sphinx-hoverxref
 Project-URL: Tracker, https://github.com/readthedocs/sphinx-hoverxref/issues
 Provides-Extra: doc
 Provides-Extra: test
```

