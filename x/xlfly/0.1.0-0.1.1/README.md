# Comparing `tmp/xlfly-0.1.0.tar.gz` & `tmp/xlfly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlfly-0.1.0.tar", max compression
+gzip compressed data, was "xlfly-0.1.1.tar", max compression
```

## Comparing `xlfly-0.1.0.tar` & `xlfly-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      384 2024-05-29 11:47:08.944426 xlfly-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      264 2024-05-30 06:25:41.526267 xlfly-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 06:59:38.107979 xlfly-0.1.0/xlfly/__init__.py
--rw-r--r--   0        0        0     3222 2024-05-29 11:47:51.017832 xlfly-0.1.0/xlfly/app.py
--rw-r--r--   0        0        0     1530 2024-05-29 11:30:48.638342 xlfly-0.1.0/xlfly/copyover.py
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 xlfly-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      384 2024-05-30 07:20:44.728985 xlfly-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      264 2024-05-30 06:25:41.526267 xlfly-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 06:59:38.107979 xlfly-0.1.1/xlfly/__init__.py
+-rw-r--r--   0        0        0     3224 2024-05-30 07:12:42.133589 xlfly-0.1.1/xlfly/app.py
+-rw-r--r--   0        0        0     1530 2024-05-29 11:30:48.638342 xlfly-0.1.1/xlfly/copyover.py
+-rw-r--r--   0        0        0   264062 2024-05-09 02:20:34.503192 xlfly-0.1.1/xlfly/icon.ico
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 xlfly-0.1.1/PKG-INFO
```

### Comparing `xlfly-0.1.0/xlfly/app.py` & `xlfly-0.1.1/xlfly/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 def main():
     # UI
     root = tk.Tk()
     root.title("Excel智慧云V3")
     root.geometry("300x70")
     root.attributes("-topmost", 1)
-    root.iconbitmap("icon.ico")
+    # root.iconbitmap("icon.ico")
 
     # put widgets
     btn_run = ttk.Button(root, text="️Hello", command=hello)
     btn_run.pack(side=tk.LEFT)
 
     btn_create_config = ttk.Button(
         root, text="生成配置页", command=lambda: exec_func(create_config)
```

### Comparing `xlfly-0.1.0/xlfly/copyover.py` & `xlfly-0.1.1/xlfly/copyover.py`

 * *Files identical despite different names*

### Comparing `xlfly-0.1.0/PKG-INFO` & `xlfly-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlfly
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

