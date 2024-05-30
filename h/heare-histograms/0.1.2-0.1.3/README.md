# Comparing `tmp/heare_histograms-0.1.2.tar.gz` & `tmp/heare_histograms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heare_histograms-0.1.2.tar", max compression
+gzip compressed data, was "heare_histograms-0.1.3.tar", max compression
```

## Comparing `heare_histograms-0.1.2.tar` & `heare_histograms-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-04-15 03:25:36.498089 heare_histograms-0.1.2/LICENSE
--rw-r--r--   0        0        0     2276 2024-04-15 03:25:36.498089 heare_histograms-0.1.2/README.md
--rw-r--r--   0        0        0      491 2024-04-15 03:25:36.498089 heare_histograms-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14196 2024-04-15 03:25:36.498089 heare_histograms-0.1.2/src/heare/histograms/__init__.py
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 heare_histograms-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-30 00:33:27.090051 heare_histograms-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2276 2024-05-30 00:33:27.090051 heare_histograms-0.1.3/README.md
+-rw-r--r--   0        0        0      491 2024-05-30 00:33:27.090051 heare_histograms-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    14304 2024-05-30 00:33:27.090051 heare_histograms-0.1.3/src/heare/histograms/__init__.py
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 heare_histograms-0.1.3/PKG-INFO
```

### Comparing `heare_histograms-0.1.2/LICENSE` & `heare_histograms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heare_histograms-0.1.2/README.md` & `heare_histograms-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `heare_histograms-0.1.2/src/heare/histograms/__init__.py` & `heare_histograms-0.1.3/src/heare/histograms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,18 @@
         """
         if self._dirty:
             self._data.sort()
             self._dirty = False
         idx = math.floor(len(self._data) * p)
         return self._data[min(idx, len(self._data) - 1)]
 
+    def mean(self) -> float:
+        total = sum(self._data)
+        return float(total) / len(self._data)
+
     # pylint: disable=method-hidden
     def sample_n(self, n: int) -> List[T]:
         """
         Sample n data points from the histogram.
 
         Args:
             n (int): The number of data points to sample.
```

### Comparing `heare_histograms-0.1.2/PKG-INFO` & `heare_histograms-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heare-histograms
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pure python histogram implementation for analysis and prediction.
 License: MIT
 Author: Sean Fitzgerald
 Author-email: sean@fitzgeralds.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

