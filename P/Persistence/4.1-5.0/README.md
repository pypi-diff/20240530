# Comparing `tmp/Persistence-4.1.tar.gz` & `tmp/Persistence-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Persistence-4.1.tar", last modified: Thu Oct  5 14:14:44 2023, max compression
+gzip compressed data, was "Persistence-5.0.tar", last modified: Thu May 30 09:12:02 2024, max compression
```

## Comparing `Persistence-4.1.tar` & `Persistence-5.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.304490 Persistence-4.1/
--rw-r--r--   0 jens       (501) staff       (20)      585 2023-10-05 13:02:42.000000 Persistence-4.1/.coveragerc
--rwxr-xr-x   0 jens       (501) staff       (20)     1992 2023-10-05 14:01:48.000000 Persistence-4.1/.manylinux-install.sh
--rwxr-xr-x   0 jens       (501) staff       (20)      509 2023-10-05 13:02:42.000000 Persistence-4.1/.manylinux.sh
--rw-r--r--   0 jens       (501) staff       (20)     2407 2023-10-05 14:01:48.000000 Persistence-4.1/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      799 2023-10-05 13:02:42.000000 Persistence-4.1/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:51:07.000000 Persistence-4.1/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:51:07.000000 Persistence-4.1/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      301 2023-10-05 13:02:42.000000 Persistence-4.1/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)     4033 2023-10-05 14:14:44.304432 Persistence-4.1/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      373 2021-11-02 08:51:07.000000 Persistence-4.1/README.rst
--rw-r--r--   0 jens       (501) staff       (20)     1801 2023-10-05 14:01:48.000000 Persistence-4.1/appveyor.yml
--rw-r--r--   0 jens       (501) staff       (20)      312 2021-11-02 08:51:07.000000 Persistence-4.1/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.300536 Persistence-4.1/include/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.302484 Persistence-4.1/include/ExtensionClass/
--rw-r--r--   0 jens       (501) staff       (20)     9572 2022-01-20 08:04:35.000000 Persistence-4.1/include/ExtensionClass/ExtensionClass.h
--rw-r--r--   0 jens       (501) staff       (20)     2521 2022-11-02 09:33:41.000000 Persistence-4.1/include/ExtensionClass/_compat.h
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.302794 Persistence-4.1/include/persistent/
--rw-r--r--   0 jens       (501) staff       (20)     1531 2022-01-20 08:04:35.000000 Persistence-4.1/include/persistent/_compat.h
--rw-r--r--   0 jens       (501) staff       (20)     5114 2022-01-20 08:04:35.000000 Persistence-4.1/include/persistent/cPersistence.h
--rw-r--r--   0 jens       (501) staff       (20)     2639 2022-01-20 08:04:35.000000 Persistence-4.1/include/persistent/ring.h
--rw-r--r--   0 jens       (501) staff       (20)      453 2023-10-05 14:14:44.304717 Persistence-4.1/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     2072 2023-10-05 14:01:48.000000 Persistence-4.1/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.300722 Persistence-4.1/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.303099 Persistence-4.1/src/Persistence/
--rw-r--r--   0 jens       (501) staff       (20)     4560 2023-01-03 12:34:46.000000 Persistence-4.1/src/Persistence/_Persistence.c
--rw-r--r--   0 jens       (501) staff       (20)     2084 2022-11-02 09:33:41.000000 Persistence-4.1/src/Persistence/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     1803 2023-01-03 12:34:46.000000 Persistence-4.1/src/Persistence/mapping.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.304104 Persistence-4.1/src/Persistence/tests/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:07.000000 Persistence-4.1/src/Persistence/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)    11315 2023-01-03 12:34:46.000000 Persistence-4.1/src/Persistence/tests/test_ec.py
--rw-r--r--   0 jens       (501) staff       (20)     1049 2021-11-02 08:51:07.000000 Persistence-4.1/src/Persistence/tests/test_mapping.py
--rw-r--r--   0 jens       (501) staff       (20)     6905 2023-01-03 12:34:46.000000 Persistence-4.1/src/Persistence/tests/test_persistent.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-10-05 14:14:44.303709 Persistence-4.1/src/Persistence.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)     4033 2023-10-05 14:14:44.000000 Persistence-4.1/src/Persistence.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      803 2023-10-05 14:14:44.000000 Persistence-4.1/src/Persistence.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-10-05 14:14:44.000000 Persistence-4.1/src/Persistence.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-01-20 08:05:12.000000 Persistence-4.1/src/Persistence.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)       62 2023-10-05 14:14:44.000000 Persistence-4.1/src/Persistence.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)       12 2023-10-05 14:14:44.000000 Persistence-4.1/src/Persistence.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1313 2023-10-05 14:01:48.000000 Persistence-4.1/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.546516 Persistence-5.0/
+-rw-r--r--   0 jens       (501) staff       (20)      606 2024-05-30 07:24:38.000000 Persistence-5.0/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2190 2024-05-30 08:33:17.000000 Persistence-5.0/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-05-30 07:24:38.000000 Persistence-5.0/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)     2564 2024-05-30 08:54:00.000000 Persistence-5.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2024-05-30 07:24:38.000000 Persistence-5.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:51:07.000000 Persistence-5.0/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:51:07.000000 Persistence-5.0/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      280 2024-05-30 07:24:38.000000 Persistence-5.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)     4191 2024-05-30 09:12:02.546456 Persistence-5.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      373 2021-11-02 08:51:07.000000 Persistence-5.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      312 2021-11-02 08:51:07.000000 Persistence-5.0/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.541869 Persistence-5.0/include/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.544106 Persistence-5.0/include/ExtensionClass/
+-rw-r--r--   0 jens       (501) staff       (20)     9572 2022-01-20 08:04:35.000000 Persistence-5.0/include/ExtensionClass/ExtensionClass.h
+-rw-r--r--   0 jens       (501) staff       (20)     2521 2022-11-02 09:33:41.000000 Persistence-5.0/include/ExtensionClass/_compat.h
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.544791 Persistence-5.0/include/persistent/
+-rw-r--r--   0 jens       (501) staff       (20)     1531 2022-01-20 08:04:35.000000 Persistence-5.0/include/persistent/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)     5114 2022-01-20 08:04:35.000000 Persistence-5.0/include/persistent/cPersistence.h
+-rw-r--r--   0 jens       (501) staff       (20)     2639 2022-01-20 08:04:35.000000 Persistence-5.0/include/persistent/ring.h
+-rw-r--r--   0 jens       (501) staff       (20)      424 2024-05-30 09:12:02.546722 Persistence-5.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     2073 2024-05-30 08:54:23.000000 Persistence-5.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.542025 Persistence-5.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.545167 Persistence-5.0/src/Persistence/
+-rw-r--r--   0 jens       (501) staff       (20)     4560 2023-01-03 12:34:46.000000 Persistence-5.0/src/Persistence/_Persistence.c
+-rw-r--r--   0 jens       (501) staff       (20)     2084 2022-11-02 09:33:41.000000 Persistence-5.0/src/Persistence/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     1803 2023-01-03 12:34:46.000000 Persistence-5.0/src/Persistence/mapping.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.546146 Persistence-5.0/src/Persistence/tests/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:07.000000 Persistence-5.0/src/Persistence/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)    11315 2023-01-03 12:34:46.000000 Persistence-5.0/src/Persistence/tests/test_ec.py
+-rw-r--r--   0 jens       (501) staff       (20)     1049 2021-11-02 08:51:07.000000 Persistence-5.0/src/Persistence/tests/test_mapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     6905 2023-01-03 12:34:46.000000 Persistence-5.0/src/Persistence/tests/test_persistent.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:12:02.545754 Persistence-5.0/src/Persistence.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)     4191 2024-05-30 09:12:02.000000 Persistence-5.0/src/Persistence.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      790 2024-05-30 09:12:02.000000 Persistence-5.0/src/Persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-30 09:12:02.000000 Persistence-5.0/src/Persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-01-20 08:05:12.000000 Persistence-5.0/src/Persistence.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)       62 2024-05-30 09:12:02.000000 Persistence-5.0/src/Persistence.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)       12 2024-05-30 09:12:02.000000 Persistence-5.0/src/Persistence.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1656 2024-05-30 08:33:17.000000 Persistence-5.0/tox.ini
```

### Comparing `Persistence-4.1/.coveragerc` & `Persistence-5.0/.coveragerc`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     src/
     .tox/*/lib/python*/site-packages/
     .tox/pypy*/site-packages/
 
 [report]
 show_missing = true
 precision = 2
+ignore_errors = True
 exclude_lines =
     except ImportError:
     if __name__ == '__main__':
     pragma: no cover
     pragma: nocover
     raise AssertionError
     raise NotImplementedError
```

### Comparing `Persistence-4.1/.manylinux-install.sh` & `Persistence-5.0/.manylinux-install.sh`

 * *Files 6% similar despite different names*

```diff
@@ -24,35 +24,40 @@
 ls -ld /cache/pip
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
-        *"cp37"*) echo 'py37';;
+        *"cp313"*) echo 'py313';;
         *"cp38"*) echo 'py38';;
         *"cp39"*) echo 'py39';;
         *"cp310"*) echo 'py310';;
         *"cp311"*) echo 'py311';;
         *"cp312"*) echo 'py312';;
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
-       [[ "${PYBIN}" == *"cp311"* ]] || \
-       [[ "${PYBIN}" == *"cp312"* ]] || \
-       [[ "${PYBIN}" == *"cp37"* ]] || \
-       [[ "${PYBIN}" == *"cp38"* ]] || \
-       [[ "${PYBIN}" == *"cp39"* ]] || \
-       [[ "${PYBIN}" == *"cp310"* ]] ; then
-        "${PYBIN}/pip" install -e /io/
-        "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+       [[ "${PYBIN}" == *"cp313/"* ]] || \
+       [[ "${PYBIN}" == *"cp311/"* ]] || \
+       [[ "${PYBIN}" == *"cp312/"* ]] || \
+       [[ "${PYBIN}" == *"cp38/"* ]] || \
+       [[ "${PYBIN}" == *"cp39/"* ]] || \
+       [[ "${PYBIN}" == *"cp310/"* ]] ; then
+        if [[ "${PYBIN}" == *"cp313/"* ]] ; then
+            "${PYBIN}/pip" install --pre -e /io/
+            "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
+        else
+            "${PYBIN}/pip" install -e /io/
+            "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        fi
         if [ `uname -m` == 'aarch64' ]; then
           cd /io/
           ${PYBIN}/pip install tox
           TOXENV=$(tox_env_map "${PYBIN}")
           ${PYBIN}/tox -e ${TOXENV}
           cd ..
         fi
```

### Comparing `Persistence-4.1/CHANGES.rst` & `Persistence-5.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+5.0 (2024-05-30)
+----------------
+
+- Drop support for Python 3.7.
+
+- Add preliminary support for Python 3.13 as of 3.13a3.
+
+- Build Windows wheels on GHA.
+
+
 4.1 (2023-10-05)
 ----------------
 
 - Add support for Python 3.12.
 
 
 4.0.post1 (2023-03-24)
```

### Comparing `Persistence-4.1/CONTRIBUTING.md` & `Persistence-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/LICENSE.txt` & `Persistence-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/PKG-INFO` & `Persistence-5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: Persistence
-Version: 4.1
+Version: 5.0
 Summary: Persistent ExtensionClass
 Home-page: https://github.com/zopefoundation/Persistence
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Zope
 Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: ExtensionClass>=4.6
 Requires-Dist: persistent>=4.1.1
 Provides-Extra: test
 Requires-Dist: zope.testrunner; extra == "test"
 
 Overview
@@ -40,14 +40,24 @@
 .. _ExtensionClass : https://pypi.org/project/ExtensionClass/
 .. _persistent : https://pypi.org/project/persistent/
 
 
 Changelog
 =========
 
+5.0 (2024-05-30)
+----------------
+
+- Drop support for Python 3.7.
+
+- Add preliminary support for Python 3.13 as of 3.13a3.
+
+- Build Windows wheels on GHA.
+
+
 4.1 (2023-10-05)
 ----------------
 
 - Add support for Python 3.12.
 
 
 4.0.post1 (2023-03-24)
```

### Comparing `Persistence-4.1/include/ExtensionClass/ExtensionClass.h` & `Persistence-5.0/include/ExtensionClass/ExtensionClass.h`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/include/ExtensionClass/_compat.h` & `Persistence-5.0/include/ExtensionClass/_compat.h`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/include/persistent/_compat.h` & `Persistence-5.0/include/persistent/_compat.h`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/include/persistent/cPersistence.h` & `Persistence-5.0/include/persistent/cPersistence.h`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/include/persistent/ring.h` & `Persistence-5.0/include/persistent/ring.h`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/setup.py` & `Persistence-5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 else:
     ext_modules = [
         Extension("Persistence._Persistence",
                   [os.path.join('src', 'Persistence', '_Persistence.c')],
                   include_dirs=['include', 'src']),
     ]
 
-version = '4.1'
+version = '5.0'
 
 setup(
     name='Persistence',
     version=version,
     url='https://github.com/zopefoundation/Persistence',
     license='ZPL 2.1',
     description='Persistent ExtensionClass',
@@ -40,25 +40,25 @@
         "Framework :: Zope",
         "Framework :: Zope :: 4",
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: Zope Public License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     ext_modules=ext_modules,
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'ExtensionClass >= 4.6',
         'persistent >= 4.1.1',
     ],
     extras_require={
         'test': ['zope.testrunner'],
     },
```

### Comparing `Persistence-4.1/src/Persistence/_Persistence.c` & `Persistence-5.0/src/Persistence/_Persistence.c`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/src/Persistence/__init__.py` & `Persistence-5.0/src/Persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/src/Persistence/mapping.py` & `Persistence-5.0/src/Persistence/mapping.py`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/src/Persistence/tests/test_ec.py` & `Persistence-5.0/src/Persistence/tests/test_ec.py`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/src/Persistence/tests/test_mapping.py` & `Persistence-5.0/src/Persistence/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/src/Persistence/tests/test_persistent.py` & `Persistence-5.0/src/Persistence/tests/test_persistent.py`

 * *Files identical despite different names*

### Comparing `Persistence-4.1/src/Persistence.egg-info/PKG-INFO` & `Persistence-5.0/src/Persistence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: Persistence
-Version: 4.1
+Version: 5.0
 Summary: Persistent ExtensionClass
 Home-page: https://github.com/zopefoundation/Persistence
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Zope
 Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: ExtensionClass>=4.6
 Requires-Dist: persistent>=4.1.1
 Provides-Extra: test
 Requires-Dist: zope.testrunner; extra == "test"
 
 Overview
@@ -40,14 +40,24 @@
 .. _ExtensionClass : https://pypi.org/project/ExtensionClass/
 .. _persistent : https://pypi.org/project/persistent/
 
 
 Changelog
 =========
 
+5.0 (2024-05-30)
+----------------
+
+- Drop support for Python 3.7.
+
+- Add preliminary support for Python 3.13 as of 3.13a3.
+
+- Build Windows wheels on GHA.
+
+
 4.1 (2023-10-05)
 ----------------
 
 - Add support for Python 3.12.
 
 
 4.0.post1 (2023-03-24)
```

### Comparing `Persistence-4.1/src/Persistence.egg-info/SOURCES.txt` & `Persistence-5.0/src/Persistence.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 .manylinux.sh
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-appveyor.yml
 buildout.cfg
 setup.cfg
 setup.py
 tox.ini
 include/ExtensionClass/ExtensionClass.h
 include/ExtensionClass/_compat.h
 include/persistent/_compat.h
```

### Comparing `Persistence-4.1/tox.ini` & `Persistence-5.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/c-code
 [tox]
 minversion = 4.0
 envlist =
     lint
-    py37,py37-pure
     py38,py38-pure
     py39,py39-pure
     py310,py310-pure
     py311,py311-pure
     py312,py312-pure
+    py313,py313-pure
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
+pip_pre = py313: true
 deps =
+    setuptools < 69
     wheel
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     PIP_NO_CACHE = 1
     py312: VIRTUALENV_PIP=23.1.2
     py312: PIP_REQUIRE_VIRTUALENV=0
@@ -38,29 +40,40 @@
 setenv =
     PURE_PYTHON=1
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage html -i
     coverage report -i -m --fail-under=97
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+deps =
+    isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
-deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
-    flake8
-    isort
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
```

