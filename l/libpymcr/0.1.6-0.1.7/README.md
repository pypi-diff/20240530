# Comparing `tmp/libpymcr-0.1.6-cp39-cp39-win_amd64.whl.zip` & `tmp/libpymcr-0.1.7-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,17 @@
-Zip file size: 203799 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat    11938 b- defN 24-Apr-26 00:18 libpymcr/IPythonMagics.py
--rw-rw-rw-  2.0 fat     7227 b- defN 24-Apr-26 00:18 libpymcr/Matlab.py
--rw-rw-rw-  2.0 fat    10743 b- defN 24-Apr-26 00:18 libpymcr/MatlabProxyObject.py
--rw-rw-rw-  2.0 fat      203 b- defN 24-Apr-26 00:18 libpymcr/__init__.py
--rw-rw-rw-  2.0 fat   458240 b- defN 24-Apr-26 00:23 libpymcr/_libpymcr.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      518 b- defN 24-Apr-26 00:22 libpymcr/_version.py
--rw-rw-rw-  2.0 fat    13420 b- defN 24-Apr-26 00:18 libpymcr/utils.py
--rw-rw-rw-  2.0 fat    35823 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2586 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      960 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/RECORD
-12 files, 541767 bytes uncompressed, 202205 bytes compressed:  62.7%
+Zip file size: 209381 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat    11938 b- defN 24-May-30 09:00 libpymcr/IPythonMagics.py
+-rw-rw-rw-  2.0 fat     7264 b- defN 24-May-30 09:00 libpymcr/Matlab.py
+-rw-rw-rw-  2.0 fat    12239 b- defN 24-May-30 09:00 libpymcr/MatlabProxyObject.py
+-rw-rw-rw-  2.0 fat      203 b- defN 24-May-30 09:00 libpymcr/__init__.py
+-rw-rw-rw-  2.0 fat   458240 b- defN 24-May-30 09:06 libpymcr/_libpymcr.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      518 b- defN 24-May-30 09:06 libpymcr/_version.py
+-rw-rw-rw-  2.0 fat    14704 b- defN 24-May-30 09:00 libpymcr/utils.py
+-rw-rw-rw-  2.0 fat    16798 b- defN 24-May-30 09:00 libpymcr/scripts/matlab2python.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 24-May-30 09:00 libpymcr/scripts/parseclass.m
+-rw-rw-rw-  2.0 fat    35823 b- defN 24-May-30 09:07 libpymcr-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2586 b- defN 24-May-30 09:07 libpymcr-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-30 09:07 libpymcr-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       70 b- defN 24-May-30 09:07 libpymcr-0.1.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-30 09:07 libpymcr-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1233 b- defN 24-May-30 09:07 libpymcr-0.1.7.dist-info/RECORD
+15 files, 563295 bytes uncompressed, 207353 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -15,23 +15,32 @@
 
 Filename: libpymcr/_version.py
 Comment: 
 
 Filename: libpymcr/utils.py
 Comment: 
 
-Filename: libpymcr-0.1.6.dist-info/LICENSE
+Filename: libpymcr/scripts/matlab2python.py
 Comment: 
 
-Filename: libpymcr-0.1.6.dist-info/METADATA
+Filename: libpymcr/scripts/parseclass.m
 Comment: 
 
-Filename: libpymcr-0.1.6.dist-info/WHEEL
+Filename: libpymcr-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: libpymcr-0.1.6.dist-info/top_level.txt
+Filename: libpymcr-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: libpymcr-0.1.6.dist-info/RECORD
+Filename: libpymcr-0.1.7.dist-info/WHEEL
+Comment: 
+
+Filename: libpymcr-0.1.7.dist-info/entry_points.txt
+Comment: 
+
+Filename: libpymcr-0.1.7.dist-info/top_level.txt
+Comment: 
+
+Filename: libpymcr-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libpymcr/Matlab.py

```diff
@@ -49,15 +49,15 @@
         else:
             raise RuntimeError('Matlab interface is not open')
 
 
 class NamespaceWrapper(object):
     def __init__(self, interface, name):
         self._interface = interface
-        self._name = name
+        self._name = name[:-1] if name.endswith('_') else name
 
     def __getattr__(self, name):
         return NamespaceWrapper(self._interface, f'{self._name}.{name}')
 
     def __call__(self, *args, **kwargs):
         nargout = kwargs.pop('nargout') if 'nargout' in kwargs.keys() else None
         nreturn = get_nlhs(self._name)
```

## libpymcr/MatlabProxyObject.py

```diff
@@ -1,9 +1,10 @@
 from io import StringIO
 from .utils import get_nlhs
+import numpy as np
 import re
 
 def wrap(inputs, interface):
     # Matlab return types must be: np.array, opaque container, str, tuple, list, dict
     if 'matlab_wrapper' in str(type(inputs)):
         return MatlabProxyObject(interface, inputs)
     elif isinstance(inputs, tuple):
@@ -21,46 +22,83 @@
         return inputs.handle
     elif isinstance(inputs, matlab_method):
         nested_func_str = f'@(obj) @(varargin) {inputs.method}(obj, varargin{{:}})'
         meth_wrapper = interface.call('str2func', nested_func_str, nargout=1)
         return interface.call('feval', meth_wrapper, inputs.proxy.handle)
     elif isinstance(inputs, tuple):
         return tuple(unwrap(v, interface) for v in inputs)
-    elif isinstance(inputs, list):
+    elif isinstance(inputs, list) or isinstance(inputs, range):
         return [unwrap(v, interface) for v in inputs]
     elif isinstance(inputs, dict):
         return {k:unwrap(v, interface) for k, v in inputs.items()}
     else:
         return inputs
 
 
+class VectorPropertyWrapper:
+    # A proxy for a Matlab (ndarray) column vector to allow single indexing
+    def __init__(self, val):
+        self.val = val
+
+    def __getitem__(self, ind):
+        return self.val[0, ind] if ind > 0 else self.val[ind]
+
+    def __setitem__(self, ind, value):
+        if ind > 0:
+            self.val[0, ind] = value
+        else:
+            self.val[ind] = value
+
+    def __repr__(self):
+        return self.val.__repr__()
+
+
 class DictPropertyWrapper:
     # A proxy for dictionary properties of classes to allow Matlab .dot syntax
     def __init__(self, val, name, parent):
-        assert isinstance(val, dict), "DictPropertyWrapper can only wrap dict objects"
         self.__dict__['val'] = val
         self.__dict__['name'] = name
         self.__dict__['parent'] = parent
 
     def __getattr__(self, name):
         rv = self.val[name]
-        if isinstance(rv, dict):
+        if isinstance(rv, dict) or isinstance(rv, list):
             rv = DictPropertyWrapper(rv, name, self)
+        elif isinstance(rv, np.ndarray) and rv.shape[0] == 1:
+            rv = VectorPropertyWrapper(rv)
         return rv
 
     def __setattr__(self, name, value):
         self.val[name] = value
         setattr(self.parent, self.name, self.val)
 
+    def __getitem__(self, name):
+        rv = self.val[name]
+        if isinstance(rv, dict) or isinstance(rv, list):
+            rv = DictPropertyWrapper(rv, name, self)
+        return rv
+
+    def __setitem__(self, name, value):
+        self.val[name] = value
+        setattr(self.parent, self.name, self.val)
+
     def __repr__(self):
         rv = "Matlab struct with fields:\n"
         for k, v in self.val.items():
             rv += f"    {k}: {v}\n"
         return rv
 
+    @property
+    def __name__(self):
+        return self.name
+
+    @property
+    def __origin__(self):
+        return getattr(type(self.parent), self.name)
+
 
 class matlab_method:
     def __init__(self, proxy, method):
         self.proxy = proxy
         self.method = method
 
     def __call__(self, *args, **kwargs):
@@ -137,15 +175,15 @@
 
         """
         m = self.interface
         # if it's a property, just retrieve it
         if name in self._getAttributeNames():
             try:
                 rv = wrap(self.interface.call('subsref', self.handle, {'type':'.', 'subs':name}), self.interface)
-                if isinstance(rv, dict):
+                if isinstance(rv, dict) or isinstance(rv, list):
                     rv = DictPropertyWrapper(rv, name, self)
                 return rv
             except TypeError:
                 return None
         # if it's a method, wrap it in a functor
         elif name in self._methods:
             return matlab_method(self, name)
@@ -164,94 +202,94 @@
 
     def __dir__(self):
         return list(set(super(MatlabProxyObject, self).__dir__() + list(self.__dict__.keys()) + self._getAttributeNames()))
 
     def __getitem__(self, key):
         if not (isinstance(key, int) or (hasattr(key, 'is_integer') and key.is_integer())) or key < 0:
             raise RuntimeError('Matlab container indices must be positive integers')
-        key = [float(key + 1)]   # Matlab uses 1-based indexing
-        return self.interface.call('subsref', self.handle, {'type':'()', 'subs':key})
+        key = (float(key + 1),)   # Matlab uses 1-based indexing
+        return wrap(self.interface.call('subsref', self.handle, {'type':'()', 'subs':key}), self.interface)
 
     def __setitem__(self, key, value):
         if not (isinstance(key, int) or (hasattr(key, 'is_integer') and key.is_integer())) or key < 0:
             raise RuntimeError('Matlab container indices must be positive integers')
         if not isinstance(value, MatlabProxyObject) or repr(value) != self.__repr__():
             raise RuntimeError('Matlab container items must be same type.')
-        access = self.interface.call('substruct', '()', [float(key + 1)])   # Matlab uses 1-based indexing
-        self.__dict__['handle'] = self.interface.call('subsasgn', self.handle, access, value)
+        access = self.interface.call('substruct', '()', (float(key + 1),))   # Matlab uses 1-based indexing
+        self.__dict__['handle'] = self.interface.call('subsasgn', self.handle, access, value.handle)
 
     def __len__(self):
         return int(self.interface.call('numel', self.handle, nargout=1))
 
     # Operator overloads
     def __eq__(self, other):
-        return self.interface.call('eq', self.handle, other, nargout=1)
+        return self.interface.call('eq', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __ne__(self, other):
-        return self.interface.call('ne', self.handle, other, nargout=1)
+        return self.interface.call('ne', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __lt__(self, other):
-        return self.interface.call('lt', self.handle, other, nargout=1)
+        return self.interface.call('lt', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __gt__(self, other):
-        return self.interface.call('gt', self.handle, other, nargout=1)
+        return self.interface.call('gt', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __le__(self, other):
-        return self.interface.call('le', self.handle, other, nargout=1)
+        return self.interface.call('le', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __ge__(self, other):
-        return self.interface.call('ge', self.handle, other, nargout=1)
+        return self.interface.call('ge', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __bool__(self):
         return self.interface.call('logical', self.handle, nargout=1)
 
     def __and__(self, other):  # bit-wise & operator (not `and` keyword)
         return self.interface.call('and', self.handle, other, nargout=1)
 
     def __or__(self, other):   # bit-wise | operator (not `or` keyword)
-        return self.interface.call('or', self.handle, other, nargout=1)
+        return self.interface.call('or', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __invert__(self):      # bit-wise ~ operator (not `not` keyword)
         return self.interface.call('not', self.handle, nargout=1)
 
     def __pos__(self):
         return self.interface.call('uplus', self.handle, nargout=1)
 
     def __neg__(self):
         return self.interface.call('uminus', self.handle, nargout=1)
 
     def __abs__(self):
         return self.interface.call('abs', self.handle, nargout=1)
 
     def __add__(self, other):
-        return self.interface.call('plus', self.handle, other, nargout=1)
+        return self.interface.call('plus', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __radd__(self, other):
-        return self.interface.call('plus', other, self.handle, nargout=1)
+        return self.interface.call('plus', unwrap(other, self.interface), self.handle, nargout=1)
 
     def __sub__(self, other):
-        return self.interface.call('minus', self.handle, other, nargout=1)
+        return self.interface.call('minus', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __rsub__(self, other):
-        return self.interface.call('minus', other, self.handle, nargout=1)
+        return self.interface.call('minus', unwrap(other, self.interface), self.handle, nargout=1)
 
     def __mul__(self, other):
-        return self.interface.call('mtimes', self.handle, other, nargout=1)
+        return self.interface.call('mtimes', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __rmul__(self, other):
-        return self.interface.call('mtimes', other, self.handle, nargout=1)
+        return self.interface.call('mtimes', unwrap(other, self.interface), self.handle, nargout=1)
 
     def __truediv__(self, other):
-        return self.interface.call('mrdivide', self.handle, other, nargout=1)
+        return self.interface.call('mrdivide', self.handle, unwrap(other, self.interface), nargout=1)
 
     def __rtruediv__(self, other):
-        return self.interface.call('mrdivide', other, self.handle, nargout=1)
+        return self.interface.call('mrdivide', unwrap(other, self.interface), self.handle, nargout=1)
 
     def __pow__(self, other):
-        return self.interface.call('mpower', self.handle, other, nargout=1)
+        return self.interface.call('mpower', self.handle, unwrap(other, self.interface), nargout=1)
 
     @property
     def __doc__(self):
         out = StringIO()
         return self.interface.call('help', self.handle, nargout=1, stdout=out)
 
     def __del__(self):
```

## libpymcr/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-26T01:02:27+0100",
+ "date": "2024-05-30T09:36:18+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "3db55072cc2bbac9b2848bb3951752a67b24a534",
- "version": "0.1.6"
+ "full-revisionid": "607ec45b72ff9fb7078d9ecef697aa84653aa4b3",
+ "version": "0.1.7"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## libpymcr/utils.py

```diff
@@ -20,15 +20,17 @@
     "INPLACE_POWER", "INPLACE_MULTIPLY", "INPLACE_DIVIDE", "INPLACE_TRUE_DIVIDE", "INPLACE_FLOOR_DIVIDE",
     "INPLACE_MODULO", "INPLACE_ADD", "INPLACE_SUBTRACT", "INPLACE_LSHIFT", "INPLACE_RSHIFT",
     "INPLACE_AND", "INPLACE_XOR", "INPLACE_OR", "COMPARE_OP", "SET_UPDATE", "BUILD_CONST_KEY_MAP",
     "CALL_FUNCTION_EX", "LOAD_METHOD", "CALL_METHOD", "DICT_MERGE", "DICT_UPDATE", "LIST_EXTEND",
 }
 
 MLVERDIC = {f'R{rv[0]}{rv[1]}':f'9.{vr}' for rv, vr in zip([[yr, ab] for yr in range(2017,2023) for ab in ['a', 'b']], range(2, 14))}
-MLVERDIC.update({'R2023a':'9.14', 'R2023b':'23.2'})
+MLVERDIC.update({'R2023a':'9.14', 'R2023b':'23.2', 'R2024a':'24.1'})
+
+MLEXEFOUND = {}
 
 def get_nret_from_dis(frame):
     # Tries to get the number of return values for a function
     # Code adapted from Mantid/Framework/PythonInterface/mantid/kernel/funcinspect.py
     ins_stack = []
     call_fun_locs = {}
     start_i = 0
@@ -37,14 +39,16 @@
     for index, ins in enumerate(dis.get_instructions(frame.f_code)):
         ins_stack.append(ins)
         if ins.opname in OPERATOR_NAMES:
             call_fun_locs[start_offset] = start_i
             start_i = index
             start_offset = ins.offset
     call_fun_locs[start_offset] = start_i
+    if last_i not in call_fun_locs:
+        return 1  # Some error in the disassembly
     last_fun_offset = call_fun_locs[last_i]
     last_i_name = ins_stack[last_fun_offset].opname
     next_i_name = ins_stack[last_fun_offset + 1].opname
     if last_i_name == 'DICT_MERGE' and next_i_name in OPERATOR_NAMES:
         last_fun_offset += 1
         last_i = ins_stack[last_fun_offset + 1].offset
     res_i_name = ins_stack[last_fun_offset + 1].opname
@@ -113,19 +117,21 @@
                 ver = dict([v.split("=") for v in tag.split() if 'mcr' in v])
                 ver = [ver[v].replace('"', '') for v in ['mcr-major-version', 'mcr-minor-version']]
                 return "{}.{}".format(*ver)
 
 
 def get_matlab_from_registry(version=None):
     # Searches for the Mathworks registry key and finds the Matlab path from that
+    if version is not None and version.startswith('R') and version in MLVERDIC.keys():
+        version = MLVERDIC[version]
     retval = []
     try:
         import winreg
     except ImportError:
-        return retval
+        return None
     for installation in ['MATLAB', 'MATLAB Runtime', 'MATLAB Compiler Runtime']:
         try:
             with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, f'SOFTWARE\\MathWorks\\{installation}') as key:
                 versions = [winreg.EnumKey(key, k) for k in range(winreg.QueryInfoKey(key)[0])]
         except (FileNotFoundError, OSError):
             pass
         else:
@@ -134,139 +140,146 @@
             for v in versions:
                 with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, f'SOFTWARE\\MathWorks\\{installation}\\{v}') as key:
                     retval.append(winreg.QueryValueEx(key, 'MATLABROOT')[0])
     return retval
 
 
 class DetectMatlab(object):
-    def __init__(self, version):
+    def __init__(self, version=None):
         self.ver = version
-        self.PLATFORM_DICT = {'Windows': ['PATH', 'dll', ''], 'Linux': ['LD_LIBRARY_PATH', 'so', 'libmw'],
-                 'Darwin': ['DYLD_LIBRARY_PATH', 'dylib', 'libmw']}
+        self.PLATFORM_DICT = {'Windows': ['PATH', 'dll', '', '.exe', ';'], 'Linux': ['LD_LIBRARY_PATH', 'so', 'libmw', '', ':'],
+                              'Darwin': ['DYLD_LIBRARY_PATH', 'dylib', 'libmw', '', ':']}
         # Note that newer Matlabs are 64-bit only
         self.ARCH_DICT = {'Windows': {'64bit': 'win64', '32bit': 'pcwin32'},
                           'Linux': {'64bit': 'glnxa64', '32bit': 'glnx86'},
                           'Darwin': {'64bit': 'maci64', '32bit': 'maci'}}
         # https://uk.mathworks.com/help/compiler/mcr-path-settings-for-run-time-deployment.html
         DIRS = ['runtime', os.path.join('sys', 'os'), 'bin', os.path.join('extern', 'bin')]
         self.REQ_DIRS = {'Windows':[DIRS[0]], 'Darwin':DIRS[:3], 'Linux':DIRS}
         self.system = platform.system()
         if self.system not in self.PLATFORM_DICT:
-            raise RuntimeError('{0} is not a supported platform.'.format(self.system))
-        (self.path_var, self.ext, self.lib_prefix) = self.PLATFORM_DICT[self.system]
+            raise RuntimeError(f'Operating system {self.system} is not supported.')
+        (self.path_var, self.ext, self.lib_prefix, self.exe_ext, self.sep) = self.PLATFORM_DICT[self.system]
         self.arch = self.ARCH_DICT[self.system][platform.architecture()[0]]
         self.required_dirs = self.REQ_DIRS[self.system]
-        if self.system == 'Windows':
+        self.dirlevel = ('..', '..')
+        self.matlab_exe = ''.join(('matlab', self.exe_ext))
+        if self.ver is None:
+            self.file_to_find = self.matlab_exe
+            self.dirlevel = ('..',)
+        elif self.system == 'Windows':
             self.file_to_find = ''.join((self.lib_prefix, 'mclmcrrt', self.ver.replace('.','_'), '.', self.ext))
-            self.sep = ';'
         elif self.system == 'Linux':
             self.file_to_find = ''.join((self.lib_prefix, 'mclmcrrt', '.', self.ext, '.', self.ver))
-            self.sep = ':'
         elif self.system == 'Darwin':
             self.file_to_find = ''.join((self.lib_prefix, 'mclmcrrt', '.', self.ver, '.', self.ext))
-            self.sep = ':'
-        else:
-            raise RuntimeError(f'Operating system {self.system} is not supported.')
 
     @property
     def ver(self):
         return self._ver
 
     @ver.setter
     def ver(self, val):
-        self._ver = str(val)
-        if self._ver.startswith('R') and self._ver in MLVERDIC.keys():
-            self._ver = MLVERDIC[self._ver]
-
-    def find_version(self, root_dir):
-        print(f'Searching for Matlab {self.ver} in {root_dir}')
+        if val is None:
+            self._ver = None
+        else:
+            self._ver = str(val)
+            if self._ver.startswith('R') and self._ver in MLVERDIC.keys():
+                self._ver = MLVERDIC[self._ver]
+
+    def _append_exe(self, exe_file):
+        if exe_file is not None:
+            global MLEXEFOUND
+            if self.ver not in MLEXEFOUND:
+                MLEXEFOUND[self.ver] = os.path.abspath(Path(exe_file).parents[1])
+
+    def find_version(self, root_dir, suppress_output=False):
+        if not suppress_output:
+            print(f'Searching for Matlab {self.ver} in {root_dir}')
         def find_file(path, filename, max_depth=3):
             """ Finds a file, will return first match"""
             for depth in range(max_depth + 1):
                 dirglobs = f'*{os.sep}'*depth
                 files = glob.glob(f'{path}{os.sep}{dirglobs}{filename}')
                 files = list(filter(os.path.isfile, files))
                 if len(files) > 0:
                     return files[0]
             return None
         lib_file = find_file(root_dir, self.file_to_find)
         if lib_file is not None:
-            lib_path = Path(lib_file)
-            arch_dir = lib_path.parts[-2]
-            self.arch = arch_dir
-            ml_subdir = lib_path.parts[-3]
-            if ml_subdir != 'runtime':
-                self.ver = ml_subdir
-            ml_path = os.path.abspath(lib_path.parents[2])
-            print(f'Found Matlab {self.ver} {self.arch} at {ml_path}')
+            ml_path = os.path.abspath(os.path.join(os.path.dirname(lib_file), *self.dirlevel))
+            if not suppress_output:
+                print(f'Found Matlab {self.ver} {self.arch} at {ml_path}')
             return ml_path
         else:
+            self._append_exe(find_file(root_dir, self.matlab_exe))
             return None
 
-    def guess_path(self, mlPath=[]):
-        GUESSES = {'Windows': [r'C:\Program Files\MATLAB', r'C:\Program Files (x86)\MATLAB', 
+    def guess_path(self, mlPath=[], suppress_output=False):
+        GUESSES = {'Windows': [r'C:\Program Files\MATLAB', r'C:\Program Files (x86)\MATLAB',
                                r'C:\Program Files\MATLAB\MATLAB Runtime', r'C:\Program Files (x86)\MATLAB\MATLAB Runtime'],
                    'Linux': ['/usr/local/MATLAB', '/opt/MATLAB', '/opt', '/usr/local/MATLAB/MATLAB_Runtime'],
                    'Darwin': ['/Applications/MATLAB', '/Applications/']}
         if self.system == 'Windows':
             mlPath += get_matlab_from_registry(self.ver) + GUESSES['Windows']
         if 'MATLABEXECUTABLE' in os.environ: # Running in CI
             ml_env = os.environ['MATLABEXECUTABLE']
             if self.system == 'Windows' and ':' not in ml_env:
                 pp = ml_env.split('/')[1:]
                 ml_env = pp[0] + ':\\' + '\\'.join(pp[1:])
-            mlPath += [os.path.abspath(os.path.join(ml_env, '..', '..'))]
+            mlPath += [os.path.abspath(os.path.join(ml_env, *self.dirlevel))]
         for possible_dir in mlPath + GUESSES[self.system]:
             if os.path.isdir(possible_dir):
-                rv = self.find_version(possible_dir)
+                rv = self.find_version(possible_dir, suppress_output)
                 if rv is not None:
                    return rv
         return None
 
     def guess_from_env(self, ld_path=None):
         if ld_path is None:
             ld_path = os.getenv(self.path_var)
-        if ld_path is None: return None
+        if ld_path is None:
+            return None
         for possible_dir in ld_path.split(self.sep):
             if os.path.exists(os.path.join(possible_dir, self.file_to_find)):
-                return os.path.abspath(os.path.join(possible_dir, '..', '..'))
+                return os.path.abspath(os.path.join(possible_dir, *self.dirlevel))
         return None
 
-    def guess_from_syspath(self):
+    def guess_from_syspath(self, suppress_output=False):
         matlab_exe = shutil.which('matlab')
         if matlab_exe is None:
             return None if self.system == 'Windows' else self.guess_from_env('PATH')
         mlbinpath = os.path.dirname(os.path.realpath(matlab_exe))
-        return self.find_version(os.path.abspath(os.path.join(mlbinpath, '..')))
+        return self.find_version(os.path.abspath(os.path.join(mlbinpath, '..')), suppress_output)
 
-    def env_not_set(self):
-        # Determines if the environment variables required by the MCR are set
-        if self.path_var not in os.environ:
-            return True
-        rt = os.path.join('runtime', self.arch)
-        pv = os.getenv(self.path_var).split(self.sep)
-        for path in [dd for dd in pv if rt in dd]:
-            if self.find_version(os.path.join(path,'..','..')) is not None:
-                return False
-        return True
-
-    def set_environment(self, mlPath=None):
-        if mlPath is None:
-            mlPath = self.guess_path()
-        if mlPath is None:
-            raise RuntimeError('Could not find Matlab')
-        req_matlab_dirs = self.sep.join([os.path.join(mlPath, sub, self.arch) for sub in self.required_dirs])
-        if self.path_var not in os.environ:
-            os.environ[self.path_var] = req_matlab_dirs
-        else:
-            os.environ[self.path_var] += self.sep + req_matlab_dirs
-        return None
+    #def env_not_set(self, suppress_output=False):
+    #    # Determines if the environment variables required by the MCR are set
+    #    if self.path_var not in os.environ:
+    #        return True
+    #    rt = os.path.join('runtime', self.arch)
+    #    pv = os.getenv(self.path_var).split(self.sep)
+    #    for path in [dd for dd in pv if rt in dd]:
+    #        if self.find_version(os.path.join(path, *self.dirlevel), suppress_output) is not None:
+    #            return False
+    #    return True
+
+    #def set_environment(self, mlPath=None):
+    #    if mlPath is None:
+    #        mlPath = self.guess_path()
+    #    if mlPath is None:
+    #        raise RuntimeError('Could not find Matlab')
+    #    req_matlab_dirs = self.sep.join([os.path.join(mlPath, sub, self.arch) for sub in self.required_dirs])
+    #    if self.path_var not in os.environ:
+    #        os.environ[self.path_var] = req_matlab_dirs
+    #    else:
+    #        os.environ[self.path_var] += self.sep + req_matlab_dirs
+    #    return None
 
 
-def checkPath(runtime_version, mlPath=None, error_if_not_found=True):
+def checkPath(runtime_version, mlPath=None, error_if_not_found=True, suppress_output=False):
     """
     Sets the environmental variables for Win, Mac, Linux
 
     :param mlPath: Path to the SDK i.e. '/MATLAB/MATLAB_Runtime/v96' or to the location where matlab is installed
     (MATLAB root directory)
     :return: None
     """
@@ -285,12 +298,18 @@
         if mlPath is None:
             mlPath = obj.guess_path()
             if mlPath is not None:
                 ld_path = obj.sep.join([os.path.join(mlPath, sub, obj.arch) for sub in obj.required_dirs])
                 os.environ[obj.path_var] = ld_path
                 #print('Set ' + os.environ.get(obj.path_var))
             elif error_if_not_found:
-                raise RuntimeError('Cannot find Matlab')
+                if obj.ver in MLEXEFOUND:
+                    raise RuntimeError(f'Found Matlab executable for version {runtime_version} ' \
+                                        'but could not find Compiler Runtime libraries.\n' \
+                                        'Please install the Matlab Compiler Runtime SDK toolbox ' \
+                                        'for this version of Matlab')
+                else:
+                    raise RuntimeError(f'Cannot find Matlab version {runtime_version}')
         #else:
         #    print('Found: ' + os.environ.get(obj.path_var))
 
     return mlPath
```

## Comparing `libpymcr-0.1.6.dist-info/LICENSE` & `libpymcr-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libpymcr-0.1.6.dist-info/METADATA` & `libpymcr-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpymcr
-Version: 0.1.6
+Version: 0.1.7
 Summary: A module to allow Python to call functions from a compiled Matlab archive
 Home-page: https://github.com/pace-neutrons/libpymcr
 Author: Duc Le
 Author-email: duc.le@stfc.ac.uk
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

## Comparing `libpymcr-0.1.6.dist-info/RECORD` & `libpymcr-0.1.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 libpymcr/IPythonMagics.py,sha256=pXQHHYagcEXw7iZGF3VMJUmyvWmQMxL-sldW-RN2SKI,11938
-libpymcr/Matlab.py,sha256=gZJ_UOMF3S4VMBCzBl5HO7kkjHlnYop0YynIaFVv9qE,7227
-libpymcr/MatlabProxyObject.py,sha256=D5dJ1rDfj03rN-rotjGLnijp8jiwUDLoDWXr2zEmO9Q,10743
+libpymcr/Matlab.py,sha256=eG_KKt9myVKFfQlgeHOrUvrukTxnpBtfpxPJdyTnX2k,7264
+libpymcr/MatlabProxyObject.py,sha256=uq-cnh1Tq65U7Ct-CkkdBcnnxtI4m4IWD4dP6jfpNYE,12239
 libpymcr/__init__.py,sha256=8JZK4bh6W7u1D08OTswo67YzlP5JxLmmHTx-9MPazqU,203
-libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=n4k2m77sI3gzEULxfMLZ7WTHeunHBk7ExRlqiPDDLdk,458240
-libpymcr/_version.py,sha256=xIQBOoQxoIhgIErrBDa-aTtbSWREZdHc3qvqr3RK_nk,518
-libpymcr/utils.py,sha256=cu80K_8s82IBWdTd4DZCNyqzJe5N1Jl1eu5pdaU_8Kw,13420
-libpymcr-0.1.6.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-libpymcr-0.1.6.dist-info/METADATA,sha256=-omDSLe_FLyCQWuBwVPgjXS59pmGm8o4UVCM7ppWOko,2586
-libpymcr-0.1.6.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-libpymcr-0.1.6.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
-libpymcr-0.1.6.dist-info/RECORD,,
+libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=DrbDorQOM3czQjGI143HYdc9_iRz2dzO_WE_7omqotg,458240
+libpymcr/_version.py,sha256=DACn5VOEa61W-wRBzP5yDFWZzRy4tfy9j-9ncODeDas,518
+libpymcr/utils.py,sha256=TJT3ETT3yVHORP1T408X0vKgU63Gkc0vPepnXygtWu0,14704
+libpymcr/scripts/matlab2python.py,sha256=sTTXJLnZ0TIxBRCsdtowxIo3UNk87v_l6txeQT8XleE,16798
+libpymcr/scripts/parseclass.m,sha256=x8HMoNio2FZCbhjToVrognm-qyVxDk_ogOAqhNfs9WU,1570
+libpymcr-0.1.7.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+libpymcr-0.1.7.dist-info/METADATA,sha256=WJAuzU2DhegZFkfDC8_efE4MegDy9_0Ua6iFp_GkkNw,2586
+libpymcr-0.1.7.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+libpymcr-0.1.7.dist-info/entry_points.txt,sha256=LLwMJdD_ZJmtAOb9NRUpAnFTFn8RFNoHI_LrR7ElyDA,70
+libpymcr-0.1.7.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
+libpymcr-0.1.7.dist-info/RECORD,,
```

