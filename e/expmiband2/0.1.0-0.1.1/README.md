# Comparing `tmp/expmiband2-0.1.0.tar.gz` & `tmp/expmiband2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expmiband2-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "expmiband2-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `expmiband2-0.1.0.tar` & `expmiband2-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0        6 2024-05-30 06:27:57.855250 expmiband2-0.1.0/.gitignore
--rw-r--r--   0        0        0     1081 2024-05-30 06:27:57.855250 expmiband2-0.1.0/LICENSE
--rw-r--r--   0        0        0      163 2024-05-30 06:27:57.855250 expmiband2-0.1.0/Pipfile
--rw-r--r--   0        0        0     4040 2024-05-30 06:27:57.855250 expmiband2-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0     1759 2024-05-30 06:27:57.855250 expmiband2-0.1.0/README.md
--rw-r--r--   0        0        0      145 2024-05-30 06:29:48.554338 expmiband2-0.1.0/expmiband2/__init__.py
--rw-r--r--   0        0        0     3270 2024-05-30 06:27:57.855250 expmiband2-0.1.0/expmiband2/authsession.py
--rw-r--r--   0        0        0     4278 2024-05-30 06:27:57.855250 expmiband2-0.1.0/expmiband2/band2.py
--rw-r--r--   0        0        0      570 2024-05-30 06:32:13.992320 expmiband2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 expmiband2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2024-05-30 06:27:57.855250 expmiband2-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1081 2024-05-30 06:27:57.855250 expmiband2-0.1.1/LICENSE
+-rw-r--r--   0        0        0      163 2024-05-30 06:27:57.855250 expmiband2-0.1.1/Pipfile
+-rw-r--r--   0        0        0     4040 2024-05-30 06:27:57.855250 expmiband2-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0     1759 2024-05-30 06:27:57.855250 expmiband2-0.1.1/README.md
+-rw-r--r--   0        0        0      145 2024-05-30 06:37:08.952835 expmiband2-0.1.1/expmiband2/__init__.py
+-rw-r--r--   0        0        0     3270 2024-05-30 06:27:57.855250 expmiband2-0.1.1/expmiband2/authsession.py
+-rw-r--r--   0        0        0     4278 2024-05-30 06:27:57.855250 expmiband2-0.1.1/expmiband2/band2.py
+-rw-r--r--   0        0        0      570 2024-05-30 06:32:13.992320 expmiband2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 06:35:39.208090 expmiband2-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-30 06:36:15.244130 expmiband2-0.1.1/tests/test_it.py
+-rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 expmiband2-0.1.1/PKG-INFO
```

### Comparing `expmiband2-0.1.0/LICENSE` & `expmiband2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.0/Pipfile.lock` & `expmiband2-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.0/README.md` & `expmiband2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.0/expmiband2/authsession.py` & `expmiband2-0.1.1/expmiband2/authsession.py`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.0/expmiband2/band2.py` & `expmiband2-0.1.1/expmiband2/band2.py`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.0/pyproject.toml` & `expmiband2-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.0/PKG-INFO` & `expmiband2-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expmiband2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python API for communicating with MiBand2
 Author-email: Anton Ptashnik <iavtomator@gmail.com>
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: bleak==0.20.1
 Requires-Dist: pyaes==1.6.1
```

