# Comparing `tmp/zodbpickle-3.3.tar.gz` & `tmp/zodbpickle-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodbpickle-3.3.tar", last modified: Tue Apr 16 06:21:42 2024, max compression
+gzip compressed data, was "zodbpickle-4.0.tar", last modified: Thu May 30 07:29:56 2024, max compression
```

## Comparing `zodbpickle-3.3.tar` & `zodbpickle-4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.430591 zodbpickle-3.3/
--rw-r--r--   0 m.howitz   (502) staff       (20)      584 2024-04-16 06:21:42.000000 zodbpickle-3.3/.coveragerc
--rwxr-xr-x   0 m.howitz   (502) staff       (20)     2255 2024-04-16 06:21:42.000000 zodbpickle-3.3/.manylinux-install.sh
--rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-04-16 06:21:42.000000 zodbpickle-3.3/.manylinux.sh
--rw-r--r--   0 m.howitz   (502) staff       (20)     5867 2024-04-16 06:21:42.000000 zodbpickle-3.3/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-04-16 06:21:42.000000 zodbpickle-3.3/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)     4824 2024-04-16 06:21:42.000000 zodbpickle-3.3/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      283 2024-04-16 06:21:42.000000 zodbpickle-3.3/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    13204 2024-04-16 06:21:42.430302 zodbpickle-3.3/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     5914 2024-04-16 06:21:42.000000 zodbpickle-3.3/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      196 2024-04-16 06:21:42.000000 zodbpickle-3.3/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.426366 zodbpickle-3.3/patches/
--rw-r--r--   0 m.howitz   (502) staff       (20)     4450 2024-04-16 06:21:42.000000 zodbpickle-3.3/patches/pickle_bytes_code.diff
--rw-r--r--   0 m.howitz   (502) staff       (20)     5287 2024-04-16 06:21:42.000000 zodbpickle-3.3/patches/pickle_bytes_tests.diff
--rw-r--r--   0 m.howitz   (502) staff       (20)      656 2024-04-16 06:21:42.430868 zodbpickle-3.3/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     3038 2024-04-16 06:21:42.000000 zodbpickle-3.3/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.423953 zodbpickle-3.3/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.427872 zodbpickle-3.3/src/zodbpickle/
--rw-r--r--   0 m.howitz   (502) staff       (20)       44 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)   205193 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/_pickle_33.c
--rw-r--r--   0 m.howitz   (502) staff       (20)      891 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/fastpickle.py
--rw-r--r--   0 m.howitz   (502) staff       (20)       24 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/pickle.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    52163 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/pickle_3.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    87531 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/pickletools_3.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1061 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/slowpickle.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.429800 zodbpickle-3.3/src/zodbpickle/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)      212 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5271 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/pickle_3_tests.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    68946 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/pickletester_3.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1363 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/test_compile_flags.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1161 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/test_pickle.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.430005 zodbpickle-3.3/src/zodbpickle.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    13204 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      826 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)       35 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)       11 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1614 2024-04-16 06:21:42.000000 zodbpickle-3.3/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:29:56.313264 zodbpickle-4.0/
+-rw-r--r--   0 jens       (501) staff       (20)      605 2024-05-30 06:57:39.000000 zodbpickle-4.0/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2189 2024-05-30 06:57:39.000000 zodbpickle-4.0/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2023-10-05 11:14:33.000000 zodbpickle-4.0/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)     5935 2024-05-30 06:59:04.000000 zodbpickle-4.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2023-10-05 11:14:33.000000 zodbpickle-4.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)     4824 2022-11-02 09:47:23.000000 zodbpickle-4.0/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      283 2024-05-24 14:23:32.000000 zodbpickle-4.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    13273 2024-05-30 07:29:56.313117 zodbpickle-4.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     5914 2022-11-02 09:47:23.000000 zodbpickle-4.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      196 2022-11-02 09:47:23.000000 zodbpickle-4.0/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:29:56.306463 zodbpickle-4.0/patches/
+-rw-r--r--   0 jens       (501) staff       (20)     4450 2022-11-02 09:47:23.000000 zodbpickle-4.0/patches/pickle_bytes_code.diff
+-rw-r--r--   0 jens       (501) staff       (20)     5287 2022-11-02 09:47:23.000000 zodbpickle-4.0/patches/pickle_bytes_tests.diff
+-rw-r--r--   0 jens       (501) staff       (20)      656 2024-05-30 07:29:56.313515 zodbpickle-4.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     3039 2024-05-30 06:59:36.000000 zodbpickle-4.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:29:56.304315 zodbpickle-4.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:29:56.309617 zodbpickle-4.0/src/zodbpickle/
+-rw-r--r--   0 jens       (501) staff       (20)       44 2023-01-03 12:38:38.000000 zodbpickle-4.0/src/zodbpickle/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)   205193 2024-05-24 14:23:32.000000 zodbpickle-4.0/src/zodbpickle/_pickle_33.c
+-rw-r--r--   0 jens       (501) staff       (20)      891 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/fastpickle.py
+-rw-r--r--   0 jens       (501) staff       (20)       24 2023-01-03 12:38:38.000000 zodbpickle-4.0/src/zodbpickle/pickle.py
+-rw-r--r--   0 jens       (501) staff       (20)    52163 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/pickle_3.py
+-rw-r--r--   0 jens       (501) staff       (20)    87531 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/pickletools_3.py
+-rw-r--r--   0 jens       (501) staff       (20)     1061 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/slowpickle.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:29:56.312626 zodbpickle-4.0/src/zodbpickle/tests/
+-rw-r--r--   0 jens       (501) staff       (20)      212 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     5271 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/tests/pickle_3_tests.py
+-rw-r--r--   0 jens       (501) staff       (20)    68946 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/tests/pickletester_3.py
+-rw-r--r--   0 jens       (501) staff       (20)     1363 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/tests/test_compile_flags.py
+-rw-r--r--   0 jens       (501) staff       (20)     1161 2023-04-20 08:27:27.000000 zodbpickle-4.0/src/zodbpickle/tests/test_pickle.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:29:56.312823 zodbpickle-4.0/src/zodbpickle.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    13273 2024-05-30 07:29:56.000000 zodbpickle-4.0/src/zodbpickle.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      826 2024-05-30 07:29:56.000000 zodbpickle-4.0/src/zodbpickle.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-30 07:29:56.000000 zodbpickle-4.0/src/zodbpickle.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-02 09:48:18.000000 zodbpickle-4.0/src/zodbpickle.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)       35 2024-05-30 07:29:56.000000 zodbpickle-4.0/src/zodbpickle.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)       11 2024-05-30 07:29:56.000000 zodbpickle-4.0/src/zodbpickle.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1615 2024-05-30 06:57:39.000000 zodbpickle-4.0/tox.ini
```

### Comparing `zodbpickle-3.3/.coveragerc` & `zodbpickle-4.0/.coveragerc`

 * *Files 14% similar despite different names*

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

### Comparing `zodbpickle-3.3/.manylinux-install.sh` & `zodbpickle-4.0/.manylinux-install.sh`

 * *Files 7% similar despite different names*

```diff
@@ -25,35 +25,33 @@
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
         *"cp313"*) echo 'py313';;
-        *"cp37"*) echo 'py37';;
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
-       [[ "${PYBIN}" == *"cp313"* ]] || \
-       [[ "${PYBIN}" == *"cp311"* ]] || \
-       [[ "${PYBIN}" == *"cp312"* ]] || \
-       [[ "${PYBIN}" == *"cp37"* ]] || \
-       [[ "${PYBIN}" == *"cp38"* ]] || \
-       [[ "${PYBIN}" == *"cp39"* ]] || \
-       [[ "${PYBIN}" == *"cp310"* ]] ; then
-        if [[ "${PYBIN}" == *"cp313"* ]] ; then
+       [[ "${PYBIN}" == *"cp313/"* ]] || \
+       [[ "${PYBIN}" == *"cp311/"* ]] || \
+       [[ "${PYBIN}" == *"cp312/"* ]] || \
+       [[ "${PYBIN}" == *"cp38/"* ]] || \
+       [[ "${PYBIN}" == *"cp39/"* ]] || \
+       [[ "${PYBIN}" == *"cp310/"* ]] ; then
+        if [[ "${PYBIN}" == *"cp313/"* ]] ; then
             "${PYBIN}/pip" install --pre -e /io/
             "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
         else
             "${PYBIN}/pip" install -e /io/
             "${PYBIN}/pip" wheel /io/ -w wheelhouse/
         fi
         if [ `uname -m` == 'aarch64' ]; then
```

### Comparing `zodbpickle-3.3/CHANGES.rst` & `zodbpickle-4.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ===========
  Changelog
 ===========
 
+4.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+
 3.3 (2024-04-16)
 ================
 
 - Build Windows wheels on GHA.
 
 - Add preliminary support for Python 3.13 as of 3.13a5.
```

### Comparing `zodbpickle-3.3/CONTRIBUTING.md` & `zodbpickle-4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/LICENSE.txt` & `zodbpickle-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/PKG-INFO` & `zodbpickle-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: zodbpickle
-Version: 3.3
+Version: 4.0
 Summary: Fork of Python 3 pickle module.
 Home-page: https://github.com/zopefoundation/zodbpickle
 Author: Python and Zope Foundation
 Author-email: zodb-dev@zope.dev
 License: PSFL 2 and ZPL 2.1
 Keywords: zodb pickle
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: License :: OSI Approved :: Python Software Foundation License
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
 Classifier: Framework :: ZODB
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: setuptools
 Provides-Extra: test
 Requires-Dist: zope.testrunner; extra == "test"
 
 ``zodbpickle`` README
 =====================
@@ -200,14 +200,20 @@
 This module provides a ``noload()`` method again.
 
 
 ===========
  Changelog
 ===========
 
+4.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+
 3.3 (2024-04-16)
 ================
 
 - Build Windows wheels on GHA.
 
 - Add preliminary support for Python 3.13 as of 3.13a5.
```

### Comparing `zodbpickle-3.3/README.rst` & `zodbpickle-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/patches/pickle_bytes_code.diff` & `zodbpickle-4.0/patches/pickle_bytes_code.diff`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/patches/pickle_bytes_tests.diff` & `zodbpickle-4.0/patches/pickle_bytes_tests.diff`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/setup.cfg` & `zodbpickle-4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/setup.py` & `zodbpickle-4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,48 +41,48 @@
 else:
     ext_modules = [Extension(name='zodbpickle._pickle',
                              sources=[EXT])]
 
 
 setup(
     name='zodbpickle',
-    version='3.3',
+    version='4.0',
     description='Fork of Python 3 pickle module.',
     author='Python and Zope Foundation',
     author_email='zodb-dev@zope.dev',
     url='https://github.com/zopefoundation/zodbpickle',
     license='PSFL 2 and ZPL 2.1',
     long_description=README,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Zope Public License',
         'License :: OSI Approved :: Python Software Foundation License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Framework :: ZODB',
         'Topic :: Database',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: Unix',
         'Operating System :: MacOS :: MacOS X',
     ],
     keywords='zodb pickle',
     platforms=['any'],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     ext_modules=ext_modules,
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     extras_require={
         'test': ['zope.testrunner'],
     },
     install_requires=[
         'setuptools',
     ],
     include_package_data=True,
```

### Comparing `zodbpickle-3.3/src/zodbpickle/_pickle_33.c` & `zodbpickle-4.0/src/zodbpickle/_pickle_33.c`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/fastpickle.py` & `zodbpickle-4.0/src/zodbpickle/fastpickle.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/pickle_3.py` & `zodbpickle-4.0/src/zodbpickle/pickle_3.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/pickletools_3.py` & `zodbpickle-4.0/src/zodbpickle/pickletools_3.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/slowpickle.py` & `zodbpickle-4.0/src/zodbpickle/slowpickle.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/tests/pickle_3_tests.py` & `zodbpickle-4.0/src/zodbpickle/tests/pickle_3_tests.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/tests/pickletester_3.py` & `zodbpickle-4.0/src/zodbpickle/tests/pickletester_3.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/tests/test_compile_flags.py` & `zodbpickle-4.0/src/zodbpickle/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle/tests/test_pickle.py` & `zodbpickle-4.0/src/zodbpickle/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/src/zodbpickle.egg-info/PKG-INFO` & `zodbpickle-4.0/src/zodbpickle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: zodbpickle
-Version: 3.3
+Version: 4.0
 Summary: Fork of Python 3 pickle module.
 Home-page: https://github.com/zopefoundation/zodbpickle
 Author: Python and Zope Foundation
 Author-email: zodb-dev@zope.dev
 License: PSFL 2 and ZPL 2.1
 Keywords: zodb pickle
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: License :: OSI Approved :: Python Software Foundation License
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
 Classifier: Framework :: ZODB
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: setuptools
 Provides-Extra: test
 Requires-Dist: zope.testrunner; extra == "test"
 
 ``zodbpickle`` README
 =====================
@@ -200,14 +200,20 @@
 This module provides a ``noload()`` method again.
 
 
 ===========
  Changelog
 ===========
 
+4.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+
 3.3 (2024-04-16)
 ================
 
 - Build Windows wheels on GHA.
 
 - Add preliminary support for Python 3.13 as of 3.13a5.
```

### Comparing `zodbpickle-3.3/src/zodbpickle.egg-info/SOURCES.txt` & `zodbpickle-4.0/src/zodbpickle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.3/tox.ini` & `zodbpickle-4.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
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
     py313,py313-pure
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
 pip_pre = py313: true
 deps =
+    setuptools < 69
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     py312: VIRTUALENV_PIP=23.1.2
     py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
```

