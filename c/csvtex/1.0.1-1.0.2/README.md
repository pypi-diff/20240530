# Comparing `tmp/csvtex-1.0.1.tar.gz` & `tmp/csvtex-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvtex-1.0.1.tar", max compression
+gzip compressed data, was "csvtex-1.0.2.tar", max compression
```

## Comparing `csvtex-1.0.1.tar` & `csvtex-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2024-05-29 08:02:31.141592 csvtex-1.0.1/LICENSE
--rw-r--r--   0        0        0     2304 2024-05-29 08:43:42.284273 csvtex-1.0.1/README.md
--rw-r--r--   0        0        0      196 2024-05-29 08:32:45.254861 csvtex-1.0.1/csvtex/__init__.py
--rw-r--r--   0        0        0     4161 2024-05-29 08:34:53.123889 csvtex-1.0.1/csvtex/main.py
--rw-r--r--   0        0        0      391 2024-05-29 09:10:31.704151 csvtex-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 csvtex-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-29 08:02:31.141592 csvtex-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2304 2024-05-29 08:43:42.284273 csvtex-1.0.2/README.md
+-rw-r--r--   0        0        0      196 2024-05-29 08:32:45.254861 csvtex-1.0.2/csvtex/__init__.py
+-rw-r--r--   0        0        0     4235 2024-05-29 22:40:28.398672 csvtex-1.0.2/csvtex/main.py
+-rw-r--r--   0        0        0      391 2024-05-29 22:40:48.202840 csvtex-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 csvtex-1.0.2/PKG-INFO
```

### Comparing `csvtex-1.0.1/LICENSE` & `csvtex-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csvtex-1.0.1/README.md` & `csvtex-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `csvtex-1.0.1/csvtex/main.py` & `csvtex-1.0.2/csvtex/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import pandas as pd
 
 PREAMBLE = r"""\documentclass[11pt, a4paper]{article}
 \usepackage{booktabs}
+\usepackage{graphicx}
 \begin{document}"""
 
-HEADER = r"""\begin{{table}}[htb]
-{indent}\centering{caption}{label}
+HEADER = r"""\begin{{table*}}[htb]
+{indent}\centering
 {indent}\begin{{tabular}}{{@{{}}{align}@{{}}}}
 {indent}{indent}\toprule"""
 
 FOOTER = r"""{indent}{indent}\bottomrule
 {indent}\end{{tabular}}
-\end{{table}}"""
+{indent}}}
+{caption}
+{label}
+\end{{table*}}"""
 
 LABEL = "\n{indent}\\label{{{label}}}"
-CAPTION = "\n{indent}\\caption{{{caption}}}"
+CAPTION = "\n{indent}\\caption{{\\footnotesize {caption}}}"
 
 
 def create_latex_table(
     file,
     sep=",",
     caption="",
     label="",
@@ -87,20 +91,22 @@
         rows.insert(0, header_row)
         rows.insert(1, indent + indent + r"\midrule")
 
     content = "\n".join(indent + indent + row for row in rows)
 
     if not fragment:
         table_header = HEADER.format(
-            label=add_label(label, indent),
-            caption=add_caption(caption, indent),
             align=column_format,
             indent=indent,
         )
-        table_footer = FOOTER.format(indent=indent)
+        table_footer = FOOTER.format(
+            caption=add_caption(caption, indent),
+            label=add_label(label, indent),
+            indent=indent,
+        )
         return "\n".join((table_header, content, table_footer))
     else:
         return content
     
 
 def format_alignment(align, length):
     """Formats the column alignment."""
@@ -133,8 +139,8 @@
         out.write("\n\n")
     print(f"The table is {'written to' if replace else 'appended to'} {outfile}")
 
 
 def create_complete_latex_document(tables, outfile, replace=False):
     """Creates a complete LaTeX document with the given tables."""
     content = [PREAMBLE] + tables + [r"\end{document}"]
-    save_latex_table("\n\n".join(content), outfile, replace)
+    save_latex_table("\n\n".join(content), outfile, replace)
```

### Comparing `csvtex-1.0.1/PKG-INFO` & `csvtex-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvtex
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 License: MIT
 Author: Scott Suk
 Author-email: scottsuk0306@gmail.com
 Requires-Python: >3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

