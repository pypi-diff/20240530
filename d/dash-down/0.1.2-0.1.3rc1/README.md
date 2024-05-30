# Comparing `tmp/dash_down-0.1.2.tar.gz` & `tmp/dash_down-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_down-0.1.2.tar", max compression
+gzip compressed data, was "dash_down-0.1.3rc1.tar", max compression
```

## Comparing `dash_down-0.1.2.tar` & `dash_down-0.1.3rc1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-08-24 09:56:39.642642 dash_down-0.1.2/LICENSE
--rw-r--r--   0        0        0     4862 2023-08-24 09:56:39.642642 dash_down-0.1.2/README.md
--rw-r--r--   0        0        0      360 2023-08-24 09:56:39.642642 dash_down-0.1.2/dash_down/__init__.py
--rw-r--r--   0        0        0     5479 2023-08-24 09:56:39.642642 dash_down-0.1.2/dash_down/directives.py
--rw-r--r--   0        0        0     3923 2023-08-24 09:56:39.642642 dash_down-0.1.2/dash_down/express.py
--rw-r--r--   0        0        0     3313 2023-08-24 09:56:39.642642 dash_down-0.1.2/dash_down/html_renderer.py
--rw-r--r--   0        0        0     1192 2023-08-24 09:56:39.642642 dash_down-0.1.2/dash_down/mantine_renderer.py
--rw-r--r--   0        0        0      851 2023-08-24 09:56:39.642642 dash_down-0.1.2/dash_down/plugins.py
--rw-r--r--   0        0        0      813 2023-08-24 09:56:39.646642 dash_down-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 dash_down-0.1.2/setup.py
--rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 dash_down-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-30 13:26:28.846035 dash_down-0.1.3rc1/LICENSE
+-rw-r--r--   0        0        0     4845 2024-05-30 13:26:28.846035 dash_down-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      360 2024-05-30 13:26:28.846035 dash_down-0.1.3rc1/dash_down/__init__.py
+-rw-r--r--   0        0        0     5479 2024-05-30 13:26:28.846035 dash_down-0.1.3rc1/dash_down/directives.py
+-rw-r--r--   0        0        0     4261 2024-05-30 13:28:12.576113 dash_down-0.1.3rc1/dash_down/express.py
+-rw-r--r--   0        0        0     3313 2024-05-30 13:26:28.846035 dash_down-0.1.3rc1/dash_down/html_renderer.py
+-rw-r--r--   0        0        0     1201 2024-05-30 13:29:59.856175 dash_down-0.1.3rc1/dash_down/mantine_renderer.py
+-rw-r--r--   0        0        0      851 2024-05-30 13:26:28.846035 dash_down-0.1.3rc1/dash_down/plugins.py
+-rw-r--r--   0        0        0      819 2024-05-30 13:31:14.256203 dash_down-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     5851 1970-01-01 00:00:00.000000 dash_down-0.1.3rc1/PKG-INFO
```

### Comparing `dash_down-0.1.2/LICENSE` & `dash_down-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_down-0.1.2/README.md` & `dash_down-0.1.3rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![Unit tests](https://github.com/emilhe/dash-down/actions/workflows/python-test.yml/badge.svg)](https://github.com/emilhe/dash-down/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/emilhe/dash-down/branch/main/graph/badge.svg?token=kZXx2N1QGY)](https://codecov.io/gh/emilhe/dash-down)
 
-The `dash-down` package provides tools to render markdown files into Plotly Dash component trees. Besides standard markdown syntax, a custom interpretation of the [directive syntax extension](https://mistune.readthedocs.io/en/latest/directives.html) makes it possible to embed Dash code blocks and/or applications (including callbacks). For a live demo, please take look at the [`dash-extensions` documentation](https://www.dash-extensions.com/getting-started/installation#a-example).
+The `dash-down` package provides tools to render markdown files into Plotly Dash component trees. Besides standard markdown syntax, a custom interpretation of the [directive syntax extension](https://mistune.readthedocs.io/en/latest/directives.html) makes it possible to embed Dash code blocks and/or applications (including callbacks). For a live demo, please take look at the [`dash-extensions` documentation](https://www.dash-extensions.com/sections/installation).
 
 ## Getting started
 
 Make sure that you have setup [poetry](https://python-poetry.org/). Then run
 
     poetry install
```

### Comparing `dash_down-0.1.2/dash_down/directives.py` & `dash_down-0.1.3rc1/dash_down/directives.py`

 * *Files identical despite different names*

### Comparing `dash_down-0.1.2/dash_down/express.py` & `dash_down-0.1.3rc1/dash_down/express.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from mistune import create_markdown
 from dash_down.directives import ApiDocDirective, DashProxyDirective, FunctionDirective
 from dash_down.html_renderer import DashHtmlRenderer
 from dash_down.mantine_renderer import DmcRenderer
 from dash_down.plugins import PluginBlueprint
 from dash_down import GITHUB_MARKDOWN_CSS, GITHUB_MARKDOWN_CSS_DARK, GITHUB_MARKDOWN_CSS_LIGHT
 
-_default_plugins_str = ['table', 'strikethrough']
+_default_plugins_str = ["table", "strikethrough"]
 
 
 def _default_plugins_class(shell, api_doc_shell, dash_proxy_shell):
     return [PluginBlueprint(shell=shell), ApiDocDirective(api_doc_shell), DashProxyDirective(shell=dash_proxy_shell)]
 
 
 def _default_plugins(shell, api_doc_shell, dash_proxy_shell):
@@ -37,48 +37,66 @@
             all_plugins.pop(match)
         except ValueError:
             pass
         all_plugins.append(plugin)
     return all_plugins
 
 
-def md_to_blueprint(renderer, md_path, plugins=None, directives=None, shell=None, api_doc_shell=None, dash_proxy_shell=None):
+def md_to_blueprint(
+    renderer,
+    md_path=None,
+    plugins=None,
+    directives=None,
+    shell=None,
+    api_doc_shell=None,
+    dash_proxy_shell=None,
+    md=None,
+):
     """
     Render a markdown file into a DashBlueprint using the provided renderer class
     :param renderer: renderer class, e.g. DashHtmlRenderer
     :param md_path: path to markdown file
     :param plugins: extra plugins to load
     :param shell: shell for the blueprint layout rendering
     :param api_doc_shell: shell for rendering of api doc directives
     :param dash_proxy_shell: shell for rendering of dash proxy directives
+    :param md: raw markdown string (alternative to file path)
     :return: DashBlueprint
     """
     plugins = _resolve_plugins(plugins, directives, shell, api_doc_shell, dash_proxy_shell)
     markdown = create_markdown(renderer=renderer(), plugins=plugins)
-    with open(md_path) as f:
-        blueprint = markdown.parse(f.read())
-    return blueprint
+    if md_path is not None:
+        with open(md_path) as f:
+            md = markdown.parse(f.read())
+    return markdown.parse(md)
 
 
-def md_to_blueprint_html(md_path: str, plugins=None, directives=None, shell=None, api_doc_shell=None, dash_proxy_shell=None) -> DashBlueprint:
+def md_to_blueprint_html(
+    md_path=None, plugins=None, directives=None, shell=None, api_doc_shell=None, dash_proxy_shell=None, md=None
+) -> DashBlueprint:
     """
     Render a markdown file into a DashBlueprint using html components.
     :param md_path: path to markdown file
     :param plugins: extra plugins to load
     :param shell: shell for the blueprint layout rendering
     :param api_doc_shell: shell for rendering of api doc directives
     :param dash_proxy_shell: shell for rendering of dash proxy directives
+    :param md: raw markdown string (alternative to file path)
+    :return: DashBlueprint
     """
-    return md_to_blueprint(DashHtmlRenderer, md_path, plugins, directives, shell, api_doc_shell, dash_proxy_shell)
+    return md_to_blueprint(DashHtmlRenderer, md_path, plugins, directives, shell, api_doc_shell, dash_proxy_shell, md)
 
 
-def md_to_blueprint_dmc(md_path: str, plugins=None, directives=None, shell=None, api_doc_shell=None, dash_proxy_shell=None) -> DashBlueprint:
+def md_to_blueprint_dmc(
+    md_path=None, plugins=None, directives=None, shell=None, api_doc_shell=None, dash_proxy_shell=None, md=None
+) -> DashBlueprint:
     """
     Render a markdown file into a DashBlueprint using dmc components.
     :param md_path: path to markdown file
     :param plugins: extra plugins to load
     :param shell: shell for the blueprint layout rendering
     :param api_doc_shell: shell for rendering of api doc directives
     :param dash_proxy_shell: shell for rendering of dash proxy directives
+    :param md: raw markdown string (alternative to file path)
     :return: DashBlueprint
     """
-    return md_to_blueprint(DmcRenderer, md_path, plugins, directives, shell, api_doc_shell, dash_proxy_shell)
+    return md_to_blueprint(DmcRenderer, md_path, plugins, directives, shell, api_doc_shell, dash_proxy_shell, md)
```

### Comparing `dash_down-0.1.2/dash_down/html_renderer.py` & `dash_down-0.1.3rc1/dash_down/html_renderer.py`

 * *Files identical despite different names*

### Comparing `dash_down-0.1.2/dash_down/mantine_renderer.py` & `dash_down-0.1.3rc1/dash_down/mantine_renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dash_mantine_components as dmc
+
 from dash_down.html_renderer import DashHtmlRenderer
 
 
 class DmcRenderer(DashHtmlRenderer):
     """
     Render markdown into Dash Mantine components.
     """
@@ -21,15 +22,15 @@
 
     def block_code(self, children, info=None):
         lang = None
         if info is not None:
             info = info.strip()
         if info:
             lang = info.split(None, 1)[0]
-        return dmc.Prism(children, language=lang)
+        return dmc.CodeHighlight(children, language=lang)
 
     def block_quote(self, text):
         return dmc.Blockquote(text)
 
     def list(self, children, ordered, level, start=None):
         return dmc.List(children, type="ordered" if ordered else "unordered")
```

### Comparing `dash_down-0.1.2/dash_down/plugins.py` & `dash_down-0.1.3rc1/dash_down/plugins.py`

 * *Files identical despite different names*

### Comparing `dash_down-0.1.2/pyproject.toml` & `dash_down-0.1.3rc1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "dash-down"
-version = "0.1.2"
+version = "0.1.3rc1"
 description = ""
 authors = ["emher <emil.h.eriksen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/emilhe/dash-down"
 repository = "https://github.com/emilhe/dash-down"
 documentation = "https://github.com/emilhe/dash-down"
 keywords = ["dash", "plotly", "markdown", "flask"]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-dash = ">=2.5.0"
+python = ">=3.8,<4.0"
+dash = ">=2.17.0"
 dash-extensions = ">=0.1.5"
-dash-mantine-components = ">=0.7.0"
+dash-mantine-components = ">=0.14.3"
 dash-iconify = "^0.1.2"
 mistune = "2.0.4"
 python-box = "^6.0.1"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.3.2"
 pytest = "^7.1.1"
-dash = {extras = ["dev", "testing"], version = ">=2.5.0"}
+dash = {extras = ["dev", "testing"], version = ">=2.17.0"}
 pytest-cov = "^3.0.0"
 pandas = ">=1.1.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dash_down-0.1.2/setup.py` & `dash_down-0.1.3rc1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,139 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dash-down
+Version: 0.1.3rc1
+Summary: 
+Home-page: https://github.com/emilhe/dash-down
+License: MIT
+Keywords: dash,plotly,markdown,flask
+Author: emher
+Author-email: emil.h.eriksen@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dash (>=2.17.0)
+Requires-Dist: dash-extensions (>=0.1.5)
+Requires-Dist: dash-iconify (>=0.1.2,<0.2.0)
+Requires-Dist: dash-mantine-components (>=0.14.3)
+Requires-Dist: mistune (==2.0.4)
+Requires-Dist: python-box (>=6.0.1,<7.0.0)
+Project-URL: Documentation, https://github.com/emilhe/dash-down
+Project-URL: Repository, https://github.com/emilhe/dash-down
+Description-Content-Type: text/markdown
 
-packages = \
-['dash_down']
+[![Unit tests](https://github.com/emilhe/dash-down/actions/workflows/python-test.yml/badge.svg)](https://github.com/emilhe/dash-down/actions/workflows/python-test.yml)
+[![codecov](https://codecov.io/gh/emilhe/dash-down/branch/main/graph/badge.svg?token=kZXx2N1QGY)](https://codecov.io/gh/emilhe/dash-down)
 
-package_data = \
-{'': ['*']}
+The `dash-down` package provides tools to render markdown files into Plotly Dash component trees. Besides standard markdown syntax, a custom interpretation of the [directive syntax extension](https://mistune.readthedocs.io/en/latest/directives.html) makes it possible to embed Dash code blocks and/or applications (including callbacks). For a live demo, please take look at the [`dash-extensions` documentation](https://www.dash-extensions.com/sections/installation).
 
-install_requires = \
-['dash-extensions>=0.1.5',
- 'dash-iconify>=0.1.2,<0.2.0',
- 'dash-mantine-components>=0.7.0',
- 'dash>=2.5.0',
- 'mistune==2.0.4',
- 'python-box>=6.0.1,<7.0.0']
-
-setup_kwargs = {
-    'name': 'dash-down',
-    'version': '0.1.2',
-    'description': '',
-    'long_description': '[![Unit tests](https://github.com/emilhe/dash-down/actions/workflows/python-test.yml/badge.svg)](https://github.com/emilhe/dash-down/actions/workflows/python-test.yml)\n[![codecov](https://codecov.io/gh/emilhe/dash-down/branch/main/graph/badge.svg?token=kZXx2N1QGY)](https://codecov.io/gh/emilhe/dash-down)\n\nThe `dash-down` package provides tools to render markdown files into Plotly Dash component trees. Besides standard markdown syntax, a custom interpretation of the [directive syntax extension](https://mistune.readthedocs.io/en/latest/directives.html) makes it possible to embed Dash code blocks and/or applications (including callbacks). For a live demo, please take look at the [`dash-extensions` documentation](https://www.dash-extensions.com/getting-started/installation#a-example).\n\n## Getting started\n\nMake sure that you have setup [poetry](https://python-poetry.org/). Then run\n\n    poetry install\n\nto install dependencies.\n\n#### Running the example\n\n    poetry run python example.py\n\n#### Running the tests\n\n    poetry run pytest\n\n## Custom content\n\nCustom content is rendered via the markdown [directive syntax extension](https://mistune.readthedocs.io/en/latest/directives.html). A directive has the following syntax,\n\n    .. directive-name:: directive value\n       :option-key: option value\n       :option-key: option value\n    \n       full featured markdown text here\n\nwhere the `directive-name` is mandatory, while the `value`, the `options` (specified as key value pairs), and the `text` are optional. \n\n#### What directives are bundled?\n\nCurrently, the bundled directives are\n\n* **api-doc** - a directive for rendering api documentation for a component\n* **dash-proxy** - a directive for rendering dash apps (including interactivity)\n\n#### How to create custom directives?\n\nThe easiest way to create a custom directive is to create a function with the following signature,\n\n```python\nfrom box import Box\nfrom dash_extensions.enrich import DashBlueprint\n\ndef directive_name(value: str, text: str, options: Box[str, str], blueprint: DashBlueprint):\n    """\n    :param value: the directive value (optional)\n    :param text: the markdown text (optional)\n    :param options: a Box object containing all key value pairs (optional)\n    :param blueprint: the DashBlueprint of the resulting Dash component tree, used e.g. for callback registration\n    :return: a Dash component\n    """\n    ...\n```\n\nSay, we want to make a new directive that yields a plot of the `iris` dataset. The code would then be along the lines of,\n\n```python\nimport plotly.express as px\nfrom box import Box\nfrom dash_extensions.enrich import dcc, DashBlueprint\n\ndef graph(value: str, text: str, options: Box[str, str], blueprint: DashBlueprint):\n    df = getattr(px.data, options.dataset)()\n    fig = px.scatter(df, x=options.x, y=options.y)\n    return dcc.Graph(figure=fig)\n```\n\nWith this directive defined, it is now possible to create a graph similar to [the one in the Dash docs](https://dash.plotly.com/dash-core-components/graph) with the following syntax,\n\n    .. graph::\n       :dataset: iris\n       :x: sepal_width\n       :y: sepal_length\n\nTo render a markdown file using the new, shiny directive, the syntax would be,\n\n```python\nfrom dash_extensions.enrich import DashProxy\nfrom dash_down.express import md_to_blueprint_dmc, GITHUB_MARKDOWN_CSS_LIGHT\n\n...\n\nblueprint = md_to_blueprint_dmc(\'path_to_your_md_file\', directives=[graph])\napp = DashProxy(blueprint=blueprint, external_stylesheets=[GITHUB_MARKDOWN_CSS_LIGHT])\n\nif __name__ == \'__main__\':\n    app.run_server()\n```\n\nA working example is bundled in the repo (see `example_custom_directive.py`).\n\n#### How to customize the layout of the rendered blueprint?\n\nThe layout of the blueprint returned by the renderer can be customized by passing a custom app shell via the `shell` keyword of the `md_to_blueprint_dmc` function. A working example is bundled in the repo (see `example_code_renderer.py`).\n\nPer default, the app shell is a `Div` element with `className="markdown-body"`. This class makes it possibly to use GitHub CSS for styling.\n\n#### How to customize the way code is rendered with the DashProxyDirective?\n\nThe layout of the Dash apps rendered via the `DashProxyDirective` can be customized via the `dash_proxy_shell` keyword of the `md_to_blueprint_dmc` function. A working example is bundled in the repo (see `example_code_renderer.py`).\n\nPer default, the app shell `Div` element with the code rendered as the first child and the resulting app rendered as the second.\n\n#### How to customize the markdown rendering itself?\n\nMake a subclass of `DashMantineRenderer` (or `DashHtmlRenderer`, if you prefer to start from raw HTML) and override the render function(s) for any element that you want to change. A good place to start would be to look at the `DashMantineRenderer` class itself for inspiration.\n',
-    'author': 'emher',
-    'author_email': 'emil.h.eriksen@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/emilhe/dash-down',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+## Getting started
 
+Make sure that you have setup [poetry](https://python-poetry.org/). Then run
+
+    poetry install
+
+to install dependencies.
+
+#### Running the example
+
+    poetry run python example.py
+
+#### Running the tests
+
+    poetry run pytest
+
+## Custom content
+
+Custom content is rendered via the markdown [directive syntax extension](https://mistune.readthedocs.io/en/latest/directives.html). A directive has the following syntax,
+
+    .. directive-name:: directive value
+       :option-key: option value
+       :option-key: option value
+    
+       full featured markdown text here
+
+where the `directive-name` is mandatory, while the `value`, the `options` (specified as key value pairs), and the `text` are optional. 
+
+#### What directives are bundled?
+
+Currently, the bundled directives are
+
+* **api-doc** - a directive for rendering api documentation for a component
+* **dash-proxy** - a directive for rendering dash apps (including interactivity)
+
+#### How to create custom directives?
+
+The easiest way to create a custom directive is to create a function with the following signature,
+
+```python
+from box import Box
+from dash_extensions.enrich import DashBlueprint
+
+def directive_name(value: str, text: str, options: Box[str, str], blueprint: DashBlueprint):
+    """
+    :param value: the directive value (optional)
+    :param text: the markdown text (optional)
+    :param options: a Box object containing all key value pairs (optional)
+    :param blueprint: the DashBlueprint of the resulting Dash component tree, used e.g. for callback registration
+    :return: a Dash component
+    """
+    ...
+```
+
+Say, we want to make a new directive that yields a plot of the `iris` dataset. The code would then be along the lines of,
+
+```python
+import plotly.express as px
+from box import Box
+from dash_extensions.enrich import dcc, DashBlueprint
+
+def graph(value: str, text: str, options: Box[str, str], blueprint: DashBlueprint):
+    df = getattr(px.data, options.dataset)()
+    fig = px.scatter(df, x=options.x, y=options.y)
+    return dcc.Graph(figure=fig)
+```
+
+With this directive defined, it is now possible to create a graph similar to [the one in the Dash docs](https://dash.plotly.com/dash-core-components/graph) with the following syntax,
+
+    .. graph::
+       :dataset: iris
+       :x: sepal_width
+       :y: sepal_length
+
+To render a markdown file using the new, shiny directive, the syntax would be,
+
+```python
+from dash_extensions.enrich import DashProxy
+from dash_down.express import md_to_blueprint_dmc, GITHUB_MARKDOWN_CSS_LIGHT
+
+...
+
+blueprint = md_to_blueprint_dmc('path_to_your_md_file', directives=[graph])
+app = DashProxy(blueprint=blueprint, external_stylesheets=[GITHUB_MARKDOWN_CSS_LIGHT])
+
+if __name__ == '__main__':
+    app.run_server()
+```
+
+A working example is bundled in the repo (see `example_custom_directive.py`).
+
+#### How to customize the layout of the rendered blueprint?
+
+The layout of the blueprint returned by the renderer can be customized by passing a custom app shell via the `shell` keyword of the `md_to_blueprint_dmc` function. A working example is bundled in the repo (see `example_code_renderer.py`).
+
+Per default, the app shell is a `Div` element with `className="markdown-body"`. This class makes it possibly to use GitHub CSS for styling.
+
+#### How to customize the way code is rendered with the DashProxyDirective?
+
+The layout of the Dash apps rendered via the `DashProxyDirective` can be customized via the `dash_proxy_shell` keyword of the `md_to_blueprint_dmc` function. A working example is bundled in the repo (see `example_code_renderer.py`).
+
+Per default, the app shell `Div` element with the code rendered as the first child and the resulting app rendered as the second.
+
+#### How to customize the markdown rendering itself?
+
+Make a subclass of `DashMantineRenderer` (or `DashHtmlRenderer`, if you prefer to start from raw HTML) and override the render function(s) for any element that you want to change. A good place to start would be to look at the `DashMantineRenderer` class itself for inspiration.
 
-setup(**setup_kwargs)
```

