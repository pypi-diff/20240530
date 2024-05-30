# Comparing `tmp/mix_n_match-0.3.0.tar.gz` & `tmp/mix_n_match-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mix_n_match-0.3.0.tar", last modified: Sun May 19 14:32:37 2024, max compression
+gzip compressed data, was "mix_n_match-0.4.0.tar", last modified: Thu May 30 17:25:06 2024, max compression
```

## Comparing `mix_n_match-0.3.0.tar` & `mix_n_match-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/mix_n_match/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/mix_n_match/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/mix_n_match.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 14:32:37.000000 mix_n_match-0.3.0/mix_n_match.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/requirements/extra.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/requirements/private.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/requirements/public.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 14:32:37.316261 mix_n_match-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-19 14:32:33.000000 mix_n_match-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:06.276538 mix_n_match-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-30 17:25:06.276538 mix_n_match-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:06.276538 mix_n_match-0.4.0/mix_n_match/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/mix_n_match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/mix_n_match/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35797 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/mix_n_match/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/mix_n_match/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:06.276538 mix_n_match-0.4.0/mix_n_match.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-30 17:25:06.000000 mix_n_match-0.4.0/mix_n_match.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-30 17:25:06.000000 mix_n_match-0.4.0/mix_n_match.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:25:06.000000 mix_n_match-0.4.0/mix_n_match.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 17:25:06.000000 mix_n_match-0.4.0/mix_n_match.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:25:06.000000 mix_n_match-0.4.0/mix_n_match.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:06.276538 mix_n_match-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/requirements/extra.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/requirements/private.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/requirements/public.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:25:06.276538 mix_n_match-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-30 17:25:02.000000 mix_n_match-0.4.0/setup.py
```

### Comparing `mix_n_match-0.3.0/LICENSE` & `mix_n_match-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mix_n_match-0.3.0/mix_n_match/correlations.py` & `mix_n_match-0.4.0/mix_n_match/correlations.py`

 * *Files identical despite different names*

### Comparing `mix_n_match-0.3.0/mix_n_match/utils.py` & `mix_n_match-0.4.0/mix_n_match/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -123,15 +123,18 @@
     SUPPORTED_METHODS = {"exact": "unique", "mode": "mode", "max": "max"}
     frequency_detector = SUPPORTED_METHODS.get(how)
     if frequency_detector is None:
         raise ValueError(
             f"Expected `how` in {sorted(SUPPORTED_METHODS)}. Got `{how}`"
         )
 
-    diff = df.select(pl.col(time_column).diff(null_behavior="drop"))
+    # -- need to sort the time column, AND drop duplicates
+    diff = df.select(
+        pl.col(time_column).unique().sort().diff(null_behavior="drop")
+    )
     frequency = getattr(diff[time_column], frequency_detector)()
 
     if how == "exact":
         num_unique_frequencies = len(frequency)
         if num_unique_frequencies != 1:
             _remaining_methods = sorted(
                 [method for method in SUPPORTED_METHODS if method != "exact"]
@@ -140,16 +143,21 @@
                 (
                     f"Got {num_unique_frequencies} unique frequencies when "
                     "expected only one. If you wish to work with non-exact "
                     f"frequencies, set `how` to one of {_remaining_methods}"
                 )
             )
 
-    frequency = frequency.item().total_seconds()
-    return frequency
+    if how != "max":  # max returns Python literal, others return Series
+        frequency = (
+            frequency.item()
+        )  # TODO this will fail if mode has multiple values!
+        # Need to think of how to resolve this issue
+
+    return frequency.total_seconds()
 
 
 # only get contiguous segments of a specific length
 def find_contiguous_segments(
     array: np.array,
     filter_mask: np.array | None = None,
     min_length: int | None = None,
@@ -200,7 +208,29 @@
     if min_length is not None:
         segment_lengths = indices_array[:, 1] - indices_array[:, 0] + 1
         indices_array = indices_array[segment_lengths >= min_length]
 
     indices_list = indices_array.tolist()
 
     return indices_list
+
+
+def generate_polars_condition(
+    expressions: list[pl.Expr], operator: str
+) -> pl.Expr:
+    """Given a list of Polars expressions, combine them using a polars
+    operation.
+
+    :param expressions: list of polars expressions
+    :param operator: string format of polars operation, e.g. "and_" or "or_"
+    :return: a single polars expression combining the expressions in the list
+
+    Example:
+        expressions = [pl.col("value") < 10, pl.col("value") > 15]
+        str(generate_polars_condition(expressions, "or_"))
+        >>> "[([(col("value")) > (dyn int: 15)]) | ([(col("value")) < (dyn int: 10)])]"  # noqa
+    """
+    final_expression = expressions.pop()
+    for expression in expressions:
+        final_expression = getattr(final_expression, operator)(expression)
+
+    return final_expression
```

### Comparing `mix_n_match-0.3.0/setup.py` & `mix_n_match-0.4.0/setup.py`

 * *Files identical despite different names*

