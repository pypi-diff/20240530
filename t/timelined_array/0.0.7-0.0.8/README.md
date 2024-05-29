# Comparing `tmp/timelined_array-0.0.7.tar.gz` & `tmp/timelined_array-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelined_array-0.0.7.tar", last modified: Tue May 28 14:51:08 2024, max compression
+gzip compressed data, was "timelined_array-0.0.8.tar", last modified: Wed May 29 22:15:57 2024, max compression
```

## Comparing `timelined_array-0.0.7.tar` & `timelined_array-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-28 14:50:56.202655 timelined_array-0.0.7/LICENSE
--rw-r--r--   0        0        0     2859 2024-05-28 14:50:56.202655 timelined_array-0.0.7/README.md
--rw-r--r--   0        0        0      613 2024-05-28 14:51:08.146571 timelined_array-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       97 2024-05-28 14:50:56.202655 timelined_array-0.0.7/src/timelined_array/__init__.py
--rw-r--r--   0        0        0    52649 2024-05-28 14:50:56.202655 timelined_array-0.0.7/src/timelined_array/time.py
--rw-r--r--   0        0        0        0 2024-05-28 14:50:56.202655 timelined_array-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 timelined_array-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-29 22:15:35.716439 timelined_array-0.0.8/LICENSE
+-rw-r--r--   0        0        0    10618 2024-05-29 22:15:35.716439 timelined_array-0.0.8/README.md
+-rw-r--r--   0        0        0      613 2024-05-29 22:15:57.720723 timelined_array-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-05-29 22:15:35.716439 timelined_array-0.0.8/src/timelined_array/__init__.py
+-rw-r--r--   0        0        0    52912 2024-05-29 22:15:35.716439 timelined_array-0.0.8/src/timelined_array/time.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:15:35.716439 timelined_array-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    10988 1970-01-01 00:00:00.000000 timelined_array-0.0.8/PKG-INFO
```

### Comparing `timelined_array-0.0.7/LICENSE` & `timelined_array-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.7/pyproject.toml` & `timelined_array-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 dependencies = [
     "numpy",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dynamic = []
-version = "0.0.7"
+version = "0.0.8"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `timelined_array-0.0.7/src/timelined_array/time.py` & `timelined_array-0.0.8/src/timelined_array/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,14 @@
     @property
     def itime(self) -> "TimeIndexer": ...
 
     def _get_array_cls(self) -> "Type": ...
 
     def transpose(self): ...
 
-    def _finish_axis_removing_operation(self, result, axis): ...
-
 
 class Timeline(np.ndarray):
     _step = None
     _max_step = None
     max_step_mult = 2
 
     def __new__(cls, input_array, uniform_space=False):
@@ -498,15 +496,15 @@
 
         final_timeline = (
             self.timeline[index[time_dimension_in_index]] if len(index) > time_dimension_in_index else self.timeline
         )
 
         return index, final_timeline, final_time_dimension
 
-    def _get_indexed_times(self, index: int | Tuple[int, ...] | slice | Tuple[slice] | List | np.ndarray):
+    def _get_indexed_times(self, index: int | Tuple[int, ...] | slice | Tuple[slice, ...] | List | np.ndarray):
         """Get indexed times based on the provided index.
 
         Args:
             index (int | Tuple[int, ...] | slice | Tuple[slice] | List | np.ndarray): The index to retrieve times from.
 
         Returns:
             np.ndarray: The indexed times based on the provided index.
@@ -527,15 +525,17 @@
 
         Returns:
             bool: True if the input object is a single element, False otherwise.
         """
 
         return obj.shape == ()
 
-    def _finish_axis_removing_operation(self, result: TimeCompatibleProtocol, axis: int | Tuple[int, ...] | None):
+    def _finish_axis_removing_operation(
+        self, result: "TimelinedArray| MaskedTimelinedArray | np.ndarray | int | float", axis: int | Tuple[int, ...]
+    ) -> "TimelinedArray| MaskedTimelinedArray | np.ndarray | int | float":
         """Finish axis removing operation.
 
         Args:
             result (TimeCompatibleProtocol): The result of the operation.
             axis (int | Tuple[int, ...] | None): The axis or axes to remove.
 
         Returns:
@@ -669,15 +669,19 @@
             else:
                 # select all with slice(None) equivalent to ":"
                 indexer.append(slice(None))
         indexer = tuple(indexer)
 
         shift_area = self.itime.__getitem__(period) if time_period else self.__getitem__(period)
 
-        return self - np.repeat(shift_area.mean(axis=axis).__getitem__(tuple(indexer)), self.shape[axis], axis=axis)
+        # if not this : we lost a dimension because we sliced one axis to a single element, no need to no .mean
+        if not len(shift_area.shape) < len(self.shape):
+            shift_area = shift_area.mean(axis=axis)
+
+        return self - np.repeat(shift_area.__getitem__(tuple(indexer)), self.shape[axis], axis=axis)
 
     def swapaxes(self: TimeCompatibleProtocol, axis1: int, axis2: int):
         """Swap the two specified axes of the TimelinedArray.
 
         Args:
             axis1 (int): The first axis to be swapped.
             axis2 (int): The second axis to be swapped.
```

