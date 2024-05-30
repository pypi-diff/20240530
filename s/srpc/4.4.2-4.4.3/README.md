# Comparing `tmp/srpc-4.4.2-cp312-none-win_amd64.whl.zip` & `tmp/srpc-4.4.3-cp312-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 281243 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-03 16:37 srpc-4.4.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2216 b- defN 24-Apr-03 16:37 srpc-4.4.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-03 16:37 srpc-4.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-03 16:37 srpc-4.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      371 b- defN 24-Apr-03 16:37 srpc-4.4.2.dist-info/RECORD
--rw-rw-rw-  2.0 fat    23040 b- defN 24-Apr-03 16:36 srpc/__init__.pyd
--rw-rw-rw-  2.0 fat   122880 b- defN 24-Apr-03 16:36 srpc/client.pyd
--rw-rw-rw-  2.0 fat   119808 b- defN 24-Apr-03 16:36 srpc/protocol.pyd
--rw-rw-rw-  2.0 fat    83968 b- defN 24-Apr-03 16:36 srpc/ring.pyd
--rw-rw-rw-  2.0 fat   129024 b- defN 24-Apr-03 16:36 srpc/server.pyd
--rw-rw-rw-  2.0 fat   151552 b- defN 24-Apr-03 16:36 srpc/ulog.pyd
-11 files, 634045 bytes uncompressed, 279917 bytes compressed:  55.9%
+Zip file size: 280552 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     1084 b- defN 24-May-30 04:51 srpc-4.4.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2207 b- defN 24-May-30 04:51 srpc-4.4.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-30 04:51 srpc-4.4.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-30 04:51 srpc-4.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      371 b- defN 24-May-30 04:51 srpc-4.4.3.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    23040 b- defN 24-May-30 04:51 srpc/__init__.pyd
+-rw-rw-rw-  2.0 fat   121856 b- defN 24-May-30 04:51 srpc/client.pyd
+-rw-rw-rw-  2.0 fat   120320 b- defN 24-May-30 04:51 srpc/protocol.pyd
+-rw-rw-rw-  2.0 fat    83968 b- defN 24-May-30 04:51 srpc/ring.pyd
+-rw-rw-rw-  2.0 fat   129024 b- defN 24-May-30 04:51 srpc/server.pyd
+-rw-rw-rw-  2.0 fat   151040 b- defN 24-May-30 04:51 srpc/ulog.pyd
+11 files, 633011 bytes uncompressed, 279226 bytes compressed:  55.9%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: srpc-4.4.2.dist-info/LICENSE
+Filename: srpc-4.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: srpc-4.4.2.dist-info/METADATA
+Filename: srpc-4.4.3.dist-info/METADATA
 Comment: 
 
-Filename: srpc-4.4.2.dist-info/WHEEL
+Filename: srpc-4.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: srpc-4.4.2.dist-info/top_level.txt
+Filename: srpc-4.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: srpc-4.4.2.dist-info/RECORD
+Filename: srpc-4.4.3.dist-info/RECORD
 Comment: 
 
 Filename: srpc/__init__.pyd
 Comment: 
 
 Filename: srpc/client.pyd
 Comment:
```

## Comparing `srpc-4.4.2.dist-info/LICENSE` & `srpc-4.4.3.dist-info/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 MIT License
 
-Copyright (c) 2021 YL Feng
+Copyright (c) 2020 YL Feng
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `srpc-4.4.2.dist-info/METADATA` & `srpc-4.4.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: srpc
-Version: 4.4.2
+Version: 4.4.3
 Summary: description
 Author-email: YL <fengyl@pku.edu.cn>
 License: MIT License
         
-        Copyright (c) 2021 YL Feng
+        Copyright (c) 2020 YL Feng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
         
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: homepage, https://gitee.com
 Project-URL: documentation, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

