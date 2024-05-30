# Comparing `tmp/seawater-3.3.4.tar.gz` & `tmp/seawater-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seawater-3.3.4.tar", last modified: Fri Aug 28 10:44:19 2015, max compression
+gzip compressed data, was "seawater-3.3.5.tar", last modified: Thu May 30 19:22:40 2024, max compression
```

## Comparing `seawater-3.3.4.tar` & `seawater-3.3.5.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 filipe    (1000) users      (100)        0 2015-08-28 10:44:19.000000 seawater-3.3.4/
-drwxr-xr-x   0 filipe    (1000) users      (100)        0 2015-08-28 10:44:19.000000 seawater-3.3.4/seawater/
--rw-r--r--   0 filipe    (1000) users      (100)      373 2015-08-28 02:42:43.000000 seawater-3.3.4/seawater/__init__.py
--rw-r--r--   0 filipe    (1000) users      (100)      547 2015-07-02 13:14:30.000000 seawater-3.3.4/seawater/constants.py
--rw-r--r--   0 filipe    (1000) users      (100)    30335 2015-07-02 14:39:12.000000 seawater-3.3.4/seawater/eos80.py
--rw-r--r--   0 filipe    (1000) users      (100)     8482 2015-07-02 14:39:12.000000 seawater-3.3.4/seawater/extras.py
--rw-r--r--   0 filipe    (1000) users      (100)     8836 2015-07-02 14:39:12.000000 seawater-3.3.4/seawater/geostrophic.py
--rw-r--r--   0 filipe    (1000) users      (100)    14990 2015-07-02 14:39:12.000000 seawater-3.3.4/seawater/library.py
-drwxr-xr-x   0 filipe    (1000) users      (100)        0 2015-08-28 10:44:19.000000 seawater-3.3.4/seawater.egg-info/
--rw-r--r--   0 filipe    (1000) users      (100)     6854 2015-08-28 10:44:19.000000 seawater-3.3.4/seawater.egg-info/PKG-INFO
--rw-r--r--   0 filipe    (1000) users      (100)      352 2015-08-28 10:44:19.000000 seawater-3.3.4/seawater.egg-info/SOURCES.txt
--rw-r--r--   0 filipe    (1000) users      (100)        1 2015-08-28 10:44:19.000000 seawater-3.3.4/seawater.egg-info/dependency_links.txt
--rw-r--r--   0 filipe    (1000) users      (100)        6 2015-08-28 10:44:19.000000 seawater-3.3.4/seawater.egg-info/requires.txt
--rw-r--r--   0 filipe    (1000) users      (100)        9 2015-08-28 10:44:19.000000 seawater-3.3.4/seawater.egg-info/top_level.txt
--rw-r--r--   0 filipe    (1000) users      (100)     1970 2015-07-02 13:14:30.000000 seawater-3.3.4/CHANGES.txt
--rw-r--r--   0 filipe    (1000) users      (100)     7870 2013-08-04 01:27:56.000000 seawater-3.3.4/LICENSE.CSIRO
--rw-r--r--   0 filipe    (1000) users      (100)     1073 2013-08-03 22:23:22.000000 seawater-3.3.4/LICENSE.txt
--rw-r--r--   0 filipe    (1000) users      (100)      103 2015-07-02 13:14:30.000000 seawater-3.3.4/MANIFEST.in
--rw-r--r--   0 filipe    (1000) users      (100)     1994 2015-07-02 14:39:12.000000 seawater-3.3.4/README.rst
--rw-r--r--   0 filipe    (1000) users      (100)     2660 2015-08-28 02:42:43.000000 seawater-3.3.4/setup.py
--rw-r--r--   0 filipe    (1000) users      (100)     6854 2015-08-28 10:44:19.000000 seawater-3.3.4/PKG-INFO
--rw-r--r--   0 filipe    (1000) users      (100)       59 2015-08-28 10:44:19.000000 seawater-3.3.4/setup.cfg
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:22:40.974404 seawater-3.3.5/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1970 2024-05-30 19:22:12.000000 seawater-3.3.5/CHANGES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     7870 2024-05-30 19:22:12.000000 seawater-3.3.5/LICENSE.CSIRO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1073 2024-05-30 19:22:12.000000 seawater-3.3.5/LICENSE.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      309 2024-05-30 19:22:12.000000 seawater-3.3.5/MANIFEST.in
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     3731 2024-05-30 19:22:40.974404 seawater-3.3.5/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1668 2024-05-30 19:22:12.000000 seawater-3.3.5/README.md
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1317 2024-05-30 19:22:12.000000 seawater-3.3.5/pyproject.toml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       53 2024-05-30 19:22:12.000000 seawater-3.3.5/requirements-dev.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       12 2024-05-30 19:22:12.000000 seawater-3.3.5/requirements.txt
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:22:40.970404 seawater-3.3.5/seawater/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1012 2024-05-30 19:22:12.000000 seawater-3.3.5/seawater/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      497 2024-05-30 19:22:12.000000 seawater-3.3.5/seawater/constants.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    30281 2024-05-30 19:22:12.000000 seawater-3.3.5/seawater/eos80.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     8425 2024-05-30 19:22:12.000000 seawater-3.3.5/seawater/extras.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     8773 2024-05-30 19:22:12.000000 seawater-3.3.5/seawater/geostrophic.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    14447 2024-05-30 19:22:12.000000 seawater-3.3.5/seawater/library.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:22:40.974404 seawater-3.3.5/seawater.egg-info/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      236 2024-05-30 19:22:40.000000 seawater-3.3.5/seawater.egg-info/SOURCES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-05-30 19:22:40.974404 seawater-3.3.5/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `seawater-3.3.4/seawater/eos80.py` & `seawater-3.3.5/seawater/eos80.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-# -*- coding: utf-8 -*-
-
-
-from __future__ import division, absolute_import
-
 import numpy as np
 
 from .constants import deg2rad, earth_radius
-from .library import T90conv, T68conv, salrt, salrp, sals, seck, smow
-
+from .library import T68conv, T90conv, salrp, salrt, sals, seck, smow
 
-__all__ = ['adtg',
-           'alpha',
-           'aonb',
-           'beta',
-           'dpth',
-           'g',
-           'salt',
-           'fp',
-           'svel',
-           'pres',
-           'dens0',
-           'dens',
-           'pden',
-           'cp',
-           'ptmp',
-           'temp']
+__all__ = [
+    "adtg",
+    "alpha",
+    "aonb",
+    "beta",
+    "dpth",
+    "g",
+    "salt",
+    "fp",
+    "svel",
+    "pres",
+    "dens0",
+    "dens",
+    "pden",
+    "cp",
+    "ptmp",
+    "temp",
+]
 
 
 def adtg(s, t, p):
-    """
-    Calculates adiabatic temperature gradient as per UNESCO 1983 routines.
+    """Calculates adiabatic temperature gradient as per UNESCO 1983 routines.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature [℃ (ITS-90)]
@@ -46,43 +41,49 @@
            adiabatic temperature gradient [℃ db :sup:`-1`]
 
     Examples
     --------
     >>> # Data from UNESCO 1983 p45.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
-    >>> t = T90conv([[ 0,  0,  0,  0,  0,  0],
-    ...                 [10, 10, 10, 10, 10, 10],
-    ...                 [20, 20, 20, 20, 20, 20],
-    ...                 [30, 30, 30, 30, 30, 30],
-    ...                 [40, 40, 40, 40, 40, 40]])
-    >>> s = [[25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35]]
+    >>> t = T90conv(
+    ...     [
+    ...         [0, 0, 0, 0, 0, 0],
+    ...         [10, 10, 10, 10, 10, 10],
+    ...         [20, 20, 20, 20, 20, 20],
+    ...         [30, 30, 30, 30, 30, 30],
+    ...         [40, 40, 40, 40, 40, 40],
+    ...     ]
+    ... )
+    >>> s = [
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ... ]
     >>> p = [0, 5000, 10000, 0, 5000, 10000]
     >>> sw.adtg(s, t, p)
-    array([[  1.68710000e-05,   1.04700000e-04,   1.69426000e-04,
-              3.58030000e-05,   1.17956500e-04,   1.77007000e-04],
-           [  1.00194580e-04,   1.60959050e-04,   2.06874170e-04,
-              1.14887280e-04,   1.71364200e-04,   2.12991770e-04],
-           [  1.73819840e-04,   2.13534000e-04,   2.44483760e-04,
-              1.84273240e-04,   2.21087800e-04,   2.49137960e-04],
-           [  2.41720460e-04,   2.64764100e-04,   2.82959590e-04,
-              2.47934560e-04,   2.69466550e-04,   2.86150390e-04],
-           [  3.07870120e-04,   3.16988600e-04,   3.23006480e-04,
-              3.09844920e-04,   3.18839700e-04,   3.24733880e-04]])
+    array([[1.6871000e-05, 1.0470000e-04, 1.6942600e-04, 3.5803000e-05,
+            1.1795650e-04, 1.7700700e-04],
+           [1.0019458e-04, 1.6095905e-04, 2.0687417e-04, 1.1488728e-04,
+            1.7136420e-04, 2.1299177e-04],
+           [1.7381984e-04, 2.1353400e-04, 2.4448376e-04, 1.8427324e-04,
+            2.2108780e-04, 2.4913796e-04],
+           [2.4172046e-04, 2.6476410e-04, 2.8295959e-04, 2.4793456e-04,
+            2.6946655e-04, 2.8615039e-04],
+           [3.0787012e-04, 3.1698860e-04, 3.2300648e-04, 3.0984492e-04,
+            3.1883970e-04, 3.2473388e-04]])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] Bryden, H. 1973. New Polynomials for thermal expansion, adiabatic
        temperature gradient and potential temperature of sea water. Deep-Sea
        Res. Vol20,401-408. doi:10.1016/0011-7471(73)90063-6
 
     """
     s, t, p = list(map(np.asanyarray, (s, t, p)))
@@ -90,24 +91,29 @@
     T68 = T68conv(t)
 
     a = [3.5803e-5, 8.5258e-6, -6.836e-8, 6.6228e-10]
     b = [1.8932e-6, -4.2393e-8]
     c = [1.8741e-8, -6.7795e-10, 8.733e-12, -5.4481e-14]
     d = [-1.1351e-10, 2.7759e-12]
     e = [-4.6206e-13, 1.8676e-14, -2.1687e-16]
-    return (a[0] + (a[1] + (a[2] + a[3] * T68) * T68) * T68 +
-            (b[0] + b[1] * T68) * (s - 35) +
-            ((c[0] + (c[1] + (c[2] + c[3] * T68) * T68) * T68) +
-             (d[0] + d[1] * T68) * (s - 35)) * p +
-            (e[0] + (e[1] + e[2] * T68) * T68) * p * p)
+    return (
+        a[0]
+        + (a[1] + (a[2] + a[3] * T68) * T68) * T68
+        + (b[0] + b[1] * T68) * (s - 35)
+        + (
+            (c[0] + (c[1] + (c[2] + c[3] * T68) * T68) * T68)
+            + (d[0] + d[1] * T68) * (s - 35)
+        )
+        * p
+        + (e[0] + (e[1] + e[2] * T68) * T68) * p * p
+    )
 
 
-def alpha(s, t, p, pt=False):
-    """
-    Calculate the thermal expansion coefficient.
+def alpha(s, t, p, *, pt=False):
+    r"""Calculate the thermal expansion coefficient.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature or potential temperature [℃ (ITS-90)]
@@ -132,20 +138,19 @@
     References
     ----------
     .. [1] McDougall, Trevor J., 1987: Neutral Surfaces. J. Phys. Oceanogr.,
        17, 1950-1964. doi: 10.1175/1520-0485(1987)017<1950:NS>2.0.CO;2
 
     """
     s, t, p, pt = list(map(np.asanyarray, (s, t, p, pt)))
-    return aonb(s, t, p, pt) * beta(s, t, p, pt)
+    return aonb(s, t, p, pt=pt) * beta(s, t, p, pt=pt)
 
 
-def aonb(s, t, p, pt=False):
-    """
-    Calculate :math:`\\alpha/\\beta`.
+def aonb(s, t, p, *, pt=False):
+    r"""Calculate :math:`\\alpha/\\beta`.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature or potential temperature [℃ (ITS-90)]
@@ -169,44 +174,53 @@
 
     References
     ----------
     .. [1] McDougall, Trevor J., 1987: Neutral Surfaces. J. Phys. Oceanogr.,
        17, 1950-1964. doi: 10.1175/1520-0485(1987)017<1950:NS>2.0.CO;2
 
     """
-
     # Ensure we use ptmp in calculations.
     s, t, p, pt = list(map(np.asanyarray, (s, t, p, pt)))
 
     if not pt:
         t = ptmp(s, t, p, 0)  # Now we have ptmp.
 
-    p = np.float_(p)
+    p = np.float64(p)
     t = T68conv(t)
 
-    c1 = np.array([-0.255019e-7, 0.298357e-5, -0.203814e-3,
-                   0.170907e-1, 0.665157e-1])
+    c1 = np.array(
+        [
+            -0.255019e-7,
+            0.298357e-5,
+            -0.203814e-3,
+            0.170907e-1,
+            0.665157e-1,
+        ],
+    )
     c2 = np.array([-0.846960e-4, 0.378110e-2])
     c2a = np.array([-0.251520e-11, -0.164759e-6, 0.0])
     c3 = -0.678662e-5
     c4 = np.array([0.791325e-8, -0.933746e-6, 0.380374e-4])
     c5 = 0.512857e-12
     c6 = -0.302285e-13
 
     # Now calculate the thermal expansion saline contraction ratio aonb.
     sm35 = s - 35.0
-    return (np.polyval(c1, t) + sm35 *
-            (np.polyval(c2, t) + np.polyval(c2a, p)) +
-            sm35 ** 2 * c3 + p * np.polyval(c4, t) +
-            c5 * (p ** 2) * (t ** 2) + c6 * p ** 3)
+    return (
+        np.polyval(c1, t)
+        + sm35 * (np.polyval(c2, t) + np.polyval(c2a, p))
+        + sm35**2 * c3
+        + p * np.polyval(c4, t)
+        + c5 * (p**2) * (t**2)
+        + c6 * p**3
+    )
 
 
-def beta(s, t, p, pt=False):
-    """
-    Calculate the saline contraction coefficient :math:`\\beta` as defined
+def beta(s, t, p, *, pt=False):
+    r"""Calculate the saline contraction coefficient :math:`\\beta` as defined
     by T.J. McDougall.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
@@ -223,23 +237,22 @@
 
     Examples
     --------
     >>> # Data from McDougall 1987
     >>> import seawater as sw
     >>> s, t, p = 40, 10, 4000
     >>> sw.beta(s, t, p, pt=True)
-    0.00072087661741618932
+    0.0007208766174161893
 
     References
     ----------
     .. [1] McDougall, Trevor J., 1987: Neutral Surfaces. J. Phys. Oceanogr.,
        17, 1950-1964. doi: 10.1175/1520-0485(1987)017<1950:NS>2.0.CO;2
 
     """
-
     s, t, p, pt = list(map(np.asanyarray, (s, t, p, pt)))
 
     # Ensure we use ptmp in calculations
     if not pt:
         t = ptmp(s, t, p, 0)  # Now we have ptmp.
 
     t = T68conv(t)
@@ -250,23 +263,26 @@
     c4 = 0.515032e-8
     c5 = np.array([-0.213127e-11, 0.192867e-9, -0.121555e-7])
     c6 = np.array([-0.175379e-14, 0.176621e-12])
     c7 = 0.121551e-17
 
     # Now calculate the thermal expansion saline contraction ratio adb
     sm35 = s - 35
-    return (np.polyval(c1, t) + sm35 *
-            (np.polyval(c2, t) + np.polyval(c3, p)) +
-            c4 * (sm35 ** 2) + p * np.polyval(c5, t) +
-            (p ** 2) * np.polyval(c6, t) + c7 * (p ** 3))
+    return (
+        np.polyval(c1, t)
+        + sm35 * (np.polyval(c2, t) + np.polyval(c3, p))
+        + c4 * (sm35**2)
+        + p * np.polyval(c5, t)
+        + (p**2) * np.polyval(c6, t)
+        + c7 * (p**3)
+    )
 
 
 def cp(s, t, p):
-    """
-    Heat Capacity of Sea Water using UNESCO 1983 polynomial.
+    """Heat Capacity of Sea Water using UNESCO 1983 polynomial.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature [℃ (ITS-90)]
@@ -279,93 +295,107 @@
          specific heat capacity [J kg :sup:`-1` C :sup:`-1`]
 
     Examples
     --------
     >>> # Data from Pond and Pickard Intro. Dyn. Oceanography 2nd ed. 1986.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
-    >>> t = T90conv([[0, 0, 0, 0, 0, 0],
-    ...              [10, 10, 10, 10, 10, 10],
-    ...              [20, 20, 20, 20, 20, 20],
-    ...              [30, 30, 30, 30, 30, 30],
-    ...             [40, 40, 40, 40, 40, 40]])
-    >>> s = [[25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35]]
+    >>> t = T90conv(
+    ...     [
+    ...         [0, 0, 0, 0, 0, 0],
+    ...         [10, 10, 10, 10, 10, 10],
+    ...         [20, 20, 20, 20, 20, 20],
+    ...         [30, 30, 30, 30, 30, 30],
+    ...         [40, 40, 40, 40, 40, 40],
+    ...     ]
+    ... )
+    >>> s = [
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ... ]
     >>> p = [0, 5000, 10000, 0, 5000, 10000]
     >>> sw.cp(s, t, p)
-    array([[ 4048.4405375 ,  3896.25585   ,  3807.7330375 ,  3986.53309476,
-             3849.26094605,  3769.11791286],
-           [ 4041.8276691 ,  3919.5550066 ,  3842.3111366 ,  3986.34061786,
-             3874.72665865,  3804.415624  ],
-           [ 4044.8438591 ,  3938.5978466 ,  3866.7400391 ,  3993.85441786,
-             3894.99294519,  3828.29059113],
-           [ 4049.0984351 ,  3952.0375476 ,  3882.9855526 ,  4000.68382238,
-             3909.24271128,  3844.32151784],
-           [ 4051.2244911 ,  3966.1132036 ,  3905.9162711 ,  4003.46192541,
-             3923.89463092,  3868.28959814]])
+    array([[4048.4405375 , 3896.25585   , 3807.7330375 , 3986.53309476,
+            3849.26094605, 3769.11791286],
+           [4041.8276691 , 3919.5550066 , 3842.3111366 , 3986.34061786,
+            3874.72665865, 3804.415624  ],
+           [4044.8438591 , 3938.5978466 , 3866.7400391 , 3993.85441786,
+            3894.99294519, 3828.29059113],
+           [4049.0984351 , 3952.0375476 , 3882.9855526 , 4000.68382238,
+            3909.24271128, 3844.32151784],
+           [4051.2244911 , 3966.1132036 , 3905.9162711 , 4003.46192541,
+            3923.89463092, 3868.28959814]])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp. Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
-
     s, t, p = list(map(np.asanyarray, (s, t, p)))
 
-    p = p / 10.  # To convert [db] to [bar] as used in UNESCO routines.
+    p = p / 10.0  # To convert [db] to [bar] as used in UNESCO routines.
     T68 = T68conv(t)
 
     # Eqn. 26 p.32.
     a = (-7.64357, 0.1072763, -1.38385e-3)
     b = (0.1770383, -4.07718e-3, 5.148e-5)
     c = (4217.4, -3.720283, 0.1412855, -2.654387e-3, 2.093236e-5)
 
-    Cpst0 = ((((c[4] * T68 + c[3]) * T68 + c[2]) * T68 + c[1]) * T68 + c[0] +
-             (a[0] + a[1] * T68 + a[2] * T68 ** 2) * s +
-             (b[0] + b[1] * T68 + b[2] * T68 ** 2) * s * s ** 0.5)
+    Cpst0 = (
+        (((c[4] * T68 + c[3]) * T68 + c[2]) * T68 + c[1]) * T68
+        + c[0]
+        + (a[0] + a[1] * T68 + a[2] * T68**2) * s
+        + (b[0] + b[1] * T68 + b[2] * T68**2) * s * s**0.5
+    )
 
     # Eqn. 28 p.33.
     a = (-4.9592e-1, 1.45747e-2, -3.13885e-4, 2.0357e-6, 1.7168e-8)
     b = (2.4931e-4, -1.08645e-5, 2.87533e-7, -4.0027e-9, 2.2956e-11)
     c = (-5.422e-8, 2.6380e-9, -6.5637e-11, 6.136e-13)
 
-    del_Cp0t0 = ((((((c[3] * T68 + c[2]) * T68 + c[1]) * T68 + c[0]) * p +
-                   ((((b[4] * T68 + b[3]) * T68 + b[2]) * T68 + b[1]) *
-                    T68 + b[0])) * p + ((((a[4] * T68 + a[3]) * T68 + a[2]) *
-                                         T68 + a[1]) * T68 + a[0])) * p)
+    del_Cp0t0 = (
+        (
+            (((c[3] * T68 + c[2]) * T68 + c[1]) * T68 + c[0]) * p
+            + ((((b[4] * T68 + b[3]) * T68 + b[2]) * T68 + b[1]) * T68 + b[0])
+        )
+        * p
+        + ((((a[4] * T68 + a[3]) * T68 + a[2]) * T68 + a[1]) * T68 + a[0])
+    ) * p
 
     # Eqn 29 p.34.
     d = (4.9247e-3, -1.28315e-4, 9.802e-7, 2.5941e-8, -2.9179e-10)
     e = (-1.2331e-4, -1.517e-6, 3.122e-8)
     f = (-2.9558e-6, 1.17054e-7, -2.3905e-9, 1.8448e-11)
     g0 = 9.971e-8
     h = (5.540e-10, -1.7682e-11, 3.513e-13)
     j1 = -1.4300e-12
 
-    S3_2 = s * s ** 0.5
+    S3_2 = s * s**0.5
 
-    del_Cpstp = ((((((d[4] * T68 + d[3]) * T68 + d[2]) * T68 + d[1]) *
-                   T68 + d[0]) * s + ((e[2] * T68 + e[1]) * T68 + e[0]) *
-                  S3_2) * p +
-                 ((((f[3] * T68 + f[2]) * T68 + f[1]) * T68 + f[0]) * s +
-                  g0 * S3_2) * p ** 2 + (((h[2] * T68 + h[1]) * T68 + h[0]) *
-                                         s + j1 * T68 * S3_2) * p ** 3)
+    del_Cpstp = (
+        (
+            ((((d[4] * T68 + d[3]) * T68 + d[2]) * T68 + d[1]) * T68 + d[0]) * s
+            + ((e[2] * T68 + e[1]) * T68 + e[0]) * S3_2
+        )
+        * p
+        + ((((f[3] * T68 + f[2]) * T68 + f[1]) * T68 + f[0]) * s + g0 * S3_2) * p**2
+        + (((h[2] * T68 + h[1]) * T68 + h[0]) * s + j1 * T68 * S3_2) * p**3
+    )
 
     return Cpst0 + del_Cp0t0 + del_Cpstp
 
 
 def dens0(s, t):
-    """
-    Density of Sea Water at atmospheric pressure.
+    """Density of Sea Water at atmospheric pressure.
 
     Parameters
     ----------
     s(p=0) : array_like
              salinity [psu (PSS-78)]
     t(p=0) : array_like
              temperature [℃ (ITS-90)]
@@ -380,46 +410,47 @@
     --------
     >>> # Data from UNESCO Tech. Paper in Marine Sci. No. 44, p22
     >>> import seawater as sw
     >>> from seawater.library import T90conv
     >>> s = [0, 0, 0, 0, 35, 35, 35, 35]
     >>> t = T90conv([0, 0, 30, 30, 0, 0, 30, 30])
     >>> sw.dens0(s, t)
-    array([  999.842594  ,   999.842594  ,   995.65113374,   995.65113374,
-            1028.10633141,  1028.10633141,  1021.72863949,  1021.72863949])
+    array([ 999.842594  ,  999.842594  ,  995.65113374,  995.65113374,
+           1028.10633141, 1028.10633141, 1021.72863949, 1021.72863949])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] Millero, F.J. and  Poisson, A. International one-atmosphere
        equation of state of seawater. Deep-Sea Res. 1981. Vol28A(6) pp625-629.
        doi:10.1016/0198-0149(81)90122-9
 
     """
-
     s, t = list(map(np.asanyarray, (s, t)))
 
     T68 = T68conv(t)
 
     # UNESCO 1983 Eqn.(13) p17.
     b = (8.24493e-1, -4.0899e-3, 7.6438e-5, -8.2467e-7, 5.3875e-9)
     c = (-5.72466e-3, 1.0227e-4, -1.6546e-6)
     d = 4.8314e-4
-    return (smow(t) + (b[0] + (b[1] + (b[2] + (b[3] + b[4] * T68) * T68) *
-            T68) * T68) * s + (c[0] + (c[1] + c[2] * T68) * T68) * s *
-            s ** 0.5 + d * s ** 2)
+    return (
+        smow(t)
+        + (b[0] + (b[1] + (b[2] + (b[3] + b[4] * T68) * T68) * T68) * T68) * s
+        + (c[0] + (c[1] + c[2] * T68) * T68) * s * s**0.5
+        + d * s**2
+    )
 
 
 def dens(s, t, p):
-    """
-    Density of Sea Water using UNESCO 1983 (EOS 80) polynomial.
+    """Density of Sea Water using UNESCO 1983 (EOS 80) polynomial.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature [℃ (ITS-90)]
@@ -436,42 +467,40 @@
     >>> # Data from Unesco Tech. Paper in Marine Sci. No. 44, p22.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
     >>> s = [0, 0, 0, 0, 35, 35, 35, 35]
     >>> t = T90conv([0, 0, 30, 30, 0, 0, 30, 30])
     >>> p = [0, 10000, 0, 10000, 0, 10000, 0, 10000]
     >>> sw.dens(s, t, p)
-    array([  999.842594  ,  1045.33710972,   995.65113374,  1036.03148891,
-            1028.10633141,  1070.95838408,  1021.72863949,  1060.55058771])
+    array([ 999.842594  , 1045.33710972,  995.65113374, 1036.03148891,
+           1028.10633141, 1070.95838408, 1021.72863949, 1060.55058771])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] Millero, F.J., Chen, C.T., Bradshaw, A., and Schleicher, K. A new
        high pressure equation of state for seawater. Deap-Sea Research., 1980,
        Vol27A, pp255-264. doi:10.1016/0198-0149(80)90016-3
 
     """
-
     s, t, p = list(map(np.asanyarray, (s, t, p)))
 
     # UNESCO 1983. Eqn..7  p.15.
     densP0 = dens0(s, t)
     K = seck(s, t, p)
-    p = p / 10.  # Convert from db to atm pressure units.
+    p = p / 10.0  # Convert from db to atm pressure units.
     return densP0 / (1 - p / K)
 
 
 def dpth(p, lat):
-    """
-    Calculates depth in meters from pressure in dbars.
+    """Calculates depth in meters from pressure in dbars.
 
     Parameters
     ----------
     p : array_like
         pressure [db].
     lat : number or array_like
           latitude in decimal degrees north [-90..+90].
@@ -482,49 +511,49 @@
         depth [meters]
 
     Examples
     --------
     >>> # UNESCO 1983 data p30.
     >>> import seawater as sw
     >>> lat = [0, 30, 45, 90]
-    >>> p = [[  500,   500,   500,  500],
-    ...      [ 5000,  5000,  5000, 5000],
-    ...      [10000, 10000, 10000, 10000]]
+    >>> p = [
+    ...     [500, 500, 500, 500],
+    ...     [5000, 5000, 5000, 5000],
+    ...     [10000, 10000, 10000, 10000],
+    ... ]
     >>> sw.dpth(p, lat)
-    array([[  496.65299239,   495.99772917,   495.3427354 ,   494.03357499],
-           [ 4915.04099112,  4908.55954332,  4902.08075214,  4889.13132561],
-           [ 9725.47087508,  9712.6530721 ,  9699.84050403,  9674.23144056]])
+    array([[ 496.65299239,  495.99772917,  495.3427354 ,  494.03357499],
+           [4915.04099112, 4908.55954332, 4902.08075214, 4889.13132561],
+           [9725.47087508, 9712.6530721 , 9699.84050403, 9674.23144056]])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     p, lat = list(map(np.asanyarray, (p, lat)))
 
     # Eqn 25, p26.  UNESCO 1983.
     c = [9.72659, -2.2512e-5, 2.279e-10, -1.82e-15]
     gam_dash = 2.184e-6
 
     lat = abs(lat)
     X = np.sin(lat * deg2rad)
     X = X * X
 
-    bot_line = (9.780318 * (1.0 + (5.2788e-3 + 2.36e-5 * X) * X) +
-                gam_dash * 0.5 * p)
+    bot_line = 9.780318 * (1.0 + (5.2788e-3 + 2.36e-5 * X) * X) + gam_dash * 0.5 * p
     top_line = (((c[3] * p + c[2]) * p + c[1]) * p + c[0]) * p
     return top_line / bot_line
 
 
 def fp(s, p):
-    """
-    Freezing point of Sea Water using UNESCO 1983 polynomial.
+    """Freezing point of Sea Water using UNESCO 1983 polynomial.
 
     Parameters
     ----------
     s : array_like
         salinity [psu (PSS-78)]
     p : array_like
         pressure [db]
@@ -534,45 +563,41 @@
     fp : array_like
         freezing point temperature [℃ (ITS-90)]
 
     Examples
     --------
     >>> # UNESCO DATA p.30.
     >>> import seawater as sw
-    >>> s = [[5, 10, 15, 20, 25, 30, 35, 40],
-    ...      [5, 10, 15, 20, 25, 30, 35, 40]]
-    >>> p = [[ 0, 0, 0, 0, 0, 0, 0, 0],
-    ...      [500, 500, 500, 500, 500, 500, 500, 500]]
+    >>> s = [[5, 10, 15, 20, 25, 30, 35, 40], [5, 10, 15, 20, 25, 30, 35, 40]]
+    >>> p = [[0, 0, 0, 0, 0, 0, 0, 0], [500, 500, 500, 500, 500, 500, 500, 500]]
     >>> sw.fp(s, p)
     array([[-0.27369757, -0.54232831, -0.81142026, -1.0829461 , -1.35804594,
             -1.63748903, -1.9218401 , -2.2115367 ],
            [-0.65010724, -0.91873798, -1.18782992, -1.45935577, -1.73445561,
             -2.01389869, -2.29824976, -2.58794636]])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
-
     s, p = list(map(np.asanyarray, (s, p)))
 
     # NOTE: P = P/10 # to convert db to Bar as used in UNESCO routines.
     # Eqn  p.29.
     a = [-0.0575, 1.710523e-3, -2.154996e-4]
     b = -7.53e-4
-    return T90conv(a[0] * s + a[1] * s * s ** 0.5 + a[2] * s ** 2 + b * p)
+    return T90conv(a[0] * s + a[1] * s * s**0.5 + a[2] * s**2 + b * p)
 
 
 def g(lat, z=0):
-    """
-    Calculates acceleration due to gravity as function of latitude.
+    """Calculates acceleration due to gravity as function of latitude.
 
     Parameters
     ----------
     lat : array_like
          latitude in decimal degrees north [-90..+90].
 
     z : number or array_like. Default z = 0
@@ -583,41 +608,39 @@
     g : array_like
         gravity [m s :sup:`-2`]
 
     Examples
     --------
     >>> import seawater as sw
     >>> sw.g(45, z=0)
-    9.8061898752053995
+    9.8061898752054
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] A.E. Gill 1982. p.54  Eqn. 3.7.15 "Atmosphere-Ocean Dynamics"
        Academic Press: New York. ISBN: 0-12-283522-0
 
     """
-
     lat, z = list(map(np.asanyarray, (lat, z)))
 
     # Eqn p27.  UNESCO 1983.
     lat = np.abs(lat)
     X = np.sin(lat * deg2rad)
     sin2 = X * X
     grav = 9.780318 * (1.0 + (5.2788e-3 + 2.36e-5 * sin2) * sin2)
     return grav / ((1 + z / earth_radius) ** 2)  # From A.E.Gill p.597.
 
 
 def pden(s, t, p, pr=0):
-    """
-    Calculates potential density of water mass relative to the specified
+    r"""Calculates potential density of water mass relative to the specified
     reference pressure by pden = dens(S, ptmp, PR).
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
@@ -637,39 +660,37 @@
     >>> # Data from Unesco Tech. Paper in Marine Sci. No. 44, p22.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
     >>> s = [0, 0, 0, 0, 35, 35, 35, 35]
     >>> t = T90conv([0, 0, 30, 30, 0, 0, 30, 30])
     >>> p = [0, 10000, 0, 10000, 0, 10000, 0, 10000]
     >>> sw.pden(s, t, p)
-    array([  999.842594  ,   999.79523994,   995.65113374,   996.36115932,
-            1028.10633141,  1028.15738545,  1021.72863949,  1022.59634627])
+    array([ 999.842594  ,  999.79523994,  995.65113374,  996.36115932,
+           1028.10633141, 1028.15738545, 1021.72863949, 1022.59634627])
 
     :math:`\\sigma_{4}` (at 4000 db)
 
     >>> sw.pden(s, t, p, 4000) - 1000
-    array([ 19.2895493 ,  19.33422519,  12.43271053,  13.27563816,
-            46.30976432,  46.48818851,  37.76150878,  38.74500757])
+    array([19.2895493 , 19.33422519, 12.43271053, 13.27563816, 46.30976432,
+           46.48818851, 37.76150878, 38.74500757])
 
     References
     ----------
     .. [1] A.E. Gill 1982. p.54  Eqn. 3.7.15 "Atmosphere-Ocean Dynamics"
        Academic Press: New York. ISBN: 0-12-283522-0
 
     """
-
     s, t, p, pr = list(map(np.asanyarray, (s, t, p, pr)))
 
     pt = ptmp(s, t, p, pr)
     return dens(s, pt, pr)
 
 
 def pres(depth, lat):
-    """
-    Calculates pressure in dbars from depth in meters.
+    """Calculates pressure in dbars from depth in meters.
 
     Parameters
     ----------
     depth : array_like
             depth [meters]
     lat : array_like
           latitude in decimal degrees north [-90..+90]
@@ -679,34 +700,33 @@
     p : array_like
            pressure [db]
 
     Examples
     --------
     >>> import seawater as sw
     >>> depth, lat = 7321.45, 30
-    >>> sw.pres(depth,lat)
-    7500.0065130118019
+    >>> sw.pres(depth, lat)
+    7500.006513011802
 
     References
     ----------
     .. [1] Saunders, Peter M., 1981: Practical Conversion of Pressure to Depth.
        J. Phys. Oceanogr., 11, 573-574.
        doi: 10.1175/1520-0485(1981)011<0573:PCOPTD>2.0.CO;2
 
     """
     depth, lat = list(map(np.asanyarray, (depth, lat)))
 
     X = np.sin(np.abs(lat * deg2rad))
-    C1 = 5.92e-3 + X ** 2 * 5.25e-3
+    C1 = 5.92e-3 + X**2 * 5.25e-3
     return ((1 - C1) - (((1 - C1) ** 2) - (8.84e-6 * depth)) ** 0.5) / 4.42e-6
 
 
 def ptmp(s, t, p, pr=0):
-    """
-    Calculates potential temperature as per UNESCO 1983 report.
+    """Calculates potential temperature as per UNESCO 1983 report.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature [℃ (ITS-90)]
@@ -720,76 +740,80 @@
     pt : array_like
          potential temperature relative to PR [℃ (ITS-90)]
 
     Examples
     --------
     >>> import seawater as sw
     >>> from seawater.library import T90conv, T68conv
-    >>> t = T90conv([[0, 0, 0, 0, 0, 0],
-    ...              [10, 10, 10, 10, 10, 10],
-    ...              [20, 20, 20, 20, 20, 20],
-    ...              [30, 30, 30, 30, 30, 30],
-    ...              [40, 40, 40, 40, 40, 40]])
-    >>> s = [[25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35],
-    ...      [25, 25, 25, 35, 35, 35]]
+    >>> t = T90conv(
+    ...     [
+    ...         [0, 0, 0, 0, 0, 0],
+    ...         [10, 10, 10, 10, 10, 10],
+    ...         [20, 20, 20, 20, 20, 20],
+    ...         [30, 30, 30, 30, 30, 30],
+    ...         [40, 40, 40, 40, 40, 40],
+    ...     ]
+    ... )
+    >>> s = [
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ... ]
     >>> p = [0, 5000, 10000, 0, 5000, 10000]
     >>> T68conv(sw.ptmp(s, t, p, pr=0))
-    array([[  0.        ,  -0.30614418,  -0.96669485,   0.        ,
-             -0.3855565 ,  -1.09741136],
-           [ 10.        ,   9.35306331,   8.46840949,  10.        ,
-              9.29063461,   8.36425752],
-           [ 20.        ,  19.04376281,  17.94265   ,  20.        ,
-             18.99845171,  17.86536441],
-           [ 30.        ,  28.75124632,  27.43529911,  30.        ,
-             28.72313484,  27.38506197],
-           [ 40.        ,  38.46068173,  36.92544552,  40.        ,
-             38.44979906,  36.90231661]])
+    array([[ 0.        , -0.30614418, -0.96669485,  0.        , -0.3855565 ,
+            -1.09741136],
+           [10.        ,  9.35306331,  8.46840949, 10.        ,  9.29063461,
+             8.36425752],
+           [20.        , 19.04376281, 17.94265   , 20.        , 18.99845171,
+            17.86536441],
+           [30.        , 28.75124632, 27.43529911, 30.        , 28.72313484,
+            27.38506197],
+           [40.        , 38.46068173, 36.92544552, 40.        , 38.44979906,
+            36.90231661]])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] Bryden, H. 1973. New Polynomials for thermal expansion, adiabatic
        temperature gradient and potential temperature of sea water. Deep-Sea
        Res. Vol20,401-408. doi:10.1016/0011-7471(73)90063-6
 
     """
-
     s, t, p, pr = list(map(np.asanyarray, (s, t, p, pr)))
 
     # Theta1.
     del_P = pr - p
     del_th = del_P * adtg(s, t, p)
     th = T68conv(t) + 0.5 * del_th
     q = del_th
 
     # Theta2.
     del_th = del_P * adtg(s, T90conv(th), p + 0.5 * del_P)
-    th = th + (1 - 1 / 2 ** 0.5) * (del_th - q)
-    q = (2 - 2 ** 0.5) * del_th + (-2 + 3 / 2 ** 0.5) * q
+    th = th + (1 - 1 / 2**0.5) * (del_th - q)
+    q = (2 - 2**0.5) * del_th + (-2 + 3 / 2**0.5) * q
 
     # Theta3.
     del_th = del_P * adtg(s, T90conv(th), p + 0.5 * del_P)
-    th = th + (1 + 1 / 2 ** 0.5) * (del_th - q)
-    q = (2 + 2 ** 0.5) * del_th + (-2 - 3 / 2 ** 0.5) * q
+    th = th + (1 + 1 / 2**0.5) * (del_th - q)
+    q = (2 + 2**0.5) * del_th + (-2 - 3 / 2**0.5) * q
 
     # Theta4.
     del_th = del_P * adtg(s, T90conv(th), p + del_P)
     return T90conv(th + (del_th - 2 * q) / 6)
 
 
 def salt(r, t, p):
-    """
-    Calculates Salinity from conductivity ratio. UNESCO 1983 polynomial.
+    r"""Calculates Salinity from conductivity ratio. UNESCO 1983 polynomial.
 
     Parameters
     ----------
     r : array_like
         conductivity ratio :math:`R = \\frac{C(S,T,P)}{C(35,15(IPTS-68),0)}`
     t : array_like
         temperature [℃ (ITS-90)]
@@ -806,35 +830,34 @@
     Data from UNESCO 1983 p9.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
     >>> r = [1, 1.2, 0.65]
     >>> t = T90conv([15, 20, 5])
     >>> p = [0, 2000, 1500]
     >>> sw.salt(r, t, p)
-    array([ 34.99999992,  37.24562765,  27.99534693])
+    array([34.99999992, 37.24562765, 27.99534693])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983.  Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap.
        in Mar. Sci., No. 44, 53 pp. Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     r, t, p = list(map(np.asanyarray, (r, t, p)))
 
     rt = salrt(t)
     rp = salrp(r, t, p)
     rt = r / (rp * rt)
     return sals(rt, t)
 
 
 def svel(s, t, p):
-    """
-    Sound Velocity in sea water using UNESCO 1983 polynomial.
+    """Sound Velocity in sea water using UNESCO 1983 polynomial.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature [℃ (ITS-90)]
@@ -848,93 +871,136 @@
 
     Examples
     --------
     Data from Pond and Pickard Intro. Dynamical Oceanography 2nd ed. 1986
 
     >>> import seawater as sw
     >>> from seawater.library import T90conv
-    >>> t = T90conv([[  0,  0,  0,  0,  0,  0],
-    ...              [ 10, 10, 10, 10, 10, 10],
-    ...              [ 20, 20, 20, 20, 20, 20],
-    ...              [ 30, 30, 30, 30, 30, 30],
-    ...              [ 40, 40, 40, 40, 40, 40]])
-    >>> s = [[ 25, 25, 25, 35, 35, 35],
-    ...      [ 25, 25, 25, 35, 35, 35],
-    ...      [ 25, 25, 25, 35, 35, 35],
-    ...      [ 25, 25, 25, 35, 35, 35],
-    ...      [ 25, 25, 25, 35, 35, 35]]
-    >>> p = [ 0, 5000, 10000, 0, 5000, 10000]
+    >>> t = T90conv(
+    ...     [
+    ...         [0, 0, 0, 0, 0, 0],
+    ...         [10, 10, 10, 10, 10, 10],
+    ...         [20, 20, 20, 20, 20, 20],
+    ...         [30, 30, 30, 30, 30, 30],
+    ...         [40, 40, 40, 40, 40, 40],
+    ...     ]
+    ... )
+    >>> s = [
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ...     [25, 25, 25, 35, 35, 35],
+    ... ]
+    >>> p = [0, 5000, 10000, 0, 5000, 10000]
     >>> sw.svel(s, t, p)
-    array([[ 1435.789875  ,  1520.358725  ,  1610.4074    ,  1449.13882813,
-             1533.96863705,  1623.15007097],
-           [ 1477.68316464,  1561.30635914,  1647.39267114,  1489.82233602,
-             1573.40946928,  1658.99115504],
-           [ 1510.31388348,  1593.59671798,  1676.80967748,  1521.4619731 ,
-             1604.4762822 ,  1687.18305631],
-           [ 1535.21434752,  1618.95631952,  1700.60547902,  1545.59485539,
-             1628.97322783,  1710.06294277],
-           [ 1553.44506636,  1638.02522336,  1719.15088536,  1563.20925247,
-             1647.29949576,  1727.83176404]])
+    array([[1435.789875  , 1520.358725  , 1610.4074    , 1449.13882813,
+            1533.96863705, 1623.15007097],
+           [1477.68316464, 1561.30635914, 1647.39267114, 1489.82233602,
+            1573.40946928, 1658.99115504],
+           [1510.31388348, 1593.59671798, 1676.80967748, 1521.4619731 ,
+            1604.4762822 , 1687.18305631],
+           [1535.21434752, 1618.95631952, 1700.60547902, 1545.59485539,
+            1628.97322783, 1710.06294277],
+           [1553.44506636, 1638.02522336, 1719.15088536, 1563.20925247,
+            1647.29949576, 1727.83176404]])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     s, t, p = list(map(np.asanyarray, (s, t, p)))
 
     # UNESCO 1983. Eqn..33  p.46.
     p = p / 10  # Convert db to bars as used in UNESCO routines.
     T68 = T68conv(t)
 
     # Eqn 34 p.46.
-    c00, c01, c02, c03, c04, c05 = (1402.388, 5.03711, -5.80852e-2, 3.3420e-4,
-                                    -1.47800e-6, 3.1464e-9)
-    c10, c11, c12, c13, c14 = (0.153563, 6.8982e-4, -8.1788e-6, 1.3621e-7,
-                               -6.1185e-10)
-    c20, c21, c22, c23, c24 = (3.1260e-5, -1.7107e-6, 2.5974e-8, -2.5335e-10,
-                               1.0405e-12)
+    c00, c01, c02, c03, c04, c05 = (
+        1402.388,
+        5.03711,
+        -5.80852e-2,
+        3.3420e-4,
+        -1.47800e-6,
+        3.1464e-9,
+    )
+    c10, c11, c12, c13, c14 = (
+        0.153563,
+        6.8982e-4,
+        -8.1788e-6,
+        1.3621e-7,
+        -6.1185e-10,
+    )
+    c20, c21, c22, c23, c24 = (
+        3.1260e-5,
+        -1.7107e-6,
+        2.5974e-8,
+        -2.5335e-10,
+        1.0405e-12,
+    )
     c30, c31, c32 = (-9.7729e-9, 3.8504e-10, -2.3643e-12)
 
-    Cw = (((((c32 * T68 + c31) * T68 + c30) * p +
-            ((((c24 * T68 + c23) * T68 + c22) * T68 + c21) * T68 + c20)) * p +
-           ((((c14 * T68 + c13) * T68 + c12) * T68 + c11) * T68 + c10)) *
-          p + ((((c05 * T68 + c04) * T68 + c03) * T68 + c02) * T68 + c01) *
-          T68 + c00)
+    Cw = (
+        (
+            (
+                ((c32 * T68 + c31) * T68 + c30) * p
+                + ((((c24 * T68 + c23) * T68 + c22) * T68 + c21) * T68 + c20)
+            )
+            * p
+            + ((((c14 * T68 + c13) * T68 + c12) * T68 + c11) * T68 + c10)
+        )
+        * p
+        + ((((c05 * T68 + c04) * T68 + c03) * T68 + c02) * T68 + c01) * T68
+        + c00
+    )
 
     # Eqn. 35. p.47
     a00, a01, a02, a03, a04 = (1.389, -1.262e-2, 7.164e-5, 2.006e-6, -3.21e-8)
-    a10, a11, a12, a13, a14 = (9.4742e-5, -1.2580e-5, -6.4885e-8, 1.0507e-8,
-                               -2.0122e-10)
+    a10, a11, a12, a13, a14 = (
+        9.4742e-5,
+        -1.2580e-5,
+        -6.4885e-8,
+        1.0507e-8,
+        -2.0122e-10,
+    )
     a20, a21, a22, a23 = (-3.9064e-7, 9.1041e-9, -1.6002e-10, 7.988e-12)
     a30, a31, a32 = (1.100e-10, 6.649e-12, -3.389e-13)
 
-    A = (((((a32 * T68 + a31) * T68 + a30) * p +
-           (((a23 * T68 + a22) * T68 + a21) * T68 + a20)) * p +
-          ((((a14 * T68 + a13) * T68 + a12) * T68 + a11) * T68 + a10)) * p +
-         (((a04 * T68 + a03) * T68 + a02) * T68 + a01) * T68 + a00)
+    A = (
+        (
+            (
+                ((a32 * T68 + a31) * T68 + a30) * p
+                + (((a23 * T68 + a22) * T68 + a21) * T68 + a20)
+            )
+            * p
+            + ((((a14 * T68 + a13) * T68 + a12) * T68 + a11) * T68 + a10)
+        )
+        * p
+        + (((a04 * T68 + a03) * T68 + a02) * T68 + a01) * T68
+        + a00
+    )
 
     # Eqn 36 p.47.
     b00, b01, b10, b11 = -1.922e-2, -4.42e-5, 7.3637e-5, 1.7945e-7
     B = b00 + b01 * T68 + (b10 + b11 * T68) * p
 
     # Eqn 37 p.47.
     d00, d10 = 1.727e-3, -7.9836e-6
     D = d00 + d10 * p
 
     # Eqn 33 p.46.
-    return Cw + A * s + B * s * s ** 0.5 + D * s ** 2
+    return Cw + A * s + B * s * s**0.5 + D * s**2
 
 
 def temp(s, pt, p, pr=0):
-    """
-    Calculates temperature from potential temperature at the reference
+    """Calculates temperature from potential temperature at the reference
     pressure PR and in situ pressure P.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     pt(p) : array_like
@@ -957,15 +1023,15 @@
     15.0
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] Bryden, H. 1973. New Polynomials for thermal expansion, adiabatic
        temperature gradient and potential temperature of sea water. Deep-Sea
        Res.  Vol20,401-408. doi:10.1016/0011-7471(73)90063-6
 
     """
     s, pt, p, pr = list(map(np.asanyarray, (s, pt, p, pr)))
```

### Comparing `seawater-3.3.4/seawater/extras.py` & `seawater-3.3.5/seawater/extras.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-# -*- coding: utf-8 -*-
-
-
-from __future__ import division, absolute_import
-
 import numpy as np
+
+from .constants import DEG2NM, NM2KM, OMEGA, Kelvin, deg2rad, gdef, rad2deg
 from .library import T68conv
-from .constants import OMEGA, DEG2NM, NM2KM, Kelvin, deg2rad, rad2deg, gdef
 
-__all__ = ['dist',
-           'f',
-           'satAr',
-           'satN2',
-           'satO2',
-           'swvel']
+__all__ = [
+    "dist",
+    "f",
+    "satAr",
+    "satN2",
+    "satO2",
+    "swvel",
+]
 
 
-def dist(lat, lon, units='km'):
-    """
-    Calculate distance between two positions on globe using the "Plane
+def dist(lat, lon, units="km"):
+    """Calculate distance between two positions on globe using the "Plane
     Sailing" method. Also uses simple geometry to calculate the bearing of
     the path between position pairs.
 
     Parameters
     ----------
     lat : array_like
           decimal degrees (+ve N, -ve S) [- 90.. +90]
@@ -38,62 +35,61 @@
                  angle of line between stations with x axis (East).
                  Range of values are -180..+180. (E=0, N=90, S=-90)
 
     Examples
     --------
     >>> import seawater as sw
     >>> sw.dist(0, [-179, 180])
-    (array([ 111.12]), array([ 180.]))
+    (array([111.12]), array([180.]))
     >>> lon = [35, 35]
     >>> lat = [41, 40]
     >>> sw.dist(lat, lon)
-    (array([ 111.12]), array([-90.]))
+    (array([111.12]), array([-90.]))
     >>> # Create a distance vector.
-    >>> lon = np.arange(30,40,1)
+    >>> lon = np.arange(30, 40, 1)
     >>> lat = 35
-    >>> np.cumsum(np.append(0, sw.dist(lat, lon, units='km')[0]))
-    array([   0.        ,   91.02417516,  182.04835032,  273.07252548,
-            364.09670065,  455.12087581,  546.14505097,  637.16922613,
-            728.19340129,  819.21757645])
+    >>> np.cumsum(np.append(0, sw.dist(lat, lon, units="km")[0]))
+    array([  0.        ,  91.02417516, 182.04835032, 273.07252548,
+           364.09670065, 455.12087581, 546.14505097, 637.16922613,
+           728.19340129, 819.21757645])
 
     References
     ----------
     .. [1] The PLANE SAILING method as described in "CELESTIAL NAVIGATION" 1989
        by Dr. P. Gormley. The Australian Antarctic Division.
 
     """
-
     lon, lat = list(map(np.asanyarray, (lon, lat)))
     lon, lat = np.broadcast_arrays(lon, lat)
 
     npositions = max(lon.shape)
 
     ind = np.arange(0, npositions - 1, 1)  # Index to first of position pairs.
 
     dlon = np.diff(lon, axis=0)
-    if np.any(np.abs(dlon) > 180):
-        flag = abs(dlon) > 180
-        dlon[flag] = -np.sign(dlon[flag]) * (360 - np.abs(dlon[flag]))
+    lon180, lon360 = 180, 360
+    if np.any(np.abs(dlon) > lon180):
+        flag = abs(dlon) > lon180
+        dlon[flag] = -np.sign(dlon[flag]) * (lon360 - np.abs(dlon[flag]))
 
     latrad = np.abs(lat * deg2rad)
     dep = np.cos((latrad[ind + 1] + latrad[ind]) / 2) * dlon
     dlat = np.diff(lat, axis=0)
-    dist = DEG2NM * (dlat ** 2 + dep ** 2) ** 0.5
+    dist = DEG2NM * (dlat**2 + dep**2) ** 0.5
 
-    if units == 'km':
+    if units == "km":
         dist = dist * NM2KM
 
     # Calculate angle to x axis.
     phaseangle = np.angle(dep + dlat * 1j) * rad2deg
     return dist, phaseangle
 
 
 def f(lat):
-    """
-    Calculates the Coriolis factor :math:`f` defined by:
+    r"""Calculates the Coriolis factor :math:`f` defined by:
 
     .. math::
         f = 2 \\Omega \\sin(lat)
 
     where:
 
     .. math::
@@ -132,16 +128,15 @@
     """
     lat = np.asanyarray(lat)
     # Eqn p27.  UNESCO 1983.
     return 2 * OMEGA * np.sin(lat * deg2rad)
 
 
 def satAr(s, t):
-    """
-    Solubility (saturation) of Argon (Ar) in sea water.
+    """Solubility (saturation) of Argon (Ar) in sea water.
 
     Parameters
     ----------
     s : array_like
         salinity [psu (PSS-78)]
     t : array_like
         temperature [℃ (ITS-90)]
@@ -152,49 +147,52 @@
             solubility of Ar [ml l :sup:`-1`]
 
     Examples
     --------
     >>> # Data from Weiss 1970.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
-    >>> t = T90conv([[ -1, -1], [ 10, 10], [ 20, 20], [ 40, 40]])
-    >>> s = [[ 20, 40], [ 20, 40], [ 20, 40], [ 20, 40]]
+    >>> t = T90conv([[-1, -1], [10, 10], [20, 20], [40, 40]])
+    >>> s = [[20, 40], [20, 40], [20, 40], [20, 40]]
     >>> sw.satAr(s, t)
-    array([[ 0.4455784 ,  0.38766011],
-           [ 0.33970659,  0.29887756],
-           [ 0.27660227,  0.24566428],
-           [ 0.19861429,  0.17937698]])
+    array([[0.4455784 , 0.38766011],
+           [0.33970659, 0.29887756],
+           [0.27660227, 0.24566428],
+           [0.19861429, 0.17937698]])
 
     References
     ----------
     .. [1] Weiss, R. F. 1970. The Solubility of Nitrogen, Oxygen and Argon in
        Water and Seawater Deep-Sea Research Vol. 17, p. 721-735.
        doi:10.1016/0011-7471(70)90037-9
 
     """
-
     s, t = list(map(np.asanyarray, (s, t)))
 
     # Convert T to Kelvin.
     t = Kelvin + T68conv(t)
 
     # Constants for Eqn (4) of Weiss 1970.
     a = [-173.5146, 245.4510, 141.8222, -21.8020]
     b = [-0.034474, 0.014934, -0.0017729]
 
     # Eqn (4) of Weiss 1970.
-    lnC = (a[0] + a[1] * (100 / t) + a[2] * np.log(t / 100) + a[3] *
-           (t / 100) + s * (b[0] + b[1] * (t / 100) + b[2] * ((t / 100) ** 2)))
+    lnC = (
+        a[0]
+        + a[1] * (100 / t)
+        + a[2] * np.log(t / 100)
+        + a[3] * (t / 100)
+        + s * (b[0] + b[1] * (t / 100) + b[2] * ((t / 100) ** 2))
+    )
 
     return np.exp(lnC)
 
 
 def satN2(s, t):
-    """
-    Solubility (saturation) of Nitrogen (N2) in sea water.
+    """Solubility (saturation) of Nitrogen (N2) in sea water.
 
     Parameters
     ----------
     s : array_like
         salinity [psu (PSS-78)]
     t : array_like
         temperature [℃ (ITS-90)]
@@ -205,50 +203,52 @@
             solubility of N2  [ml l :sup:`-1`]
 
     Examples
     --------
     >>> # Data from Weiss 1970.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
-    >>> t = T90conv([[ -1, -1], [ 10, 10], [ 20, 20], [ 40, 40]])
-    >>> s = [[ 20, 40], [ 20, 40], [ 20, 40], [ 20, 40]]
+    >>> t = T90conv([[-1, -1], [10, 10], [20, 20], [40, 40]])
+    >>> s = [[20, 40], [20, 40], [20, 40], [20, 40]]
     >>> sw.satN2(s, t)
-    array([[ 16.27952432,  14.00784526],
-           [ 12.64036196,  11.01277257],
-           [ 10.46892822,   9.21126859],
-           [  7.78163876,   6.95395099]])
-
+    array([[16.27952432, 14.00784526],
+           [12.64036196, 11.01277257],
+           [10.46892822,  9.21126859],
+           [ 7.78163876,  6.95395099]])
 
     References
     ----------
     .. [1] Weiss, R. F. 1970. The Solubility of Nitrogen, Oxygen and Argon in
        Water and Seawater Deep-Sea Research Vol. 17, p. 721-735.
        doi:10.1016/0011-7471(70)90037-9
 
     """
-
     s, t = list(map(np.asanyarray, (s, t)))
 
     # Convert T to Kelvin.
     t = Kelvin + T68conv(t)
 
     # Constants for Eqn (4) of Weiss 1970.
     a = (-172.4965, 248.4262, 143.0738, -21.7120)
     b = (-0.049781, 0.025018, -0.0034861)
 
     # Eqn (4) of Weiss 1970.
-    lnC = (a[0] + a[1] * (100 / t) + a[2] * np.log(t / 100) + a[3] *
-           (t / 100) + s * (b[0] + b[1] * (t / 100) + b[2] * ((t / 100) ** 2)))
+    lnC = (
+        a[0]
+        + a[1] * (100 / t)
+        + a[2] * np.log(t / 100)
+        + a[3] * (t / 100)
+        + s * (b[0] + b[1] * (t / 100) + b[2] * ((t / 100) ** 2))
+    )
 
     return np.exp(lnC)
 
 
 def satO2(s, t):
-    """
-    Solubility (saturation) of Oxygen (O2) in sea water.
+    """Solubility (saturation) of Oxygen (O2) in sea water.
 
     Parameters
     ----------
     s : array_like
         salinity [psu (PSS-78)]
     t : array_like
         temperature [℃ (ITS-68)]
@@ -259,49 +259,52 @@
             solubility of O2  [ml l :sup:`-1` ]
 
     Examples
     --------
     >>> # Data from Weiss 1970.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
-    >>> t = T90conv([[ -1, -1], [ 10, 10], [ 20, 20], [ 40, 40]])
-    >>> s = [[ 20, 40], [ 20, 40], [ 20, 40], [ 20, 40]]
+    >>> t = T90conv([[-1, -1], [10, 10], [20, 20], [40, 40]])
+    >>> s = [[20, 40], [20, 40], [20, 40], [20, 40]]
     >>> sw.satO2(s, t)
-    array([[ 9.162056  ,  7.98404249],
-           [ 6.95007741,  6.12101928],
-           [ 5.64401453,  5.01531004],
-           [ 4.0495115 ,  3.65575811]])
+    array([[9.162056  , 7.98404249],
+           [6.95007741, 6.12101928],
+           [5.64401453, 5.01531004],
+           [4.0495115 , 3.65575811]])
 
     References
     ----------
     .. [1] Weiss, R. F. 1970. The Solubility of Nitrogen, Oxygen and Argon in
        Water and Seawater Deep-Sea Research Vol. 17, p. 721-735.
        doi:10.1016/0011-7471(70)90037-9
 
     """
-
     s, t = list(map(np.asanyarray, (s, t)))
 
     # Convert T to Kelvin.
     t = Kelvin + T68conv(t)
 
     # Constants for Eqn (4) of Weiss 1970.
     a = (-173.4292, 249.6339, 143.3483, -21.8492)
     b = (-0.033096, 0.014259, -0.0017000)
 
     # Eqn (4) of Weiss 1970.
-    lnC = (a[0] + a[1] * (100 / t) + a[2] * np.log(t / 100) + a[3] *
-           (t / 100) + s * (b[0] + b[1] * (t / 100) + b[2] * ((t / 100) ** 2)))
+    lnC = (
+        a[0]
+        + a[1] * (100 / t)
+        + a[2] * np.log(t / 100)
+        + a[3] * (t / 100)
+        + s * (b[0] + b[1] * (t / 100) + b[2] * ((t / 100) ** 2))
+    )
 
     return np.exp(lnC)
 
 
 def swvel(length, depth):
-    """
-    Calculates surface wave velocity.
+    """Calculates surface wave velocity.
 
     length : array_like
             wave length
     depth : array_like
             water depth [meters]
 
     Returns
@@ -309,13 +312,13 @@
     speed : array_like
             surface wave speed [m s :sup:`-1`]
 
     Examples
     --------
     >>> import seawater as sw
     >>> sw.swvel(10, 100)
-    3.9493270848342941
+    3.949327084834294
 
     """
     length, depth = list(map(np.asanyarray, (length, depth)))
     k = 2.0 * np.pi / length
     return np.sqrt(gdef * np.tanh(k * depth) / k)
```

### Comparing `seawater-3.3.4/seawater/geostrophic.py` & `seawater-3.3.5/seawater/geostrophic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# -*- coding: utf-8 -*-
-
-
-from __future__ import division, absolute_import
-
 import numpy as np
 
+from .constants import db2Pascal, gdef
+from .eos80 import dens, dpth, g, pden
 from .extras import dist, f
 from .library import atleast_2d
-from .eos80 import dens, dpth, g, pden
-from .constants import db2Pascal, gdef
 
-__all__ = ['bfrq',
-           'svan',
-           'gpan',
-           'gvel']
+__all__ = [
+    "bfrq",
+    "svan",
+    "gpan",
+    "gvel",
+]
 
 
 def bfrq(s, t, p, lat=None):
-    """
-    Calculates Brünt-Väisälä Frequency squared (N :sup:`2`) at the mid
+    r"""Calculates Brünt-Väisälä Frequency squared (N :sup:`2`) at the mid
     depths from the equation:
 
     .. math::
         N^{2} = \\frac{-g}{\\sigma_{\\theta}} \\frac{d\\sigma_{\\theta}}{dz}
 
     Also calculates Potential Vorticity from:
 
@@ -50,69 +46,67 @@
            planetary potential vorticity (M-1xN)  [ m s :sup:`-1`]
     p_ave : array_like
             mid pressure between P grid (M-1xN) [db]
 
     Examples
     --------
     >>> import seawater as sw
-    >>> s = [[0, 0, 0], [15, 15, 15], [30, 30, 30],[35,35,35]]
-    >>> t = [[15]*3]*4
+    >>> s = [[0, 0, 0], [15, 15, 15], [30, 30, 30], [35, 35, 35]]
+    >>> t = [[15] * 3] * 4
     >>> p = [[0], [250], [500], [1000]]
-    >>> lat = [30,32,35]
+    >>> lat = [30, 32, 35]
     >>> sw.bfrq(s, t, p, lat)[0]
-    array([[  4.51543648e-04,   4.51690708e-04,   4.51920753e-04],
-           [  4.45598092e-04,   4.45743207e-04,   4.45970207e-04],
-           [  7.40996788e-05,   7.41238078e-05,   7.41615525e-05]])
+    array([[4.51543648e-04, 4.51690708e-04, 4.51920753e-04],
+           [4.45598092e-04, 4.45743207e-04, 4.45970207e-04],
+           [7.40996788e-05, 7.41238078e-05, 7.41615525e-05]])
 
     References
     ----------
     .. [1] A.E. Gill 1982. p.54  Eqn. 3.7.15 "Atmosphere-Ocean Dynamics"
        Academic Press: New York. ISBN: 0-12-283522-0
 
     .. [2] Jackett, David R., Trevor J. Mcdougall, 1995: Minimal Adjustment of
        Hydrographic Profiles to Achieve Static Stability. J. Atmos. Oceanic
        Technol., 12, 381-389.
        doi: 10.1175/1520-0426(1995)012<0381:MAOHPT>2.0.CO;2
 
     """
-
     s, t, p = list(map(np.asanyarray, (s, t, p)))
     s, t, p = np.broadcast_arrays(s, t, p)
     s, t, p = list(map(atleast_2d, (s, t, p)))
 
     if lat is None:
-        z, cor, grav = p, np.NaN, np.ones(p.shape) * gdef
+        z, cor, grav = p, np.nan, np.ones(p.shape) * gdef
     else:
         lat = np.asanyarray(lat)
         z = dpth(p, lat)
         grav = g(lat, -z)  # -z because `grav` expects height as argument.
         cor = f(lat)
 
-    p_ave = (p[0:-1, ...] + p[1:, ...]) / 2.
+    p_ave = (p[0:-1, ...] + p[1:, ...]) / 2.0
 
     pden_up = pden(s[0:-1, ...], t[0:-1, ...], p[0:-1, ...], p_ave)
     pden_lo = pden(s[1:, ...], t[1:, ...], p[1:, ...], p_ave)
 
-    mid_pden = (pden_up + pden_lo) / 2.
+    mid_pden = (pden_up + pden_lo) / 2.0
     dif_pden = pden_up - pden_lo
 
-    mid_g = (grav[0:-1, ...] + grav[1:, ...]) / 2.
+    mid_g = (grav[0:-1, ...] + grav[1:, ...]) / 2.0
 
     dif_z = np.diff(z, axis=0)
 
     n2 = -mid_g * dif_pden / (dif_z * mid_pden)
 
     q = -cor * dif_pden / (dif_z * mid_pden)
 
     return n2, q, p_ave
 
 
 def svan(s, t, p=0):
-    """
-    Specific Volume Anomaly calculated as
+    """Specific Volume Anomaly calculated as
     svan = 1 / dens(s, t, p) - 1 / dens(35, 0, p).
 
     Note that it is often quoted in literature as 1e8 * units.
 
     Parameters
     ----------
     s(p) : array_like
@@ -129,40 +123,39 @@
 
     Examples
     --------
     >>> # Data from Unesco Tech. Paper in Marine Sci. No. 44, p22.
     >>> import seawater as sw
     >>> from seawater.library import T90conv
     >>> s = [[0, 1, 2], [15, 16, 17], [30, 31, 32], [35, 35, 35]]
-    >>> t = T90conv([[15]*3]*4)
+    >>> t = T90conv([[15] * 3] * 4)
     >>> p = [[0], [250], [500], [1000]]
     >>> sw.svan(s, t, p)
-    array([[  2.82371949e-05,   2.74626498e-05,   2.66921126e-05],
-           [  1.68453274e-05,   1.60993333e-05,   1.53543515e-05],
-           [  5.80768118e-06,   5.07784980e-06,   4.34876387e-06],
-           [  2.30490099e-06,   2.30490099e-06,   2.30490099e-06]])
+    array([[2.82371949e-05, 2.74626498e-05, 2.66921126e-05],
+           [1.68453274e-05, 1.60993333e-05, 1.53543515e-05],
+           [5.80768118e-06, 5.07784980e-06, 4.34876387e-06],
+           [2.30490099e-06, 2.30490099e-06, 2.30490099e-06]])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] S. Pond & G.Pickard 2nd Edition 1986 Introductory Dynamical
        Oceanography Pergamon Press Sydney. ISBN 0-08-028728-X
 
     """
     s, t, p = list(map(np.asanyarray, (s, t, p)))
     return 1 / dens(s, t, p) - 1 / dens(35, 0, p)
 
 
 def gpan(s, t, p):
-    """
-    Geopotential Anomaly calculated as the integral of svan from the
+    """Geopotential Anomaly calculated as the integral of svan from the
     the sea surface to the bottom. THUS RELATIVE TO SEA SURFACE.
 
     Adapted method from Pond and Pickard (p76) to calculate gpan relative to
     sea surface whereas Pond and Pickard calculated relative to the deepest
     common depth.  Note that older literature may use units of "dynamic
     decimeter" for above.
 
@@ -183,47 +176,45 @@
            [m :sup:`3` kg :sup:`-1`
            Pa = m :sup:`2` s :sup:`-2` = J kg :sup:`-1`]
 
     Examples
     --------
     >>> # Data from Unesco Tech. Paper in Marine Sci. No. 44, p22.
     >>> import seawater as sw
-    >>> s = [[0, 1, 2], [15, 16, 17], [30, 31, 32], [35,35,35]]
-    >>> t = [[15]*3]*4
+    >>> s = [[0, 1, 2], [15, 16, 17], [30, 31, 32], [35, 35, 35]]
+    >>> t = [[15] * 3] * 4
     >>> p = [[0], [250], [500], [1000]]
     >>> sw.gpan(s, t, p)
-    array([[   0.        ,    0.        ,    0.        ],
-           [  56.35465209,   54.45399428,   52.55961152],
-           [  84.67266947,   80.92724333,   77.19028933],
-           [ 104.95799186,   99.38799979,   93.82834339]])
+    array([[  0.        ,   0.        ,   0.        ],
+           [ 56.35465209,  54.45399428,  52.55961152],
+           [ 84.67266947,  80.92724333,  77.19028933],
+           [104.95799186,  99.38799979,  93.82834339]])
 
     References
     ----------
     .. [1] S. Pond & G.Pickard 2nd Edition 1986 Introductory Dynamical
        Oceanography Pergamon Press Sydney. ISBN 0-08-028728-X
 
     """
-
     s, t, p = list(map(np.asanyarray, (s, t, p)))
     s, t, p = np.broadcast_arrays(s, t, p)
     s, t, p = list(map(atleast_2d, (s, t, p)))
 
     svn = svan(s, t, p)
 
     # NOTE: Assumes that pressure is the first dimension!
-    mean_svan = (svn[1:, ...] + svn[0:-1, ...]) / 2.
+    mean_svan = (svn[1:, ...] + svn[0:-1, ...]) / 2.0
     top = svn[0, ...] * p[0, ...] * db2Pascal
     bottom = (mean_svan * np.diff(p, axis=0)) * db2Pascal
     ga = np.concatenate((top[None, ...], bottom), axis=0)
     return np.cumsum(ga, axis=0).squeeze()
 
 
 def gvel(ga, lat, lon):
-    """
-    Calculates geostrophic velocity given the geopotential anomaly and
+    """Calculates geostrophic velocity given the geopotential anomaly and
     position of each station.
 
     Parameters
     ----------
     ga : array_like
          geopotential anomaly relative to the sea surface.
     lat : array_like
@@ -239,41 +230,52 @@
 
     Examples
     --------
     >>> import numpy as np
     >>> import seawater as sw
     >>> lon = np.array([-30, -30, -30, -30, -30])
     >>> lat = np.linspace(-22, -21, 5)
-    >>> t = np.array([[0,  0,  0,  0,  0],
-    ...               [10, 10, 10, 10, 10],
-    ...               [20, 20, 20, 20, 20],
-    ...               [30, 30, 30, 30, 30],
-    ...               [40, 40, 40, 40, 40]])
-    >>> s = np.array([[25, 25, 25, 35, 35],
-    ...               [25, 25, 25, 35, 35],
-    ...               [25, 25, 25, 35, 35],
-    ...               [25, 25, 25, 35, 35],
-    ...               [25, 25, 25, 35, 35]])
-    >>> p = np.array([[0, 5000, 10000, 0, 5000],
-    ...               [0, 5000, 10000, 0, 5000],
-    ...               [0, 5000, 10000, 0, 5000],
-    ...               [0, 5000, 10000, 0, 5000],
-    ...               [0, 5000, 10000, 0, 5000]])
+    >>> t = np.array(
+    ...     [
+    ...         [0, 0, 0, 0, 0],
+    ...         [10, 10, 10, 10, 10],
+    ...         [20, 20, 20, 20, 20],
+    ...         [30, 30, 30, 30, 30],
+    ...         [40, 40, 40, 40, 40],
+    ...     ]
+    ... )
+    >>> s = np.array(
+    ...     [
+    ...         [25, 25, 25, 35, 35],
+    ...         [25, 25, 25, 35, 35],
+    ...         [25, 25, 25, 35, 35],
+    ...         [25, 25, 25, 35, 35],
+    ...         [25, 25, 25, 35, 35],
+    ...     ]
+    ... )
+    >>> p = np.array(
+    ...     [
+    ...         [0, 5000, 10000, 0, 5000],
+    ...         [0, 5000, 10000, 0, 5000],
+    ...         [0, 5000, 10000, 0, 5000],
+    ...         [0, 5000, 10000, 0, 5000],
+    ...         [0, 5000, 10000, 0, 5000],
+    ...     ]
+    ... )
     >>> ga = sw.gpan(s, t, p)
     >>> sw.gvel(ga, lat, lon)
     array([[ 231.74785186,  197.54291221, -436.64938045,    0.        ],
            [ 231.74785186,  197.54291221, -436.64938045,    0.        ],
            [ 231.74785186,  197.54291221, -436.64938045,    0.        ],
            [ 231.74785186,  197.54291221, -436.64938045,    0.        ],
            [ 231.74785186,  197.54291221, -436.64938045,    0.        ]])
 
     References
     ----------
     .. [1] S. Pond & G.Pickard 2nd Edition 1986 Introductory Dynamical
        Oceanography Pergamon Press Sydney. ISBN 0-08-028728-X
 
     """
-
     ga, lon, lat = list(map(np.asanyarray, (ga, lon, lat)))
-    distm = dist(lat, lon, units='km')[0] * 1e3
+    distm = dist(lat, lon, units="km")[0] * 1e3
     lf = f((lat[0:-1] + lat[1:]) / 2) * distm
     return -np.diff(ga, axis=1) / lf
```

### Comparing `seawater-3.3.4/seawater/library.py` & `seawater-3.3.5/seawater/library.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-# -*- coding: utf-8 -*-
-
-
-from __future__ import division, absolute_import
-
 import numpy as np
 
-
-__all__ = ['cndr',
-           'salds',
-           'salrp',
-           'salrt',
-           'seck',
-           'sals',
-           'smow',
-           'T68conv',
-           'T90conv']
+__all__ = [
+    "cndr",
+    "salds",
+    "salrp",
+    "salrt",
+    "seck",
+    "sals",
+    "smow",
+    "T68conv",
+    "T90conv",
+]
 
 
 # Constants.
 a = [0.0080, -0.1692, 25.3851, 14.0941, -7.0261, 2.7081]
 b = [0.0005, -0.0056, -0.0066, -0.0375, 0.0636, -0.0144]
 c = [0.6766097, 2.00564e-2, 1.104259e-4, -6.9698e-7, 1.0031e-9]
 d = [3.426e-2, 4.464e-4, 4.215e-1, -3.107e-3]
 e = [2.070e-5, -6.370e-10, 3.989e-15]
 k = 0.0162
 
 
 def cndr(s, t, p):
-    """
-    Calculates conductivity ratio.
+    """Calculates conductivity ratio.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
            temperature [℃ (ITS-90)]
@@ -48,23 +43,23 @@
     --------
     >>> # Data from UNESCO 1983 p9.
     >>> import seawater as sw
     >>> t = T90conv([0, 10, 0, 10, 10, 30])
     >>> p = [0, 0, 1000, 1000, 0, 0]
     >>> s = [25, 25, 25, 25, 40, 40]
     >>> sw.cndr(s, t, p)
-    array([ 0.49800825,  0.65499015,  0.50624434,  0.66297496,  1.00007311,
-            1.52996697])
+    array([0.49800825, 0.65499015, 0.50624434, 0.66297496, 1.00007311,
+           1.52996697])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.UNESCO.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     s, t, p = list(map(np.asanyarray, (s, t, p)))
 
     T68 = T68conv(t)
 
     shape = s.shape
@@ -72,16 +67,15 @@
     # Do a Newton-Raphson iteration for inverse interpolation of Rt from s.
     Rx = []
     for S, T in zip(s, t):
         Rx_loop = np.sqrt(S / 35.0)  # first guess at Rx = sqrt(Rt).
         SInc = sals(Rx_loop * Rx_loop, T)  # S Increment (guess) from Rx.
         iloop = 0
         while True:
-            # FIXME: I believe that T / 1.00024 isn't correct here.  But I'm
-            # reproducing seawater up to its bugs!
+            # NOTE: I believe that T / 1.00024 isn't correct here.
             Rx_loop = Rx_loop + (S - SInc) / salds(Rx_loop, T / 1.00024 - 15)
             SInc = sals(Rx_loop * Rx_loop, T)
             iloop += 1
             dels = abs(SInc - S)
             if (dels > 1.0e-10) and (iloop < 100):
                 pass
             else:
@@ -89,32 +83,30 @@
 
         Rx.append(Rx_loop)
 
     Rx = np.array(Rx).reshape(shape)
 
     # Once Rt found, corresponding to each (s,t) evaluate r.
     # Eqn(4) p.8 UNESCO 1983.
-    A = (d[2] + d[3] * T68)
-    B = 1 + d[0] * T68 + d[1] * T68 ** 2
-    C = p * (e[0] + e[1] * p + e[2] * p ** 2)
+    A = d[2] + d[3] * T68
+    B = 1 + d[0] * T68 + d[1] * T68**2
+    C = p * (e[0] + e[1] * p + e[2] * p**2)
 
     # Eqn(6) p.9 UNESCO 1983.
-    Rt = Rx ** 2
+    Rt = Rx**2
     rt = salrt(t)
     # Rtrt  = rt * Rt # NOTE: unused in the code, but present in the original.
     D = B - A * rt * Rt
     E = rt * Rt * A * (B + C)
-    r = np.sqrt(np.abs(D ** 2 + 4 * E)) - D
-    r = 0.5 * r / A
-    return r
+    r = np.sqrt(np.abs(D**2 + 4 * E)) - D
+    return 0.5 * r / A
 
 
 def salds(rtx, delt):
-    """
-    Calculates Salinity differential (:math:`\\frac{dS}{d(\\sqrt{Rt})}`) at
+    r"""Calculates Salinity differential (:math:`\\frac{dS}{d(\\sqrt{Rt})}`) at
     constant temperature.
 
     Parameters
     ----------
     rtx : array_like
           :math:`\\sqrt{rt}`
     delt : array_like
@@ -127,41 +119,38 @@
 
     Examples
     --------
     >>> # Data from UNESCO 1983 p9.
     >>> import numpy as np
     >>> import seawater as sw
     >>> delt = T90conv([15, 20, 5]) - 15
-    >>> rtx  = np.array([ 1, 1.0568875, 0.81705885]) ** 0.5
+    >>> rtx = np.array([1, 1.0568875, 0.81705885]) ** 0.5
     >>> sw.salds(rtx, delt)
-    array([ 78.31921607,  81.5689307 ,  68.19023687])
+    array([78.31921607, 81.5689307 , 68.19023687])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.UNESCO.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     rtx, delt = list(map(np.asanyarray, (rtx, delt)))
 
-    ds = (a[1] +
-          (2 * a[2] + (3 * a[3] + (4 * a[4] + 5 * a[5] * rtx) * rtx) * rtx) *
-          rtx + (delt / (1 + k * delt)) *
-          (b[1] +
-           (2 * b[2] + (3 * b[3] + (4 * b[4] + 5 * b[5] * rtx) * rtx) * rtx) *
-           rtx))
-
-    return ds
+    return (
+        a[1]
+        + (2 * a[2] + (3 * a[3] + (4 * a[4] + 5 * a[5] * rtx) * rtx) * rtx) * rtx
+        + (delt / (1 + k * delt))
+        * (b[1] + (2 * b[2] + (3 * b[3] + (4 * b[4] + 5 * b[5] * rtx) * rtx) * rtx) * rtx)
+    )
 
 
 def salrp(r, t, p):
-    """
-    Equation for Rp used in calculating salinity. UNESCO 1983 polynomial.
+    r"""Equation for Rp used in calculating salinity. UNESCO 1983 polynomial.
 
     .. math::
         Rp(S,T,P) = \\frac{C(S,T,P)}{C(S,T,0)}
 
 
     Parameters
     ----------
@@ -180,38 +169,36 @@
     Examples
     --------
     >>> import seawater as sw
     >>> r = [1, 1.2, 0.65]
     >>> t = T90conv([15, 20, 5])
     >>> p = [0, 2000, 1500]
     >>> sw.salrp(r, t, p)
-    array([ 1.        ,  1.01694294,  1.02048638])
+    array([1.        , 1.01694294, 1.02048638])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     r, t, p = list(map(np.asanyarray, (r, t, p)))
 
     # Eqn(4) p.8 UNESCO.
     T68 = T68conv(t)
 
-    rp = (1 + (p * (e[0] + e[1] * p + e[2] * p ** 2)) /
-          (1 + d[0] * T68 + d[1] * T68 ** 2 + (d[2] + d[3] * T68) * r))
-
-    return rp
+    return 1 + (p * (e[0] + e[1] * p + e[2] * p**2)) / (
+        1 + d[0] * T68 + d[1] * T68**2 + (d[2] + d[3] * T68) * r
+    )
 
 
 def salrt(t):
-    """
-    Equation for rt used in calculating salinity. UNESCO 1983 polynomial.
+    r"""Equation for rt used in calculating salinity. UNESCO 1983 polynomial.
 
     .. math::
         rt(t) = \\frac{C(35,t,0)}{C(35,15(\\textrm{IPTS-68}), 0)}
 
 
     Parameters
     ----------
@@ -225,33 +212,32 @@
 
     Examples
     --------
     >>> # Data from UNESCO 1983 p9.
     >>> import seawater as sw
     >>> t = T90conv([15, 20, 5])
     >>> sw.salrt(t)
-    array([ 1.        ,  1.11649272,  0.77956585])
+    array([1.        , 1.11649272, 0.77956585])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     t = np.asanyarray(t)
     T68 = T68conv(t)
     # Eqn (3) p.7 UNESCO.
     return c[0] + (c[1] + (c[2] + (c[3] + c[4] * T68) * T68) * T68) * T68
 
 
 def seck(s, t, p=0):
-    """
-    Secant Bulk Modulus (K) of Sea Water using Equation of state 1980.
+    """Secant Bulk Modulus (K) of Sea Water using Equation of state 1980.
     UNESCO polynomial implementation.
 
     Parameters
     ----------
     s(p) : array_like
            salinity [psu (PSS-78)]
     t(p) : array_like
@@ -268,23 +254,23 @@
     --------
     >>> # Data from Unesco Tech. Paper in Marine Sci. No. 44, p22.
     >>> import seawater as sw
     >>> s = [0, 0, 0, 0, 35, 35, 35, 35]
     >>> t = T90conv([0, 0, 30, 30, 0, 0, 30, 30])
     >>> p = [0, 10000, 0, 10000, 0, 10000, 0, 10000]
     >>> sw.seck(s, t, p)
-    array([ 19652.21      ,  22977.2115    ,  22336.0044572 ,  25656.8196222 ,
-            21582.27006823,  24991.99729129,  23924.21823158,  27318.32472464])
+    array([19652.21      , 22977.2115    , 22336.0044572 , 25656.8196222 ,
+           21582.27006823, 24991.99729129, 23924.21823158, 27318.32472464])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] Millero, F.J. and  Poisson, A. International one-atmosphere equation
        of state of seawater. Deep-Sea Res. 1981. Vol28A(6) pp625-629.
        doi:10.1016/0198-0149(81)90122-9
 
     """
     s, t, p = list(map(np.asanyarray, (s, t, p)))
@@ -306,29 +292,35 @@
     # e0 = -1930.06
     e = [19652.21, 148.4206, -2.327105, 1.360477e-2, -5.155288e-5]
     KW = e[0] + (e[1] + (e[2] + (e[3] + e[4] * T68) * T68) * T68) * T68
 
     # Sea water terms of secant bulk modulus at atmos. pressure.
     j0 = 1.91075e-4
     i = [2.2838e-3, -1.0981e-5, -1.6078e-6]
-    A = AW + (i[0] + (i[1] + i[2] * T68) * T68 + j0 * s ** 0.5) * s
+    A = AW + (i[0] + (i[1] + i[2] * T68) * T68 + j0 * s**0.5) * s
 
     m = [-9.9348e-7, 2.0816e-8, 9.1697e-10]
     B = BW + (m[0] + (m[1] + m[2] * T68) * T68) * s  # Eqn 18.
 
     f = [54.6746, -0.603459, 1.09987e-2, -6.1670e-5]
     g = [7.944e-2, 1.6483e-2, -5.3009e-4]
-    K0 = (KW + (f[0] + (f[1] + (f[2] + f[3] * T68) * T68) * T68 +
-                (g[0] + (g[1] + g[2] * T68) * T68) * s ** 0.5) * s)  # Eqn 16.
+    K0 = (
+        KW
+        + (
+            f[0]
+            + (f[1] + (f[2] + f[3] * T68) * T68) * T68
+            + (g[0] + (g[1] + g[2] * T68) * T68) * s**0.5
+        )
+        * s
+    )  # Eqn 16.
     return K0 + (A + B * p) * p  # Eqn 15.
 
 
 def sals(rt, t):
-    """
-    Salinity of sea water as a function of Rt and T.  UNESCO 1983 polynomial.
+    r"""Salinity of sea water as a function of Rt and T.  UNESCO 1983 polynomial.
 
     Parameters
     ----------
     rt : array_like
          :math:`rt(s,t) = \\frac{C(s,t,0)}{C(35, t(\\textrm{IPTS-68}), 0)}`
     t : array_like
         temperature [℃ (ITS-90)]
@@ -341,43 +333,41 @@
     Examples
     --------
     >>> # Data from UNESCO 1983 p9.
     >>> import seawater as sw
     >>> t = T90conv([15, 20, 5])
     >>> rt = [1, 1.0568875, 0.81705885]
     >>> sw.sals(rt, t)
-    array([ 35.        ,  37.24562718,  27.99534701])
+    array([35.        , 37.24562718, 27.99534701])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.UNESCO.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     """
     rt, t = list(map(np.asanyarray, (rt, t)))
 
     # Eqn (1) & (2) p6,7 UNESCO.
     del_T68 = T68conv(t) - 15
 
     Rtx = (rt) ** 0.5
-    del_S = ((del_T68 / (1 + k * del_T68)) *
-             (b[0] + (b[1] + (b[2] + (b[3] + (b[4] + b[5] * Rtx) *
-                                      Rtx) * Rtx) * Rtx) * Rtx))
-    s = a[0] + (a[1] + (a[2] + (a[3] + (a[4] + a[5] * Rtx) *
-                                Rtx) * Rtx) * Rtx) * Rtx
+    del_S = (del_T68 / (1 + k * del_T68)) * (
+        b[0] + (b[1] + (b[2] + (b[3] + (b[4] + b[5] * Rtx) * Rtx) * Rtx) * Rtx) * Rtx
+    )
+    s = a[0] + (a[1] + (a[2] + (a[3] + (a[4] + a[5] * Rtx) * Rtx) * Rtx) * Rtx) * Rtx
     s += del_S
 
     return s
 
 
 def smow(t):
-    """
-    Density of Standard Mean Ocean Water (Pure Water) using EOS 1980.
+    """Density of Standard Mean Ocean Water (Pure Water) using EOS 1980.
 
     Parameters
     ----------
     t : array_like
         temperature [℃ (ITS-90)]
 
     Returns
@@ -387,42 +377,46 @@
 
     Examples
     --------
     >>> # Data from UNESCO Tech. Paper in Marine Sci. No. 44, p22.
     >>> import seawater as sw
     >>> t = T90conv([0, 0, 30, 30, 0, 0, 30, 30])
     >>> sw.smow(t)
-    array([ 999.842594  ,  999.842594  ,  995.65113374,  995.65113374,
-            999.842594  ,  999.842594  ,  995.65113374,  995.65113374])
+    array([999.842594  , 999.842594  , 995.65113374, 995.65113374,
+           999.842594  , 999.842594  , 995.65113374, 995.65113374])
 
     References
     ----------
     .. [1] Fofonoff, P. and Millard, R.C. Jr UNESCO 1983. Algorithms for
        computation of fundamental properties of seawater. UNESCO Tech. Pap. in
        Mar. Sci., No. 44, 53 pp.  Eqn.(31) p.39.
-       http://unesdoc.unesco.org/images/0005/000598/059832eb.pdf
+       https://unesdoc.unesco.org/ark:/48223/pf0000059832_eng
 
     .. [2] Millero, F.J. and  Poisson, A. International one-atmosphere equation
        of state of seawater. Deep-Sea Res. 1981. Vol28A(6) pp625-629.
        doi:10.1016/0198-0149(81)90122-9
 
     """
     t = np.asanyarray(t)
 
-    a = (999.842594, 6.793952e-2, -9.095290e-3, 1.001685e-4, -1.120083e-6,
-         6.536332e-9)
+    a = (
+        999.842594,
+        6.793952e-2,
+        -9.095290e-3,
+        1.001685e-4,
+        -1.120083e-6,
+        6.536332e-9,
+    )
 
     T68 = T68conv(t)
-    return (a[0] + (a[1] + (a[2] + (a[3] + (a[4] + a[5] * T68) * T68) * T68) *
-            T68) * T68)
+    return a[0] + (a[1] + (a[2] + (a[3] + (a[4] + a[5] * T68) * T68) * T68) * T68) * T68
 
 
 def T68conv(T90):
-    """
-    Convert ITS-90 temperature to IPTS-68
+    """Convert ITS-90 temperature to IPTS-68.
 
     :math:`T68  = T90 * 1.00024`
 
     Parameters
     ----------
     t : array_like
            temperature [℃ (ITS-90)]
@@ -452,17 +446,16 @@
        Southampton, United Kingdom, 10.
 
     """
     T90 = np.asanyarray(T90)
     return T90 * 1.00024
 
 
-def T90conv(t, t_type='T68'):
-    """
-    Convert IPTS-68 or IPTS-48 to temperature to ITS-90.
+def T90conv(t, t_type="T68"):
+    """Convert IPTS-68 or IPTS-48 to temperature to ITS-90.
 
     T48 apply to all data collected prior to 31/12/1967.
     T68 apply to all data collected between 01/10/1968 and 31/12/1989.
 
     .. math::
         T90 = T68 / 1.00024
 
@@ -487,57 +480,48 @@
     0.5 ℃ for conversion between IPTS-68 and ITS-90 over the
     oceanographic temperature range.
 
     Examples
     --------
     >>> T90conv(20.004799999999999)
     20.0
-    >>> T90conv(20., t_type='T48')
-    19.988162840918179
+    >>> T90conv(20.0, t_type="T48")
+    19.98816284091818
 
     References
     ----------
     .. [1] Saunders, P. M., 1991: The International Temperature Scale of 1990,
        ITS-90. WOCE Newsletter, No. 10, WOCE International Project Office,
        Southampton, United Kingdom, 10.
 
-    .. [2] International Temperature Scales of 1948, 1968 and 1990, an ICES
-       note, available from http://www.ices.dk/ocean/procedures/its.htm
-
     """
     t = np.asanyarray(t)
 
-    if t_type == 'T68':
+    if t_type == "T68":
         T90 = t / 1.00024
-    elif t_type == 'T48':
+    elif t_type == "T48":
         T90 = (t - 4.4e-6 * t * (100 - t)) / 1.00024
     else:
-        raise NameError("Unrecognized temperature type.  Try 'T68'' or 'T48'")
+        msg = "Unrecognized temperature type.  Try 'T68'' or 'T48'"
+        raise NameError(msg)
 
     return T90
 
 
 def atleast_2d(*arys):
-    """
-    Same as numpy atleast_2d, but with the single dimension last, instead of
+    """Same as numpy atleast_2d, but with the single dimension last, instead of
     first.
 
     """
     res = []
     for ary in arys:
-        ary = np.asanyarray(ary)
-        if len(ary.shape) == 0:
-            result = ary.reshape(1, 1)
-        elif len(ary.shape) == 1:
-            result = ary[:, np.newaxis]
+        arry = np.asanyarray(ary)
+        if len(arry.shape) == 0:
+            result = arry.reshape(1, 1)
+        elif len(arry.shape) == 1:
+            result = arry[:, np.newaxis]
         else:
-            result = ary
+            result = arry
         res.append(result)
     if len(res) == 1:
         return res[0]
-    else:
-        return res
-
-
-if __name__ == '__main__':
-    import doctest
-    doctest.testmod()
+    return res
```

### Comparing `seawater-3.3.4/CHANGES.txt` & `seawater-3.3.5/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `seawater-3.3.4/LICENSE.CSIRO` & `seawater-3.3.5/LICENSE.CSIRO`

 * *Files identical despite different names*

### Comparing `seawater-3.3.4/LICENSE.txt` & `seawater-3.3.5/LICENSE.txt`

 * *Files identical despite different names*

