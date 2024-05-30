# Comparing `tmp/anycrc-0.7.5.tar.gz` & `tmp/anycrc-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.7.5.tar", last modified: Wed May 22 03:39:13 2024, max compression
+gzip compressed data, was "anycrc-0.7.6.tar", last modified: Thu May 30 17:45:06 2024, max compression
```

## Comparing `anycrc-0.7.5.tar` & `anycrc-0.7.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-22 03:39:07.000000 anycrc-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-22 03:39:13.167848 anycrc-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-22 03:39:07.000000 anycrc-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.163848 anycrc-0.7.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-22 03:39:07.000000 anycrc-0.7.5/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-22 03:39:07.000000 anycrc-0.7.5/lib/crcany/crcdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-05-22 03:39:07.000000 anycrc-0.7.5/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 03:39:07.000000 anycrc-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:39:13.167848 anycrc-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-22 03:39:07.000000 anycrc-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.163848 anycrc-0.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/anycrc.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:06.682062 anycrc-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 17:45:02.000000 anycrc-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-30 17:45:06.682062 anycrc-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-30 17:45:02.000000 anycrc-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:06.678062 anycrc-0.7.6/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:06.678062 anycrc-0.7.6/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-30 17:45:02.000000 anycrc-0.7.6/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-30 17:45:02.000000 anycrc-0.7.6/lib/crcany/crcdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-05-30 17:45:02.000000 anycrc-0.7.6/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 17:45:02.000000 anycrc-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:45:06.682062 anycrc-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-30 17:45:02.000000 anycrc-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:06.678062 anycrc-0.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:06.682062 anycrc-0.7.6/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 17:45:02.000000 anycrc-0.7.6/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-30 17:45:02.000000 anycrc-0.7.6/src/anycrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-30 17:45:02.000000 anycrc-0.7.6/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    17843 2024-05-30 17:45:02.000000 anycrc-0.7.6/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:06.682062 anycrc-0.7.6/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-30 17:45:06.000000 anycrc-0.7.6/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 17:45:06.000000 anycrc-0.7.6/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:45:06.000000 anycrc-0.7.6/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 17:45:06.000000 anycrc-0.7.6/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.7.5/LICENSE` & `anycrc-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.5/PKG-INFO` & `anycrc-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

### Comparing `anycrc-0.7.5/README.md` & `anycrc-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.5/lib/crcany/crc.c` & `anycrc-0.7.6/lib/crcany/crc.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.5/lib/crcany/crcdbl.c` & `anycrc-0.7.6/lib/crcany/crcdbl.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.5/lib/crcany/model.c` & `anycrc-0.7.6/lib/crcany/model.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.5/setup.py` & `anycrc-0.7.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         
 else:
     compile_args = ['-fopenmp', '-O2']
     link_args = ['-fopenmp', '-O2']
     
 setup(
     name = 'anycrc',
-    version = '0.7.5',
+    version = '0.7.6',
     package_dir = {"": "src"},
     cmdclass={"build_ext": Build},
     ext_modules = [
         Extension(
             name='anycrc.anycrc',
             extra_compile_args=compile_args,
             extra_link_args=link_args,
```

### Comparing `anycrc-0.7.5/src/anycrc/anycrc.pyx` & `anycrc-0.7.6/src/anycrc/anycrc.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from libc.stdint cimport uintmax_t
 from .models import models, aliases
 import sys
 
 ctypedef uintmax_t word_t
 
 cdef extern from '../../lib/crcany/model.h':
-    cdef const unsigned short WORDCHARS
     cdef const unsigned short WORDBITS
     
     ctypedef struct model_t:
         unsigned short width
         short cycle
         short back
         char ref
@@ -59,15 +58,15 @@
         cdef unsigned endian = 1 if sys.byteorder == 'little' else 0
         refin = 'true' if ref_in else 'false'
         refout = 'true' if ref_out else 'false'
         
         if width > WORDBITS * 2:
             raise ValueError('CRC width is larger than what is allowed')
             
-        string = f'width={width} poly={poly} init={init} refin={refin} refout={refout} xorout={xor_out} check={check} residue={residue} name=""'.encode('utf-8')
+        string = f'width={width} poly={poly} init={init} refin={refin} refout={refout} xorout={xor_out} check={check} residue={residue} name=""'.encode('ascii')
         
         cdef int error_code = read_model(&self.model, string, 0)
         
         if error_code != 0:
             raise ValueError('An error occurred while retrieving the model, check the arguments passed to the CRC class')
             
         process_model(&self.model)
@@ -196,8 +195,8 @@
     
 def Model(name):
     if name in models:
         return CRC(*models[name])
     elif name in aliases:
         return CRC(*models[aliases[name]])
     else:
-        raise ValueError('CRC model not found')
+        raise ValueError('CRC model not found')
```

### Comparing `anycrc-0.7.5/src/anycrc/models.py` & `anycrc-0.7.6/src/anycrc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# taken from Greg Cook's CRC catalogue: https://reveng.sourceforge.io/crc-catalogue/
+# Taken from Greg Cook's CRC catalogue: https://reveng.sourceforge.io/crc-catalogue/all.htm
 
 from collections import namedtuple
 
 model = namedtuple('model', ['width', 'poly', 'init', 'refin', 'refout', 'xorout', 'check', 'residue'], defaults=(0, 0))
 
 models = {
     'CRC4-G-704': model(width=4, poly=0x3, init=0x0, refin=True, refout=True, xorout=0x0, check=0x7, residue=0x0),
@@ -133,15 +133,15 @@
     'CRC11': 'CRC11-FLEXRAY',
     '3GPP': 'CRC12-UMTS',
     'CRC12': 'CRC12-UMTS',
     'X-CRC12': 'CRC12-DECT',
     'CRC15': 'CRC15-CAN',
     'ARC': 'CRC16-ARC',
     'CRC16': 'CRC16-ARC',
-    'CRC15-ACORN': 'CRC16-XMODEM',
+    'CRC16-ACORN': 'CRC16-XMODEM',
     'CRC16-AUG-CCITT': 'CRC16-SPI-FUJITSU',
     'CRC16-AUTOSAR': 'CRC16-IBM-3740',
     'CRC16-BLUETOOTH': 'CRC16-KERMIT',
     'CRC16-BUYPASS': 'CRC16-UMTS',
     'CRC16-CCITT': 'CRC16-KERMIT',
     'CRC16-CCITT-FALSE': 'CRC16-IBM-3740',
     'CRC16-CCITT-TRUE': 'CRC16-KERMIT',
@@ -168,16 +168,16 @@
     'X-CRC16': 'CRC16-DECT-X',
     'XMODEM': 'CRC16-XMODEM',
     'ZMODEM': 'CRC16-XMODEM',
     'CRC24': 'CRC24-OPENPGP',
     'B-CRC32': 'CRC32-BZIP2',
     'CRC32': 'CRC32-ISO-HDLC',
     'CRC32C': 'CRC32-ISCSI',
-    'CRC32Q': 'CRC32-AIXM',
     'CRC32D': 'CRC32-BASE91-D',
+    'CRC32Q': 'CRC32-AIXM',
     'CRC32-AAL5': 'CRC32-BZIP2',
     'CRC32-ADCCP': 'CRC32-ISO-HDLC',
     'CRC32-DECT-B': 'CRC32-BZIP2',
     'CRC32-BASE91-C': 'CRC32-ISCSI',
     'CRC32-CASTAGNOLI': 'CRC32-ISCSI',
     'CRC32-INTERLAKEN': 'CRC32-ISCSI',
     'CRC32-POSIX': 'CRC32-CKSUM',
```

### Comparing `anycrc-0.7.5/src/anycrc.egg-info/PKG-INFO` & `anycrc-0.7.6/src/anycrc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

