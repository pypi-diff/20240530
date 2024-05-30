# Comparing `tmp/femtoapiwrap-0.5.3-py3-none-any.whl.zip` & `tmp/femtoapiwrap-0.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 45259 bytes, number of entries: 13
+Zip file size: 45221 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     1383 b- defN 23-Feb-07 14:05 femtoapiwrap/__init__.py
--rw-rw-rw-  2.0 fat       22 b- defN 23-Feb-07 14:08 femtoapiwrap/_version.py
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-30 14:29 femtoapiwrap/_version.py
 -rw-rw-rw-  2.0 fat    81748 b- defN 23-Mar-07 13:27 femtoapiwrap/api.py
 -rw-rw-rw-  2.0 fat     6322 b- defN 23-Feb-07 14:05 femtoapiwrap/errors.py
 -rw-rw-rw-  2.0 fat     3205 b- defN 23-Feb-07 14:05 femtoapiwrap/utils.py
 -rw-rw-rw-  2.0 fat     1843 b- defN 23-Feb-07 14:05 femtoapiwrap/hi/__init__.py
 -rw-rw-rw-  2.0 fat    22926 b- defN 23-Feb-07 12:24 femtoapiwrap/hi/_highapi.py
--rw-rw-rw-  2.0 fat    31109 b- defN 23-Feb-09 14:26 femtoapiwrap/hi/_mescfile.py
--rw-rw-rw-  2.0 fat    18092 b- defN 23-Mar-31 08:08 femtoapiwrap-0.5.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     7015 b- defN 23-Mar-31 08:08 femtoapiwrap-0.5.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-31 08:08 femtoapiwrap-0.5.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Mar-31 08:08 femtoapiwrap-0.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1065 b- defN 23-Mar-31 08:08 femtoapiwrap-0.5.3.dist-info/RECORD
-13 files, 174835 bytes uncompressed, 43489 bytes compressed:  75.1%
+-rw-rw-rw-  2.0 fat    31108 b- defN 24-May-30 14:16 femtoapiwrap/hi/_mescfile.py
+-rw-rw-rw-  2.0 fat    18092 b- defN 24-May-30 14:29 femtoapiwrap-0.5.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     6803 b- defN 24-May-30 14:29 femtoapiwrap-0.5.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-30 14:29 femtoapiwrap-0.5.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-30 14:29 femtoapiwrap-0.5.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1065 b- defN 24-May-30 14:29 femtoapiwrap-0.5.4.dist-info/RECORD
+13 files, 174622 bytes uncompressed, 43451 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: femtoapiwrap/hi/_highapi.py
 Comment: 
 
 Filename: femtoapiwrap/hi/_mescfile.py
 Comment: 
 
-Filename: femtoapiwrap-0.5.3.dist-info/LICENSE.txt
+Filename: femtoapiwrap-0.5.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: femtoapiwrap-0.5.3.dist-info/METADATA
+Filename: femtoapiwrap-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: femtoapiwrap-0.5.3.dist-info/WHEEL
+Filename: femtoapiwrap-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: femtoapiwrap-0.5.3.dist-info/top_level.txt
+Filename: femtoapiwrap-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: femtoapiwrap-0.5.3.dist-info/RECORD
+Filename: femtoapiwrap-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## femtoapiwrap/_version.py

```diff
@@ -1 +1 @@
-__version__ = '0.5.3'
+__version__ = '0.5.4'
```

## femtoapiwrap/hi/_mescfile.py

```diff
@@ -789,15 +789,15 @@
             raise _err.EmptyJsonError('ReferenceViewport')
         if (version := subtree['referenceViewportFormatVersion']) != cls.JSON_VERSION:
             raise _err.JsonVersionError('ReferenceViewport', version, cls.JSON_VERSION)
         viewports = subtree['viewports']
         return [cls(
             layer_idx=i,
             rot=quat2rot(vp['geomTransRot']),
-            transl=_np.array(vp['geomTransTransl'], dtype=_np.float32),
+            transl=_np.array(vp['geomTransTransl'], dtype=_np.double),
             height=vp['height'],
             width=vp['width']
         ) for i, vp in enumerate(viewports)]
 
     def to_tree(self, self_only: bool = False) -> dict[str, _t.Any]:
         """Converts the object to MESc JSON format.
```

## Comparing `femtoapiwrap-0.5.3.dist-info/LICENSE.txt` & `femtoapiwrap-0.5.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `femtoapiwrap-0.5.3.dist-info/METADATA` & `femtoapiwrap-0.5.4.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,208 @@
-Metadata-Version: 2.1
-Name: femtoapiwrap
-Version: 0.5.3
-Summary: FemtoAPI Python wrapper
-Home-page: https://femtonics.eu
-Author: Femtonics Ltd.
-Author-email: support@femtonics.eu
-License: GNU General Public License v2 (GPLv2)
-Keywords: FemtoAPI
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Typing :: Typed
-Requires-Python: <=3.8.13,>=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-Requires-Dist: femtoapi (==1.0.0)
-Requires-Dist: PySide2
-Requires-Dist: numpy
-Requires-Dist: scipy (>=1.2.0)
-Requires-Dist: upolygon (==0.1.8)
-Provides-Extra: doc
-Requires-Dist: sphinx ; extra == 'doc'
-Requires-Dist: docutils (==0.18.1) ; extra == 'doc'
-Requires-Dist: sphinx-rtd-theme ; extra == 'doc'
-Provides-Extra: examples
-Requires-Dist: h5py ; extra == 'examples'
-Requires-Dist: Pillow (==9.1.1) ; extra == 'examples'
-Requires-Dist: matplotlib ; extra == 'examples'
-Provides-Extra: test
-Requires-Dist: coverage ; extra == 'test'
-
-=======================
-FemtoAPI Python Wrapper
-=======================
-
-Contents
-========
-
-This project contains a Python wrapper for calling the `Femto API`_ functions
-of MESc software and additional utilities for handling the data obtained from
-the API.
-These are bundled in the ``femtoapiwrap`` package that gets installed using
-basic setup.
-
-For sample implementations for basic use cases, see the scripts in folder
-``examples/basic``.
-
-Modules (it's enough to import ``femtoapiwrap`` only):
-
-* ``femtoapiwrap.api``: the low-level API functions
-* ``femtoapiwrap.hi``: high-level types and methods
-* ``femtoapiwrap.utils``: miscellaneous functions
-* ``femtoapiwrap.errors``: custom exceptions
-
-.. _`Femto API`: https://femtonics.atlassian.net/wiki/spaces/API2
-
-Install
-=======
-
-Basic Setup
------------
-
-.. code:: console
-
-    $ cd <project-root>
-    $ pip install -U .
-
-Checking version:
-
-.. code:: python
-
-    import femtoapiwrap
-    print(femtoapiwrap.__version__)
-
-Running Examples
-----------------
-
-Examples require additional dependencies, which can be installed like this:
-
-.. code:: console
-
-    $ pip install -U .[examples]
-
-Generating Documentation
-------------------------
-
-.. code:: console
-
-    $ cd <project-root>
-    $ pip install -U .[doc]
-    $ cd doc
-    $ make clean
-    $ make html
-
-Then you can find the documentation at ``<project-root>/doc/_build/index.html``.
-Rebuilding often requires the deletion of ``<project-root>/doc/parts/stubs`` too.
-
-Running Tests
--------------
-
-Run tests with coverage report:
-
-.. code:: console
-
-    $ cd <project-root>
-    $ pip install .[test]
-    $ cd <project-root>/tests
-    $ coverage run --source femtoapiwrap -m unittest discover && coverage report
-
-Some test cases need an accessible microscope or a running measurement.
-By default, these are skipped and can be activated by setting ``1`` to the
-environment variables ``FEMTOAPIWRAP_TEST_MICROSCOPE`` or ``FEMTOAPIWRAP_TEST_ONLINE``
-respectively.
-
-Purchase
-========
-
-To purchase FemtoAPI please contact `sales@femtonics.eu <sales@femtonics.eu>`_.
-
-Disclaimer
-==========
-
-IN NO EVENT SHALL FEMTONICS BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL,
-INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE
-USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF FEMTONICS HAS BEEN ADVISED
-OF THE POSSIBILITY OF SUCH DAMAGE.
-
-FEMTONICS SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
-THE SOFTWARE AND ACCOMPANYING DOCUMENTATION, IF ANY, PROVIDED HEREUNDER IS
-PROVIDED "AS IS". FEMTONICS HAS NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT,
-UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
-
-Changelog
-=========
-
-0.5.2
-    ``hi.UnitMeta``
-        New attributes ``t_step_in_ms``, ``t_length_in_ms``,
-        ``t_length_in_ms_actual``, ``file_handle`` and ``fs``.
-    ``hi.Roi.from_tree``
-        Fixed loading optional fields (e. g. ``viewport_index``).
-0.5.1
-    ``hi.HighFemtoApi.read_points``
-        Fix: no longer raises ``EmptyJsonError`` when there are no points in the file.
-    ``hi.Roi.to_px_coords``
-        New parameter ``closed``, with plotting example
-0.5.0
-    ``hi.Point.from_px_coords``
-        Support for 3D points as well.
-    ``hi.Roi``
-        **Breaking change:** removed attributes ``viewport_rot`` and
-        ``viewport_transl`` due to expected removal from FemtoAPI JSON object.
-
-        New attributes ``first_z_plane`` and ``last_z_plane`` for planned
-        support of ROIs in zStack measurements (not yet implemented in MESc).
-    ``hi.Roi.from_px_coords``
-        **Breaking change:** replaced parameter ``viewport`` with ``viewport_index``.
-    ``hi.Roi.to_tree``
-        **Breaking change:** removed parameters as the corresponding tree fields
-        can be filled from the attributes.
-    ``hi.{FileMeta, SessionMeta}.from_tree``
-        Temporary fix to allow converted old MESc files pass the version validation.
-0.4.0
-    ``errors.*``
-        **Breaking changes:** Exceptions are no longer inherited from ``IOError``
-        as that was merged with ``OSError`` and ``FemtoApiWrapError`` subclasses
-        do not strictly related to OS error codes.
-
-        PEP-8 compliant and more informative naming:
-
-        * ``ConnectionFailed`` -> ``ApiConnectionError``
-        * ``MicroscopeTimedOut`` -> ``MeasurementTimeoutError``
-        * ``NodeNotFound`` -> ``NodeNotFoundError``
-        * ``NoMetaData`` -> ``EmptyJsonError``
-        * ``InvalidDimension`` -> ``DimensionError``
-        * ``InvalidPointGroup`` -> ``PointSeriesKeyError``
-        * ``UnsupportedVersion`` -> ``JsonVersionError``
-
-    ``errors.ApiCommandError``
-        New exception to contain error information about FemtoAPI command failures.
-    ``errors.ApiLoginError``
-        New exception.
-    ``errors.NoMeasurementUnit``
-        **Removed**, merged with ``NodeNotFoundError``
-    ``errors.InvalidMeasurementType``
-        **Removed**, it was unused.
-0.3.1
-    ``hi.Roi``
-        Added attribute ``background`` based on the previously unprocessed
-        JSON-attribute ``"role"``.
-    ``hi.Roi.from_px_coords``
-        Added parameter ``background``.
-0.3.0
-    ``hi.HighFemtoApi.online_frames``
-        Fixed to take into account the actual number of frames received from MESc.
-        **Breaking change:** The actual start index is now included in the iterator.
-        Introduced the parameter ``strict`` to enforce chunks of equal length.
-0.2.0.post1
-    Relaxed dependency version requirements.
-0.2.0
-    Initial public release.
+Metadata-Version: 2.1
+Name: femtoapiwrap
+Version: 0.5.4
+Summary: FemtoAPI Python wrapper
+Home-page: https://femtonics.eu
+Author: Femtonics Ltd.
+Author-email: support@femtonics.eu
+License: GNU General Public License v2 (GPLv2)
+Keywords: FemtoAPI
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Topic :: Scientific/Engineering
+Classifier: Typing :: Typed
+Requires-Python: <=3.8.13,>=3.8
+Description-Content-Type: text/x-rst
+Requires-Dist: femtoapi (==1.0.0)
+Requires-Dist: PySide2
+Requires-Dist: numpy
+Requires-Dist: scipy (>=1.2.0)
+Requires-Dist: upolygon (==0.1.8)
+Provides-Extra: doc
+Requires-Dist: sphinx ; extra == 'doc'
+Requires-Dist: docutils (==0.18.1) ; extra == 'doc'
+Requires-Dist: sphinx-rtd-theme ; extra == 'doc'
+Provides-Extra: examples
+Requires-Dist: h5py ; extra == 'examples'
+Requires-Dist: Pillow (==9.1.1) ; extra == 'examples'
+Requires-Dist: matplotlib ; extra == 'examples'
+Provides-Extra: test
+Requires-Dist: coverage ; extra == 'test'
+
+=======================
+FemtoAPI Python Wrapper
+=======================
+
+Contents
+========
+
+This project contains a Python wrapper for calling the `Femto API`_ functions
+of MESc software and additional utilities for handling the data obtained from
+the API.
+These are bundled in the ``femtoapiwrap`` package that gets installed using
+basic setup.
+
+For sample implementations for basic use cases, see the scripts in folder
+``examples/basic``.
+
+Modules (it's enough to import ``femtoapiwrap`` only):
+
+* ``femtoapiwrap.api``: the low-level API functions
+* ``femtoapiwrap.hi``: high-level types and methods
+* ``femtoapiwrap.utils``: miscellaneous functions
+* ``femtoapiwrap.errors``: custom exceptions
+
+.. _`Femto API`: https://femtonics.atlassian.net/wiki/spaces/API2
+
+Install
+=======
+
+Basic Setup
+-----------
+
+.. code:: console
+
+    $ cd <project-root>
+    $ pip install -U .
+
+Checking version:
+
+.. code:: python
+
+    import femtoapiwrap
+    print(femtoapiwrap.__version__)
+
+Running Examples
+----------------
+
+Examples require additional dependencies, which can be installed like this:
+
+.. code:: console
+
+    $ pip install -U .[examples]
+
+Generating Documentation
+------------------------
+
+.. code:: console
+
+    $ cd <project-root>
+    $ pip install -U .[doc]
+    $ cd doc
+    $ make clean
+    $ make html
+
+Then you can find the documentation at ``<project-root>/doc/_build/index.html``.
+Rebuilding often requires the deletion of ``<project-root>/doc/parts/stubs`` too.
+
+Running Tests
+-------------
+
+Run tests with coverage report:
+
+.. code:: console
+
+    $ cd <project-root>
+    $ pip install .[test]
+    $ cd <project-root>/tests
+    $ coverage run --source femtoapiwrap -m unittest discover && coverage report
+
+Some test cases need an accessible microscope or a running measurement.
+By default, these are skipped and can be activated by setting ``1`` to the
+environment variables ``FEMTOAPIWRAP_TEST_MICROSCOPE`` or ``FEMTOAPIWRAP_TEST_ONLINE``
+respectively.
+
+Purchase
+========
+
+To purchase FemtoAPI please contact `sales@femtonics.eu <sales@femtonics.eu>`_.
+
+Disclaimer
+==========
+
+IN NO EVENT SHALL FEMTONICS BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL,
+INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE
+USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF FEMTONICS HAS BEEN ADVISED
+OF THE POSSIBILITY OF SUCH DAMAGE.
+
+FEMTONICS SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
+THE SOFTWARE AND ACCOMPANYING DOCUMENTATION, IF ANY, PROVIDED HEREUNDER IS
+PROVIDED "AS IS". FEMTONICS HAS NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT,
+UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
+
+Changelog
+=========
+
+0.5.2
+    ``hi.UnitMeta``
+        New attributes ``t_step_in_ms``, ``t_length_in_ms``,
+        ``t_length_in_ms_actual``, ``file_handle`` and ``fs``.
+    ``hi.Roi.from_tree``
+        Fixed loading optional fields (e. g. ``viewport_index``).
+0.5.1
+    ``hi.HighFemtoApi.read_points``
+        Fix: no longer raises ``EmptyJsonError`` when there are no points in the file.
+    ``hi.Roi.to_px_coords``
+        New parameter ``closed``, with plotting example
+0.5.0
+    ``hi.Point.from_px_coords``
+        Support for 3D points as well.
+    ``hi.Roi``
+        **Breaking change:** removed attributes ``viewport_rot`` and
+        ``viewport_transl`` due to expected removal from FemtoAPI JSON object.
+
+        New attributes ``first_z_plane`` and ``last_z_plane`` for planned
+        support of ROIs in zStack measurements (not yet implemented in MESc).
+    ``hi.Roi.from_px_coords``
+        **Breaking change:** replaced parameter ``viewport`` with ``viewport_index``.
+    ``hi.Roi.to_tree``
+        **Breaking change:** removed parameters as the corresponding tree fields
+        can be filled from the attributes.
+    ``hi.{FileMeta, SessionMeta}.from_tree``
+        Temporary fix to allow converted old MESc files pass the version validation.
+0.4.0
+    ``errors.*``
+        **Breaking changes:** Exceptions are no longer inherited from ``IOError``
+        as that was merged with ``OSError`` and ``FemtoApiWrapError`` subclasses
+        do not strictly related to OS error codes.
+
+        PEP-8 compliant and more informative naming:
+
+        * ``ConnectionFailed`` -> ``ApiConnectionError``
+        * ``MicroscopeTimedOut`` -> ``MeasurementTimeoutError``
+        * ``NodeNotFound`` -> ``NodeNotFoundError``
+        * ``NoMetaData`` -> ``EmptyJsonError``
+        * ``InvalidDimension`` -> ``DimensionError``
+        * ``InvalidPointGroup`` -> ``PointSeriesKeyError``
+        * ``UnsupportedVersion`` -> ``JsonVersionError``
+
+    ``errors.ApiCommandError``
+        New exception to contain error information about FemtoAPI command failures.
+    ``errors.ApiLoginError``
+        New exception.
+    ``errors.NoMeasurementUnit``
+        **Removed**, merged with ``NodeNotFoundError``
+    ``errors.InvalidMeasurementType``
+        **Removed**, it was unused.
+0.3.1
+    ``hi.Roi``
+        Added attribute ``background`` based on the previously unprocessed
+        JSON-attribute ``"role"``.
+    ``hi.Roi.from_px_coords``
+        Added parameter ``background``.
+0.3.0
+    ``hi.HighFemtoApi.online_frames``
+        Fixed to take into account the actual number of frames received from MESc.
+        **Breaking change:** The actual start index is now included in the iterator.
+        Introduced the parameter ``strict`` to enforce chunks of equal length.
+0.2.0.post1
+    Relaxed dependency version requirements.
+0.2.0
+    Initial public release.
+
+
```

## Comparing `femtoapiwrap-0.5.3.dist-info/RECORD` & `femtoapiwrap-0.5.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 femtoapiwrap/__init__.py,sha256=oyT855nCXZlqoNPF_RnSfOCzOPWbZUQaj6SK8B3_5iY,1383
-femtoapiwrap/_version.py,sha256=TFkACo7SKbVpSQl32OCSCNmy1zVX-jsQX6dAXMbWmkU,22
+femtoapiwrap/_version.py,sha256=YYYpMsC3ActrKnohyOQTZhA6i4ZGdIcgCekNZ1_03lo,22
 femtoapiwrap/api.py,sha256=oliZWi9XEbgu7J2279cgb6SludGoeKqgi8xjdUtCllU,81748
 femtoapiwrap/errors.py,sha256=DeZwBfoIWz-2_oBMu6w_slKykj5m16Ysnrz_-PgEjFk,6322
 femtoapiwrap/utils.py,sha256=Yel7uN92mYrS7gDqTRLUX4SfDMucDAyPsSHq-r2aFx0,3205
 femtoapiwrap/hi/__init__.py,sha256=Fwt5A-Wunqc1XNoEKbpB_76Xf574ZXnVlhw2HYZw4Kk,1843
 femtoapiwrap/hi/_highapi.py,sha256=A1TZuKuBbdPcMFsYcT2bOB8gMCkuAf4AMnsoPBJSZ5o,22926
-femtoapiwrap/hi/_mescfile.py,sha256=rX-Itj1qe8BMAIQ-h5T_TdAGweTPacHqOs4p-EaiBV0,31109
-femtoapiwrap-0.5.3.dist-info/LICENSE.txt,sha256=gXf5dRMhNSbfLPYYTY_5hsZ1r7UU1OaKQEAQUhuIBkM,18092
-femtoapiwrap-0.5.3.dist-info/METADATA,sha256=Jwq0JwQiGne5bJdnYooPxC_65Bv2sxnQ1PXq6jSxSBs,7015
-femtoapiwrap-0.5.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-femtoapiwrap-0.5.3.dist-info/top_level.txt,sha256=8TMMffpuV6UVH3o_70r7G16J3O2ZEvppWQkCK87-Jg0,13
-femtoapiwrap-0.5.3.dist-info/RECORD,,
+femtoapiwrap/hi/_mescfile.py,sha256=0LEIxLvw1IH2avGGFqwGz8luDjyCnfIAY89rSHoNMiU,31108
+femtoapiwrap-0.5.4.dist-info/LICENSE.txt,sha256=gXf5dRMhNSbfLPYYTY_5hsZ1r7UU1OaKQEAQUhuIBkM,18092
+femtoapiwrap-0.5.4.dist-info/METADATA,sha256=YvJ9avFYb35nhYMQjkQmm19iHLExhAPGH27EDdKgyoc,6803
+femtoapiwrap-0.5.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+femtoapiwrap-0.5.4.dist-info/top_level.txt,sha256=8TMMffpuV6UVH3o_70r7G16J3O2ZEvppWQkCK87-Jg0,13
+femtoapiwrap-0.5.4.dist-info/RECORD,,
```

