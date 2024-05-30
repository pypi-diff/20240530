# Comparing `tmp/examy-0.1.4.tar.gz` & `tmp/examy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examy-0.1.4.tar", max compression
+gzip compressed data, was "examy-0.1.7.tar", max compression
```

## Comparing `examy-0.1.4.tar` & `examy-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    18092 2024-05-26 10:54:25.496595 examy-0.1.4/LICENSE
--rw-r--r--   0        0        0        8 2024-05-26 10:54:25.496595 examy-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-05-26 10:54:25.496595 examy-0.1.4/examy/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-26 10:54:25.496595 examy-0.1.4/examy/fetchers/new_web_layout/optimized.py
--rw-r--r--   0        0        0     1730 2024-05-26 10:54:25.496595 examy-0.1.4/examy/fetchers/new_web_layout/utils/process_html.py
--rw-r--r--   0        0        0     4000 2024-05-26 10:54:25.496595 examy-0.1.4/examy/fetchers/new_web_layout/utils/webpage_actions.py
--rw-r--r--   0        0        0      253 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/ExamDescriptor.py
--rw-r--r--   0        0        0     1884 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/ExamReport.py
--rw-r--r--   0        0        0      716 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/Ranking.py
--rw-r--r--   0        0        0     1604 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/Student.py
--rw-r--r--   0        0        0      127 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/Test.py
--rw-r--r--   0        0        0      535 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/TestResult.py
--rw-r--r--   0        0        0      191 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/exceptions.py
--rw-r--r--   0        0        0     2095 2024-05-26 10:54:25.496595 examy-0.1.4/examy/models/fetcher.py
--rw-r--r--   0        0        0      635 2024-05-26 10:54:25.496595 examy-0.1.4/examy/utils/__init__.py
--rw-r--r--   0        0        0     4872 2024-05-26 10:54:25.496595 examy-0.1.4/examy/utils/export.py
--rw-r--r--   0        0        0     4234 2024-05-26 10:54:25.496595 examy-0.1.4/examy/utils/manager.py
--rw-r--r--   0        0        0     1152 2024-05-26 10:54:25.496595 examy-0.1.4/examy/utils/stgroup.py
--rw-r--r--   0        0        0      552 2024-05-26 10:54:25.496595 examy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 examy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-05-30 12:52:34.550769 examy-0.1.7/LICENSE
+-rw-r--r--   0        0        0        8 2024-05-30 12:52:34.550769 examy-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 12:52:34.550769 examy-0.1.7/examy/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-30 12:52:34.550769 examy-0.1.7/examy/fetchers/new_web_layout/optimized.py
+-rw-r--r--   0        0        0     1730 2024-05-30 12:52:34.550769 examy-0.1.7/examy/fetchers/new_web_layout/utils/process_html.py
+-rw-r--r--   0        0        0     4000 2024-05-30 12:52:34.550769 examy-0.1.7/examy/fetchers/new_web_layout/utils/webpage_actions.py
+-rw-r--r--   0        0        0      253 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/ExamDescriptor.py
+-rw-r--r--   0        0        0     1884 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/ExamReport.py
+-rw-r--r--   0        0        0      716 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/Ranking.py
+-rw-r--r--   0        0        0     1604 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/Student.py
+-rw-r--r--   0        0        0      127 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/Test.py
+-rw-r--r--   0        0        0      535 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/TestResult.py
+-rw-r--r--   0        0        0      191 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/exceptions.py
+-rw-r--r--   0        0        0     2095 2024-05-30 12:52:34.554769 examy-0.1.7/examy/models/fetcher.py
+-rw-r--r--   0        0        0      635 2024-05-30 12:52:34.554769 examy-0.1.7/examy/utils/__init__.py
+-rw-r--r--   0        0        0     4872 2024-05-30 12:52:34.554769 examy-0.1.7/examy/utils/export.py
+-rw-r--r--   0        0        0     4230 2024-05-30 12:52:34.554769 examy-0.1.7/examy/utils/manager.py
+-rw-r--r--   0        0        0     1152 2024-05-30 12:52:34.554769 examy-0.1.7/examy/utils/stgroup.py
+-rw-r--r--   0        0        0      552 2024-05-30 12:52:34.554769 examy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 examy-0.1.7/PKG-INFO
```

### Comparing `examy-0.1.4/LICENSE` & `examy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/fetchers/new_web_layout/optimized.py` & `examy-0.1.7/examy/fetchers/new_web_layout/optimized.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/fetchers/new_web_layout/utils/process_html.py` & `examy-0.1.7/examy/fetchers/new_web_layout/utils/process_html.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/fetchers/new_web_layout/utils/webpage_actions.py` & `examy-0.1.7/examy/fetchers/new_web_layout/utils/webpage_actions.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/models/ExamReport.py` & `examy-0.1.7/examy/models/ExamReport.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/models/Ranking.py` & `examy-0.1.7/examy/models/Ranking.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/models/Student.py` & `examy-0.1.7/examy/models/Student.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/models/TestResult.py` & `examy-0.1.7/examy/models/TestResult.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/models/fetcher.py` & `examy-0.1.7/examy/models/fetcher.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/utils/__init__.py` & `examy-0.1.7/examy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/utils/export.py` & `examy-0.1.7/examy/utils/export.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/examy/utils/manager.py` & `examy-0.1.7/examy/utils/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         err_list = self.errored_students[self._exam_descriptor.exam_name]
 
         try:
             fetcher.fetch(st, self._exam_descriptor)
             res = st.reports[-1]
             logger.info(
-                f"Get: {st.name}: ok; score={res.score}, net={res.net}, "
+                f"{st.name}: ok; score={res.score}, net={res.net}, "
                 f"class_rank={res.ranks.class_rank}, school_rank={res.ranks.school_rank}"
             )
             with self.errored_students_lock:
                 if st in err_list:
                     err_list.remove(st)
         except StudentDidNotTakeExam:
             logger.info(f"{st.name} did not take the exam named '{self._exam_descriptor.exam_name}'")
@@ -101,15 +101,15 @@
             count = len(students_to_fetch)
         else:
             raise ValueError(f"Invalid subset '{subset}'")
 
         with ThreadPoolExecutor(initializer=self._set_driver, max_workers=max_workers) as executor:
             for i, _ in enumerate(executor.map(self._fetch_single, students_to_fetch), 1):
                 # for loop is required for waiting for the results
-                logger.info(f"{i}/{count} done.")
+                logger.debug(f"{i}/{count} done.")
 
         for i in self._drivers.values():
             i.quit()
 
         self._drivers = {}
         self._fetcher_type = None
         self._exam_descriptor = None
```

### Comparing `examy-0.1.4/examy/utils/stgroup.py` & `examy-0.1.7/examy/utils/stgroup.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.4/pyproject.toml` & `examy-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "examy"
-version = "0.1.4"
+version = "0.1.7"
 description = ""
 authors = ["Eren Akgün <iobthedev@outlook.com>"]
 readme = "README.md"
 license = "GPL-2.0-only"
 repository = "https://github.com/insanolanbiri/examy"
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `examy-0.1.4/PKG-INFO` & `examy-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: examy
-Version: 0.1.4
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/insanolanbiri/examy
 License: GPL-2.0-only
 Author: Eren Akgün
 Author-email: iobthedev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

