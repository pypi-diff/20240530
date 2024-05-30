# Comparing `tmp/zhinst_seqc_compiler-24.4.57831-cp39-cp39-win_amd64.whl.zip` & `tmp/zhinst_seqc_compiler-24.4.59173-cp310-cp310-manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4429904 bytes, number of entries: 8
--rw-r--r--  2.0 fat      137 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/__init__.py
--rw-r--r--  2.0 fat     2304 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/__init__.pyi
--rw-r--r--  2.0 fat  9896448 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/_seqc_compiler.pyd
--rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/py.typed
-?rw-r--r--  2.0 fat     2826 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.57831.dist-info/METADATA
-?rw-r--r--  2.0 fat       95 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.57831.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1084 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.57831.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 fat      739 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.57831.dist-info/RECORD
-8 files, 9903633 bytes uncompressed, 4428594 bytes compressed:  55.3%
+Zip file size: 6478535 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      129 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/__init__.py
+-rw-r--r--  2.0 unx     2241 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/__init__.pyi
+-rwxr-xr-x  2.0 unx 19427216 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/_seqc_compiler.so
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 zhinst/seqc_compiler/py.typed
+?rw-r--r--  2.0 unx     2826 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.59173.dist-info/METADATA
+?rw-r--r--  2.0 unx      109 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.59173.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1065 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.59173.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx      740 b- defN 20-Feb-02 00:00 zhinst_seqc_compiler-24.4.59173.dist-info/RECORD
+8 files, 19434326 bytes uncompressed, 6477227 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: zhinst/seqc_compiler/__init__.py
 Comment: 
 
 Filename: zhinst/seqc_compiler/__init__.pyi
 Comment: 
 
-Filename: zhinst/seqc_compiler/_seqc_compiler.pyd
+Filename: zhinst/seqc_compiler/_seqc_compiler.so
 Comment: 
 
 Filename: zhinst/seqc_compiler/py.typed
 Comment: 
 
-Filename: zhinst_seqc_compiler-24.4.57831.dist-info/METADATA
+Filename: zhinst_seqc_compiler-24.4.59173.dist-info/METADATA
 Comment: 
 
-Filename: zhinst_seqc_compiler-24.4.57831.dist-info/WHEEL
+Filename: zhinst_seqc_compiler-24.4.59173.dist-info/WHEEL
 Comment: 
 
-Filename: zhinst_seqc_compiler-24.4.57831.dist-info/licenses/LICENSE.txt
+Filename: zhinst_seqc_compiler-24.4.59173.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: zhinst_seqc_compiler-24.4.57831.dist-info/RECORD
+Filename: zhinst_seqc_compiler-24.4.59173.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhinst/seqc_compiler/__init__.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-from ._seqc_compiler import (
-    __doc__,
-    __version__,
-    __commit_hash__,
-    compile_seqc,
-)
-
-__all__ = ["compile_seqc"]
+from ._seqc_compiler import (
+    __doc__,
+    __version__,
+    __commit_hash__,
+    compile_seqc,
+)
+
+__all__ = ["compile_seqc"]
```

## zhinst/seqc_compiler/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,63 +1,63 @@
-"""Zurich Instruments LabOne SeqC Compiler."""
-from typing import (
-    List,
-    Union,
-    Any,
-    Dict,
-    Optional,
-    Tuple,
-)
-
-_STUB_VERSION_HASH = "0fd488097b9819466360ef953fb4e124"
-
-def compile_seqc(
-    code: str,
-    devtype: str,
-    options: Union[str, List[str]],
-    index: int,
-    samplerate: Optional[float] = None,
-    sequencer: Optional[str] = None,
-    wavepath: Optional[str] = None,
-    waveforms: Optional[str] = None,
-    filename: Optional[str] = None,
-) -> Tuple[bytes, Dict[str, Any]]:
-    """Compile the sequencer code.
-
-    This function is a purely static function that does not require an
-    active connection to a Data Server.
-
-    .. versionadded:: 22.08
-
-    Args:
-        code: SeqC input
-        devtype: target device type, e.g., HDAWG8, SHFQC
-        options: list of device options, or string of
-            options separated by newlines as returned by node
-            /dev.../features/options.
-        index: index of the AWG core
-        samplerate: target sample rate of the sequencer
-            Mandatory and only respected for HDAWG. Should match the
-            value set on the device:
-            `/dev.../system/clocks/sampleclock/freq`.
-        sequencer: one of 'qa', 'sg', or 'auto'.
-            Mandatory for SHFQC.
-        wavepath: path to directory with waveforms. Defaults to
-            path used by LabOne UI or AWG Module.
-        waveforms: list of CSV waveform files separated by ';'.
-            Defaults to an empty list. Set to `None` to include
-            all CSV files in `wavepath`.
-        filename: name of embedded ELF filename.
-
-    Returns:
-        Tuple (elf, extra) of binary ELF data for sequencer and extra
-        dictionary with compiler output.
-
-    Note:
-        The same function is available in the `zhinst-seqc-compiler`
-        package. `zhinst.core.compile_seqc` will forward the call to
-        `zhinst.seqc_compiler.compile_seqc` if a compatible version of
-        this package is installed. A version is compatible if major and
-        minor package versions match, and the revision of
-        `zhinst-seqc-compiler` is greater or equal to the revision of
-        `zhinst-core`. A warning will be issued if the versions do not
-        match."""
+"""Zurich Instruments LabOne SeqC Compiler."""
+from typing import (
+    List,
+    Union,
+    Any,
+    Dict,
+    Optional,
+    Tuple,
+)
+
+_STUB_VERSION_HASH = "0fd488097b9819466360ef953fb4e124"
+
+def compile_seqc(
+    code: str,
+    devtype: str,
+    options: Union[str, List[str]],
+    index: int,
+    samplerate: Optional[float] = None,
+    sequencer: Optional[str] = None,
+    wavepath: Optional[str] = None,
+    waveforms: Optional[str] = None,
+    filename: Optional[str] = None,
+) -> Tuple[bytes, Dict[str, Any]]:
+    """Compile the sequencer code.
+
+    This function is a purely static function that does not require an
+    active connection to a Data Server.
+
+    .. versionadded:: 22.08
+
+    Args:
+        code: SeqC input
+        devtype: target device type, e.g., HDAWG8, SHFQC
+        options: list of device options, or string of
+            options separated by newlines as returned by node
+            /dev.../features/options.
+        index: index of the AWG core
+        samplerate: target sample rate of the sequencer
+            Mandatory and only respected for HDAWG. Should match the
+            value set on the device:
+            `/dev.../system/clocks/sampleclock/freq`.
+        sequencer: one of 'qa', 'sg', or 'auto'.
+            Mandatory for SHFQC.
+        wavepath: path to directory with waveforms. Defaults to
+            path used by LabOne UI or AWG Module.
+        waveforms: list of CSV waveform files separated by ';'.
+            Defaults to an empty list. Set to `None` to include
+            all CSV files in `wavepath`.
+        filename: name of embedded ELF filename.
+
+    Returns:
+        Tuple (elf, extra) of binary ELF data for sequencer and extra
+        dictionary with compiler output.
+
+    Note:
+        The same function is available in the `zhinst-seqc-compiler`
+        package. `zhinst.core.compile_seqc` will forward the call to
+        `zhinst.seqc_compiler.compile_seqc` if a compatible version of
+        this package is installed. A version is compatible if major and
+        minor package versions match, and the revision of
+        `zhinst-seqc-compiler` is greater or equal to the revision of
+        `zhinst-core`. A warning will be issued if the versions do not
+        match."""
```

## Comparing `zhinst_seqc_compiler-24.4.57831.dist-info/METADATA` & `zhinst_seqc_compiler-24.4.59173.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhinst-seqc-compiler
-Version: 24.4.57831
+Version: 24.4.59173
 Summary: Zurich Instruments SeqC compiler
 Project-URL: Documentation, https://docs.zhinst.com/labone_api_user_manual
 Author-email: Zurich Instruments AG <info@zhinst.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `zhinst_seqc_compiler-24.4.57831.dist-info/licenses/LICENSE.txt` & `zhinst_seqc_compiler-24.4.59173.dist-info/licenses/LICENSE.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2020 Zurich Instruments AG
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2020 Zurich Instruments AG
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

