# Comparing `tmp/sphinxawesome_theme-5.1.5.tar.gz` & `tmp/sphinxawesome_theme-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-5.1.5.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-5.1.6.tar", max compression
```

## Comparing `sphinxawesome_theme-5.1.5.tar` & `sphinxawesome_theme-5.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1066 2024-05-28 07:43:51.780524 sphinxawesome_theme-5.1.5/LICENSE
--rw-r--r--   0        0        0     2294 2024-05-28 07:43:51.780524 sphinxawesome_theme-5.1.5/README.md
--rw-r--r--   0        0        0     2770 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/pyproject.toml
--rw-r--r--   0        0        0     7311 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0     1194 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     4166 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/deprecated.py
--rw-r--r--   0        0        0     1394 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2841 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/genindex.html
--rw-r--r--   0        0        0     7675 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12745 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0     1013 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1192 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     5135 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     3242 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/logos.py
--rw-r--r--   0        0        0      895 2024-05-28 07:43:51.784524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     7816 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0     1603 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      656 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      932 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1226 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     2462 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      416 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar_main_nav_links.html
--rw-r--r--   0        0        0      256 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar_toc.html
--rw-r--r--   0        0        0    21956 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
--rw-r--r--   0        0        0    30184 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff
--rw-r--r--   0        0        0    21088 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
--rw-r--r--   0        0        0    28620 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
--rw-r--r--   0        0        0    23072 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
--rw-r--r--   0        0        0    23148 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
--rw-r--r--   0        0        0    30232 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
--rw-r--r--   0        0        0    29416 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
--rw-r--r--   0        0        0    28636 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
--rw-r--r--   0        0        0    22188 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
--rw-r--r--   0        0        0    21820 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
--rw-r--r--   0        0        0     4495 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-docsearch.css
--rw-r--r--   0        0        0        0 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-docsearch.js
--rw-r--r--   0        0        0     1338 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-sphinx-design.css
--rw-r--r--   0        0        0        0 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-sphinx-design.js
--rw-r--r--   0        0        0    27896 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
--rw-r--r--   0        0        0    49637 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.css
--rw-r--r--   0        0        0    56408 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.js
--rw-r--r--   0        0        0       93 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
--rw-r--r--   0        0        0      470 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0      353 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/toc.html
--rw-r--r--   0        0        0     2369 2024-05-28 07:43:51.788524 sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/toc.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-30 16:11:22.285508 sphinxawesome_theme-5.1.6/LICENSE
+-rw-r--r--   0        0        0     2294 2024-05-30 16:11:22.285508 sphinxawesome_theme-5.1.6/README.md
+-rw-r--r--   0        0        0     2770 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7311 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0     1194 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     4166 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/deprecated.py
+-rw-r--r--   0        0        0     1394 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     2841 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/genindex.html
+-rw-r--r--   0        0        0     7675 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    13010 2024-05-30 16:11:22.289507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0     1013 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1192 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     5135 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     3242 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/logos.py
+-rw-r--r--   0        0        0      895 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     7816 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0     1603 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      656 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      932 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1226 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     2462 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      416 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/sidebar_main_nav_links.html
+-rw-r--r--   0        0        0      256 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/sidebar_toc.html
+-rw-r--r--   0        0        0    21956 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
+-rw-r--r--   0        0        0    30184 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff
+-rw-r--r--   0        0        0    21088 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
+-rw-r--r--   0        0        0    28620 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
+-rw-r--r--   0        0        0    23072 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
+-rw-r--r--   0        0        0    23148 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
+-rw-r--r--   0        0        0    30232 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
+-rw-r--r--   0        0        0    29416 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
+-rw-r--r--   0        0        0    28636 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
+-rw-r--r--   0        0        0    22188 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
+-rw-r--r--   0        0        0    21820 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
+-rw-r--r--   0        0        0     4495 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/awesome-docsearch.css
+-rw-r--r--   0        0        0        0 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/awesome-docsearch.js
+-rw-r--r--   0        0        0     1338 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/awesome-sphinx-design.css
+-rw-r--r--   0        0        0        0 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/awesome-sphinx-design.js
+-rw-r--r--   0        0        0    27896 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
+-rw-r--r--   0        0        0    49637 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/theme.css
+-rw-r--r--   0        0        0    56408 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/theme.js
+-rw-r--r--   0        0        0       93 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
+-rw-r--r--   0        0        0      470 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0      353 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/toc.html
+-rw-r--r--   0        0        0     2369 2024-05-30 16:11:22.293507 sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/toc.py
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.6/PKG-INFO
```

### Comparing `sphinxawesome_theme-5.1.5/LICENSE` & `sphinxawesome_theme-5.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/README.md` & `sphinxawesome_theme-5.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/pyproject.toml` & `sphinxawesome_theme-5.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "5.1.5"
+version = "5.1.6"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
```

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/deprecated.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/deprecated.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/genindex.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/header.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/highlighting.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,33 +64,29 @@
 
 # type alias
 TokenType = Union[_TokenType, int]  # For Python 3.8
 TokenStream = Generator[Tuple[TokenType, str], None, None]
 
 
 def _replace_placeholders(
-    ttype: _TokenType, value: str, regex: Pattern[str]
+    ttype: TokenType, value: str, regex: Pattern[str]
 ) -> TokenStream:
     """Replace every occurence of ``regex`` with ``Generic.Emph`` token."""
     last = 0
     for match in regex.finditer(value):
         start, end = match.start(), match.end()
         if start != last:
             yield ttype, value[last:start]
         yield Generic.Emph, value[start:end]
         last = end
     if last != len(value):
         yield ttype, value[last:]
 
 
-# Without the comment, `mypy` throws a fit:
-# Cannot subclass Filter, is type `Any`
-
-
-class AwesomePlaceholders(Filter):  # type: ignore[misc]
+class AwesomePlaceholders(Filter):  # type: ignore
     """A Pygments filter for marking up placeholder text.
 
     You can define the text to highlight with the ``hl_text`` option.
     To add the filter to a Pygments lexer, use the ``add_filter`` method:
 
     .. code-block:: python
 
@@ -107,18 +103,15 @@
         self.placeholders_re = re.compile(
             r"|".join([re.escape(x) for x in placeholders if x])
         )
 
     def filter(
         self: AwesomePlaceholders, _lexer: Any, stream: TokenStream
     ) -> TokenStream:
-        """Filter on all tokens.
-
-        The ``lexer`` instance is required by the parent class, but isn't used here.
-        """
+        """Filter on all tokens."""
         regex = self.placeholders_re
         for ttype, value in stream:
             yield from _replace_placeholders(ttype, value, regex)
 
 
 class AwesomeHtmlFormatter(HtmlFormatter):  # type: ignore
     """Custom Pygments HTML formatter for highlighting added or removed lines.
@@ -206,22 +199,22 @@
             if self.full:
                 source = self._wrap_full(source, outfile)
 
         for _, piece in source:
             outfile.write(piece)
 
 
-class AwesomeCodeBlock(CodeBlock):
+class AwesomeCodeBlock(CodeBlock):  # type: ignore
     """An extension of the Sphinx ``code-block`` directive to handle additional options.
 
     - ``:emphasize-added:`` highlight added lines
     - ``:emphasize-removed:`` highlight removed lines
     - ``:emphasize-text:`` highlight placeholder text
 
-    The job of the directive is to set the correct options to the ``literal_block`` node,
+    The job of the directive is to set the correct options for the ``literal_block`` node,
     which represents a code block in the parsed reStructuredText tree.
     When transforming the abstract tree to HTML,
     Sphinx passes these options to the ``highlight_block`` method,
     which is a wrapper around Pygments' ``highlight`` method.
     Handling these options is then a job of the ``AwesomePygmentsBridge``.
     """
 
@@ -254,42 +247,56 @@
                     % (nlines, linespec),
                     location=location,
                 )
             return [i + 1 for i in line_numbers if i < nlines]
         except ValueError as err:
             return [document.reporter.warning(err, line=self.lineno)]
 
+    def _extra_args(
+        self: AwesomeCodeBlock,
+        node: Node,
+        hl_added: list[int] | None,
+        hl_removed: list[int] | None,
+    ) -> None:
+        """Set extra attributes for line highlighting."""
+        extra_args = node.get("highlight_args", {})  # type: ignore[attr-defined]
+
+        if hl_added is not None:
+            extra_args["hl_added"] = hl_added
+        if hl_removed is not None:
+            extra_args["hl_removed"] = hl_removed
+        if "emphasize-text" in self.options:
+            extra_args["hl_text"] = self.options["emphasize-text"]
+
     def run(self: AwesomeCodeBlock) -> list[Node]:
         """Handle parsing extra options for highlighting."""
-        literal_nodes = super().run()
+        literal_nodes: list[Node] = super().run()
 
         hl_added = self._get_line_numbers("emphasize-added")
         hl_removed = self._get_line_numbers("emphasize-removed")
 
-        # `literal_nodes` is either `[literal_block]`, or `[caption, literal_block]`
         for node in literal_nodes:
+            # Code blocks with caption [container > (caption + literal_block)]
+            if isinstance(node, nodes.container):
+                for nnode in node.children:
+                    if isinstance(nnode, nodes.literal_block):
+                        self._extra_args(nnode, hl_added, hl_removed)
+            # Code blocks without caption [literal_block]
             if isinstance(node, nodes.literal_block):
-                extra_args = node.get("highlight_args", {})
-
-                if hl_added is not None:
-                    extra_args["hl_added"] = hl_added
-                if hl_removed is not None:
-                    extra_args["hl_removed"] = hl_removed
-                if "emphasize-text" in self.options:
-                    extra_args["hl_text"] = self.options["emphasize-text"]
+                self._extra_args(node, hl_added, hl_removed)
 
         return literal_nodes
 
 
 # These external references are needed, or you'll get a maximum recursion depth error
 pygmentsbridge_get_lexer = PygmentsBridge.get_lexer
 pygmentsbridge_highlight_block = PygmentsBridge.highlight_block
 
 
-class AwesomePygmentsBridge(PygmentsBridge):
+class AwesomePygmentsBridge(PygmentsBridge):  # type: ignore
     """Monkey-patch the Pygments methods to handle highlighting placeholder text."""
 
     def get_lexer(
         self: AwesomePygmentsBridge,
         source: str,
         lang: str,
         opts: dict[str, Any] | None = None,
@@ -297,55 +304,52 @@
         location: Any = None,
     ) -> Lexer:
         """Monkey-patch the ``PygmentsBridge.get_lexer`` method.
 
         Adds a filter to lexers if the ``hl_text`` option is present.
         """
         lexer = pygmentsbridge_get_lexer(self, source, lang, opts, force, location)
+        hl_text = opts.get("hl_text") if opts else None
+
+        if hl_text:
+            lexer.add_filter(AwesomePlaceholders(hl_text=hl_text))
 
-        if opts and "hl_text" in opts:
-            lexer.add_filter(AwesomePlaceholders(hl_text=opts["hl_text"]))
         return lexer
 
     def highlight_block(
         self: AwesomePygmentsBridge,
         source: str,
         lang: str,
         opts: dict[str, Any] | None = None,
         force: bool = False,
         location: Any = None,
         **kwargs: Any,
     ) -> str:
         """Monkey-patch the ``PygmentsBridge.highlight_block`` method.
 
-        This method is called, when Sphinx transforms the abstract document tree
-        to HTML and encounters code blocks.
-        The ``hl_text`` option is passed in the ``kwargs`` dictionary.
-        For the ``get_lexer`` method, we need to pass it in the ``opts`` dictionary.
+        This method is called when Sphinx transforms the abstract document tree to HTML and encounters code blocks.
         """
         if opts is None:
             opts = {}
 
         hl_text = get_list_opt(kwargs, "hl_text", [])
 
         if hl_text:
             opts["hl_text"] = hl_text
 
-        return pygmentsbridge_highlight_block(
+        return pygmentsbridge_highlight_block(  # type: ignore
             self, source, lang, opts, force, location, **kwargs
         )
 
 
 def setup(app: Sphinx) -> dict[str, Any]:
     """Set up this internal extension."""
     PygmentsBridge.html_formatter = AwesomeHtmlFormatter
-    PygmentsBridge.get_lexer = AwesomePygmentsBridge.get_lexer  # type: ignore
-    PygmentsBridge.highlight_block = (  # type: ignore
-        AwesomePygmentsBridge.highlight_block  # type: ignore
-    )
+    PygmentsBridge.get_lexer = AwesomePygmentsBridge.get_lexer  # type: ignore[assignment]
+    PygmentsBridge.highlight_block = AwesomePygmentsBridge.highlight_block  # type: ignore[assignment]
     directives.register_directive("code-block", AwesomeCodeBlock)
 
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/jsonimpl.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/layout.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/logos.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/logos.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/page.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/page.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/scrolltop.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-docsearch.css` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/awesome-docsearch.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/awesome-sphinx-design.css` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/awesome-sphinx-design.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.css` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/theme.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/static/theme.js` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/static/theme.js`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/src/sphinxawesome_theme/toc.py` & `sphinxawesome_theme-5.1.6/src/sphinxawesome_theme/toc.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.5/PKG-INFO` & `sphinxawesome_theme-5.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 5.1.5
+Version: 5.1.6
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.5 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.6 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

