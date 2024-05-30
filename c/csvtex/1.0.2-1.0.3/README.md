# Comparing `tmp/csvtex-1.0.2.tar.gz` & `tmp/csvtex-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvtex-1.0.2.tar", max compression
+gzip compressed data, was "csvtex-1.0.3.tar", max compression
```

## Comparing `csvtex-1.0.2.tar` & `csvtex-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2024-05-29 08:02:31.141592 csvtex-1.0.2/LICENSE
--rw-r--r--   0        0        0     2304 2024-05-29 08:43:42.284273 csvtex-1.0.2/README.md
--rw-r--r--   0        0        0      196 2024-05-29 08:32:45.254861 csvtex-1.0.2/csvtex/__init__.py
--rw-r--r--   0        0        0     4235 2024-05-29 22:40:28.398672 csvtex-1.0.2/csvtex/main.py
--rw-r--r--   0        0        0      391 2024-05-29 22:40:48.202840 csvtex-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 csvtex-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-29 08:02:31.141592 csvtex-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2304 2024-05-29 08:43:42.284273 csvtex-1.0.3/README.md
+-rw-r--r--   0        0        0      197 2024-05-29 23:31:10.520185 csvtex-1.0.3/csvtex/__init__.py
+-rw-r--r--   0        0        0     4341 2024-05-29 23:25:20.865221 csvtex-1.0.3/csvtex/main.py
+-rw-r--r--   0        0        0      391 2024-05-29 23:31:41.352447 csvtex-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 csvtex-1.0.3/PKG-INFO
```

### Comparing `csvtex-1.0.2/LICENSE` & `csvtex-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csvtex-1.0.2/README.md` & `csvtex-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `csvtex-1.0.2/csvtex/main.py` & `csvtex-1.0.3/csvtex/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,27 @@
 {label}
 \end{{table*}}"""
 
 LABEL = "\n{indent}\\label{{{label}}}"
 CAPTION = "\n{indent}\\caption{{\\footnotesize {caption}}}"
 
 
+def latex_escape(text):
+    latex_special_chars = {
+        "#": r"\#",
+        "$": r"\$",
+        "%": r"\%",
+        "&": r"\&",
+        "_": r"\_",
+        "{": r"\{",
+        "}": r"\}",
+    }
+    return str(text).translate(str.maketrans(latex_special_chars))
+
+
 def create_latex_table(
     file,
     sep=",",
     caption="",
     label="",
     align="c",
     units=None,
@@ -50,29 +63,20 @@
 
     Returns:
         str: LaTeX code for the table.
     """
     df = pd.read_csv(file, sep=sep, header=0 if header else None)
 
     if escape:
-        df = df.map(
-            lambda x: str(x).translate(
-                str.maketrans(
-                    {
-                        "#": r"\#",
-                        "$": r"\$",
-                        "%": r"\%",
-                        "&": r"\&",
-                        "_": r"\_",
-                        "{": r"\{",
-                        "}": r"\}",
-                    }
-                )
-            )
+        df = df.apply(
+            lambda col: col.apply(latex_escape) if col.dtype == object else col
         )
+        if header:
+            df.columns = [latex_escape(col) for col in df.columns]
+
     indent = "" if fragment else "    "
 
     column_format = format_alignment(align, len(df.columns))
 
     if header:
         header_row = " & ".join(df.columns) + r" \\"
     else:
@@ -102,15 +106,15 @@
             caption=add_caption(caption, indent),
             label=add_label(label, indent),
             indent=indent,
         )
         return "\n".join((table_header, content, table_footer))
     else:
         return content
-    
+
 
 def format_alignment(align, length):
     """Formats the column alignment."""
     if any(ch not in "lcr" for ch in align):
         align = "c"
 
     if len(align) == 1:
@@ -122,25 +126,27 @@
 
 
 def add_label(label, indent):
     """Creates a table label."""
     return LABEL.format(label=label, indent=indent) if label else ""
 
 
-def add_caption(caption, indent):
+def add_caption(caption, indent, escape=True):
     """Creates a table caption."""
-    return CAPTION.format(caption=caption, indent=indent) if caption else ""
+    if escape:
+        caption = latex_escape(caption)
+    return f"\n{indent}\\caption{{\\footnotesize {caption}}}" if caption else ""
 
 
 def save_latex_table(table, outfile, replace=False):
     """Saves the LaTeX table to a file."""
     mode = "w" if replace else "a"
     with open(outfile, mode) as out:
         out.write(table)
         out.write("\n\n")
     print(f"The table is {'written to' if replace else 'appended to'} {outfile}")
 
 
 def create_complete_latex_document(tables, outfile, replace=False):
     """Creates a complete LaTeX document with the given tables."""
     content = [PREAMBLE] + tables + [r"\end{document}"]
-    save_latex_table("\n\n".join(content), outfile, replace)
+    save_latex_table("\n\n".join(content), outfile, replace)
```

### Comparing `csvtex-1.0.2/PKG-INFO` & `csvtex-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvtex
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 License: MIT
 Author: Scott Suk
 Author-email: scottsuk0306@gmail.com
 Requires-Python: >3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

