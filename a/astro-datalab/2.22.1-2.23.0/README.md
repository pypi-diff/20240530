# Comparing `tmp/astro-datalab-2.22.1.tar.gz` & `tmp/astro_datalab-2.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-datalab-2.22.1.tar", last modified: Mon Dec  4 21:40:44 2023, max compression
+gzip compressed data, was "astro_datalab-2.23.0.tar", last modified: Wed May 29 21:09:20 2024, max compression
```

## Comparing `astro-datalab-2.22.1.tar` & `astro_datalab-2.23.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:44.355257 astro-datalab-2.22.1/
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     1153 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/LICENSE
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     1274 2023-12-04 21:40:44.355109 astro-datalab-2.22.1/PKG-INFO
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     7088 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/README.md
-drwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:44.354590 astro-datalab-2.22.1/astro_datalab.egg-info/
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     1274 2023-12-04 21:40:44.000000 astro-datalab-2.22.1/astro_datalab.egg-info/PKG-INFO
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)      871 2023-12-04 21:40:44.000000 astro-datalab-2.22.1/astro_datalab.egg-info/SOURCES.txt
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)        1 2023-12-04 21:40:44.000000 astro-datalab-2.22.1/astro_datalab.egg-info/dependency_links.txt
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)       92 2023-12-04 21:40:44.000000 astro-datalab-2.22.1/astro_datalab.egg-info/requires.txt
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)        7 2023-12-04 21:40:44.000000 astro-datalab-2.22.1/astro_datalab.egg-info/top_level.txt
-drwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:44.345151 astro-datalab-2.22.1/dl/
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    17615 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/Util.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)       40 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/__init__.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)       23 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/__version__.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    34019 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/authClient.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    63909 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/dltasks.py
-drwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:44.347322 astro-datalab-2.22.1/dl/helpers/
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/helpers/__init__.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)      503 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/helpers/all.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     2625 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/helpers/cluster.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     4786 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/helpers/crossmatch.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    11808 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/helpers/legacy.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     3846 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/helpers/plot.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     8178 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/helpers/utils.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)   118203 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/queryClient.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    36893 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/resClient.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    84587 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/specClient.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    88985 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/dl/storeClient.py
-drwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:44.347921 astro-datalab-2.22.1/scripts/
--rwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)     7065 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/scripts/datalab
--rwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)     5508 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/scripts/mountvofs
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)      106 2023-12-04 21:40:44.355818 astro-datalab-2.22.1/setup.cfg
--rwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)     2319 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/setup.py
-drwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:44.348837 astro-datalab-2.22.1/tests/
--rwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)     4160 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/tests/test_datalab.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     6022 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/tests/test_helpers.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     2737 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/tests/test_util.py
-drwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)        0 2023-12-04 21:40:44.354067 astro-datalab-2.22.1/vos/
--rwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)   145204 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/BitVector.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     5505 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/CacheMetaData.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    58004 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/CadcCache.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     4385 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/NodeCache.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     3700 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/SharedLock.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)       49 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/__init__.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)       18 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/__version__.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     4450 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/cantop.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     2662 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/commonparser.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    27992 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/fuse.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    26162 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/html2text.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)      530 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/logExceptions.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)     2028 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/md5_cache.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)      352 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/utils.py
--rwxr-xr-x   0 igor.suarez-sola   (502) wheel        (0)    28522 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/vofs.py
--rw-r--r--   0 igor.suarez-sola   (502) wheel        (0)    94348 2023-12-04 21:40:33.000000 astro-datalab-2.22.1/vos/vos.py
+drwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)        0 2024-05-29 21:09:20.673583 astro_datalab-2.23.0/
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     1153 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/LICENSE
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     3224 2024-05-29 21:09:20.673464 astro_datalab-2.23.0/PKG-INFO
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     7727 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/README.md
+drwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)        0 2024-05-29 21:09:20.672753 astro_datalab-2.23.0/astro_datalab.egg-info/
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     3224 2024-05-29 21:09:20.000000 astro_datalab-2.23.0/astro_datalab.egg-info/PKG-INFO
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)      888 2024-05-29 21:09:20.000000 astro_datalab-2.23.0/astro_datalab.egg-info/SOURCES.txt
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)        1 2024-05-29 21:09:20.000000 astro_datalab-2.23.0/astro_datalab.egg-info/dependency_links.txt
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)      771 2024-05-29 21:09:20.000000 astro_datalab-2.23.0/astro_datalab.egg-info/requires.txt
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)        7 2024-05-29 21:09:20.000000 astro_datalab-2.23.0/astro_datalab.egg-info/top_level.txt
+drwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)        0 2024-05-29 21:09:20.662667 astro_datalab-2.23.0/dl/
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    17615 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/dl/Util.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)       40 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/__init__.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)       23 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/dl/__version__.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    34019 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/authClient.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    64368 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/dl/dltasks.py
+drwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)        0 2024-05-29 21:09:20.664950 astro_datalab-2.23.0/dl/helpers/
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)        0 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/helpers/__init__.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)      503 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/helpers/all.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     2625 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/helpers/cluster.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     4786 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/helpers/crossmatch.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    11808 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/helpers/legacy.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     3846 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/helpers/plot.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     8178 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/dl/helpers/utils.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)   126014 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/dl/queryClient.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    36893 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/dl/resClient.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    84587 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/dl/specClient.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    88985 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/dl/storeClient.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     1908 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/requirements.txt
+drwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)        0 2024-05-29 21:09:20.665687 astro_datalab-2.23.0/scripts/
+-rwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)     7065 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/scripts/datalab
+-rwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)     5508 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/scripts/mountvofs
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)      148 2024-05-29 21:09:20.673929 astro_datalab-2.23.0/setup.cfg
+-rwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)     1991 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/setup.py
+drwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)        0 2024-05-29 21:09:20.666559 astro_datalab-2.23.0/tests/
+-rwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)     4160 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/tests/test_datalab.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     6022 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/tests/test_helpers.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     2737 2024-05-29 21:07:34.000000 astro_datalab-2.23.0/tests/test_util.py
+drwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)        0 2024-05-29 21:09:20.672233 astro_datalab-2.23.0/vos/
+-rwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)   145204 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/BitVector.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     5505 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/CacheMetaData.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    58004 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/CadcCache.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     4385 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/NodeCache.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     3700 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/SharedLock.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)       49 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/__init__.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)       18 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/__version__.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     4450 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/cantop.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     2662 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/commonparser.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    27992 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/fuse.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    26162 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/html2text.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)      530 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/logExceptions.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)     2028 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/md5_cache.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)      352 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/utils.py
+-rwxr-xr-x   0 igor.suarez-sola   (502) staff       (20)    28522 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/vofs.py
+-rw-r--r--   0 igor.suarez-sola   (502) staff       (20)    94348 2022-12-20 18:04:48.000000 astro_datalab-2.23.0/vos/vos.py
```

### Comparing `astro-datalab-2.22.1/LICENSE` & `astro_datalab-2.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/README.md` & `astro_datalab-2.23.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,39 +33,57 @@
 The easiest way to install the ``datalab`` client is via pip:
 
 ```
 pip install --ignore-installed --no-cache-dir astro-datalab
 ```
 
 The flags `--ignore-installed` and `--no-cache-dir` should ensure that the latest version is pulled freshly from the internet.
-
 ### Install from sources
 
-You can also install the ``datalab`` client from source on
+You can also install the `datalab` client from source on 
 [GitHub](https://github.com/astro-datalab/datalab.git):
 
-```
-git clone https://github.com/astro-datalab/datalab.git
-cd datalab
-python setup.py install
-```
-
-If you want it installed in your private Python repository (because
-you maintain multiple Python instances on your machine) then do:
-
-```
-python setup.py install --user
-```
-
-Finally, if you intend to mount the virtual storage as a local
-filesystem, you will need to touch a file in your home directory:
+1. Clone the repository and enter the directory:
+   ```bash
+   git clone https://github.com/astro-datalab/datalab.git
+   cd datalab
+   ```
+
+2. Ensure you have the latest version of pip and setuptools:
+   ```bash
+   python -m pip install --upgrade pip setuptools
+   ```
+
+3. Build the package:
+   ```bash
+   python -m pip install build
+   python -m build
+   ```
+
+4. Install the package:
+   ```bash
+   pip install dist/astro_datalab-<version>-py3-none-any.whl
+   ```
+   Replace `<version>` with the actual version of the package.
+
+If you want it installed in your private Python repository (because you
+maintain multiple Python instances on your machine), you can use the
+`--user` flag:
+   ```bash
+   pip install --user dist/astro_datalab-<version>-py3-none-any.whl
+   ```
+
+Finally, if you intend to mount the virtual storage as a local filesystem,
+you will need to touch a file in your home directory:
+   ```bash
+   touch ~/.netrc
+   ```
 
-```
-touch ~/.netrc
-```
+Note: Replace `<version>` in the `pip install` command with the actual version
+number of the `astro_datalab` package, such as `2.23.0`.
 
 ## Configuration update: If you upgraded from a version prior to v2.20.0
 
 With version v2.20.0, the `datalab` package changed internal service
 URLs to point to our new noirlab.edu domain (the old noao.edu domain
 expired on Nov 29, 2021). If you had `datalab` installed previously,
 your local configuration file will still point to the old domain and
@@ -83,15 +101,14 @@
 Finally, log in again:
 
 ```
 datalab login
 ```
 
 and that should be it.
-</div>
 
 ## Documentation
 
 ### ``datalab`` command line client
 
 To check the currently installed version of `datalab`:
 
@@ -235,8 +252,8 @@
 ```
 
 or unmount the space when you log out of Data Lab:
 
 ```
 datalab logout --unmount=/tmp/vospace
 ```
--->
+-->
```

### Comparing `astro-datalab-2.22.1/astro_datalab.egg-info/SOURCES.txt` & `astro_datalab-2.23.0/astro_datalab.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+requirements.txt
 setup.cfg
 setup.py
 astro_datalab.egg-info/PKG-INFO
 astro_datalab.egg-info/SOURCES.txt
 astro_datalab.egg-info/dependency_links.txt
 astro_datalab.egg-info/requires.txt
 astro_datalab.egg-info/top_level.txt
```

### Comparing `astro-datalab-2.22.1/dl/Util.py` & `astro_datalab-2.23.0/dl/Util.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/authClient.py` & `astro_datalab-2.23.0/dl/authClient.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/dltasks.py` & `astro_datalab-2.23.0/dl/dltasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -814,14 +814,17 @@
                               required=False))
         self.addOption("profile",
             Option("profile", "", "Service profile to use",
                 required=False, default="default"))
         self.addOption("timeout",
             Option("timeout", "", "Requested query timeout",
                 required=False, default="120"))
+        self.addOption("stream",
+                       Option("stream", "", "stream results, requires output filename to be set.",
+                              required=False, default=False))
         self.addStdOptions()
 
     def run(self):
         token = getUserToken (self)
 
         # Get the query string to be used.  This can either be supplied
         # directly or by specifying a filename.
@@ -851,15 +854,16 @@
             if self.profile.value != "" and self.profile.value is not None:
                 queryClient.set_profile (profile=self.profile.value)
 
         # Workarounds for the "async" option to the query using getattr().
         try:
             res = queryClient.query (token, adql=adql, sql=sql,
                         fmt=self.fmt.value, out=self.out.value,
-                        async_=getattr(self,"async").value, drop=self.drop.value, timeout=self.timeout.value)
+                        async_=getattr(self,"async").value, drop=self.drop.value, timeout=self.timeout.value,
+                        stream=self.stream.value)
 
             if getattr(self,"async").value:
                 print (res)                         # Return the JobID
             elif self.out.value== '' or self.out.value is None:
                 print (res)                         # Return the results
         except Exception as e:
             if not getattr(self,"async").value and str(e) is not None:
@@ -891,19 +895,22 @@
     '''
         Get the async query results.
     '''
     def __init__(self, datalab):
         Task.__init__(self, datalab, 'qresults', 'Get the async query results')
         self.addOption("jobId", Option("jobId", "",
                         "Query Job ID", required=True))
+        self.addOption("fname", Option("fname", "",
+                                       "File name to save the results", required=False, default=None))
         self.addStdOptions()
 
     def run(self):
         token = getUserToken(self)
-        print (queryClient.results (token, jobId=self.jobId.value))
+        print (queryClient.results (token, jobId=self.jobId.value,
+                                    fname=self.fname.value))
 
 
 class QueryStatus(Task):
     '''
         Get the async query job status.
     '''
     def __init__(self, datalab):
```

### Comparing `astro-datalab-2.22.1/dl/helpers/cluster.py` & `astro_datalab-2.23.0/dl/helpers/cluster.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/helpers/crossmatch.py` & `astro_datalab-2.23.0/dl/helpers/crossmatch.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/helpers/legacy.py` & `astro_datalab-2.23.0/dl/helpers/legacy.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/helpers/plot.py` & `astro_datalab-2.23.0/dl/helpers/plot.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/helpers/utils.py` & `astro_datalab-2.23.0/dl/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/queryClient.py` & `astro_datalab-2.23.0/dl/queryClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,19 @@
                results  (token=None, jobId=None, delete=True, profile='default')
                  error  (token, jobId, profile='default')
                  error  (optval, jobId=None, profile='default')
                  error  (token=None, jobId=None, profile='default')
                  abort  (token, jobId, profile='default')
                  abort  (optval, jobId=None, profile='default')
                  abort  (token=None, jobId=None, profile='default')
-                  wait  (token, jobId, wait=3, verbose=False, 
+                  wait  (token, jobId, wait=3, verbose=False,
                          profile='default')
-                  wait  (optval, jobId=None, wait=3, verbose=False, 
+                  wait  (optval, jobId=None, wait=3, verbose=False,
                          profile='default')
-                  wait  (token=None, jobId=None, wait=3, verbose=False, 
+                  wait  (token=None, jobId=None, wait=3, verbose=False,
                          profile='default')
 
              mydb_list  (optval, table=None, **kw)
              mydb_list  (table=None, token=None, **kw)
            mydb_create  (token, table, schema, **kw)
            mydb_create  (table, schema, token=None, **kw)
            mydb_insert  (token, table, data, **kw)
@@ -90,15 +90,14 @@
 
 __authors__ = 'Mike Fitzpatrick <mike.fitzpatrick@noirlab.edu>, Matthew Graham <mjg@caltech.edu.edu>, Data Lab <datalab@noirlab.edu>'
 try:
     from querymanager.__version__ import __version__
 except ImportError as e:
     from dl.__version__ import __version__
 
-
 import requests
 try:
     from urllib import quote_plus               # Python 2
 except ImportError:
     from urllib.parse import quote_plus         # Python 3
 try:
     from cStringIO import StringIO
@@ -109,14 +108,16 @@
 import json
 import time
 import os
 import sys
 import collections
 import ast, csv
 import pandas
+import pycurl
+import certifi
 from tempfile import NamedTemporaryFile
 
 from dl import resClient
 from dl import storeClient
 from dl.helpers.utils import convert
 if os.path.isfile('./Util.py'):			# use local dev copy
     from Util import multimethod
@@ -172,31 +173,110 @@
 if os.path.exists('/tmp/SM_SVC_URL'):
     with open('/tmp/SM_SVC_URL') as fd:
         SM_SERVICE_URL = fd.read().strip()
 if os.path.exists('/tmp/RM_SVC_URL'):
     with open('/tmp/RM_SVC_URL') as fd:
         RM_SERVICE_URL = fd.read().strip()
 
-# Default sync query timeout default (300sec)
+# Default Sync query timeout default (300sec)
 DEF_TIMEOUT_REQUEST = 300
 
 
+#####################################################################
+# START - supporting functions for pycurl download code
+def human_readable_size(size, decimal_places=2):
+    """
+    Converts a size in bytes to a human-readable format (e.g., KB, MB, GB).
+
+    :param size: Size in bytes.
+    :param decimal_places: Number of decimal places to format.
+    :return: Human-readable size string.
+    """
+    for unit in ['B', 'KB', 'MB', 'GB', 'TB', 'PB']:
+        if size < 1024.0:
+            break
+        size /= 1024.0
+    return f"{size:.{decimal_places}f} {unit}"
+
+
+def human_readable_time(seconds, decimal_places=2):
+    """
+    Converts time in seconds to a human-readable format (hours:minutes:seconds).
+
+    :param seconds: Time in seconds.
+    :param decimal_places: Number of decimal places for the seconds part.
+    :return: Human-readable time string.
+    """
+    hours, remainder = divmod(seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    if hours > 0:
+        return f"{int(hours)}h:{int(minutes)}m:{seconds:.{decimal_places}f}s"
+    elif minutes > 0:
+        return f"{int(minutes)}m:{seconds:.{decimal_places}f}s"
+    else:
+        return f"{seconds:.{decimal_places}f}s"
+
+
+def progress_report(download_t, download_d, upload_t, upload_d):
+    """
+    Callback function to report the progress of a download or upload operation.
+
+    This function is designed to be used with pycurl to periodically report the
+    progress of file transfer operations. It prints updates to the console at
+    intervals specified by the `progress.report_interval`.
+
+    Parameters:
+    - download_t (int): Total size of the download in bytes.
+    - download_d (int): Number of bytes downloaded so far.
+    - upload_t (int): Total size of the upload in bytes (not used in this context).
+    - upload_d (int): Number of bytes uploaded so far (not used in this context).
+    """
+    now = time.time()  # Current time for calculating the interval and rate.
+    # Check if it's time to report progress (based on the specified interval).
+    if now - progress_report.last_report_time >= progress_report.report_interval:
+        elapsed_time = now - progress_report.start_time  # Total time elapsed since the start of the download.
+        # Calculate the download rate in kilobytes per second.
+        rate = download_d / elapsed_time / 1024
+        # Print the progress update, showing the amount downloaded, time elapsed, and current download rate.
+        print(
+            f"\rDownloaded {human_readable_size(download_d)} in"
+            f" {human_readable_time(elapsed_time)} at {rate:.2f} KB/s",
+            end="")
+        progress_report.last_report_time = now  # Update the last report time to the current time.
+
+
+def setup_progress():
+    """
+    Setup the progress reporting.
+    """
+    progress_report.start_time = time.time()
+    progress_report.last_report_time = progress_report.start_time
+    progress_report.report_interval = 5  # seconds between reports
+
+# END - Supporting functions for pycurl download code
+#####################################################################
 
 # ####################################################################
 #  Query Client error class
 # ####################################################################
 
 class queryClientError(Exception):
     def __init__(self, message):
         self.message = message
 
     def __str__(self):
         return self.message
 
 
+class DLHTTPException(Exception):
+    def __init__(self, status_code, message):
+        self.status_code = status_code
+        self.error_message = message
+        super().__init__(f"DL HTTP Error {status_code}: {message}")
+
 # ####################################################################
 #  Module Functions
 # ####################################################################
 
 # --------------------------------------------------------------------
 # ISALIVE -- Ping the Query Manager service to see if it responds.
 #
@@ -258,29 +338,29 @@
     MultiMethod Usage::
 
         queryClient.list_profiles (token)
         queryClient.list_profiles ()
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     profile : str
-        A specific profile configuration to list.  If None, a list of
+        A specific profile configuration to list. If ``None``, a list of
         profiles available to the given auth token is returned.
 
     format : str
-        Result format: One of 'text' or 'json'
+        Result format: One of 'text' or 'json'.
 
     Returns
     -------
-    profiles : list/dict
+    profiles : list or dict
         A list of the names of the supported profiles or a dictionary of
-        the specific profile
+        the specific profile.
 
     Example
     -------
     .. code-block:: python
 
         profiles = queryClient.list_profiles()
         profiles = queryClient.list_profiles(token)
@@ -305,86 +385,71 @@
 #
 @multimethod('qc',1,False)
 def schema(value, format='text', profile=None):
     return qc_client._schema (value=value, format=format, profile=profile)
 
 @multimethod('qc',0,False)
 def schema(value='', format='text', profile=None):
-    '''Return information about a data service schema.
+    '''[DEPRECATED] Return information about a data service schema.
 
     Usage::
 
         schema (value='', format='text', profile=None)
 
     Parameters
     ----------
     value : str
-        Schema object to return: Of the form <schema>[.<table>[.<column]]
+        Schema object to return: Of the form <schema>[.<table>[.<column]].
 
     profile : str
         The name of the service profile to use. The list of available
         profiles can be retrieved from the service (see function
-        :func:`queryClient.list_profiles()`)
+        :func:`queryClient.list_profiles()`).
 
     format : str
-        Result format:  One of 'text' or 'json'  (NOT CURRENTLY USED)
+        Result format:  One of 'text' or 'json'  (NOT CURRENTLY USED).
 
     Returns
     -------
     Anything?
 
-    Example
-    -------
-    .. code-block:: python
-
-        # List the available schema
-        queryClient.schema("", "text", "default")
-
-        # List the tables in the USNO schema
-        queryClient.schema("usno", "text", "default")
-
-        # List the columns of the USNO-A2 table
-        queryClient.schema("usno.a2", "text", "default")
-
-        # List the attributes of the USNO-A2 'raj2000' column
-        queryClient.schema("usno.a2.raj2000", "text", "default")
     '''
     return qc_client._schema (value=value, format=format, profile=profile)
 
 # --------------------------------------------------------------------
 # SERVICES -- List public storage services
 #
 def services(name=None, svc_type=None, mode='list', profile='default'):
     '''Search or list available data services.
 
-    Usage:
+    Usage::
         services (name=None, svc_type=None, mode='list', profile='default')
 
     Parameters
     ----------
     name : str
-        Schema object to return: Of the form <schema>[.<table>[.<column]]
+        Schema object to return: Of the form <schema>[.<table>[.<column]].
 
     svc_type : str
-        Limit results to specified service type.  Supported options are
-	'tap', 'sia', 'scs', or 'vos'.
+        Limit results to specified service type. Supported options are
+        'tap', 'sia', 'scs', or 'vos'.
 
     mode : str
-	Query mode:
+        Print output as either 'list' or 'resolve'.
 
     profile : str
         The name of the service profile to use. The list of available
         profiles can be retrieved from the service (see function
-        :func:`queryClient.list_profiles()`)
+        :func:`queryClient.list_profiles()`).
 
     Returns
     -------
-	If mode is 'list' then a human-readable list of matching services is
-	returned.  If mode is 'resolve' then a JSON string of matching services
-	is returned un the form "{<svc_name> : <svc_url>, ....}"
+    If mode is 'list' then a human-readable list of matching services is
+    returned.  If mode is 'resolve' then a JSON string of matching services
+    is returned un the form "{<svc_name> : <svc_url>, ....}".
 
     Example
     -------
     .. code-block:: python
 
         # List the available SIA services
         queryClient.services(svc_type="sia")
@@ -440,50 +505,49 @@
     MultiMethod Usage::
 
         queryClient.query (token, query, <args>)
         queryClient.query (token | query, <args>)
 
     Parameters
     ----------
-    token : str
-        Secure token obtained via :func:`authClient.login()`
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     adql : str or None
         ADQL query string that will be passed to the DB query manager, e.g.
 
         .. code-block:: python
 
-            adql='select top 3 ra,dec from gaia_dr1.gaia_source'
+            adql='select top 3 ra,dec from gaia_dr3.gaia_source'
 
     sql : str or None
         SQL query string that will be passed to the DB query manager, e.g.
 
         .. code-block:: python
 
-            sql='select ra,dec from gaia_dr1.gaia_source limit 3'
+            sql='select ra,dec from gaia_dr3.gaia_source limit 3'
 
     fmt : str
         Format of result to be returned by the query. Permitted values are:
 
           * 'csv'          The returned result is a comma-separated string
                            that looks like a csv file (newlines at the end
-                           of every row) [DEFAULT]
-          * 'csv-noheader' A csv result with no column headers (data only)
-          * 'ascii'        Same, but the column separator is a tab \t
-          * 'array'        Returns a NumPy array
-          * 'pandas'       Returns a Pandas DataFrame
-          * 'structarray'  Numpy structured array (aka 'record array')
-          * 'table'        Returns an Astropy Table object
+                           of every row) [DEFAULT].
+          * 'csv-noheader' A csv result with no column headers (data only).
+          * 'ascii'        Same, but the column separator is a tab \t.
+          * 'array'        Returns a NumPy array.
+          * 'pandas'       Returns a Pandas DataFrame.
+          * 'structarray'  Numpy structured array (aka 'record array').
+          * 'table'        Returns an Astropy Table object.
 
             The following formats may be used when saving a file to
             virtual storage on the server:
 
-          * 'fits'         FITS binary
-          * 'hdf5'         HDF5 file                (NOT YET IMPLEMENTED)
-          * 'votable'      An XML-formatted VOTable
+          * 'fits'         FITS binary.
+          * 'votable'      An XML-formatted VOTable.
 
     out : str or None
         The output filename to create on the local machine, the URI of a
         VOSpace or MyDB resource to create, or ``None`` if the result is
         to be returned directly to the caller.
 
     async_ : bool
@@ -495,76 +559,74 @@
         runs a Synchroneous query.
 
         ``async_`` replaces the previous ``async`` parameter, because ``async``
         was promoted to a keyword in Python 3.7. Users of Python versions
         prior to 3.7 can continue to use the ``async`` keyword.
 
     drop : bool
-        If ``True``, then if the query is saving to mydb where the same table
-        name already exists, it will overwrite the old mydb table.
+        If ``True``, then if the query is saving to MyDB where the same table
+        name already exists, it will overwrite the old MyDB table.
 
     profile : str or None
-        The Query Manager profile to use for this call.  If ``None`` then
-        the default profile is used.  Available profiles may be listed
-        using the :func:`queryClient.list_profiles()`
+        The Query Manager profile to use for this call. If ``None`` then
+        the default profile is used. Available profiles may be listed
+        using the :func:`queryClient.list_profiles()`.
 
     **kw : dict
-        Optional keyword arguments.  Supported keywords currently include:
+        Optional keyword arguments. Supported keywords currently include:
 
            wait = False
-               Wait for asynchronous queries to complete? If enabled,
-               the query() method will submit the job in async mode
+               Wait for Asynchronous queries to complete? If enabled,
+               the query() method will submit the job in Async mode
                and then poll for results internally before returning.
-               the default is to return the job ID immediately and let
+               The default is to return the job ID immediately and let
                the client poll for job status and return results.
 
            timeout = 300
                Requested timeout (in seconds) for a query. For a Sync
                query, this value sets a session timeout request in the
                database that will abort the query at the specified time.
                A maximum value of 600 seconds is permitted.  If the
-               ``wait`` option is enabled for an ASync query, this is the
+               ``wait`` option is enabled for an Async query, this is the
                maximum time the query will be allowed to run before an
                abort() is issued on the job.  The maximum timeout for
-               an ASync job is 24-hrs (86400 sec).
+               an Async job is 24-hrs (86400 sec).
 
            poll = 1
-               ASync job polling time in seconds.
+               Async job polling time in seconds.
 
            verbose = False
-               Print verbose messages during ASync job.
+               Print verbose messages during Async job.
 
     Returns
     -------
     result : str
-        If ``async=False``, the return value is the result of the
+        If ``async_=False``, the return value is the result of the
         query as a formatted string (see ``fmt``). Otherwise the
         result string is a job token, with which later the
-        Asynchroneaous query's status can be checked
+        Asynchronous query's status can be checked
         (:func:`queryClient.status()`), and the result retrieved (see
-        :func:`queryClient.result()`.
+        :func:`queryClient.result()`).
 
     Example
     -------
-    Get security token first, see :func:`authClient.login()`. Then:
-
     .. code-block:: python
 
-        query = 'select ra,dec from gaia_dr1.gaia_source limit 3'
-        response = queryClient.query(token, adql=query, fmt='csv')
-        print response
+        query = 'select ra,dec from gaia_dr3.gaia_source limit 3'
+        response = queryClient.query(adql=query, fmt='csv')
+        print (response)
 
     This prints
 
     .. code::
 
           ra,dec
-          315.002571989537842,35.2662974820284489
-          315.00408275885701,35.2665448169895797
-          314.996334457679438,35.2673478725552698
+          314.14738713961134,37.33643208345386
+          314.1588238386895,37.33682543157976
+          314.1519366421579,37.33533842266872
     '''
     return qc_client._query (token=def_token(token), adql=adql, sql=sql,
                              fmt=fmt, out=out, async_=async_, drop=drop,
                              profile=profile,
                              **kw)
 
 
@@ -586,73 +648,71 @@
     else:
         # optval is probably a jobId
         return qc_client._status (token=def_token(None), jobId=optval,
                                   profile=profile)
 
 @multimethod('qc',0,False)
 def status(token=None, jobId=None, profile='default'):
-    '''Get the status of an asynchronous query.
+    '''Get the status of an Asynchronous query.
 
     Usage::
 
         status (token=None, jobId=None)
 
     MultiMethod Usage::
 
         queryClient.status (jobId)
         queryClient.status (token, jobId)
         queryClient.status (token, jobId=<id>)
         queryClient.status (jobId=<str>)
 
     Use the authentication token and the jobId of a previously issued
-    asynchronous query to check the query's current status.
+    Asynchronous query to check the query's current status.
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     jobId : str
-        The jobId returned when issuing an asynchronous query via
-        :func:`queryClient.query()` with ``async=True``.
+        The jobId returned when issuing an Asynchronous query via
+        :func:`queryClient.query()` with ``async_=True``.
 
     Returns
     -------
     status : str
-
-        Either 'QUEUED' or 'EXECUTING' or 'COMPLETED'. If the token &
+        Either ``QUEUED`` or ``EXECUTING`` or ``COMPLETED``. If the token &
         jobId combination does not correspond to an actual job, then a
         HTML-formatted error message is returned. If there is a
-        problem with the backend, the returned value can be 'ERROR'.
+        problem with the backend, the returned value can be ``ERROR``.
 
-        When status is 'COMPLETED', you can retrieve the results of
-        the query via :func:`queryClient.results()`
+        When status is ``COMPLETED``, you can retrieve the results of
+        the query via :func:`queryClient.results()`.
 
     Example
     -------
     .. code-block:: python
 
         import time
-        query = 'select ra,dec from gaia_dr1.gaia_source limit 200000'
-        jobId = queryClient.query(token, adql=query, fmt='csv', async=True)
+        query = 'select ra,dec from gaia_dr3.gaia_source limit 200000'
+        jobId = queryClient.query(adql=query, fmt='csv', async_=True)
         while True:
-            status = queryClient.status(token, jobId)
-            print "time index =", time.localtime()[5], "   status =", status
+            status = queryClient.status(jobId)
+            print ("time index =", time.localtime()[5], "   status =", status)
             if status == 'COMPLETED':
                 break
             time.sleep(1)
 
     This prints
 
     .. code::
 
         time index = 16    status = EXECUTING
         time index = 17    status = EXECUTING
         time index = 18    status = COMPLETED
-
     '''
     return qc_client._status (token=def_token(token), jobId=jobId,
                               profile=profile)
 
 
 # --------------------------------------------------------------------
 # JOBS -- Get a list of the user's Async jobs.
@@ -685,148 +745,151 @@
 
         queryClient.jobs (jobId)
         queryClient.jobs (token, jobId)
         queryClient.jobs (token, jobId=<id>)
         queryClient.jobs (jobId=<str>)
 
     Use the authentication token and the jobId of a previously issued
-    asynchronous query to check the query's current status.
+    Asynchronous query to check the query's current status.
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     jobId : str
-        The jobId returned when issuing an asynchronous query via
-        :func:`queryClient.query()` with ``async=True``.
+        The jobId returned when issuing an Asynchronous query via
+        :func:`queryClient.query()` with ``async_=True``.
 
     format : str
         Format of the result.  Support values include 'text' for a simple
         formatted table suitable for printing, or 'json' for a JSON
         string of the full matching record(s).
 
     status : str
-        If status='all' then all async jobs are returned, otherwise this
+        If ``status='all'`` then all Async jobs are returned, otherwise this
         value may be used to return only those jobs with the specified
         status.  Allowed values are:
 
-                all             Return all jobs
-                EXECUTING       Job is still running
-                COMPLETED       Job completed successfully
-                ERROR           Job exited with an error
-                ABORTED         Job was aborted by the user
+          * 'all'       Return all jobs.
+          * 'EXECUTING' Job is still running.
+          * 'COMPLETED' Job completed successfully.
+          * 'ERROR'     Job exited with an error.
+          * 'ABORTED'   Job was aborted by the user.
 
     option : str
-	If 'list' then the matching records are returned, if 'delete' then
+        If ``list`` then the matching records are returned, if ``delete`` then
         the records are removed from the database (e.g. to clear up long
         job lists of completed jobs).
 
     Returns
     -------
     joblist : str
-        Returns a list of async query jobs submitted by the user in the
-        last 30 days, possibly filtered by the 'status' parameter.  The
+        Returns a list of Async query jobs submitted by the user in the
+        last 30 days, possibly filtered by the ``status`` parameter. The
         'json' format option allows the caller to format the full contents
         of the job record beyond the supplied simple 'text' option.
 
     Example
     -------
     .. code-block:: python
 
-        print (queryClient.jobs(token, jobId))
+        print (queryClient.jobs(jobId))
 
     This prints
 
     .. code::
 
         JobID              Start              End                 Status
         tfu8zpn2tkrlfyr9e  07-22-20T13:10:22  07-22-20T13:34:12   COMPLETED
         k8uznptrkkl29ryef  07-22-20T14:09:45                      EXECUTING
               :                   :                 :                :
-
     '''
     return qc_client._jobs (token=def_token(token), jobId=jobId,
                             format=format, status=status, option=option)
 
 
 # --------------------------------------------------------------------
 # RESULTS -- Get the results of an Asynchronous query
 #
 @multimethod('qc',2,False)
-def results(token, jobId, fname=None, delete=True, profile='default'):
-    return qc_client._results (token=def_token(token), jobId=jobId, 
-                               fname=fname, delete=True, profile=profile)
+def results(token, jobId, fname=None, delete=True, profile='default', progress=False):
+    return qc_client._results (token=def_token(token), jobId=jobId,
+                               fname=fname, delete=True, profile=profile, progress=progress)
 
 @multimethod('qc',1,False)
-def results(optval, jobId=None, fname=None, delete=True, profile='default'):
+def results(optval, jobId=None, fname=None, delete=True, profile='default', progress=False):
     if optval is not None and is_auth_token(optval):
         # optval looks like a token
         return qc_client._results (token=def_token(optval), jobId=jobId,
-                                   fname=fname, delete=delete, profile=profile)
+                                   fname=fname, delete=delete, profile=profile, progress=progress)
     else:
         # optval is probably a jobId
         return qc_client._results (token=def_token(None), jobId=optval,
-                                   fname=fname, delete=delete, profile=profile)
+                                   fname=fname, delete=delete, profile=profile, progress=progress)
 
 @multimethod('qc',0,False)
-def results(token=None, jobId=None, fname=None, delete=True, profile='default'):
-    '''Retrieve the results of an asynchronous query, once completed.
+def results(token=None, jobId=None, fname=None, delete=True, profile='default', progress=False):
+    '''Retrieve the results of an Asynchronous query, once completed.
 
     Usage::
 
         results (token=None, jobId=None, delete=True)
 
     MultiMethod Usage::
 
         queryClient.results (jobId)
         queryClient.results (token, jobId)
         queryClient.results (token, jobId=<id>)
         queryClient.results (jobId=<str>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     jobId : str
-        The jobId returned when issuing an asynchronous query via
-        :func:`queryClient.query()` with ``async=True``.
+        The jobId returned when issuing an Asynchronous query via
+        :func:`queryClient.query()` with ``async_=True``.
+
+    progress: bool
+        Set to ``False`` by default. If progress set to ``True`` it will
+        report the download progress.
 
     Returns
     -------
     results : str
 
     Example
     -------
     .. code-block:: python
 
-        # issue an async query (here a tiny one just for this example)
-        query = 'select ra,dec from gaia_dr1.gaia_source limit 3'
-        jobId = queryClient.query(token, adql=query, fmt='csv', async=True)
+        # issue an Async query (here a tiny one just for this example)
+        query = 'select ra,dec from gaia_dr3.gaia_source limit 3'
+        jobId = queryClient.query(adql=query, fmt='csv', async_=True)
 
         # ensure job completes...then check status and retrieve results
         time.sleep(4)
-        if queryClient.status(token, jobId) == 'COMPLETED':
-            results = queryClient.results(token,jobId)
-            print type(results)
-            print results
+        if queryClient.status(jobId) == 'COMPLETED':
+            results = queryClient.results(jobId)
+            print (type(results))
+            print (results)
 
     This prints
 
     .. code::
 
         <type 'str'>
         ra,dec
-        301.37502633933002,44.4946851014515588
-        301.371102372343785,44.4953207577355698
-        301.385106974224186,44.4963443903961604
+        314.14738713961134,37.33643208345386
+        314.1588238386895,37.33682543157976
+        314.1519366421579,37.33533842266872
     '''
-    return qc_client._results (token=def_token(token), jobId=jobId, 
-                               fname=fname, delete=True, profile=profile)
+    return qc_client._results (token=def_token(token), jobId=jobId,
+                               fname=fname, delete=True, profile=profile, progress=progress)
 
 
 # --------------------------------------------------------------------
 # ERROR -- Get the error message of a failed Asynchronous query
 #
 @multimethod('qc',2,False)
 def error(token, jobId, profile='default'):
@@ -842,64 +905,61 @@
     else:
         # optval is probably a jobId
         return qc_client._error (token=def_token(None), jobId=optval,
                                  profile=profile)
 
 @multimethod('qc',0,False)
 def error(token=None, jobId=None, profile='default'):
-    '''Retrieve the error of an asynchronous query, once completed.
+    '''Retrieve the error of an Asynchronous query, once completed.
 
     Usage::
 
         error (token=None, jobId=None)
 
     MultiMethod Usage::
 
         queryClient.error (jobId)
         queryClient.error (token, jobId)
         queryClient.error (token, jobId=<id>)
         queryClient.error (jobId=<str>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     jobId : str
-        The jobId returned when issuing an asynchronous query via
-        :func:`queryClient.query()` with ``async=True``.
+        The jobId returned when issuing an Asynchronous query via
+        :func:`queryClient.query()` with ``async_=True``.
 
     Returns
     -------
     error : str
 
     Example
     -------
     .. code-block:: python
 
-        # issue an async query (here a tiny one just for this example)
-        query = 'select ra,dec from gaia_dr1.gaia_source limit 3'
-        jobId = queryClient.query(token, adql=query, fmt='csv', async=True)
+        # issue an Async query (here a tiny one just for this example)
+        query = 'select ra,dec1 from gaia_dr3.gaia_source limit 3'
+        jobId = queryClient.query(adql=query, fmt='csv', async_=True)
 
         # ensure job completes...then check status and retrieve error
         time.sleep(4)
-        if queryClient.status(token, jobId) == 'ERROR':
-            error = queryClient.error(token,jobId)
-            print type(error)
-            print error
+        if queryClient.status(jobId) == 'ERROR':
+            error = queryClient.error(jobId)
+            print (type(error))
+            print (error)
 
     This prints
 
     .. code::
 
-        <type 'str'>
-        ra,dec
-        301.37502633933002,44.4946851014515588
-        301.371102372343785,44.4953207577355698
-        301.385106974224186,44.4963443903961604
+        <class 'str'>
+        Error: IllegalArgumentException: Column [dec1] does not exist.
     '''
     return qc_client._error (token=def_token(token), jobId=jobId,
                              profile=profile)
 
 
 # --------------------------------------------------------------------
 # ABORT -- Abort the specified Asynchronous job.
@@ -918,108 +978,110 @@
     else:
         # optval is probably a jobId
         return qc_client._abort (token=def_token(None), jobId=optval,
                                  profile=profile)
 
 @multimethod('qc',0,False)
 def abort(token=None, jobId=None, profile='default'):
-    '''Abort the specified asynchronous job.
+    '''Abort the specified Asynchronous job.
 
     Usage::
 
         abort (token=None, jobId=None)
 
     MultiMethod Usage::
 
         queryClient.abort (token, jobId)
         queryClient.abort (jobId)
         queryClient.abort (token, jobId=<id>)
         queryClient.abort (jobId=<str>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     jobId : str
         The jobId to abort.
 
     Returns
     -------
     results : str
 
     Example
     -------
     .. code-block:: python
 
-        # issue an async query (here a tiny one just for this example)
-        query = 'select ra,dec from gaia_dr1.gaia_source limit 3'
-        jobId = queryClient.query(token, adql=query, fmt='csv', async=True)
+        # issue an Async query (here a tiny one just for this example)
+        query = 'select ra,dec from gaia_dr3.gaia_source limit 3'
+        jobId = queryClient.query(adql=query, fmt='csv', async_=True)
 
         # ensure job completes...then check status and retrieve results
         time.sleep(4)
-        if queryClient.status(token, jobId) == 'COMPLETED':
-            results = queryClient.results(token,jobId)
-            print type(results)
-            print results
+        if queryClient.status(jobId) == 'COMPLETED':
+            results = queryClient.results(jobId)
+            print (type(results))
+            print (results)
 
     This prints
 
     .. code::
 
-        <type 'str'>
+        <class 'str'>
         ra,dec
-        301.37502633933002,44.4946851014515588
-        301.371102372343785,44.4953207577355698
-        301.385106974224186,44.4963443903961604
+        314.14738713961134,37.33643208345386
+        314.1588238386895,37.33682543157976
+        314.1519366421579,37.33533842266872
     '''
     return qc_client._abort (token=def_token(token), jobId=jobId,
                              profile=profile)
 
 
     # --------------------------
     # --------------------------
 
 # --------------------------------------------------------------------
-# WAIT -- Wait for completion of asynchronous job.
+# WAIT -- Wait for completion of Asynchronous job.
 #
 @multimethod('qc',2,False)
 def wait(token, jobId, wait=3, verbose=False, profile='default'):
-    '''Usage:  queryClient.wait (token, jobID)
+    '''Usage::  queryClient.wait (token, jobID)
     '''
     return qc_client._wait (token=def_token(token), jobId=jobId, wait=wait,
                             verbose=verbose, profile=profile)
 
 @multimethod('qc',1,False)
 def wait(optval, jobId=None, wait=3, verbose=False, profile='default'):
-    '''Usage:  queryClient.wait (jobID)
+    '''Usage::  queryClient.wait (jobID)
                queryClient.wait (token, jobId=<id>)
     '''
     if optval is not None and is_auth_token(optval):
         # optval looks like a token
         return qc_client._wait (token=def_token(optval), jobId=jobId, wait=wait,
                                 verbose=verbose, profile=profile)
     else:
         # optval is probably a jobId
         return qc_client._wait (token=def_token(None), jobId=optval, wait=wait,
                                 verbose=verbose, profile=profile)
 
 @multimethod('qc',0,False)
 def wait(token=None, jobId=None, wait=3, verbose=False, profile='default'):
-    '''Usage:  queryClient.wait (jobID=<str>)
-    '''
-    '''Loop until an async job has completed.
+    '''Loop until an Async job has completed.
+
+    Usage::
+
+        queryClient.wait (jobID=<str>)
 
     Parameters
     ----------
-    jobid : str
+    jobId : str
         The job ID string of a submitted query job.
 
-    wait : int | float
-        Wait for `wait` seconds before checking status again. Default: 3sec
+    wait : int or float
+        Wait for ``wait`` seconds before checking status again. Default: 3sec.
     '''
     return qc_client._wait (token=def_token(token), jobId=jobId, wait=wait,
                             verbose=verbose, profile=profile)
 
 
 
 # -----------------------------
@@ -1055,26 +1117,26 @@
         queryClient.list (token, table)
         queryClient.list (table)
         queryClient.list (token, table=<id>)
         queryClient.list ()
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    table: str
+    table : str
         The specific table to list (returns the table schema), or
         an empty string to return a list of the names of all tables.
 
     Returns
     -------
     listing : str
         The list of tables in the user's MyDB or the schema of the
-        named table
+        named table.
 
     Example
     -------
     .. code-block:: python
 
         # List the tables
         queryClient.list()
@@ -1096,44 +1158,37 @@
         return qc_client.mydb_drop (token=def_token(optval), table=table)
     else:
         # optval is likely a table
         return qc_client.mydb_drop (token=def_token(None), table=optval)
 
 @multimethod('qc',0,False)
 def drop(table=None, token=None):
-    '''Drop the specified table from the user's MyDB
+    '''[DEPRECATED] Drop the specified table from the user's MyDB.
 
     Usage::
 
         drop (table=None, token=None)
 
     MultiMethod Usage::
 
         queryClient.drop (token, table)
         queryClient.drop (table)
         queryClient.drop (token, table=<id>)
         queryClient.drop (table=<str>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    table: str
-        The specific table to drop
+    table : str
+        The specific table to drop.
 
     Returns
     -------
-
-    Example
-    -------
-    .. code-block:: python
-
-        # List the tables
-        queryClient.drop('foo1')
     '''
     return qc_client.mydb_drop (token=def_token(token), table=table)
 
 
 
 # -----------------------------
 #  MyDB Functions (New API)
@@ -1165,26 +1220,26 @@
 
         queryClient.mydb_list (table)
         queryClient.mydb_list (token, table=<str>)
         queryClient.mydb_list (table=<str>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     table: str
         The specific table to list (returns the table schema), or
         an empty string to return a list of the names of all tables.
 
     Returns
     -------
     listing : str
         The list of tables in the user's MyDB or the schema of the
-        named table
+        named table.
 
     Example
     -------
     .. code-block:: python
 
         # List the tables
         queryClient.mydb_list()
@@ -1200,41 +1255,41 @@
 @multimethod('qc',3,False)
 def mydb_create(token, table, schema, **kw):
     return qc_client._mydb_create (token=def_token(None), table=table,
                               schema=schema, **kw)
 
 @multimethod('qc',2,False)
 def mydb_create(table, schema, token=None, **kw):
-    '''Create a table in the user's MyDB
+    '''Create a table in the user's MyDB.
 
     Usage::
 
         mydb_create (table, schema, token=None, **kw)
 
     MultiMethod Usage::
 
         queryClient.mydb_create (token, table, <schema_dict>)
         queryClient.mydb_create (table, <schema_dict>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     table: str
-        The name of the table to create
+        The name of the table to create.
 
     schema: str or dict
         The schema is CSV text containing the name of the column and
         it's PostgreSQL data type.  If set as a 'str' type it is either
-        a CSV string, or the name of a file containing the CSV.  If passed
+        a CSV string, or the name of a file containing the CSV. If passed
         as a 'dict' type, it is a dictionary object where keys are the
         column names and values are the data types.
 
-    drop: bool   (optional)
+    drop: bool [Optional]
         Drop any existing table of the same name before creating new one.
 
     Returns
     -------
 
     Example
     -------
@@ -1259,55 +1314,56 @@
 @multimethod('qc',3,False)
 def mydb_insert(token, table, data, **kw):
     return qc_client._mydb_insert (token=def_token(token), table=table,
                                    data=data, **kw)
 
 @multimethod('qc',2,False)
 def mydb_insert(table, data, token=None, **kw):
-    '''Insert data into a table in the user's MyDB
+    '''Insert data into a table in the user's MyDB.
 
     Usage::
 
         mydb_insert (table, data, token=None, **kw)
 
     MultiMethod Usage::
 
         queryClient.mydb_insert (token, table, <filename>)
         queryClient.mydb_insert (token, table, <data_object>)
         queryClient.mydb_insert (table, <filename>)
         queryClient.mydb_insert (table, <data_object>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
     table: str
-        The name of the table to append
+        The name of the table to append.
 
     data: str or data object
         The schema is CSV text containing the name of the column and
-        it's PostgreSQL data type.  If set as a 'str' type it is either
+        it's PostgreSQL data type. If set as a 'str' type it is either
         a CSV string, or the name of a file containing the CSV data. If
         passed as a tabular data object, it is converted to CSV and sent
         to the service.
 
-    csv_header: bool        [OPTIONAL]
+    csv_header: bool [Optional]
         If True, then the CSV data object contains a CSV header line, i.e.
-        the first line is a row of column names.  Otherwise, no column
+        the first line is a row of column names. Otherwise, no column
         names are assumed and the column order must match the table schema.
 
     Returns
     -------
 
     Example
     -------
     .. code-block:: python
 
-        # Insert data into a MyDB table named 'foo'.
+        # Insert data from a CSV file called 'data.csv' into a MyDB table
+        # named 'foo'.
         queryClient.mydb_insert ('foo', 'data.csv')
     '''
     return qc_client._mydb_insert (token=def_token(token), table=table,
                                    data=data, **kw)
 
 
 # --------------------------------------------------------------------
@@ -1321,62 +1377,64 @@
     except Exception as e:
         return (str(e))
 
     return result
 
 @multimethod('qc',2,False)
 def mydb_import(table, data, token=None, **kw):
-    '''Import data into a table in the user's MyDB
+    '''Import data into a table in the user's MyDB.
 
     Usage::
 
         mydb_import (table, data, token=None, **kw)
 
     MultiMethod Usage::
 
         queryClient.mydb_import (token, table, data)
         queryClient.mydb_import (table, data)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    table: str
-        The name of the table to be loaded
-
-    data: str or data object
-        The data file or python object to be loaded.  The 'data' value
-        may be one of the following types::
+    table : str
+        The name of the table to be loaded.
 
-            filename	    A CSV file of data
-            string		    A string containing CSV data
-            Pandas DataFrame    A Pandas DataFrame object
-                :                   :        :       :
+    data : str or data object
+        The data file or python object to be loaded. The ``data`` value
+        may be one of the following types:
+
+          * filename -- A CSV file of data.
+          * string -- A string containing CSV data.
+          * Pandas DataFrame -- A Pandas DataFrame object.
 
         Additional object types can be added provided the data can be
         converted to a CSV format.
 
-    schema: str	[OPTIONAL]
+    schema : str [Optional]
         If set, this is a filename or string containing a schema for the
-        data table to be created.  A schema contains a comma-delimited row
+        data table to be created. A schema contains a comma-delimited row
         for each column containing the column name and it's Postgres data
-        type.  If not set, the schema is determined automatically from
+        type. If not set, the schema is determined automatically from
         the data.
 
-    append: bool   	[Optional]
-        append any existing table of the same name.
+    append : bool [Optional]
+        Append any existing table of the same name.
 
-    verbose: bool       [Optional]
+    verbose : bool [Optional]
         Be verbose about operations.
 
     Returns
     -------
-        schema	A string containing the table schema
-        data_obj	The CSV data to be imported (possibly converted)
+    schema : str
+        A string containing the table schema.
+
+    data_obj : str or data object
+        The CSV data to be imported (possibly converted).
 
     Example
     -------
     .. code-block:: python
 
         # Import data into a MyDB table named 'foo' from file 'data.csv'.
         schema, data = queryClient.mydb_import ('foo', 'data.csv')
@@ -1395,43 +1453,43 @@
 #
 @multimethod('qc',2,False)
 def mydb_truncate(token, table):
     return qc_client._mydb_truncate (token=def_token(token), table=table)
 
 @multimethod('qc',1,False)
 def mydb_truncate(table, token=None):
-    '''Truncate the specified table in the user's MyDB
+    '''Truncate the specified table in the user's MyDB.
 
     Usage::
 
         mydb_truncate (table, token=None)
 
     MultiMethod Usage::
 
         queryClient.mydb_truncate (token, table)
         queryClient.mydb_truncate (table)
         queryClient.mydb_truncate (token, table=<id>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    table: str
+    table : str
         The specific table to truncate.
 
     Returns
     -------
 
     Example
     -------
     .. code-block:: python
 
         # Truncate the table 'foo'
-        queryClient.truncate('foo')
+        queryClient.mydb_truncate('foo')
     '''
     return qc_client._mydb_truncate (token=def_token(token), table=table)
 
 # --------------------------------------------------------------------
 # MYDB_INDEX -- Index a column in a user's MyDB table.
 #
 @multimethod('qc',3,False)
@@ -1454,101 +1512,102 @@
                                      column=opt2, q3c=q3c, cluster=cluster,
                                      async_=async_)
 
 
 @multimethod('qc',1,False)
 def mydb_index(table, column='', token=None, q3c=None, cluster=False,
                async_=False):
-    '''Index the specified column in a table in the user's MyDB
+    '''Index the specified column in a table in the user's MyDB.
 
     MultiMethod Usage::
 
         queryClient.mydb_index (table, colunm)
         queryClient.mydb_index (token, table, column)
         queryClient.mydb_index (table, column, token=None)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    table: str
-        The table to be indexed
+    table : str
+        The table containing the column to be indexed.
 
-    column: str
-        The column
+    column : str
+        The column to be indexed.
 
-    q3c: str
+    q3c : str
         A comma-delimited list of two column names giving the RA and Dec
-        positions (decimal degrees) to be used to Q3C index the table.  If
+        positions (decimal degrees) to be used to Q3C index the table. If
         None, no Q3C index will be computed.
 
-    cluster: bool
+    cluster : bool
         If enabled, data table will be rewritten to cluster on the Q3C index
-        for efficiency.  Only used when 'q3c' columns are specified.
+        for efficiency. Only used when 'q3c' columns are specified.
 
-    async_: bool
-	If enabled, index commands will be submitted asynchronously.
+    async_ : bool
+        If enabled, index commands will be submitted Asynchronously.
 
     Returns
     -------
-	command status
+    command status
 
     Example
     -------
     .. code-block:: python
 
-	# Index the table's "id" column
-        queryClient.index('foo1', 'id')
+    # In the 'foo1' table, index the 'id' column
+        queryClient.mydb_index('foo1', 'id')
 
-	# Index and cluster the table by position
-        queryClient.index('foo1', q3c='ra,dec', cluster=True)
+    # Index and cluster the table by position
+        queryClient.mydb_index('foo1', q3c='ra,dec', cluster=True)
     '''
     return qc_client._mydb_index(token=def_token(token), table=table,
                                  column=column, q3c=q3c, cluster=cluster,
                                  async_=async_)
 
 # --------------------------------------------------------------------
 # MYDB_DROP -- Drop the named table from a user's MyDB.
 #
 @multimethod('qc',2,False)
 def mydb_drop(token, table):
     return qc_client._mydb_drop (token=def_token(token), table=table)
 
 @multimethod('qc',1,False)
 def mydb_drop(table, token=None):
-    '''Drop the specified table from the user's MyDB
+    '''Drop the specified table from the user's MyDB.
 
     Usage::
 
         mydb_drop (table, token=None)
 
     MultiMethod Usage::
 
         queryClient.mydb_drop (token, table)
         queryClient.mydb_drop (table)
         queryClient.mydb_drop (token, table=<id>)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    table: str
-        The specific table to drop
+    table : str
+        The specific table to drop.
 
     Returns
     -------
+    command status
 
     Example
     -------
     .. code-block:: python
 
         # Drop the 'foo1' table
-        queryClient.drop('foo1')
+        queryClient.mydb_drop('foo1')
     '''
     return qc_client._mydb_drop (token=def_token(token), table=table)
 
 
 # --------------------------------------------------------------------
 # MYDB_FLUSH -- Flush user's MyDB tables from temporary space
 #
@@ -1562,90 +1621,92 @@
 @multimethod('qc',3,False)
 def mydb_rename(token, source, target):
     return qc_client._mydb_rename (token=def_token(token),
                                 source=source, target=target)
 
 @multimethod('qc',2,False)
 def mydb_rename(source, target, token=None):
-    '''Rename a table in the user's MyDB to a new name
+    '''Rename a table in the user's MyDB to a new name.
 
     Usage::
 
         mydb_rename (source, target, token=None)
 
     MultiMethod Usage::
 
         queryClient.mydb_rename (token, source, target)
         queryClient.mydb_rename (source, target)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    source: str
-        The old table name
+    source : str
+        The old table name.
 
-    target: str
-        The new table name
+    target : str
+        The new table name.
 
     Returns
     -------
+    command status
 
     Example
     -------
     .. code-block:: python
 
-        # Copy table 'foo' to a new table, 'bar'
-        queryClient.mydb_rename ('foo', 'bar')
+        # Rename table 'foo' to a new name, 'bar'
+        queryClient.mydb_rename('foo', 'bar')
     '''
     return qc_client._mydb_rename (source, target, token=def_token(token))
 
 
 # --------------------------------------------------------------------
 # MYDB_COPY -- Copy a table in the user's MyDB.
 #
 @multimethod('qc',3,False)
 def mydb_copy(token, source, target):
     return qc_client._mydb_copy (token=def_token(token),
                               source=source, target=target)
 
 @multimethod('qc',2,False)
 def mydb_copy(source, target, token=None):
-    '''Copy a table in the user's MyDB to a new name
+    '''Copy a table in the user's MyDB to a new name.
 
     Usage::
 
         mydb_copy (source, target, token=None)
 
     MultiMethod Usage::
 
         queryClient.mydb_copy (token, source, target)
         queryClient.mydb_copy (source, target)
 
     Parameters
     ----------
-    token : str
-        Authentication token (see function :func:`authClient.login()`)
+    token : str [Optional]
+        Authentication token (see function :func:`authClient.login()`).
 
-    source: str
-        The old table name, i.e. the table to be copied
+    source : str
+        The old table name, i.e. the table to be copied.
 
-    target: str
-        The new table name, i.e. the table to be created
+    target : str
+        The new table name, i.e. the table to be created.
 
     Returns
     -------
+    command status
 
     Example
     -------
     .. code-block:: python
 
         # Copy table 'foo' to a new table, 'bar'
-        queryClient.mydb_copy ('foo', 'bar')
+        queryClient.mydb_copy('foo', 'bar')
     '''
     return qc_client._mydb_copy (source, target, token=def_token(token))
 
 
 
 
 # ###################################
@@ -1678,27 +1739,27 @@
         resClient.set_svc_url(self.rm_svc_url)
         storeClient.set_svc_url(self.sm_svc_url)
 
 
     def isAlive(self, svc_url=None, timeout=5):
         '''Check whether the QueryManager service at the given URL is
            alive and responding.  This is a simple call to the root
-           service URL or ping() method.
+           service URL or ``ping()`` method.
 
         Parameters
         ----------
         svc_url : str
             The Query Service URL to ping.
         timeout : int
-            Call will assume to have failed if 'timeout' seconds pass.
+            Call will assume to have failed if ``timeout`` seconds pass.
 
         Returns
         -------
         result : bool
-            True if service responds properly, False otherwise
+            ``True`` if service responds properly, ``False`` otherwise.
 
         Example
         -------
         .. code-block:: python
 
             if queryClient.isAlive():
                 print ("Query Manager is alive")
@@ -1730,15 +1791,15 @@
         -------
         Nothing
 
         Example
         -------
         .. code-block:: python
 
-            queryClient.set_svc_url ("http://localhost:7002")
+            queryClient.set_svc_url("http://localhost:7002")
         '''
         if svc_url is not None:
             self.svc_url = qcToString(svc_url.strip('/'))
 
     def get_svc_url(self):
         '''Get the currently-used Query Manager serice URL.
 
@@ -1763,15 +1824,15 @@
         '''Set the service profile to be used.
 
         Parameters
         ----------
         profile : str
             The name of the profile to use. The list of available profiles
             can be retrieved from the service (see function
-            func:`queryClient.list_profiles()`)
+            :func:`queryClient.list_profiles()`).
 
         Returns
         -------
         Nothing
 
         Example
         -------
@@ -1787,15 +1848,16 @@
         Parameters
         ----------
         None
 
         Returns
         -------
         profile : str
-            The name of the current profile used with the Query Manager service
+            The name of the current profile used with the Query Manager
+            service.
 
         Example
         -------
         .. code-block:: python
 
             print ("Query Service profile = " + queryClient.get_profile())
         '''
@@ -1803,50 +1865,48 @@
 
     def set_timeout_request(self, nsec):
         '''Set the requested Sync query timeout value (in seconds).
 
         Parameters
         ----------
         nsec : int
-            The number of seconds requested before a sync query timeout occurs.
-            The service may cap this as a server defined maximum.
+            The number of seconds requested before a Sync query timeout
+            occurs. The service may cap this as a server defined maximum.
 
         Returns
         -------
         Nothing
 
         Example
         -------
         .. code-block:: python
 
-            # set the sync query timeout request to 30 seconds
+            # set the Sync query timeout request to 30 seconds
             queryClient.set_timeout_request(30)
-
         '''
         self.timeout_request = nsec
 
     def get_timeout_request(self):
         '''Get the current Sync query timeout value.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        result: int
-            Current sync query timeout value.
+        result : int
+            Current Sync query timeout value in seconds.
 
         Example
         -------
         .. code-block:: python
 
             # get the current timeout value
             print (queryClient.get_timeout_request())
-
         '''
         return self.timeout_request
 
 
     # ###########################
     #  Utility Methods
     # ###########################
@@ -1992,22 +2052,32 @@
         '''
 
         # Process optional keyword arguments.
         if 'async' in kw:
             async_ = kw['async']
         if 'format' in kw:              # alias for 'fmt'
             fmt = kw['format']
+        if 'progress' in kw:
+            progress = kw['progress']
+        else:
+            progress = False
 
         timeout = self.timeout_request 	# set requested timeout on the query
         if 'timeout' in kw:
             timeout = int(kw['timeout'])
 
-        wait = self.async_wait 		# see if we wait for an Async result
+        # Determine whether to wait based on 'wait' in kw or the class
+        # attribute self.async_wait but don't modify self.async_wait based
+        # on the 'wait' argument passed in.
         if async_ and 'wait' in kw:
-            self.async_wait = wait = kw['wait']
+            # use 'wait' in passed in kw if it's boolean otherwise use async_wait
+            wait = bool(kw['wait']) if isinstance(kw['wait'], bool) else self.async_wait
+        else:
+            # Otherwise, use the value of self.async_wait.
+            wait = self.async_wait
 
         stream = False 		        # set a streaming request and adjust
         if 'stream' in kw:
             stream = kw['stream']
             if stream:
                 timeout = 0
                 async_ = False
@@ -2047,46 +2117,69 @@
             raise queryClientError("No query specified")
 
         if profile != "default":        	# append the service profile
             dburl += "&profile=%s" % profile
         else:
             dburl += "&profile=%s" % self.svc_profile
 
+
         # Make the service call.  In a streaming request we force a Sync
         # operation and by setting the timeout to zero let it run as long as
-        # needed.  Once a JM is implemented an ASync save will be possible.
+        # needed.  Once a JM is implemented an Async save will be possible.
         # Note:  Results may still be limited by the memory available to
         # contain the result string, especially in notebook environments.
         if stream:
             if (out is not None and out != '') and not async_:
                 # If we're saving a local file (e.g. in a notebook directory),
                 # save the file here. Results saved to VOSpace/MyDB are handled
                 # on the server side.
                 if out[:7] == 'file://':
                     out = out[7:]
+
+                # Because the VOSpace/MyDB are handled on the server side. Set
+                # the local file to None.
+                # Note: The "out" file information is already a parameter in the URL
+                #       going to the server.
                 if ':' in out and out[:out.index(':')] in ['vos', 'mydb']:
                     out = None
+
                 try:
-                    resp = self.getStreamURL(dburl, headers=headers,
-                                                    fname=out)
+                    resp = self.getStreamURL(dburl, headers=headers, fname=out, progress=progress)
+                except DLHTTPException as e:
+                    return e.error_message.strip()
                 except Exception as e:
                     print ('Error in getStreamURL: %s' %  qcToString(str(e)))
                     return qcToString(str(e))
 
+                # TODO: understand code
+                #  At this point, two things could have happened.
+                #  1.- out is a localfile and the results got saved locally
+                #  2.- out is a vos container or a mydb table and the results
+                #      have been saved server-side
+                #  The response in "resp" should only be the status of the requests.
+                #  If that's correct under what condition the below makes sense?
                 if 'noheader' in fmt:
                     strval = qcToString(resp).strip()
                     strval = strval[strval.find('\n')+1:]
                 else:
                     strval = qcToString(resp)
-                if (out is not None and out != ''):
+
+                # TODO: understand code
+                #  Here two things are possible:
+                #  1.- out was set to a local file and strval is the status of the response
+                #  2.- out was set to vos or mydb and handled serverside. Therefore
+                #      strval should contain no data but just the status, it could be
+                #      the status is returned in a format that is not a string.
+                #      However the result comes empty.
+                if out is not None and out != '':
                     return strval
                 else:
                     # Otherwise, simply return the result of the query.
                     if fmt in ['pandas','array','structarray','table']:
-                        return convert (strval,fmt)
+                        return convert(strval,fmt)
                     else:
                         return strval
 
         # If we're not streaming the request result, process it here.
         r = requests.get (dburl, headers=headers, timeout=timeout)
         if r.status_code != 200:
             raise queryClientError (r.text)
@@ -2096,15 +2189,15 @@
         # in byte format that can't be necessarily converted to string. So
         # now the conversion happens downstream on an as-needed basis.
 
         resp = r.content
 
         if async_ and wait:
             # Sync query timeouts are handled on the server.  If waiting
-            # for an async query, loop until job is completed or the timeout
+            # for an Async query, loop until job is completed or the timeout
             # expires.
             resp = qcToString(resp)
             jobId = resp
             stat = self._status (token=token, jobId=jobId, profile=profile)
             tval = 0
             while (stat not in ['COMPLETED','ERROR']):
                 if verbose: print (stat)
@@ -2129,20 +2222,20 @@
             if tval > timeout:
                 if verbose:
                     print ('Timeout (%d sec) exceeded' % timeout)
                 raise queryClientError ('Query timeout exceeded')
             elif stat not in ['COMPLETED','ERROR']:
                 resp = stat
             elif stat == 'ERROR':
-		# Retrieve Async error.
+                # Retrieve Async error.
                 if verbose:
                     print ('Retrieving error')
                 resp = self._error (token=token, jobId=jobId, profile=profile)
             elif stat == 'COMPLETED':
-		# Retrieve Async results.  A save to vos/mydb is handled below.
+                # Retrieve Async results.  A save to vos/mydb is handled below.
                 if verbose:
                     print ('Retrieving results')
                 resp = self._results (token=token, jobId=jobId, profile=profile)
 
         if (out is not None and out != '') and not async_:
             # If we're saving to a local file (e.g. in a notebook directory),
             # save the file here. Results saved to VOSpace or MyDB are handled
@@ -2159,48 +2252,51 @@
         else:
             # Otherwise, simply return the result of the query.
             if 'noheader' in fmt:
                 strval = qcToString(resp).strip()
                 strval = strval[strval.find('\n')+1:]
             else:
                 strval = qcToString(resp)
-            if fmt in ['pandas','array','structarray','table']:
+
+            if async_ and not wait:
+                return strval  # this case should only be a job ID
+            elif fmt in ['pandas','array','structarray','table']:
                 return convert (strval, fmt)
             else:
                 return strval
 
 
     # --------------------------
     # Async jobs status()
     # --------------------------
 
     @multimethod('_qc',2,True)
     def status(self, token, jobId, profile='default'):
-        '''Usage:  queryClient.status (token, jobID)
+        '''Usage::  queryClient.status (token, jobID)
         '''
         return self._status (token=def_token(token), jobId=jobId,
                              profile=profile)
 
     @multimethod('_qc',1,True)
     def status(self, optval, jobId=None, profile='default'):
-        '''Usage:  queryClient.status (jobID)
-                   queryClient.status (token, jobId=<id>)
+        '''Usage::  queryClient.status (jobID)
+                    queryClient.status (token, jobId=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self._status (token=def_token(optval), jobId=jobId,
                                  profile=profile)
         else:
             # optval is probably a jobId
             return self._status (token=def_token(None), jobId=optval,
                                  profile=profile)
 
     @multimethod('_qc',0,True)
     def status(self, token=None, jobId=None, profile='default'):
-        '''Usage:  queryClient.status (jobID=<str>)
+        '''Usage::  queryClient.status (jobID=<str>)
         '''
         return self._status (token=def_token(token), jobId=jobId,
                              profile=profile)
 
     def _status(self, token=None, jobId=None, profile='default'):
         '''Implementation of the status() method.
         '''
@@ -2218,24 +2314,24 @@
 
     # --------------------------
     # Async jobs list
     # --------------------------
 
     @multimethod('_qc',2,True)
     def jobs(self, token, jobId, format='text', status='all', option='list'):
-        '''Usage:  queryClient.jobs (token, jobID)
+        '''Usage::  queryClient.jobs (token, jobID)
         '''
         return self._jobs (token=def_token(token), jobId=jobId,
                            format=format, status=status, option=option)
 
     @multimethod('_qc',1,True)
     def jobs(self, optval, jobId=None, format='text', status='all',
               option='list'):
-        '''Usage:  queryClient.jobs (jobID)
-                   queryClient.jobs (token, jobId=<id>)
+        '''Usage::  queryClient.jobs (jobID)
+                    queryClient.jobs (token, jobId=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self._jobs (token=def_token(optval), jobId=jobId,
                                format=format, status=status, option=option)
         else:
             # optval is probably a jobId
@@ -2265,85 +2361,87 @@
 
 
     # --------------------------
     # Async jobs results()
     # --------------------------
 
     @multimethod('_qc',2,True)
-    def results(self, token, jobId, fname=None, delete=True, profile='default'):
-        '''Usage:  queryClient.results (token, jobID)
+    def results(self, token, jobId, fname=None, delete=True, profile='default', progress=False):
+        '''Usage::  queryClient.results (token, jobID)
         '''
         return self._results (token=def_token(token), jobId=jobId,
-                              fname=fname, delete=delete, profile=profile)
+                              fname=fname, delete=delete, profile=profile, progress=progress)
 
     @multimethod('_qc',1,True)
-    def results(self, optval, jobId=None, fname=None, delete=True, profile='default'):
-        '''Usage:  queryClient.results (jobID)
-                   queryClient.results (token, jobId=<id>)
+    def results(self, optval, jobId=None, fname=None, delete=True, profile='default', progress=False):
+        '''Usage::  queryClient.results (jobID)
+                    queryClient.results (token, jobId=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self._results (token=def_token(optval), jobId=jobId,
-                                  fname=fname, delete=delete, profile=profile)
+                                  fname=fname, delete=delete, profile=profile, progress=progress)
         else:
             # optval is probably a jobId
             return self._results (token=def_token(None), jobId=optval,
-                                  fname=fname, delete=delete, profile=profile)
+                                  fname=fname, delete=delete, profile=profile, progress=progress)
 
     @multimethod('_qc',0,True)
-    def results(self, token=None, jobId=None, fname=None, delete=True, profile='default'):
-        '''Usage:  queryClient.results (jobID=<str>)
+    def results(self, token=None, jobId=None, fname=None, delete=True, profile='default', progress=False):
+        '''Usage::  queryClient.results (jobID=<str>)
         '''
         return self._results (token=def_token(token), jobId=jobId,
-                              fname=fname, delete=delete, profile=profile)
+                              fname=fname, delete=delete, profile=profile, progress=progress)
 
-    def _results(self, token=None, jobId=None, fname=None, delete=True, profile='default'):
+    def _results(self, token=None, jobId=None, fname=None, delete=True, profile='default', progress=False):
         '''Implementation of the results() method.
         '''
         headers = self.getHeaders (token)
 
         dburl = '%s/results?jobid=%s&delete=%s' % (self.svc_url, jobId, delete)
         if profile != "default":
             dburl += "&profile=%s" % profile
         elif self.svc_profile != "default":
             dburl += "&profile=%s" % self.svc_profile
 
-        #r = requests.get (dburl, headers=headers)
-        r = self.getStreamURL(dburl, headers=headers, fname=fname)
-        return qcToString(r)
+        try:
+            r = self.getStreamURL(dburl, headers=headers, fname=fname, progress=progress)
+            return qcToString(r)
+        except DLHTTPException as e:
+            return e.error_message
 
 
     # --------------------------
     # Async jobs error()
     # --------------------------
 
     @multimethod('_qc',2,True)
     def error(self, token, jobId, profile='default'):
-        '''Usage:  queryClient.error (token, jobID)
+        '''Usage::  queryClient.error (token, jobID)
         '''
         return self._error (token=def_token(token), jobId=jobId,
                             profile=profile)
 
     @multimethod('_qc',1,True)
     def error(self, optval, jobId=None, profile='default'):
-        '''Usage:  queryClient.error (jobID)
-                     queryClient.error (token, jobId=<id>)
+        '''Usage::  queryClient.error (jobID)
+                    queryClient.error (token, jobId=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self._error (token=def_token(optval), jobId=jobId,
                                 profile=profile)
         else:
             # optval is probably a jobId
             return self._error (token=def_token(None), jobId=optval,
                                 profile=profile)
 
     @multimethod('_qc',0,True)
     def error(self, token=None, jobId=None, profile='default'):
-        '''Usage:  queryClient.error (jobID=<str>)
+        '''Usage::  queryClient.error (jobID=<str>)
         '''
         return self._error (token=def_token(token), jobId=jobId,
                             profile=profile)
 
     def _error(self, token=None, jobId=None, profile='default'):
         '''Implementation of the error() method.
         '''
@@ -2361,36 +2459,36 @@
 
     # --------------------------
     # Async job abort()
     # --------------------------
 
     @multimethod('_qc',2,True)
     def abort(self, token, jobId, profile='default'):
-        '''Usage:  queryClient.abort (token, jobID)
+        '''Usage::  queryClient.abort (token, jobID)
         '''
         return self._abort (token=def_token(token), jobId=jobId,
                             profile=profile)
 
     @multimethod('_qc',1,True)
     def abort(self, optval, jobId=None, profile='default'):
-        '''Usage:  queryClient.abort (jobID)
-                   queryClient.abort (token, jobId=<id>)
+        '''Usage::  queryClient.abort (jobID)
+                    queryClient.abort (token, jobId=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self._abort (token=def_token(optval), jobId=jobId,
                             profile=profile)
         else:
             # optval is probably a jobId
             return self._abort (token=def_token(None), jobId=optval,
                             profile=profile)
 
     @multimethod('_qc',0,True)
     def abort(self, token=None, jobId=None, profile='default'):
-        '''Usage:  queryClient.abort (jobID=<str>)
+        '''Usage::  queryClient.abort (jobID=<str>)
         '''
         return self._abort (token=def_token(token), jobId=jobId,
                             profile=profile)
 
     def _abort(self, token=None, jobId=None, profile='default'):
         '''Implementation of the abort() method.
         '''
@@ -2408,52 +2506,52 @@
 
     # --------------------------
     # Async job wait()
     # --------------------------
 
     @multimethod('_qc',2,True)
     def wait(self, token, jobId, wait=3, verbose=False, profile='default'):
-        '''Usage:  queryClient.wait (token, jobID)
+        '''Usage::  queryClient.wait (token, jobID)
         '''
         return self._wait (token=def_token(token), jobId=jobId, wait=wait,
                            verbose=verbose, profile=profile)
 
     @multimethod('_qc',1,True)
     def wait(self, optval, jobId=None, wait=3, verbose=False, profile='default'):
-        '''Usage:  queryClient.wait (jobID)
-                   queryClient.wait (token, jobId=<id>)
+        '''Usage::  queryClient.wait (jobID)
+                    queryClient.wait (token, jobId=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self._wait (token=def_token(optval), jobId=jobId, wait=wait,
                                verbose=verbose, profile=profile)
         else:
             # optval is probably a jobId
             return self._wait (token=def_token(None), jobId=optval, wait=wait,
                                verbose=verbose, profile=profile)
 
     @multimethod('_qc',0,True)
     def wait(self, token=None, jobId=None, wait=3, verbose=False, profile='default'):
-        '''Usage:  queryClient.wait (jobID=<str>)
+        '''Usage::  queryClient.wait (jobID=<str>)
         '''
         return self._wait (token=def_token(token), jobId=jobId, wait=wait,
                            verbose=verbose, profile=profile)
 
     def _wait(self, token=None, jobId=None, wait=3, verbose=False, profile='default'):
         '''Implementation of the wait() method.
 
-           Loop until an async job has completed.
+           Loop until an Async job has completed.
 
         Parameters
         ----------
         jobid : str
             The job ID string of a submitted query job.
 
         wait : int | float
-            Wait for `wait` seconds before checking status again. Default: 3sec
+            Wait for ``wait`` seconds before checking status again. Default: 3sec.
         '''
 
         while True:
             status = qc_client._status(token=token,jobId=jobId,profile=profile)
             if verbose:
                 print(status)
             if status in ('QUEUED','EXECUTING'):
@@ -2471,88 +2569,88 @@
     #  MyDB Methods
     # ###########################
 
     # LIST -- List the tables or table schema in the user's MyDB.
     #
     @multimethod('_qc',2,True)
     def list(self, token, table):
-        '''Usage:  queryClient.list (token, table)
+        '''Usage::  queryClient.list (token, table)
         '''
         return self.mydb_list (token=def_token(token), table=table)
 
     @multimethod('_qc',1,True)
     def list(self, optval, table=None):
-        '''Usage:  queryClient.list (table)
-                   queryClient.list (token, table=<id>)
+        '''Usage::  queryClient.list (table)
+                    queryClient.list (token, table=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self.mydb_list (token=def_token(optval), table=table)
         else:
             # optval is probably a table
             return self.mydb_list (token=def_token(None), table=optval)
 
     @multimethod('_qc',0,True)
     def list(self, token=None, table=None):
-        '''Usage:  queryClient.list (table=<str>)
+        '''Usage::  queryClient.list (table=<str>)
         '''
         return self.mydb_list (token=def_token(token), table=table)
 
 
     # DROP -- Drop the specified table from the user's MyDB
     #
     @multimethod('_qc',2,True)
     def drop(self, token, table):
-        '''Usage:  queryClient.drop (token, table)
+        '''Usage::  queryClient.drop (token, table)
         '''
         return self.mydb_drop (token=def_token(token), table=table)
 
     @multimethod('_qc',1,True)
     def drop(self, optval, table=None):
-        '''Usage:  queryClient.drop (table)
-                   queryClient.drop (token, table=<id>)
+        '''Usage::  queryClient.drop (table)
+                    queryClient.drop (token, table=<id>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self.mydb_drop (token=def_token(optval), table=table)
         else:
             # optval is probably a table
             return self.mydb_drop (token=def_token(None), table=optval)
 
     @multimethod('_qc',0,True)
     def drop(self, token=None, table=None):
-        '''Usage:  queryClient.drop (table=<str>)
+        '''Usage::  queryClient.drop (table=<str>)
         '''
         return self.mydb_drop (token=def_token(token), table=table)
 
 
     # -----------------------------
     #  MyDB Functions (New API)
     # -----------------------------
 
     # --------------------------------------------------------------------
     # MYDB_LIST -- List the tables or table schema in a user's MyDB.
     #
     @multimethod('_qc',1,True)
     def mydb_list(self, optval, table=None, index=False, **kw):
-        '''Usage:  queryClient.mydb_list (table)
-                   queryClient.mydb_list (token, table=<str>)
+        '''Usage::  queryClient.mydb_list (table)
+                    queryClient.mydb_list (token, table=<str>)
         '''
         if optval is not None and is_auth_token(optval):
             # optval looks like a token
             return self._mydb_list (token=def_token(optval), table=table,
                                     index=index, **kw)
         else:
             # optval is probably a table
             return self._mydb_list (token=def_token(None), table=optval,
                                     index=index, **kw)
 
     @multimethod('_qc',0,True)
     def mydb_list(self, token=None, table=None, index=False, **kw):
-        '''Usage:  queryClient.mydb_list (table=<str>)
+        '''Usage::  queryClient.mydb_list (table=<str>)
         '''
         return self._mydb_list (token=def_token(token), table=table,
                                 index=index, **kw)
 
     def _mydb_list(self, token=None, table=None, index=False, **kw):
         '''Implementation of the mydb_list() method.
         '''
@@ -2576,22 +2674,22 @@
 
 
     # --------------------------------------------------------------------
     # MYDB_CREATE -- Copy a table in the user's MyDB.
     #
     @multimethod('_qc',3,True)
     def mydb_create(self, token, table, schema, **kw):
-        '''Usage:  queryClient.mydb_create (token, table, <schema_dict>)
+        '''Usage::  queryClient.mydb_create (token, table, <schema_dict>)
         '''
         return self._mydb_create (token=def_token(None), table=table,
                                   schema=schema, **kw)
 
     @multimethod('_qc',2,True)
     def mydb_create(self, table, schema, token=None, **kw):
-        '''Usage:  queryClient.mydb_create (table, <schema_dict>)
+        '''Usage::  queryClient.mydb_create (table, <schema_dict>)
         '''
         return self._mydb_create (token=def_token(None), table=table,
                                   schema=schema, **kw)
 
     def _mydb_create(self, token, table, schema, **kw):
         '''Implementation of the mydb_create() method.
         '''
@@ -2643,24 +2741,24 @@
 
     # --------------------------------------------------------------------
     # MYDB_INSERT -- Insert data into a table in the user's MyDB from a local
     # file or python data object.
     #
     @multimethod('_qc',3,True)
     def mydb_insert(self, token, table, data, **kw):
-        '''Usage:  queryClient.mydb_insert (token, table, <filename>)
-                   queryClient.mydb_insert (token, table, <data_object>)
+        '''Usage::  queryClient.mydb_insert (token, table, <filename>)
+                    queryClient.mydb_insert (token, table, <data_object>)
         '''
         return self._mydb_insert (token=def_token(token), table=table,
                                   data=data, **kw)
 
     @multimethod('_qc',2,True)
     def mydb_insert(self, table, data, token=None, **kw):
-        '''Usage:  queryClient.mydb_insert (table, <filename>)
-                   queryClient.mydb_insert (table, <data_object>)
+        '''Usage::  queryClient.mydb_insert (table, <filename>)
+                    queryClient.mydb_insert (table, <data_object>)
         '''
         return self._mydb_insert (token=def_token(token), table=table,
                                   data=data, **kw)
 
     def _mydb_insert(self, token=None, table=None, data=None, **kw):
         '''Implementation of the mydb_create() method.
         '''
@@ -2735,22 +2833,22 @@
 
 
     # --------------------------------------------------------------------
     # MYDB_IMPORT -- Import a file or Python object to a MyDB table.
     #
     @multimethod('_qc',3,True)
     def mydb_import(self, token, table, data, **kw):
-        '''Usage:  queryClient.mydb_import (token, table, data)
+        '''Usage::  queryClient.mydb_import (token, table, data)
         '''
         return self._mydb_import (token=def_token(token), table=table,
                                   data=data, **kw)
 
     @multimethod('_qc',2,True)
     def mydb_import(self, table, data, token=None, **kw):
-        '''Usage:  queryClient.mydb_import (table, data)
+        '''Usage::  queryClient.mydb_import (table, data)
         '''
         return self._mydb_import (token=def_token(token), table=table,
                                   data=data, **kw)
 
     def _mydb_import(self, token=None, table=None, data=None, **kw):
         '''Implementation of the mydb_create() method.
         '''
@@ -2847,21 +2945,21 @@
 
 
     # --------------------------------------------------------------------
     # MYDB_TRUNCATE -- Truncate a table in the user's MyDB.
     #
     @multimethod('_qc',2,True)
     def mydb_truncate(self, token, table):
-        '''Usage:  queryClient.mydb_truncate (token, table)
+        '''Usage::  queryClient.mydb_truncate (token, table)
         '''
         return self._mydb_truncate (token=def_token(token), table=table)
 
     @multimethod('_qc',1,True)
     def mydb_truncate(self, table, token=None):
-        '''Usage:  queryClient.mydb_truncate (table)
+        '''Usage::  queryClient.mydb_truncate (table)
         '''
         return self._mydb_truncate (token=def_token(token), table=table)
 
     def _mydb_truncate(self, token=None, table=None):
         '''Implementation of the mydb_truncate() method.
         '''
         headers = self.getHeaders (token)
@@ -2883,24 +2981,24 @@
 
     # --------------------------------------------------------------------
     # MYDB_INDEX -- Index a column in a user's MyDB table.
     #
     @multimethod('_qc',3,True)
     def mydb_index(self, token, table, column, q3c=None, cluster=False,
                     async_=False):
-        '''Usage:  queryClient.mydb_index (token, table, column)
+        '''Usage::  queryClient.mydb_index (token, table, column)
         '''
         return self._mydb_index(token=def_token(token), table=table,
                                 column=column, q3c=q3c, cluster=cluster,
                                 async_=async_)
 
     @multimethod('_qc',2,True)
     def mydb_index(self, opt1, opt2, token=None, q3c=None, cluster=False,
                     async_=False):
-        '''Usage:  queryClient.mydb_index (table, colunm)
+        '''Usage::  queryClient.mydb_index (table, colunm)
         '''
         if q3c is not None and len(opt1.split('.')) >= 4:
             # opt1 looks like a token and q3c is set, opt2 must be a table
             return self._mydb_index(token=def_token(opt1), table=opt2,
                                     column='', q3c=q3c, cluster=cluster,
                                     async_=async_)
         else:
@@ -2952,22 +3050,22 @@
 
 
     # --------------------------------------------------------------------
     # MYDB_DROP -- Drop the named table from a user's MyDB.
     #
     @multimethod('_qc',2,True)
     def mydb_drop(self, token, table):
-        '''Usage:  queryClient.mydb_drop (token, table)
+        '''Usage::  queryClient.mydb_drop (token, table)
         '''
         return self._mydb_drop (token=def_token(token), table=table)
 
     @multimethod('_qc',1,True)
     def mydb_drop(self, table, token=None):
-        '''Usage:  queryClient.mydb_drop (table)
-                     queryClient.mydb_drop (token, table=<id>)
+        '''Usage::  queryClient.mydb_drop (table)
+                    queryClient.mydb_drop (token, table=<id>)
         '''
         return self._mydb_drop (token=def_token(token), table=table)
 
     def _mydb_drop(self, token=None, table=None):
         '''Implementation of the mydb_drop() method.
         '''
         headers = self.getHeaders (token)
@@ -2985,16 +3083,15 @@
         else:
             return 'OK'
 
     # --------------------------------------------------------------------
     # MYDB_FLUSH -- Drop the temporary tables in mydb schema in tapdb DB
     #
     def _mydb_flush(self, token=None):
-        '''Usage:  queryClient.mydb_flush ()
-
+        '''Usage::  queryClient.mydb_flush ()
         '''
         headers = self.getHeaders(token)
 
         dburl = '%s/flush' % (self.svc_url)
         if self.svc_profile != "default":
             dburl += "?profile=%s" % self.svc_profile
 
@@ -3005,22 +3102,22 @@
             return 'OK'
 
     # --------------------------------------------------------------------
     # MYDB_RENAME -- Rename a table in the user's MyDB.
     #
     @multimethod('_qc',3,True)
     def mydb_rename(self, token, source, target):
-        '''Usage:  queryClient.mydb_rename (token, source, target)
+        '''Usage::  queryClient.mydb_rename (token, source, target)
         '''
         return self._mydb_rename (token=def_token(token),
                                     source=source, target=target)
 
     @multimethod('_qc',2,True)
     def mydb_rename(self, source, target, token=None):
-        '''Usage:  queryClient.mydb_rename (source, target)
+        '''Usage::  queryClient.mydb_rename (source, target)
         '''
         return self._mydb_rename (source=source, target=target,
                                   token=def_token(token))
 
     def _mydb_rename(self, source='', target='', token=None):
         '''Implementation of the mydb_rename() method.
         '''
@@ -3042,22 +3139,22 @@
             return 'OK'
 
     # --------------------------------------------------------------------
     # MYDB_COPY -- Copy a table in the user's MyDB.
     #
     @multimethod('_qc',3,True)
     def mydb_copy(self, token, source, target):
-        '''Usage:  queryClient.mydb_copy (token, source, target)
+        '''Usage::  queryClient.mydb_copy (token, source, target)
         '''
         return self._mydb_copy (token=def_token(token),
                                   source=source, target=target)
 
     @multimethod('_qc',2,True)
     def mydb_copy(self, source, target, token=None):
-        '''Usage:  queryClient.mydb_copy (source, target)
+        '''Usage::  queryClient.mydb_copy (source, target)
         '''
         return self._mydb_copy (source=source, target=target,
                                 token=def_token(token))
 
     def _mydb_copy(self, source='', target='', token=None):
         '''Implementation of the mydb_copy() method.
         '''
@@ -3193,22 +3290,72 @@
             hdrs = self.getHeaders (token)
             resp = requests.get("%s%s" % (svc_url, path), headers=hdrs)
 
         except Exception as e:
             raise queryClientError(str(e))
         return resp
 
+    def pycurl_download(self, url, headers, fname=None, progress=False):
+        setup_progress()
+
+        buffer = BytesIO() if fname is None else None
+
+        c = pycurl.Curl()
+        c.setopt(c.URL, url)
+        # Specify the CA certificates file from certifi
+        c.setopt(c.CAINFO, certifi.where())
+        try:
+            if progress:
+                c.setopt(c.NOPROGRESS, not progress)
+                c.setopt(c.XFERINFOFUNCTION, progress_report)
+            # Set custom headers if provided
+            if headers:
+                # Convert headers dict to a list of 'Key: Value' strings
+                headers_list = [f"{key}: {value}" for key, value in headers.items()]
+                c.setopt(c.HTTPHEADER, headers_list)
+
+            if fname is None:
+                c.setopt(c.WRITEDATA, buffer)
+            else:
+                with open(fname, 'wb') as f:
+                    c.setopt(c.WRITEDATA, f)
+                    c.perform()  # Perform the file download within the context manager when destination is specified
+
+            if fname is None:
+                c.perform()  # Perform the download when writing to buffer/STDOUT
+
+            total_downloaded = c.getinfo(pycurl.SIZE_DOWNLOAD)
+            c.close()
 
-    def getStreamURL (self, url, headers, fname=None, chunk_size=1048576):
+            elapsed_time = time.time() - progress_report.start_time
+
+            if not progress:
+                print(f"\nTotal time: {human_readable_time(elapsed_time)} for {human_readable_size(total_downloaded)}")
+
+        except pycurl.error as e:
+            print(f"Error in pycurl_download occurred: {str(e)}")
+            raise queryClientError(str(e))
+        except Exception as e:
+            print(f"Error in pycurl_download occurred: {str(e)}")
+            raise queryClientError(str(e))
+        finally:
+            c.close()
+
+        if buffer:
+            return buffer.getvalue()  # Return the contents of the buffer
+        else:
+            return "OK"
+
+    def request_download(self, url, headers, fname=None, chunk_size=1048576):
         ''' Get the specified URL in a streaming fashion.  This allows for
             large downloads without hitting timeout limits.
         '''
         r = requests.get(url, headers=headers, stream=True)
         if r.status_code != 200:
-            return r.status_code, r.text
+            raise DLHTTPException(r.status_code, r.text)
         else:
             try:
                 # Download the request in chunks to avoid timeouts.
                 #clen = min(chunk_size, r.headers.get('content-length'))
                 if fname is not None and fname != '':
                     with open(fname, 'wb', 0) as fd:
                         for chunk in r.iter_content(chunk_size=chunk_size):
@@ -3224,14 +3371,22 @@
             except IOError as e:
                 print ('IOError in getStreamURL: %s' %  qcToString(str(e)))
                 raise queryClientError(str(e))
             except Exception as e:
                 print ('Error in getStreamURL: %s' %  qcToString(str(e)))
                 raise queryClientError(str(e))
 
+    def getStreamURL(self, url, headers, fname=None, chunk_size=1048576, progress=False):
+        try:
+            import pycurl
+            # If pycurl is imported successfully, use the pycurl download method
+            return self.pycurl_download(url, headers, fname=fname, progress=False)
+        except ImportError:
+            # If pycurl is not installed, fallback to the Flask request download method
+            return self.request_download(url, headers, fname=fname, chunk_size=chunk_size)
 
     def chunked_upload(self, token, local_file, remote_file):
         '''A streaming file uploader.
         '''
         debug = False
         init = True
         CHUNK_SIZE = 4 * 1024 * 1024                   # 16MB chunks
```

### Comparing `astro-datalab-2.22.1/dl/resClient.py` & `astro_datalab-2.23.0/dl/resClient.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/specClient.py` & `astro_datalab-2.23.0/dl/specClient.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/dl/storeClient.py` & `astro_datalab-2.23.0/dl/storeClient.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/scripts/datalab` & `astro_datalab-2.23.0/scripts/datalab`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/scripts/mountvofs` & `astro_datalab-2.23.0/scripts/mountvofs`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/setup.py` & `astro_datalab-2.23.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from distutils.core import setup
 import sys
 import os
+import glob
 from dl.__version__ import __version__ as dl_version
+from setuptools import setup, find_packages
+
 #from vos.__version__ import vos_version
 
 #if sys.version_info[0] > 2:
 #    print 'The vos package is only compatible with Python version 2.n'
 #    sys.exit(-1)
 
 ## Build the list of scripts to be installed.
 script_dir = 'scripts'
 scripts = []
 for script in os.listdir(script_dir):
     if script[-1] in [ "~", "#"]:
         continue
     scripts.append(os.path.join(script_dir,script))
 
-try:
-    from setuptools import setup, find_packages
-    has_setuptools = True
-except:
-    from distutils.core import setup
-    has_setuptools = False
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
 
 import unittest
 def my_test_suite():
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover('tests', pattern='test_*.py')
     return test_suite
 
@@ -49,14 +47,10 @@
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: GNU Affero General Public License v3',
           'Operating System :: POSIX',
           'Programming Language :: Python',
           'Topic :: Scientific/Engineering :: Astronomy',
         ], 
-      install_requires=['requests>=2.7', 'httplib2', 'numpy>=1.13',
-                        'astropy', 'pyvo', 'matplotlib','pandas',
-                        'pycurl_requests','specutils'],
-      requires=['requests (>=2.7)', 'httplib2', 'numpy (>=1.13)', 
-                'astropy', 'pyvo', 'matplotlib','pandas',
-                'pycurl_requests','specutils']
+      install_requires=requirements,
+      data_files=[('', ['requirements.txt'])],
       )
```

### Comparing `astro-datalab-2.22.1/tests/test_datalab.py` & `astro_datalab-2.23.0/tests/test_datalab.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/tests/test_helpers.py` & `astro_datalab-2.23.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/tests/test_util.py` & `astro_datalab-2.23.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/BitVector.py` & `astro_datalab-2.23.0/vos/BitVector.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/CacheMetaData.py` & `astro_datalab-2.23.0/vos/CacheMetaData.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/CadcCache.py` & `astro_datalab-2.23.0/vos/CadcCache.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/NodeCache.py` & `astro_datalab-2.23.0/vos/NodeCache.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/SharedLock.py` & `astro_datalab-2.23.0/vos/SharedLock.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/cantop.py` & `astro_datalab-2.23.0/vos/cantop.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/commonparser.py` & `astro_datalab-2.23.0/vos/commonparser.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/fuse.py` & `astro_datalab-2.23.0/vos/fuse.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/html2text.py` & `astro_datalab-2.23.0/vos/html2text.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/logExceptions.py` & `astro_datalab-2.23.0/vos/logExceptions.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/md5_cache.py` & `astro_datalab-2.23.0/vos/md5_cache.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/vofs.py` & `astro_datalab-2.23.0/vos/vofs.py`

 * *Files identical despite different names*

### Comparing `astro-datalab-2.22.1/vos/vos.py` & `astro_datalab-2.23.0/vos/vos.py`

 * *Files identical despite different names*

