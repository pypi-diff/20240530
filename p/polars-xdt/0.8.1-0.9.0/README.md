# Comparing `tmp/polars_xdt-0.8.1.tar.gz` & `tmp/polars_xdt-0.9.0.tar.gz`

## Comparing `polars_xdt-0.8.1.tar` & `polars_xdt-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 polars_xdt-0.8.1/Cargo.toml
--rw-r--r--   0     1001      127     3510 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      125 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/.gitignore
--rw-r--r--   0     1001      127      846 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/.readthedocs.yaml
--rw-r--r--   0     1001      127     5243 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1077 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/LICENSE
--rw-r--r--   0     1001      127      770 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/Makefile
--rw-r--r--   0     1001      127     2463 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/README.md
--rw-r--r--   0     1001      127     6148 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/assets/.DS_Store
--rw-r--r--   0     1001      127   929982 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/assets/polars-business.png
--rw-r--r--   0     1001      127     1447 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/bump_version.py
--rw-r--r--   0     1001      127      420 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/API.rst
--rw-r--r--   0     1001      127      634 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/Makefile
--rw-r--r--   0     1001      127      140 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.ExprXDTNamespace.ceil.rst
--rw-r--r--   0     1001      127      178 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.ExprXDTNamespace.format_localized.rst
--rw-r--r--   0     1001      127      189 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.ExprXDTNamespace.from_local_datetime.rst
--rw-r--r--   0     1001      127      160 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.ExprXDTNamespace.is_workday.rst
--rw-r--r--   0     1001      127      157 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.ExprXDTNamespace.offset_by.rst
--rw-r--r--   0     1001      127      183 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.ExprXDTNamespace.to_local_datetime.rst
--rw-r--r--   0     1001      127      111 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.date_range.rst
--rw-r--r--   0     1001      127      120 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/api/polars_xdt.workday_count.rst
--rw-r--r--   0     1001      127     1562 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/conf.py
--rw-r--r--   0     1001      127      403 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/index.rst
--rw-r--r--   0     1001      127      461 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/installation.rst
--rw-r--r--   0     1001      127      123 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/requirements-docs.txt
--rw-r--r--   0     1001      127     3377 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/docs/tutorial.rst
--rw-r--r--   0     1001      127      314 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/dprint.json
--rw-r--r--   0     1001      127     1543 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/licenses/NUMPY_LICENSE.txt
--rw-r--r--   0     1001      127     1634 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/licenses/PANDAS_LICENSE.txt
--rw-r--r--   0     1001      127       19 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/polars_xdt/.mypy.ini
--rw-r--r--   0     1001      127    25082 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/polars_xdt/__init__.py
--rw-r--r--   0     1001      127       17 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/polars_xdt/_internal.pyi
--rw-r--r--   0     1001      127        0 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/polars_xdt/py.typed
--rw-r--r--   0     1001      127     4902 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/polars_xdt/ranges.py
--rw-r--r--   0     1001      127       71 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/requirements.txt
--rw-r--r--   0     1001      127     7659 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/business_days.rs
--rw-r--r--   0     1001      127     3543 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/expressions.rs
--rw-r--r--   0     1001      127     3715 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/format_localized.rs
--rw-r--r--   0     1001      127     2088 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/is_workday.rs
--rw-r--r--   0     1001      127      459 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/lib.rs
--rw-r--r--   0     1001      127     3279 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/sub.rs
--rw-r--r--   0     1001      127     5900 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/timezone.rs
--rw-r--r--   0     1001      127     3542 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/src/to_julian.rs
--rw-r--r--   0     1001      127      516 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/ceil_test.py
--rw-r--r--   0     1001      127      929 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/julian_date_test.py
--rw-r--r--   0     1001      127     7465 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/test_business_offsets.py
--rw-r--r--   0     1001      127     2269 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/test_date_range.py
--rw-r--r--   0     1001      127     2691 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/test_format_localized.py
--rw-r--r--   0     1001      127     2323 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/test_is_busday.py
--rw-r--r--   0     1001      127     4628 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/test_sub.py
--rw-r--r--   0     1001      127     3213 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/tests/test_timezone.py
--rw-r--r--   0     1001      127    42154 2024-01-07 14:09:19.000000 polars_xdt-0.8.1/Cargo.lock
--rw-r--r--   0     1001      127     1674 2024-01-07 14:09:14.000000 polars_xdt-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 polars_xdt-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 polars_xdt-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      127     3510 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      125 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/.gitignore
+-rw-r--r--   0     1001      127      846 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/.readthedocs.yaml
+-rw-r--r--   0     1001      127     5243 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1077 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/LICENSE
+-rw-r--r--   0     1001      127      770 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/Makefile
+-rw-r--r--   0     1001      127     2463 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/README.md
+-rw-r--r--   0     1001      127     6148 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/assets/.DS_Store
+-rw-r--r--   0     1001      127   929982 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/assets/polars-business.png
+-rw-r--r--   0     1001      127     1447 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/bump_version.py
+-rw-r--r--   0     1001      127      511 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/API.rst
+-rw-r--r--   0     1001      127      634 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/Makefile
+-rw-r--r--   0     1001      127      140 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.ExprXDTNamespace.ceil.rst
+-rw-r--r--   0     1001      127      178 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.ExprXDTNamespace.format_localized.rst
+-rw-r--r--   0     1001      127      189 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.ExprXDTNamespace.from_local_datetime.rst
+-rw-r--r--   0     1001      127      160 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.ExprXDTNamespace.is_workday.rst
+-rw-r--r--   0     1001      127      157 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.ExprXDTNamespace.offset_by.rst
+-rw-r--r--   0     1001      127      183 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.ExprXDTNamespace.to_local_datetime.rst
+-rw-r--r--   0     1001      127      111 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.date_range.rst
+-rw-r--r--   0     1001      127      120 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/api/polars_xdt.workday_count.rst
+-rw-r--r--   0     1001      127     1562 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/conf.py
+-rw-r--r--   0     1001      127      403 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/index.rst
+-rw-r--r--   0     1001      127      461 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/installation.rst
+-rw-r--r--   0     1001      127      123 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/requirements-docs.txt
+-rw-r--r--   0     1001      127     3377 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/docs/tutorial.rst
+-rw-r--r--   0     1001      127      314 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/dprint.json
+-rw-r--r--   0     1001      127     1543 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/licenses/NUMPY_LICENSE.txt
+-rw-r--r--   0     1001      127     1634 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/licenses/PANDAS_LICENSE.txt
+-rw-r--r--   0     1001      127       19 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/polars_xdt/.mypy.ini
+-rw-r--r--   0     1001      127    28852 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/polars_xdt/__init__.py
+-rw-r--r--   0     1001      127       17 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/polars_xdt/_internal.pyi
+-rw-r--r--   0     1001      127        0 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/polars_xdt/py.typed
+-rw-r--r--   0     1001      127     4902 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/polars_xdt/ranges.py
+-rw-r--r--   0     1001      127       71 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/requirements.txt
+-rw-r--r--   0     1001      127     7659 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/business_days.rs
+-rw-r--r--   0     1001      127     4734 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/expressions.rs
+-rw-r--r--   0     1001      127     3715 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/format_localized.rs
+-rw-r--r--   0     1001      127     2088 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/is_workday.rs
+-rw-r--r--   0     1001      127      476 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      127     3279 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/sub.rs
+-rw-r--r--   0     1001      127     5900 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/timezone.rs
+-rw-r--r--   0     1001      127     3542 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/to_julian.rs
+-rw-r--r--   0     1001      127     1417 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/src/utc_offsets.rs
+-rw-r--r--   0     1001      127      516 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/ceil_test.py
+-rw-r--r--   0     1001      127      929 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/julian_date_test.py
+-rw-r--r--   0     1001      127     3151 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/offsets_test.py
+-rw-r--r--   0     1001      127     7465 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/test_business_offsets.py
+-rw-r--r--   0     1001      127     2269 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/test_date_range.py
+-rw-r--r--   0     1001      127     2691 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/test_format_localized.py
+-rw-r--r--   0     1001      127     2323 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/test_is_busday.py
+-rw-r--r--   0     1001      127     4628 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/test_sub.py
+-rw-r--r--   0     1001      127     3213 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/tests/test_timezone.py
+-rw-r--r--   0     1001      127    42154 2024-01-07 19:56:22.000000 polars_xdt-0.9.0/Cargo.lock
+-rw-r--r--   0     1001      127     1674 2024-01-07 19:56:18.000000 polars_xdt-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 polars_xdt-0.9.0/PKG-INFO
```

### Comparing `polars_xdt-0.8.1/Cargo.toml` & `polars_xdt-0.9.0/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars_xdt"
-version = "0.8.1"
+version = "0.9.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "polars_xdt"
 crate-type = ["cdylib"]
```

### Comparing `polars_xdt-0.8.1/.github/workflows/CI.yml` & `polars_xdt-0.9.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/.readthedocs.yaml` & `polars_xdt-0.9.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/CODE_OF_CONDUCT.md` & `polars_xdt-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/LICENSE` & `polars_xdt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/Makefile` & `polars_xdt-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/README.md` & `polars_xdt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/assets/.DS_Store` & `polars_xdt-0.9.0/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/assets/polars-business.png` & `polars_xdt-0.9.0/assets/polars-business.png`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/bump_version.py` & `polars_xdt-0.9.0/bump_version.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/docs/Makefile` & `polars_xdt-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/docs/conf.py` & `polars_xdt-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/docs/tutorial.rst` & `polars_xdt-0.9.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/licenses/NUMPY_LICENSE.txt` & `polars_xdt-0.9.0/licenses/NUMPY_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/licenses/PANDAS_LICENSE.txt` & `polars_xdt-0.9.0/licenses/PANDAS_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/polars_xdt/__init__.py` & `polars_xdt-0.9.0/polars_xdt/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -574,14 +574,108 @@
         result = (
             pl.when(self._expr == truncated)
             .then(self._expr)
             .otherwise(truncated.dt.offset_by(every))
         )
         return cast(XDTExpr, result)
 
+    def base_utc_offset(self) -> XDTExpr:
+        """
+        Base offset from UTC.
+
+        This is usually constant for all datetimes in a given time zone, but
+        may vary in the rare case that a country switches time zone, like
+        Samoa (Apia) did at the end of 2011.
+
+        Returns
+        -------
+        Expr
+            Expression of data type :class:`Duration`.
+
+        See Also
+        --------
+        dst_offset : Daylight savings offset from UTC.
+
+        Examples
+        --------
+        >>> from datetime import datetime
+        >>> import polars_xdt  # noqa: F401
+        >>> df = pl.DataFrame(
+        ...     {
+        ...         "ts": [datetime(2011, 12, 29), datetime(2012, 1, 1)],
+        ...     }
+        ... )
+        >>> df = df.with_columns(
+        ...     pl.col("ts").dt.replace_time_zone("Pacific/Apia")
+        ... )
+        >>> df.with_columns(
+        ...     pl.col("ts").xdt.base_utc_offset().alias("base_utc_offset")
+        ... )
+        shape: (2, 2)
+        ┌────────────────────────────┬─────────────────┐
+        │ ts                         ┆ base_utc_offset │
+        │ ---                        ┆ ---             │
+        │ datetime[μs, Pacific/Apia] ┆ duration[ms]    │
+        ╞════════════════════════════╪═════════════════╡
+        │ 2011-12-29 00:00:00 -10    ┆ -11h            │
+        │ 2012-01-01 00:00:00 +14    ┆ 13h             │
+        └────────────────────────────┴─────────────────┘
+        """
+        result = self._expr.register_plugin(
+            lib=lib,
+            symbol="base_utc_offset",
+            is_elementwise=True,
+            args=[],
+        )
+        return cast(XDTExpr, result)
+
+    def dst_offset(self) -> XDTExpr:
+        """
+        Additional offset currently in effect (typically due to daylight saving time).
+
+        Returns
+        -------
+        Expr
+            Expression of data type :class:`Duration`.
+
+        See Also
+        --------
+        base_utc_offset : Base offset from UTC.
+
+        Examples
+        --------
+        >>> from datetime import datetime
+        >>> import polars_xdt  # noqa: F401
+        >>> df = pl.DataFrame(
+        ...     {
+        ...         "ts": [datetime(2020, 10, 25), datetime(2020, 10, 26)],
+        ...     }
+        ... )
+        >>> df = df.with_columns(
+        ...     pl.col("ts").dt.replace_time_zone("Europe/London")
+        ... )
+        >>> df.with_columns(pl.col("ts").xdt.dst_offset().alias("dst_offset"))
+        shape: (2, 2)
+        ┌─────────────────────────────┬──────────────┐
+        │ ts                          ┆ dst_offset   │
+        │ ---                         ┆ ---          │
+        │ datetime[μs, Europe/London] ┆ duration[ms] │
+        ╞═════════════════════════════╪══════════════╡
+        │ 2020-10-25 00:00:00 BST     ┆ 1h           │
+        │ 2020-10-26 00:00:00 GMT     ┆ 0ms          │
+        └─────────────────────────────┴──────────────┘
+        """
+        result = self._expr.register_plugin(
+            lib=lib,
+            symbol="dst_offset",
+            is_elementwise=True,
+            args=[],
+        )
+        return cast(XDTExpr, result)
+
 
 class XDTExpr(pl.Expr):
     @property
     def xdt(self) -> ExprXDTNamespace:
         return ExprXDTNamespace(self)
```

### Comparing `polars_xdt-0.8.1/polars_xdt/ranges.py` & `polars_xdt-0.9.0/polars_xdt/ranges.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/src/business_days.rs` & `polars_xdt-0.9.0/src/business_days.rs`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/src/expressions.rs` & `polars_xdt-0.9.0/src/expressions.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #![allow(clippy::unit_arg, clippy::unused_unit)]
 use crate::business_days::*;
 use crate::format_localized::*;
 use crate::is_workday::*;
 use crate::sub::*;
 use crate::timezone::*;
 use crate::to_julian::*;
+use crate::utc_offsets::*;
+use chrono_tz::Tz;
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
 use serde::Deserialize;
+use std::str::FromStr;
 #[derive(Deserialize)]
 pub struct BusinessDayKwargs {
     holidays: Vec<i32>,
     weekmask: [bool; 7],
     roll: Option<String>,
 }
 
@@ -22,18 +25,24 @@
 }
 #[derive(Deserialize)]
 pub struct FormatLocalizedKwargs {
     format: String,
     locale: String,
 }
 
-fn bday_output(input_fields: &[Field]) -> PolarsResult<Field> {
+fn same_output(input_fields: &[Field]) -> PolarsResult<Field> {
     let field = input_fields[0].clone();
     Ok(field)
 }
+fn duration_ms(input_fields: &[Field]) -> PolarsResult<Field> {
+    Ok(Field::new(
+        input_fields[0].name(),
+        DataType::Duration(TimeUnit::Milliseconds),
+    ))
+}
 
 pub fn to_local_datetime_output(input_fields: &[Field]) -> PolarsResult<Field> {
     let field = input_fields[0].clone();
     let dtype = match field.dtype {
         DataType::Datetime(unit, _) => DataType::Datetime(unit, None),
         _ => polars_bail!(InvalidOperation:
             "dtype '{}' not supported", field.dtype
@@ -49,15 +58,15 @@
         _ => polars_bail!(InvalidOperation:
             "dtype '{}' not supported", field.dtype
         ),
     };
     Ok(Field::new(&field.name, dtype))
 }
 
-#[polars_expr(output_type_func=bday_output)]
+#[polars_expr(output_type_func=same_output)]
 fn advance_n_days(inputs: &[Series], kwargs: BusinessDayKwargs) -> PolarsResult<Series> {
     let s = &inputs[0];
     let n = &inputs[1].cast(&DataType::Int32)?;
     let weekmask = kwargs.weekmask;
     let holidays = kwargs.holidays;
     let roll = kwargs.roll.unwrap();
 
@@ -106,7 +115,31 @@
 }
 
 #[polars_expr(output_type=Float64)]
 fn to_julian_date(inputs: &[Series]) -> PolarsResult<Series> {
     let s = &inputs[0];
     impl_to_julian_date(s)
 }
+
+#[polars_expr(output_type_func=duration_ms)]
+fn base_utc_offset(inputs: &[Series]) -> PolarsResult<Series> {
+    let s = &inputs[0];
+    match s.dtype() {
+        DataType::Datetime(time_unit, Some(time_zone)) => {
+            let time_zone = Tz::from_str(time_zone).unwrap();
+            Ok(impl_base_utc_offset(s.datetime()?, time_unit, &time_zone).into_series())
+        }
+        _ => polars_bail!(InvalidOperation: "base_utc_offset only works on Datetime type."),
+    }
+}
+
+#[polars_expr(output_type_func=duration_ms)]
+fn dst_offset(inputs: &[Series]) -> PolarsResult<Series> {
+    let s = &inputs[0];
+    match s.dtype() {
+        DataType::Datetime(time_unit, Some(time_zone)) => {
+            let time_zone = Tz::from_str(time_zone).unwrap();
+            Ok(impl_dst_offset(s.datetime()?, time_unit, &time_zone).into_series())
+        }
+        _ => polars_bail!(InvalidOperation: "base_utc_offset only works on Datetime type."),
+    }
+}
```

### Comparing `polars_xdt-0.8.1/src/format_localized.rs` & `polars_xdt-0.9.0/src/format_localized.rs`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/src/is_workday.rs` & `polars_xdt-0.9.0/src/is_workday.rs`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/src/sub.rs` & `polars_xdt-0.9.0/src/sub.rs`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/src/timezone.rs` & `polars_xdt-0.9.0/src/timezone.rs`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/src/to_julian.rs` & `polars_xdt-0.9.0/src/to_julian.rs`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/ceil_test.py` & `polars_xdt-0.9.0/tests/ceil_test.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/julian_date_test.py` & `polars_xdt-0.9.0/tests/julian_date_test.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/test_business_offsets.py` & `polars_xdt-0.9.0/tests/test_business_offsets.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/test_date_range.py` & `polars_xdt-0.9.0/tests/test_date_range.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/test_format_localized.py` & `polars_xdt-0.9.0/tests/test_format_localized.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/test_is_busday.py` & `polars_xdt-0.9.0/tests/test_is_busday.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/test_sub.py` & `polars_xdt-0.9.0/tests/test_sub.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/tests/test_timezone.py` & `polars_xdt-0.9.0/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/Cargo.lock` & `polars_xdt-0.9.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -953,15 +953,15 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_xdt"
-version = "0.8.1"
+version = "0.9.0"
 dependencies = [
  "chrono",
  "chrono-tz",
  "jemallocator",
  "polars",
  "polars-arrow",
  "polars-ops",
```

### Comparing `polars_xdt-0.8.1/pyproject.toml` & `polars_xdt-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_xdt-0.8.1/PKG-INFO` & `polars_xdt-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-xdt
-Version: 0.8.1
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Time Series Extras (e.g. business day utilities) for Polars
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 Requires-Python: >=3.8
```

