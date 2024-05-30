# Comparing `tmp/continuedfractions-0.12.7.tar.gz` & `tmp/continuedfractions-0.12.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.12.7.tar", last modified: Fri May 17 18:11:14 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.8.tar", last modified: Thu May 30 08:28:54 2024, max compression
```

## Comparing `continuedfractions-0.12.7.tar` & `continuedfractions-0.12.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.7/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.7/LICENSE
--rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.12.7/README.md
--rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.12.7/README.md
--rw-r--r--   0        0        0     3506 2024-05-17 18:11:14.142914 continuedfractions-0.12.7/pyproject.toml
--rw-r--r--   0        0        0    31312 2024-05-15 20:00:55.929517 continuedfractions-0.12.7/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.7/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    35383 2024-05-17 18:03:00.181544 continuedfractions-0.12.7/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.7/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-05-17 17:47:35.471630 continuedfractions-0.12.7/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24420 1970-01-01 00:00:00.000000 continuedfractions-0.12.7/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.8/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.8/LICENSE
+-rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.12.8/README.md
+-rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.12.8/README.md
+-rw-r--r--   0        0        0     3506 2024-05-30 08:28:54.284468 continuedfractions-0.12.8/pyproject.toml
+-rw-r--r--   0        0        0    32416 2024-05-30 08:03:34.043292 continuedfractions-0.12.8/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.8/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    35383 2024-05-17 21:03:20.372072 continuedfractions-0.12.8/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.8/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-30 07:01:29.530607 continuedfractions-0.12.8/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24420 1970-01-01 00:00:00.000000 continuedfractions-0.12.8/PKG-INFO
```

### Comparing `continuedfractions-0.12.7/LICENSE` & `continuedfractions-0.12.8/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.7/README.md` & `continuedfractions-0.12.8/README.md`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.7/pyproject.toml` & `continuedfractions-0.12.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.12.7"
+version = "0.12.8"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.12.7/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.8/src/continuedfractions/continuedfraction.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 sys.path.insert(0, str(Path(__file__).parent.parent))
 
 from continuedfractions.lib import (
     continued_fraction_rational,
     convergent,
     fraction_from_elements,
     left_mediant,
+    mediant,
     right_mediant,
 )
 
 
 class ContinuedFraction(Fraction):
     """An object-oriented representation of a (finite) simple continued fraction.
 
@@ -510,17 +511,14 @@
            p_k &= a_kp_{k - 1} + p_{k - 2} \\\\
            q_k &= a_kq_{k - 1} + q_{k - 2},        \\hskip{3em}    k \\geq 3
            \\end{align}
 
         where :math:`p_0 = a_0`, :math:`q_0 = 1`, :math:`p_1 = p_1p_0 + 1`,
         and :math:`q_1 = p_1`.
 
-        The method is cached (with :py:func:`functools.cache`), which makes
-        calls after the initial call much faster.
-
         Parameters
         ----------
         k : int
             The order of the convergent, as described above.
 
         Returns
         -------
@@ -549,17 +547,14 @@
     @functools.lru_cache
     def convergents(self) -> MappingProxyType[int, ContinuedFraction]:
         """:py:class:`types.MappingProxyType`: An immutable dict of all :math:`k`-order convergents of the continued fraction, keyed by order.
 
         Each convergent is indexed by its order and is also a
         :py:class:`ContinuedFraction` instance.
 
-        The property is cached (with :py:func:`functools.lru_cache`), which makes
-        calls after the initial call much faster.
-
         Examples
         --------
         >>> cf = ContinuedFraction('3.245')
         >>> cf.convergents
         mappingproxy({0: ContinuedFraction(3, 1), 1: ContinuedFraction(13, 4), 2: ContinuedFraction(159, 49), 3: ContinuedFraction(649, 200)})
         >>> cf.convergents[0], cf.convergents[2]
         (ContinuedFraction(3, 1), ContinuedFraction(159, 49))
@@ -573,17 +568,14 @@
     @functools.lru_cache
     def even_order_convergents(self) -> MappingProxyType[int, ContinuedFraction]:
         """:py:class:`types.MappingProxyType`: An immutable dict of all even-order convergents of the continued fraction, keyed by order.
 
         Each convergent is indexed by its order and is also a
         :py:class:`ContinuedFraction` instance.
 
-        The property is cached (with :py:func:`functools.lru_cache`), which makes
-        calls after the initial call much faster.
-
         Examples
         --------
         >>> ContinuedFraction('3.245').even_order_convergents
         mappingproxy({0: ContinuedFraction(3, 1), 2: ContinuedFraction(159, 49)})
         """
         return MappingProxyType({
             k: self.convergents[k]
@@ -594,17 +586,14 @@
     @functools.lru_cache
     def odd_order_convergents(self) -> MappingProxyType[int, ContinuedFraction]:
         """:py:class:`types.MappingProxyType`: An immutable dict of all odd-order convergents of the continued fraction, keyed by order.
 
         Each convergent is indexed by its order and is also a
         :py:class:`ContinuedFraction` instance.
 
-        The property is cached (with :py:func:`functools.lru_cache`), which makes
-        calls after the initial call much faster.
-
         Examples
         --------
         >>> ContinuedFraction('3.245').odd_order_convergents
         mappingproxy({1: ContinuedFraction(13, 4), 3: ContinuedFraction(649, 200)})
         """
         return MappingProxyType({
             k: self.convergents[k]
@@ -620,17 +609,14 @@
         obtained from the original by "removing" the elements of the :math:`(k - 1)`-st
         convergent :math:`C_{k - 1} = (a_0,a_1,\\ldots,a_{k - 1})`.
 
         .. math::
 
             R_k = a_k + \\cfrac{1}{a_{k + 1} + \\cfrac{1}{a_{k + 2} \\ddots }}
 
-        The method is cached (with :py:func:`functools.cache`), which makes calls
-        after the initial call much faster.
-
         Parameters
         ----------
         k : int
             The index of the remainder, as described above.
 
         Returns
         -------
@@ -788,17 +774,14 @@
           \\lim_{k \\to \\infty} \\frac{ka + c}{kb + d} &= \\frac{a}{b} \\\\
           \\lim_{k \\to \\infty} \\frac{a + kc}{b + kd} &= \\frac{c}{d}
           \\end{align}
 
         For more information consult the
         `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/mediants.html>`_.
 
-        The method is cached (with :py:func:`functools.cache`), which makes calls
-        after the initial call much faster.
-
         Parameters
         ----------
         other : fractions.Fraction, ContinuedFraction
             The second fraction to use to calculate the :math:`k`-th mediant with
             the first.
         
         k : int, default=1
@@ -826,14 +809,56 @@
         ContinuedFraction(301, 502)
         >>> assert c1.left_mediant(c2, k=2) < c1.right_mediant(c2, k=2)
         >>> assert c1.left_mediant(c2, k=3) < c1.right_mediant(c2, k=3)
         >>> assert c1.left_mediant(c2, k=100) < c1.right_mediant(c2, k=100)
         """
         return self.__class__(right_mediant(self, other, k=k))
 
+    @functools.cache
+    def mediant(self, other: Fraction, /) -> ContinuedFraction:
+        """Returns the simple mediant of the continued fraction with another continued fraction instance.
+        
+        The simple mediant of two rational numbers :math:`r = \\frac{a}{b}`
+        and :math:`s = \\frac{c}{d}`, where :math:`b, d, b + d \\neq 0`, is
+        defined as:
+        
+        .. math::
+
+           \\frac{a + c}{b + d}
+
+        The resulting value :math:`\\frac{a + c}{b + d}` is the same as the
+        1st order left- or right-mediant of :math:`r = \\frac{a}{b}`
+        and :math:`s = \\frac{c}{d}`. So this method would produce the same
+        result as the :py:meth:`~continuedfractions.continuedfraction.ContinuedFraction.left_mediant`
+        or :py:meth:`~continuedfractions.continuedfraction.ContinuedFraction.right_mediant`
+        methods where the order :math:`k` is set to :math:`1`.
+
+        For more information consult the
+        `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/mediants.html>`_.
+
+        Parameters
+        ----------
+        other : fractions.Fraction, ContinuedFraction
+            The other continued fraction instance.
+        
+        Returns
+        -------
+        ContinuedFraction
+            The simple mediant of the original fraction and the other continued
+            fraction instance.
+
+        Examples
+        --------
+        >>> ContinuedFraction(1, 2).mediant(ContinuedFraction(3, 5))
+        ContinuedFraction(4, 7)
+        >>> assert ContinuedFraction(1, 2).mediant(ContinuedFraction(3, 5)) == ContinuedFraction(1, 2).left_mediant(ContinuedFraction(3, 5), k=1)
+        >>> assert ContinuedFraction(1, 2).mediant(ContinuedFraction(3, 5)) == ContinuedFraction(1, 2).right_mediant(ContinuedFraction(3, 5), k=1)
+        """
+        return self.__class__(mediant(self, other))
+
 
 if __name__ == "__main__":      # pragma: no cover
     # Doctest the module from the project root using
     #
     #     python -m doctest -v src/continuedfractions/continuedfraction.py
     #
     # NOTE: the doctest examples using where `float` or ``decimal.Decimal``
```

### Comparing `continuedfractions-0.12.7/src/continuedfractions/lib.py` & `continuedfractions-0.12.8/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.7/src/continuedfractions/sequences.py` & `continuedfractions-0.12.8/src/continuedfractions/sequences.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.7/src/continuedfractions/utils.py` & `continuedfractions-0.12.8/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.7/PKG-INFO` & `continuedfractions-0.12.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.12.7
+Version: 0.12.8
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
```

