# Comparing `tmp/libmem-5.0.0rc0.tar.gz` & `tmp/libmem-5.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmem-5.0.0rc0.tar", last modified: Tue Apr 16 18:32:06 2024, max compression
+gzip compressed data, was "libmem-5.0.0rc6.tar", last modified: Thu May 30 15:44:42 2024, max compression
```

## Comparing `libmem-5.0.0rc0.tar` & `libmem-5.0.0rc6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/
--rw-r--r--   0 user      (1000) user      (1000)       37 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)    10546 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    10012 2024-04-16 18:29:37.000000 libmem-5.0.0rc0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       99 2024-04-10 14:57:23.000000 libmem-5.0.0rc0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-16 18:32:06.365788 libmem-5.0.0rc0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     4510 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/setup.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.363788 libmem-5.0.0rc0/src/
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.363788 libmem-5.0.0rc0/src/libmem/
--rw-r--r--   0 user      (1000) user      (1000)     7967 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/src/libmem/__init__.py
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/src/libmem/_libmem/
--rw-r--r--   0 user      (1000) user      (1000)    40715 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/src/libmem/_libmem/libmem-py.c
--rw-r--r--   0 user      (1000) user      (1000)    13552 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/src/libmem/_libmem/types.h
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/src/libmem.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    10546 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      296 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       15 2024-04-16 18:32:06.000000 libmem-5.0.0rc0/src/libmem.egg-info/top_level.txt
-drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-04-16 18:32:06.364788 libmem-5.0.0rc0/tests/
--rw-r--r--   0 user      (1000) user      (1000)    14338 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/tests/test_mock.py
--rw-r--r--   0 user      (1000) user      (1000)     6846 2024-04-16 18:29:11.000000 libmem-5.0.0rc0/tests/tests.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-05-30 15:44:42.853122 libmem-5.0.0rc6/
+-rw-r--r--   0 user      (1000) user      (1000)       37 2024-04-16 18:29:11.000000 libmem-5.0.0rc6/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)    10799 2024-05-30 15:44:42.852122 libmem-5.0.0rc6/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    10265 2024-04-16 18:53:02.000000 libmem-5.0.0rc6/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       99 2024-04-10 14:57:23.000000 libmem-5.0.0rc6/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-30 15:44:42.853122 libmem-5.0.0rc6/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     4510 2024-05-30 12:28:55.000000 libmem-5.0.0rc6/setup.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-05-30 15:44:42.851122 libmem-5.0.0rc6/src/
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-05-30 15:44:42.851122 libmem-5.0.0rc6/src/libmem/
+-rw-r--r--   0 user      (1000) user      (1000)    12879 2024-05-30 14:16:02.000000 libmem-5.0.0rc6/src/libmem/__init__.py
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-05-30 15:44:42.852122 libmem-5.0.0rc6/src/libmem/_libmem/
+-rw-r--r--   0 user      (1000) user      (1000)    42207 2024-05-30 13:45:23.000000 libmem-5.0.0rc6/src/libmem/_libmem/libmem-py.c
+-rw-r--r--   0 user      (1000) user      (1000)    16546 2024-05-30 12:45:35.000000 libmem-5.0.0rc6/src/libmem/_libmem/types.h
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-05-30 15:44:42.852122 libmem-5.0.0rc6/src/libmem.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    10799 2024-05-30 15:44:42.000000 libmem-5.0.0rc6/src/libmem.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      296 2024-05-30 15:44:42.000000 libmem-5.0.0rc6/src/libmem.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-30 15:44:42.000000 libmem-5.0.0rc6/src/libmem.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       15 2024-05-30 15:44:42.000000 libmem-5.0.0rc6/src/libmem.egg-info/top_level.txt
+drwxr-sr-x   0 user      (1000) user      (1000)        0 2024-05-30 15:44:42.852122 libmem-5.0.0rc6/tests/
+-rw-r--r--   0 user      (1000) user      (1000)    14338 2024-04-16 18:29:11.000000 libmem-5.0.0rc6/tests/test_mock.py
+-rw-r--r--   0 user      (1000) user      (1000)     8725 2024-05-30 14:43:45.000000 libmem-5.0.0rc6/tests/tests.py
```

### Comparing `libmem-5.0.0rc0/PKG-INFO` & `libmem-5.0.0rc6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmem
-Version: 5.0.0rc0
+Version: 5.0.0rc6
 Summary: Advanced Game Hacking Library (Windows/Linux/FreeBSD)
 Home-page: https://github.com/rdbo/libmem
 Author: rdbo
 Project-URL: Documentation, https://github.com/rdbo/libmem/blob/master/docs/DOCS.md
 Project-URL: Bug Tracker, https://github.com/rdbo/libmem/issues
 Project-URL: Discord Server, https://discord.com/invite/Qw8jsPD99X
 Keywords: gamehacking memory process hooking detouring hacking winapi linux freebsd
@@ -131,14 +131,22 @@
 print(f"{code} : {inst.bytes}")
 
 print("[*] Disassembly:")
 inst = LM_Disassemble(bytearray(b"\x55"))
 print(f"{inst.bytes} : {inst.mnemonic} {inst.op_str}")
 ```
 
+## Unnoficial Bindings
+These bindings are done by the community/third-parties and are not affiliated with the libmem project or its author.
+
+Their code can have their own licenses as well, diverging from libmem's.
+
+- [Nim_Libmem](https://github.com/Hypnootika/Nim_Libmem)
+- [Crazymem (NodeJS)](https://github.com/karliky/Crazymem)
+
 ## CMake Usage (without installing)
 Add the following commands to your `CMakeLists.txt`.
 
 They will fetch `libmem-config.cmake` from the root of this repository, which will download libmem binaries for your system and include libmem in your CMake project.
 
 ```cmake
 include(FetchContent)
@@ -379,9 +387,7 @@
 Made with libmem:  
 - [AssaultCube Multihack](https://github.com/rdbo/AssaultCube-Multihack)  
 - [X-Inject](https://github.com/rdbo/x-inject)  
 - [DirectX9 BaseHook](https://github.com/rdbo/DX9-BaseHook)  
 - [DirectX11 BaseHook](https://github.com/rdbo/DX11-BaseHook)  
 - [OpenGL BaseHook](https://github.com/rdbo/GL-BaseHook)  
 - [Counter-Strike 1.6 BaseHook](https://github.com/rdbo/cstrike-basehook)  
-- [Crazymem - NodeJS Memory Library](https://github.com/karliky/Crazymem)  
-
```

### Comparing `libmem-5.0.0rc0/README.md` & `libmem-5.0.0rc6/src/libmem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: libmem
+Version: 5.0.0rc6
+Summary: Advanced Game Hacking Library (Windows/Linux/FreeBSD)
+Home-page: https://github.com/rdbo/libmem
+Author: rdbo
+Project-URL: Documentation, https://github.com/rdbo/libmem/blob/master/docs/DOCS.md
+Project-URL: Bug Tracker, https://github.com/rdbo/libmem/issues
+Project-URL: Discord Server, https://discord.com/invite/Qw8jsPD99X
+Keywords: gamehacking memory process hooking detouring hacking winapi linux freebsd
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 ![libmem-logo](https://raw.githubusercontent.com/rdbo/libmem/master/LOGO.png)  
 ### Advanced Game Hacking Library (C/C++/Rust/Python) (Windows/Linux/FreeBSD)
 ### Made by rdbo
 #  
 
 ## Discord Server
 https://discord.com/invite/Qw8jsPD99X
@@ -118,14 +131,22 @@
 print(f"{code} : {inst.bytes}")
 
 print("[*] Disassembly:")
 inst = LM_Disassemble(bytearray(b"\x55"))
 print(f"{inst.bytes} : {inst.mnemonic} {inst.op_str}")
 ```
 
+## Unnoficial Bindings
+These bindings are done by the community/third-parties and are not affiliated with the libmem project or its author.
+
+Their code can have their own licenses as well, diverging from libmem's.
+
+- [Nim_Libmem](https://github.com/Hypnootika/Nim_Libmem)
+- [Crazymem (NodeJS)](https://github.com/karliky/Crazymem)
+
 ## CMake Usage (without installing)
 Add the following commands to your `CMakeLists.txt`.
 
 They will fetch `libmem-config.cmake` from the root of this repository, which will download libmem binaries for your system and include libmem in your CMake project.
 
 ```cmake
 include(FetchContent)
@@ -366,9 +387,7 @@
 Made with libmem:  
 - [AssaultCube Multihack](https://github.com/rdbo/AssaultCube-Multihack)  
 - [X-Inject](https://github.com/rdbo/x-inject)  
 - [DirectX9 BaseHook](https://github.com/rdbo/DX9-BaseHook)  
 - [DirectX11 BaseHook](https://github.com/rdbo/DX11-BaseHook)  
 - [OpenGL BaseHook](https://github.com/rdbo/GL-BaseHook)  
 - [Counter-Strike 1.6 BaseHook](https://github.com/rdbo/cstrike-basehook)  
-- [Crazymem - NodeJS Memory Library](https://github.com/karliky/Crazymem)  
-
```

### Comparing `libmem-5.0.0rc0/setup.py` & `libmem-5.0.0rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from urllib.request import urlretrieve
 import tarfile
 
 additional_include_dirs = []
 additional_library_dirs = []
 
 def get_version():
-    return "5.0.0-pre0"
+    return "5.0.0-pre6"
 
 def get_operating_system():
     if sys.platform.find("bsd") != -1:
         return "bsd"
 
     if sys.platform == "win32":
         return "windows"
```

### Comparing `libmem-5.0.0rc0/src/libmem/_libmem/libmem-py.c` & `libmem-5.0.0rc6/src/libmem/_libmem/libmem-py.c`

 * *Files 6% similar despite different names*

```diff
@@ -36,23 +36,30 @@
 
 #define DECL_GLOBAL_PROT(var) { \
 	global = PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", var); \
 	PyObject_SetAttrString(pymod, #var, global); \
 	Py_DECREF(global); \
 }
 
+#define DECL_GLOBAL_ARCH(var) { \
+	global = PyObject_CallFunction((PyObject *)&py_lm_arch_t, "i", var); \
+	PyObject_SetAttrString(pymod, #var, global); \
+	Py_DECREF(global); \
+}
+
 static lm_bool_t
 _py_LM_EnumProcessesCallback(lm_process_t *pproc,
 			     lm_void_t    *arg)
 {
 	PyObject *pylist = (PyObject *)arg;
 	py_lm_process_obj *pyproc;
 
 	pyproc = (py_lm_process_obj *)PyObject_CallObject((PyObject *)&py_lm_process_t, NULL);
 	pyproc->proc = *pproc;
+	pyproc->arch = (py_lm_arch_obj *)PyObject_CallFunction((PyObject *)&py_lm_arch_t, "i", pyproc->proc.arch);
 
 	PyList_Append(pylist, (PyObject *)pyproc);
 
 	return LM_TRUE;
 }
 
 static PyObject *
@@ -81,14 +88,15 @@
 	py_lm_process_obj *pyproc;
 
 	if (!LM_GetProcess(&proc))
 		return Py_BuildValue("");
 
 	pyproc = (py_lm_process_obj *)PyObject_CallObject((PyObject *)&py_lm_process_t, NULL);
 	pyproc->proc = proc;
+	pyproc->arch = (py_lm_arch_obj *)PyObject_CallFunction((PyObject *)&py_lm_arch_t, "i", pyproc->proc.arch);
 
 	return (PyObject *)pyproc;
 }
 
 /****************************************/
 
 static PyObject *
@@ -103,41 +111,38 @@
 		return NULL;
 
 	if (!LM_GetProcessEx(pid, &proc))
 		return Py_BuildValue("");
 
 	pyproc = (py_lm_process_obj *)PyObject_CallObject((PyObject *)&py_lm_process_t, NULL);
 	pyproc->proc = proc;
+	pyproc->arch = (py_lm_arch_obj *)PyObject_CallFunction((PyObject *)&py_lm_arch_t, "i", pyproc->proc.arch);
 
 	return (PyObject *)pyproc;
 }
 
 /****************************************/
 
 static PyObject *
 py_LM_FindProcess(PyObject *self,
 		  PyObject *args)
 {
 	lm_char_t         *procstr;
 	lm_process_t       proc;
 	py_lm_process_obj *pyproc;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "u", &procstr))
-			return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "s", &procstr))
 		return NULL;
-#	endif
 
 	if (!LM_FindProcess(procstr, &proc))
 		return Py_BuildValue("");
 
 	pyproc = (py_lm_process_obj *)PyObject_CallObject((PyObject *)&py_lm_process_t, NULL);
 	pyproc->proc = proc;
+	pyproc->arch = (py_lm_arch_obj *)PyObject_CallFunction((PyObject *)&py_lm_arch_t, "i", pyproc->proc.arch);
 
 	return (PyObject *)pyproc;
 }
 
 /****************************************/
 
 static PyObject *
@@ -154,14 +159,23 @@
 
 	Py_RETURN_FALSE;
 }
 
 /****************************************/
 
 static PyObject *
+py_LM_GetBits(PyObject *self,
+		    PyObject *args)
+{
+	return PyLong_FromSize_t(LM_GetBits());
+}
+
+/****************************************/
+
+static PyObject *
 py_LM_GetSystemBits(PyObject *self,
 		    PyObject *args)
 {
 	return PyLong_FromSize_t(LM_GetSystemBits());
 }
 
 /****************************************/
@@ -275,14 +289,15 @@
 		return NULL;
 
 	if (!LM_GetThreadProcess(&pythread->thread, &proc))
 		return Py_BuildValue("");
 
 	pyproc = (py_lm_process_obj *)PyObject_CallObject((PyObject *)&py_lm_process_t, NULL);
 	pyproc->proc = proc;
+	pyproc->arch = (py_lm_arch_obj *)PyObject_CallFunction((PyObject *)&py_lm_arch_t, "i", pyproc->proc.arch);
 
 	return (PyObject *)pyproc;
 }
 
 /****************************************/
 
 static lm_bool_t
@@ -346,21 +361,16 @@
 py_LM_FindModule(PyObject *self,
 		 PyObject *args)
 {
 	lm_char_t        *modstr;
 	lm_module_t       mod;
 	py_lm_module_obj *pymodule;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "u", &modstr))
-			return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "s", &modstr))
 		return NULL;
-#	endif
 
 	if (!LM_FindModule(modstr, &mod))
 		return Py_BuildValue("");
 
 	pymodule = (py_lm_module_obj *)PyObject_CallObject((PyObject *)&py_lm_module_t, NULL);
 	pymodule->mod = mod;
 
@@ -374,21 +384,16 @@
 		   PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_char_t         *modstr;
 	lm_module_t        mod;
 	py_lm_module_obj  *pymodule;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "Ou", &pyproc, &modstr))
-			return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "Os", &pyproc, &modstr))
 		return NULL;
-#	endif
 
 	if (!LM_FindModuleEx(&pyproc->proc, modstr, &mod))
 		return Py_BuildValue("");
 
 	pymodule = (py_lm_module_obj *)PyObject_CallObject((PyObject *)&py_lm_module_t, NULL);
 	pymodule->mod = mod;
 
@@ -401,21 +406,16 @@
 py_LM_LoadModule(PyObject *self,
 		 PyObject *args)
 {
 	lm_char_t        *modpath;
 	lm_module_t       mod;
 	py_lm_module_obj *pymodule;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "u", &modpath))
-			return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "s", &modpath))
 		return NULL;
-#	endif
 
 	if (!LM_LoadModule(modpath, &mod))
 		return Py_BuildValue("");
 
 	pymodule = (py_lm_module_obj *)PyObject_CallObject((PyObject *)&py_lm_module_t, NULL);
 	pymodule->mod = mod;
 
@@ -429,21 +429,16 @@
 		   PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_char_t         *modpath;
 	lm_module_t        mod;
 	py_lm_module_obj  *pymodule;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "Ou", &pyproc, &modpath))
-			return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "Os", &pyproc, &modpath))
 		return NULL;
-#	endif
 
 	if (!LM_LoadModuleEx(&pyproc->proc, modpath, &mod))
 		return Py_BuildValue("");
 
 	pymodule = (py_lm_module_obj *)PyObject_CallObject((PyObject *)&py_lm_module_t, NULL);
 	pymodule->mod = mod;
 
@@ -528,15 +523,15 @@
 /****************************************/
 
 static PyObject *
 py_LM_FindSymbolAddress(PyObject *self,
 			PyObject *args)
 {
 	py_lm_module_obj *pymodule;
-	lm_cchar_t       *symname;
+	lm_char_t        *symname;
 	lm_address_t      symaddr;
 
 	if (!PyArg_ParseTuple(args, "Os", &pymodule, &symname))
 		return NULL;
 
 	symaddr = LM_FindSymbolAddress(&pymodule->mod, symname);
 	if (symaddr == LM_ADDRESS_BAD)
@@ -547,28 +542,28 @@
 
 /****************************************/
 
 static PyObject *
 py_LM_DemangleSymbol(PyObject *self,
 		     PyObject *args)
 {
-	lm_cchar_t  *symbol;
-	lm_cstring_t newsym;
+	lm_char_t  *symbol;
+	lm_char_t  *newsym;
 	PyObject    *pynewsym;
 
 	if (!PyArg_ParseTuple(args, "s", &symbol))
 		return NULL;
 
-	newsym = LM_DemangleSymbol(symbol, (lm_cchar_t *)LM_NULLPTR, 0);
+	newsym = LM_DemangleSymbol(symbol, (lm_char_t *)LM_NULLPTR, 0);
 	if (!newsym)
 		return Py_BuildValue("");
 
 	pynewsym = PyUnicode_FromString(newsym);
 
-	LM_FreeDemangleSymbol(newsym);
+	LM_FreeDemangledSymbol(newsym);
 
 	return pynewsym;
 }
 
 /****************************************/
 
 static PyObject *
@@ -596,15 +591,15 @@
 /****************************************/
 
 static PyObject *
 py_LM_FindSymbolAddressDemangled(PyObject *self,
 				 PyObject *args)
 {
 	py_lm_module_obj *pymodule;
-	lm_cchar_t       *symname;
+	lm_char_t       *symname;
 	lm_address_t      symaddr;
 
 	if (!PyArg_ParseTuple(args, "Os", &pymodule, &symname))
 		return NULL;
 
 	symaddr = LM_FindSymbolAddressDemangled(&pymodule->mod, symname);
 	if (symaddr == LM_ADDRESS_BAD)
@@ -612,114 +607,114 @@
 
 	return (PyObject *)PyLong_FromSize_t(symaddr);
 }
 
 /****************************************/
 
 static lm_bool_t
-_py_LM_EnumPagesCallback(lm_page_t *ppage,
-			 lm_void_t *arg)
+_py_LM_EnumSegmentsCallback(lm_segment_t *psegment,
+			    lm_void_t *arg)
 {
 	PyObject *pylist = (PyObject *)arg;
-	py_lm_page_obj *pypage;
+	py_lm_segment_obj *pysegment;
 
-	pypage = (py_lm_page_obj *)PyObject_CallObject((PyObject *)&py_lm_page_t, NULL);
-	pypage->page = *ppage;
-	pypage->prot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", pypage->page.prot);
+	pysegment = (py_lm_segment_obj *)PyObject_CallObject((PyObject *)&py_lm_segment_t, NULL);
+	pysegment->segment = *psegment;
+	pysegment->prot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", pysegment->segment.prot);
 
-	PyList_Append(pylist, (PyObject *)pypage);
+	PyList_Append(pylist, (PyObject *)pysegment);
 
 	return LM_TRUE;
 }
 
 static PyObject *
-py_LM_EnumPages(PyObject *self,
+py_LM_EnumSegments(PyObject *self,
 		PyObject *args)
 {
 	PyObject *pylist = PyList_New(0);
 	if (!pylist)
 		return NULL;
 
-	if (!LM_EnumPages(_py_LM_EnumPagesCallback, (lm_void_t *)pylist)) {
+	if (!LM_EnumSegments(_py_LM_EnumSegmentsCallback, (lm_void_t *)pylist)) {
 		Py_DECREF(pylist); /* destroy list */
 		pylist = Py_BuildValue("");
 	}
 
 	return pylist;
 }
 
 /****************************************/
 
 static PyObject *
-py_LM_EnumPagesEx(PyObject *self,
+py_LM_EnumSegmentsEx(PyObject *self,
 		  PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	PyObject *pylist;
 
 	if (!PyArg_ParseTuple(args, "O", &pyproc))
 		return NULL;
 	
 	pylist = PyList_New(0);
 	if (!pylist)
 		return NULL;
 
-	if (!LM_EnumPagesEx(&pyproc->proc, _py_LM_EnumPagesCallback, (lm_void_t *)pylist)) {
+	if (!LM_EnumSegmentsEx(&pyproc->proc, _py_LM_EnumSegmentsCallback, (lm_void_t *)pylist)) {
 		Py_DECREF(pylist); /* destroy list */
 		pylist = Py_BuildValue("");
 	}
 
 	return pylist;
 }
 
 /****************************************/
 
 static PyObject *
-py_LM_GetPage(PyObject *self,
-	      PyObject *args)
+py_LM_FindSegment(PyObject *self,
+		  PyObject *args)
 {
 	lm_address_t address;
-	lm_page_t page;
-	py_lm_page_obj *pypage;
+	lm_segment_t segment;
+	py_lm_segment_obj *pysegment;
 
 	if (!PyArg_ParseTuple(args, "n", &address))
 		return NULL;
 
-	if (!LM_GetPage(address, &page))
+	if (!LM_FindSegment(address, &segment))
 		return Py_BuildValue("");
 
-	pypage = (py_lm_page_obj *)PyObject_CallObject((PyObject *)&py_lm_page_t, NULL);
-	pypage->page = page;
-	pypage->prot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", pypage->page.prot);
+	pysegment = (py_lm_segment_obj *)PyObject_CallObject((PyObject *)&py_lm_segment_t, NULL);
+	pysegment->segment = segment;
+	pysegment->prot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", pysegment->segment.prot);
 
-	return (PyObject *)pypage;
+	return (PyObject *)pysegment;
 }
 
 /****************************************/
 
 static PyObject *
-py_LM_GetPageEx(PyObject *self,
+py_LM_FindSegmentEx(PyObject *self,
 		PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t address;
-	lm_page_t page;
-	py_lm_page_obj *pypage;
+	lm_segment_t segment;
+	py_lm_segment_obj *pysegment;
 
 	if (!PyArg_ParseTuple(args, "On", &pyproc, &address))
 		return NULL;
 
-	if (!LM_GetPageEx(&pyproc->proc, address, &page))
+	if (!LM_FindSegmentEx(&pyproc->proc, address, &segment))
 		return Py_BuildValue("");
 
-	pypage = (py_lm_page_obj *)PyObject_CallObject((PyObject *)&py_lm_page_t, NULL);
-	pypage->page = page;
-	pypage->prot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", pypage->page.prot);
+	pysegment = (py_lm_segment_obj *)PyObject_CallObject((PyObject *)&py_lm_segment_t, NULL);
+	pysegment->segment = segment;
+	pysegment->prot = (py_lm_prot_obj *)PyObject_CallFunction((PyObject *)&py_lm_prot_t, "i", pysegment->segment.prot);
 
-	return (PyObject *)pypage;
+	return (PyObject *)pysegment;
 }
 
 /****************************************/
 
 static PyObject *
 py_LM_ReadMemory(PyObject *self,
 		 PyObject *args)
@@ -728,25 +723,25 @@
 	lm_size_t size;
 	lm_byte_t *dst;
 	PyObject *pybuf;
 
 	if (!PyArg_ParseTuple(args, "nn", &src, &size))
 		return NULL;
 
-	dst = LM_MALLOC(size);
+	dst = malloc(size);
 	if (!dst)
 		return Py_BuildValue("");
 
 	if (LM_ReadMemory(src, dst, size) == size) {
 		pybuf = PyByteArray_FromStringAndSize((const char *)dst, size);
 	} else {
 		pybuf = Py_BuildValue("");
 	}
 
-	LM_FREE(dst);
+	free(dst);
 
 	return pybuf;
 }
 
 /****************************************/
 
 static PyObject *
@@ -758,44 +753,44 @@
 	lm_size_t size;
 	lm_byte_t *dst;
 	PyObject *pybuf;
 
 	if (!PyArg_ParseTuple(args, "Onn", &pyproc, &src, &size))
 		return NULL;
 
-	dst = LM_MALLOC(size);
+	dst = malloc(size);
 	if (!dst)
 		return Py_BuildValue("");
 
 	if (LM_ReadMemoryEx(&pyproc->proc, src, dst, size) == size) {
 		pybuf = PyByteArray_FromStringAndSize((const char *)dst, size);
 	} else {
 		pybuf = Py_BuildValue("");
 	}
 
-	LM_FREE(dst);
+	free(dst);
 
 	return pybuf;
 }
 
 /****************************************/
 
 static PyObject *
 py_LM_WriteMemory(PyObject *self,
 		  PyObject *args)
 {
 	lm_address_t dst;
 	PyObject *pysrc;
-	lm_bytearr_t src;
+	lm_bytearray_t src;
 	lm_size_t size;
 
 	if (!PyArg_ParseTuple(args, "nY", &dst, &pysrc))
 		return NULL;
 
-	src = (lm_bytearr_t)PyByteArray_AsString(pysrc);
+	src = (lm_bytearray_t)PyByteArray_AsString(pysrc);
 	size = (lm_size_t)PyByteArray_Size(pysrc);
 
 	if (LM_WriteMemory(dst, src, size) != size)
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
 }
@@ -805,21 +800,21 @@
 static PyObject *
 py_LM_WriteMemoryEx(PyObject *self,
 		    PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	lm_address_t dst;
 	PyObject *pysrc;
-	lm_bytearr_t src;
+	lm_bytearray_t src;
 	lm_size_t size;
 
 	if (!PyArg_ParseTuple(args, "OnY", &pyproc, &dst, &pysrc))
 		return NULL;
 
-	src = (lm_bytearr_t)PyByteArray_AsString(pysrc);
+	src = (lm_bytearray_t)PyByteArray_AsString(pysrc);
 	size = (lm_size_t)PyByteArray_Size(pysrc);
 
 	if (LM_WriteMemoryEx(&pyproc->proc, dst, src, size) != size)
 		Py_RETURN_FALSE;
 
 	Py_RETURN_TRUE;
 }
@@ -1008,25 +1003,25 @@
 	if (!PyArg_ParseTuple(args, "nO", &base, &pyoffsets))
 		return NULL;
 
 	noffsets = PyList_Size(pyoffsets);
 	if (noffsets == 0)
 		return PyLong_FromSize_t(base);
 
-	offsets = LM_CALLOC(sizeof(lm_address_t), noffsets);
+	offsets = calloc(sizeof(lm_address_t), noffsets);
 	if (!offsets)
 		return NULL;
 
 	for (i = 0; i < noffsets; ++i) {
 		offsets[i] = (lm_address_t)PyLong_AsSize_t(PyList_GetItem(pyoffsets, i));
 	}
 
 	pointer = LM_DeepPointer(base, offsets, noffsets);
 
-	LM_FREE(offsets);
+	free(offsets);
 
 	if (pointer == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(pointer);
 }
 
@@ -1047,25 +1042,25 @@
 	if (!PyArg_ParseTuple(args, "OnO", &pyproc, &base, &pyoffsets))
 		return NULL;
 
 	noffsets = PyList_Size(pyoffsets);
 	if (noffsets == 0)
 		return PyLong_FromSize_t(base);
 
-	offsets = LM_CALLOC(sizeof(lm_address_t), noffsets);
+	offsets = calloc(sizeof(lm_address_t), noffsets);
 	if (!offsets)
 		return NULL;
 
 	for (i = 0; i < noffsets; ++i) {
 		offsets[i] = (lm_address_t)PyLong_AsSize_t(PyList_GetItem(pyoffsets, i));
 	}
 
 	pointer = LM_DeepPointerEx(&pyproc->proc, base, offsets, noffsets);
 
-	LM_FREE(offsets);
+	free(offsets);
 
 	if (pointer == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(pointer);
 }
 
@@ -1074,22 +1069,22 @@
 static PyObject *
 py_LM_DataScan(PyObject *self,
 	       PyObject *args)
 {
 	PyObject *pydata;
 	lm_address_t addr;
 	lm_size_t scansize;
-	lm_bytearr_t data;
+	lm_bytearray_t data;
 	lm_size_t size;
 	lm_address_t scan_match;
 
 	if (!PyArg_ParseTuple(args, "Ynn", &pydata, &addr, &scansize))
 		return NULL;
 
-	data = (lm_bytearr_t)PyByteArray_AsString(pydata);
+	data = (lm_bytearray_t)PyByteArray_AsString(pydata);
 	size = (lm_size_t)PyByteArray_Size(pydata);
 
 	scan_match = LM_DataScan(data, size, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(scan_match);
@@ -1101,22 +1096,22 @@
 py_LM_DataScanEx(PyObject *self,
 		 PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	PyObject *pydata;
 	lm_address_t addr;
 	lm_size_t scansize;
-	lm_bytearr_t data;
+	lm_bytearray_t data;
 	lm_size_t size;
 	lm_address_t scan_match;
 
 	if (!PyArg_ParseTuple(args, "OYnn", &pyproc, &pydata, &addr, &scansize))
 		return NULL;
 
-	data = (lm_bytearr_t)PyByteArray_AsString(pydata);
+	data = (lm_bytearray_t)PyByteArray_AsString(pydata);
 	size = (lm_size_t)PyByteArray_Size(pydata);
 
 	scan_match = LM_DataScanEx(&pyproc->proc, data, size, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(scan_match);
@@ -1128,26 +1123,21 @@
 py_LM_PatternScan(PyObject *self,
 		  PyObject *args)
 {
 	PyObject *pypattern;
 	lm_char_t *mask;
 	lm_address_t addr;
 	lm_size_t scansize;
-	lm_bytearr_t pattern;
+	lm_bytearray_t pattern;
 	lm_address_t scan_match;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "Yunn", &pypattern, &mask, &addr, &scansize))
-		return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "Ysnn", &pypattern, &mask, &addr, &scansize))
 		return NULL;
-#	endif
 
-	pattern = (lm_bytearr_t)PyByteArray_AsString(pypattern);
+	pattern = (lm_bytearray_t)PyByteArray_AsString(pypattern);
 
 	scan_match = LM_PatternScan(pattern, mask, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(scan_match);
 }
@@ -1159,26 +1149,21 @@
 		    PyObject *args)
 {
 	py_lm_process_obj *pyproc;
 	PyObject *pypattern;
 	lm_char_t *mask;
 	lm_address_t addr;
 	lm_size_t scansize;
-	lm_bytearr_t pattern;
+	lm_bytearray_t pattern;
 	lm_address_t scan_match;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "OYunn", &pyproc, &pypattern, &mask, &addr, &scansize))
-		return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "OYsnn", &pyproc, &pypattern, &mask, &addr, &scansize))
 		return NULL;
-#	endif
 
-	pattern = (lm_bytearr_t)PyByteArray_AsString(pypattern);
+	pattern = (lm_bytearray_t)PyByteArray_AsString(pypattern);
 
 	scan_match = LM_PatternScanEx(&pyproc->proc, pattern, mask, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(scan_match);
 }
@@ -1190,21 +1175,16 @@
 	      PyObject *args)
 {
 	lm_char_t *sig;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_address_t scan_match;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "unn", &sig, &addr, &scansize))
-		return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "snn", &sig, &addr, &scansize))
 		return NULL;
-#	endif
 
 	scan_match = LM_SigScan(sig, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(scan_match);
 }
@@ -1217,118 +1197,40 @@
 {
 	py_lm_process_obj *pyproc;
 	lm_char_t *sig;
 	lm_address_t addr;
 	lm_size_t scansize;
 	lm_address_t scan_match;
 
-#	if LM_CHARSET == LM_CHARSET_UC
-	if (!PyArg_ParseTuple(args, "Ounn", &pyproc, &sig, &addr, &scansize))
-		return NULL;
-#	else
 	if (!PyArg_ParseTuple(args, "Osnn", &pyproc, &sig, &addr, &scansize))
 		return NULL;
-#	endif
 
 	scan_match = LM_SigScanEx(&pyproc->proc, sig, addr, scansize);
 	if (scan_match == LM_ADDRESS_BAD)
 		return Py_BuildValue("");
 
 	return PyLong_FromSize_t(scan_match);
 }
 
 /****************************************/
 
 static PyObject *
-py_LM_HookCode(PyObject *self,
-	       PyObject *args)
-{
-	lm_address_t from;
-	lm_address_t to;
-	lm_address_t trampoline;
-	lm_size_t    size;
-
-	if (!PyArg_ParseTuple(args, "nn", &from, &to))
-		return NULL;
-
-	size = LM_HookCode(from, to, &trampoline);
-	if (!size)
-		return Py_BuildValue("");
-
-	return Py_BuildValue("(nn)", trampoline, size);
-}
-
-/****************************************/
-
-static PyObject *
-py_LM_HookCodeEx(PyObject *self,
-		 PyObject *args)
+py_LM_GetArchitecture(PyObject *self,
+		      PyObject *args)
 {
-	py_lm_process_obj *pyproc;
-	lm_address_t from;
-	lm_address_t to;
-	lm_address_t trampoline;
-	lm_size_t    size;
-
-	if (!PyArg_ParseTuple(args, "Onn", &pyproc, &from, &to))
-		return NULL;
-
-	size = LM_HookCodeEx(&pyproc->proc, from, to, &trampoline);
-	if (!size)
-		return Py_BuildValue("");
-
-	return Py_BuildValue("(nn)", trampoline, size);
-}
-
-/****************************************/
-
-static PyObject *
-py_LM_UnhookCode(PyObject *self,
-		 PyObject *args)
-{
-	lm_address_t from;
-	lm_address_t trampoline;
-	lm_size_t    size;
-
-	if (!PyArg_ParseTuple(args, "n(nn)", &from, &trampoline, &size))
-		return NULL;
-
-	if (!LM_UnhookCode(from, trampoline, size))
-		Py_RETURN_FALSE;
-
-	Py_RETURN_TRUE;
-}
-
-/****************************************/
-
-static PyObject *
-py_LM_UnhookCodeEx(PyObject *self,
-		   PyObject *args)
-{
-	py_lm_process_obj *pyproc;
-	lm_address_t from;
-	lm_address_t trampoline;
-	lm_size_t    size;
-
-	if (!PyArg_ParseTuple(args, "On(nn)", &pyproc, &from, &trampoline, &size))
-		return NULL;
-
-	if (!LM_UnhookCodeEx(&pyproc->proc, from, trampoline, size))
-		Py_RETURN_FALSE;
-
-	Py_RETURN_TRUE;
+	return PyObject_CallFunction((PyObject *)&py_lm_arch_t, "i", LM_GetArchitecture());
 }
 
 /****************************************/
 
 static PyObject *
 py_LM_Assemble(PyObject *self,
 	       PyObject *args)
 {
-	lm_cstring_t code;
+	lm_string_t code;
 	lm_inst_t inst;
 	py_lm_inst_obj *pyinst;
 
 	if (!PyArg_ParseTuple(args, "s", &code))
 		return NULL;
 
 	if (!LM_Assemble(code, &inst))
@@ -1342,31 +1244,31 @@
 
 /****************************************/
 
 static PyObject *
 py_LM_AssembleEx(PyObject *self,
 		 PyObject *args)
 {
-	lm_cstring_t code;
-	lm_size_t bits;
+	lm_string_t code;
+	py_lm_arch_obj *pyarch;
 	lm_address_t runtime_addr;
-	lm_bytearr_t codebuf;
+	lm_byte_t *codebuf;
 	lm_size_t codelen;
 	PyObject *pycodebuf;
 
-	if (!PyArg_ParseTuple(args, "snn", &code, &bits, &runtime_addr))
+	if (!PyArg_ParseTuple(args, "sOn", &code, &pyarch, &runtime_addr))
 		return NULL;
 
-	codelen = LM_AssembleEx(code, bits, runtime_addr, &codebuf);
+	codelen = LM_AssembleEx(code, pyarch->arch, runtime_addr, &codebuf);
 	if (!codelen)
 		return Py_BuildValue("");
 
 	pycodebuf = PyByteArray_FromStringAndSize((const char *)codebuf, codelen);
 
-	LM_FreeCodeBuffer(codebuf);
+	LM_FreePayload(codebuf);
 
 	return pycodebuf;
 }
 
 /****************************************/
 
 static PyObject *
@@ -1392,28 +1294,28 @@
 /****************************************/
 
 static PyObject *
 py_LM_DisassembleEx(PyObject *self,
 		    PyObject *args)
 {
 	lm_address_t code;
-	lm_size_t bits;
+	py_lm_arch_obj *pyarch;
 	lm_size_t size;
 	lm_size_t count;
 	lm_address_t runtime_addr;
 	lm_inst_t *insts;
 	lm_size_t inst_count;
 	PyObject *pyinsts;
 	lm_size_t i;
 	py_lm_inst_obj *pyinst;
 
-	if (!PyArg_ParseTuple(args, "nnnnn", &code, &bits, &size, &count, &runtime_addr))
+	if (!PyArg_ParseTuple(args, "nOnnn", &code, &pyarch, &size, &count, &runtime_addr))
 		return NULL;
 
-	inst_count = LM_DisassembleEx(code, bits, size, count, runtime_addr, &insts);
+	inst_count = LM_DisassembleEx(code, pyarch->arch, size, count, runtime_addr, &insts);
 	if (!inst_count)
 		return Py_BuildValue("");
 
 	pyinsts = PyList_New((Py_ssize_t)inst_count);
 	for (i = 0; i < inst_count; ++i) {
 		pyinst = (py_lm_inst_obj *)PyObject_CallObject((PyObject *)&py_lm_inst_t, NULL);
 		pyinst->inst = insts[i];
@@ -1464,20 +1366,103 @@
 		return Py_BuildValue("");
 
 	return (PyObject *)PyLong_FromSize_t(aligned_length);
 }
 
 /****************************************/
 
+static PyObject *
+py_LM_HookCode(PyObject *self,
+	       PyObject *args)
+{
+	lm_address_t from;
+	lm_address_t to;
+	lm_address_t trampoline;
+	lm_size_t    size;
+
+	if (!PyArg_ParseTuple(args, "nn", &from, &to))
+		return NULL;
+
+	size = LM_HookCode(from, to, &trampoline);
+	if (!size)
+		return Py_BuildValue("");
+
+	return Py_BuildValue("(nn)", trampoline, size);
+}
+
+/****************************************/
+
+static PyObject *
+py_LM_HookCodeEx(PyObject *self,
+		 PyObject *args)
+{
+	py_lm_process_obj *pyproc;
+	lm_address_t from;
+	lm_address_t to;
+	lm_address_t trampoline;
+	lm_size_t    size;
+
+	if (!PyArg_ParseTuple(args, "Onn", &pyproc, &from, &to))
+		return NULL;
+
+	size = LM_HookCodeEx(&pyproc->proc, from, to, &trampoline);
+	if (!size)
+		return Py_BuildValue("");
+
+	return Py_BuildValue("(nn)", trampoline, size);
+}
+
+/****************************************/
+
+static PyObject *
+py_LM_UnhookCode(PyObject *self,
+		 PyObject *args)
+{
+	lm_address_t from;
+	lm_address_t trampoline;
+	lm_size_t    size;
+
+	if (!PyArg_ParseTuple(args, "n(nn)", &from, &trampoline, &size))
+		return NULL;
+
+	if (!LM_UnhookCode(from, trampoline, size))
+		Py_RETURN_FALSE;
+
+	Py_RETURN_TRUE;
+}
+
+/****************************************/
+
+static PyObject *
+py_LM_UnhookCodeEx(PyObject *self,
+		   PyObject *args)
+{
+	py_lm_process_obj *pyproc;
+	lm_address_t from;
+	lm_address_t trampoline;
+	lm_size_t    size;
+
+	if (!PyArg_ParseTuple(args, "On(nn)", &pyproc, &from, &trampoline, &size))
+		return NULL;
+
+	if (!LM_UnhookCodeEx(&pyproc->proc, from, trampoline, size))
+		Py_RETURN_FALSE;
+
+	Py_RETURN_TRUE;
+}
+
+/****************************************/
+
 static PyMethodDef libmem_methods[] = {
 	{ "LM_EnumProcesses", py_LM_EnumProcesses, METH_NOARGS, "Lists all current living processes" },
 	{ "LM_GetProcess", py_LM_GetProcess, METH_NOARGS, "Gets information about the calling process" },
 	{ "LM_GetProcessEx", py_LM_GetProcessEx, METH_VARARGS, "Gets information about a process from a process ID" },
 	{ "LM_FindProcess", py_LM_FindProcess, METH_VARARGS, "Searches for an existing process" },
 	{ "LM_IsProcessAlive", py_LM_IsProcessAlive, METH_VARARGS, "Checks if a process is alive" },
+	{ "LM_GetBits", py_LM_GetBits, METH_VARARGS, "Checks if a process is alive" },
 	{ "LM_GetSystemBits", py_LM_GetSystemBits, METH_VARARGS, "Checks if a process is alive" },
 	/****************************************/
 	{ "LM_EnumThreads", py_LM_EnumThreads, METH_NOARGS, "Lists all threads from the calling process" },
 	{ "LM_EnumThreadsEx", py_LM_EnumThreadsEx, METH_VARARGS, "Lists all threads from the calling process" },
 	{ "LM_GetThread", py_LM_GetThread, METH_NOARGS, "Get information about the calling thread" },
 	{ "LM_GetThreadEx", py_LM_GetThreadEx, METH_VARARGS, "Get information about a remote thread" },
 	{ "LM_GetThreadProcess", py_LM_GetThreadProcess, METH_VARARGS, "Gets information about a process from a thread" },
@@ -1493,18 +1478,18 @@
 	/****************************************/
 	{ "LM_EnumSymbols", py_LM_EnumSymbols, METH_VARARGS, "Lists all symbols from a module" },
 	{ "LM_FindSymbolAddress", py_LM_FindSymbolAddress, METH_VARARGS, "Searches for a symbol in a module" },
 	{ "LM_DemangleSymbol", py_LM_DemangleSymbol, METH_VARARGS, "Demangles a mangled symbol from a module" },
 	{ "LM_EnumSymbolsDemangled", py_LM_EnumSymbolsDemangled, METH_VARARGS, "Lists all demangled symbols from a module" },
 	{ "LM_FindSymbolAddressDemangled", py_LM_FindSymbolAddressDemangled, METH_VARARGS, "Searches for a demangled symbol in a module" },
 	/****************************************/
-	{ "LM_EnumPages", py_LM_EnumPages, METH_NOARGS, "Lists all pages from the calling process" },
-	{ "LM_EnumPagesEx", py_LM_EnumPagesEx, METH_VARARGS, "Lists all pages from a remote process" },
-	{ "LM_GetPage", py_LM_GetPage, METH_VARARGS, "Get information about the page of an address in the current process" },
-	{ "LM_GetPageEx", py_LM_GetPageEx, METH_VARARGS, "Get information about the page of an address in a remote process" },
+	{ "LM_EnumSegments", py_LM_EnumSegments, METH_NOARGS, "Lists all segments from the calling process" },
+	{ "LM_EnumSegmentsEx", py_LM_EnumSegmentsEx, METH_VARARGS, "Lists all segments from a remote process" },
+	{ "LM_FindSegment", py_LM_FindSegment, METH_VARARGS, "Get information about the segment of an address in the current process" },
+	{ "LM_FindSegmentEx", py_LM_FindSegmentEx, METH_VARARGS, "Get information about the segment of an address in a remote process" },
 	/****************************************/
 	{ "LM_ReadMemory", py_LM_ReadMemory, METH_VARARGS, "Read memory from the calling process" },
 	{ "LM_ReadMemoryEx", py_LM_ReadMemoryEx, METH_VARARGS, "Read memory from a remote process" },
 	{ "LM_WriteMemory", py_LM_WriteMemory, METH_VARARGS, "Write memory to the calling process" },
 	{ "LM_WriteMemoryEx", py_LM_WriteMemoryEx, METH_VARARGS, "Write memory to a remote process" },
 	{ "LM_SetMemory", py_LM_SetMemory, METH_VARARGS, "Set memory to a byte in the current process" },
 	{ "LM_SetMemoryEx", py_LM_SetMemoryEx, METH_VARARGS, "Set memory to a byte in a remote process" },
@@ -1525,14 +1510,15 @@
 	{ "LM_SigScanEx", py_LM_SigScanEx, METH_VARARGS, "Search for a byte signature that can contain filters in a remote process" },
 	/****************************************/
 	{ "LM_HookCode", py_LM_HookCode, METH_VARARGS, "Hook/detour code in the current process, returning a gateway/trampoline" },
 	{ "LM_HookCodeEx", py_LM_HookCodeEx, METH_VARARGS, "Hook/detour code in a remote process, returning a gateway/trampoline" },
 	{ "LM_UnhookCode", py_LM_UnhookCode, METH_VARARGS, "Unhook/restore code in the current process" },
 	{ "LM_UnhookCodeEx", py_LM_UnhookCodeEx, METH_VARARGS, "Unhook/restore code in a remote process" },
 	/****************************************/
+	{ "LM_GetArchitecture", py_LM_GetArchitecture, METH_VARARGS, "Gets the current processor architecture" },
 	{ "LM_Assemble", py_LM_Assemble, METH_VARARGS, "Assemble instruction from text" },
 	{ "LM_AssembleEx", py_LM_AssembleEx, METH_VARARGS, "Assemble instructions from text" },
 	{ "LM_Disassemble", py_LM_Disassemble, METH_VARARGS, "Disassemble instruction from an address in the current process" },
 	{ "LM_DisassembleEx", py_LM_DisassembleEx, METH_VARARGS, "Disassemble instructions from an address in the current process" },
 	{ "LM_CodeLength", py_LM_CodeLength, METH_VARARGS, "Get the minimum instruction aligned length for a code region in the current process" },
 	{ "LM_CodeLengthEx", py_LM_CodeLengthEx, METH_VARARGS, "Get the minimum instruction aligned length for a code region in a remote process" },
 	{ NULL, NULL, 0, NULL }
@@ -1563,23 +1549,26 @@
 
 	if (PyType_Ready(&py_lm_symbol_t) < 0)
 		goto ERR_PYMOD;
 
 	if (PyType_Ready(&py_lm_prot_t) < 0)
 		goto ERR_PYMOD;
 
-	if (PyType_Ready(&py_lm_page_t) < 0)
+	if (PyType_Ready(&py_lm_segment_t) < 0)
 		goto ERR_PYMOD;
 
 	if (PyType_Ready(&py_lm_inst_t) < 0)
 		goto ERR_PYMOD;
 
 	if (PyType_Ready(&py_lm_vmt_t) < 0)
 		goto ERR_PYMOD;
 
+	if (PyType_Ready(&py_lm_arch_t) < 0)
+		goto ERR_PYMOD;
+
 	pymod = PyModule_Create(&libmem_mod);
 	if (!pymod)
 		goto ERR_PYMOD;
 	
 	/* types */
 	Py_INCREF(&py_lm_process_t);
 	if (PyModule_AddObject(pymod, "lm_process_t",
@@ -1602,52 +1591,92 @@
 		goto ERR_SYMBOL;
 
 	Py_INCREF(&py_lm_prot_t);
 	if (PyModule_AddObject(pymod, "lm_prot_t",
 			       (PyObject *)&py_lm_prot_t) < 0)
 		goto ERR_PROT;
 
-	Py_INCREF(&py_lm_page_t);
-	if (PyModule_AddObject(pymod, "lm_page_t",
-			       (PyObject *)&py_lm_page_t) < 0)
-		goto ERR_PAGE;
+	Py_INCREF(&py_lm_segment_t);
+	if (PyModule_AddObject(pymod, "lm_segment_t",
+			       (PyObject *)&py_lm_segment_t) < 0)
+		goto ERR_SEGMENT;
 
 	Py_INCREF(&py_lm_inst_t);
 	if (PyModule_AddObject(pymod, "lm_inst_t",
 			       (PyObject *)&py_lm_inst_t) < 0)
 		goto ERR_INST;
 
 	Py_INCREF(&py_lm_vmt_t);
 	if (PyModule_AddObject(pymod, "lm_vmt_t",
 			       (PyObject *)&py_lm_vmt_t) < 0)
 		goto ERR_VMT;
 
+	Py_INCREF(&py_lm_arch_t);
+	if (PyModule_AddObject(pymod, "lm_arch_t",
+			       (PyObject *)&py_lm_arch_t) < 0)
+		goto ERR_ARCH;
+
 	/* global variables */
 	DECL_GLOBAL_PROT(LM_PROT_X);
 	DECL_GLOBAL_PROT(LM_PROT_R);
 	DECL_GLOBAL_PROT(LM_PROT_W);
 	DECL_GLOBAL_PROT(LM_PROT_XR);
 	DECL_GLOBAL_PROT(LM_PROT_XW);
 	DECL_GLOBAL_PROT(LM_PROT_RW);
 	DECL_GLOBAL_PROT(LM_PROT_XRW);
-	DECL_GLOBAL_LONG(LM_BITS);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_ARMV7);
+	DECL_GLOBAL_ARCH(LM_ARCH_ARMV8);
+	DECL_GLOBAL_ARCH(LM_ARCH_THUMBV7);
+	DECL_GLOBAL_ARCH(LM_ARCH_THUMBV8);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_ARMV7EB);
+	DECL_GLOBAL_ARCH(LM_ARCH_THUMBV7EB);
+	DECL_GLOBAL_ARCH(LM_ARCH_ARMV8EB);
+	DECL_GLOBAL_ARCH(LM_ARCH_THUMBV8EB);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_AARCH64);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_MIPS);
+	DECL_GLOBAL_ARCH(LM_ARCH_MIPS64);
+	DECL_GLOBAL_ARCH(LM_ARCH_MIPSEL);
+	DECL_GLOBAL_ARCH(LM_ARCH_MIPSEL64);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_X86_16);
+	DECL_GLOBAL_ARCH(LM_ARCH_X86);
+	DECL_GLOBAL_ARCH(LM_ARCH_X64);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_PPC32);
+	DECL_GLOBAL_ARCH(LM_ARCH_PPC64);
+	DECL_GLOBAL_ARCH(LM_ARCH_PPC64LE);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_SPARC);
+	DECL_GLOBAL_ARCH(LM_ARCH_SPARC64);
+	DECL_GLOBAL_ARCH(LM_ARCH_SPARCEL);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_SYSZ);
+
+	DECL_GLOBAL_ARCH(LM_ARCH_MAX);
 
 	goto EXIT; /* no errors */
 
+ERR_ARCH:
+	Py_DECREF(&py_lm_arch_t);
+	Py_DECREF(pymod);
 ERR_VMT:
 	Py_DECREF(&py_lm_vmt_t);
 	Py_DECREF(pymod);
 ERR_INST:
 	Py_DECREF(&py_lm_inst_t);
 	Py_DECREF(pymod);
 ERR_PROT:
 	Py_DECREF(&py_lm_prot_t);
 	Py_DECREF(pymod);
-ERR_PAGE:
-	Py_DECREF(&py_lm_page_t);
+ERR_SEGMENT:
+	Py_DECREF(&py_lm_segment_t);
 	Py_DECREF(pymod);
 ERR_SYMBOL:
 	Py_DECREF(&py_lm_symbol_t);
 	Py_DECREF(pymod);
 ERR_MODULE:
 	Py_DECREF(&py_lm_module_t);
 	Py_DECREF(pymod);
```

### Comparing `libmem-5.0.0rc0/src/libmem/_libmem/types.h` & `libmem-5.0.0rc6/src/libmem/_libmem/types.h`

 * *Files 16% similar despite different names*

```diff
@@ -22,26 +22,114 @@
 
 #ifndef LIBMEM_TYPES_H
 #define LIBMEM_TYPES_H
 
 #include <libmem/libmem.h>
 #include <Python.h>
 #include <structmember.h>
+#include <stddef.h>
 
 #define T_SIZE T_PYSSIZET
 
+/****************************************/
+
+/* lm_arch_t */
+typedef struct {
+	PyObject_HEAD
+	lm_arch_t arch;
+} py_lm_arch_obj;
+
+int
+py_lm_arch_init(PyObject *self,
+		PyObject *args,
+		PyObject *kwds)
+{
+	lm_arch_t arch;
+	py_lm_arch_obj *pyarch = (py_lm_arch_obj *)self;
+
+	if (!PyArg_ParseTuple(args, "i", &arch))
+		return -1;
+
+	pyarch->arch = arch;
+
+	return 0;
+}
+
+PyObject *
+py_lm_arch_str(PyObject *self)
+{
+	py_lm_arch_obj *pyarch = (py_lm_arch_obj *)self;
+	const char *archstr;
+
+	switch (pyarch->arch) {
+	case LM_ARCH_ARMV7: archstr = "LM_ARCH_ARMV7"; break;
+	case LM_ARCH_ARMV8: archstr = "LM_ARCH_ARMV8"; break;
+	case LM_ARCH_THUMBV7: archstr = "LM_ARCH_THUMBV7"; break;
+	case LM_ARCH_THUMBV8: archstr = "LM_ARCH_THUMBV8"; break;
+
+	case LM_ARCH_ARMV7EB: archstr = "LM_ARCH_ARMV7EB"; break;
+	case LM_ARCH_THUMBV7EB: archstr = "LM_ARCH_THUMBV7EB"; break;
+	case LM_ARCH_ARMV8EB: archstr = "LM_ARCH_ARMV8EB"; break;
+	case LM_ARCH_THUMBV8EB: archstr = "LM_ARCH_THUMBV8EB"; break;
+
+	case LM_ARCH_AARCH64: archstr = "LM_ARCH_AARCH64"; break;
+
+	case LM_ARCH_MIPS: archstr = "LM_ARCH_MIPS"; break;
+	case LM_ARCH_MIPS64: archstr = "LM_ARCH_MIPS64"; break;
+	case LM_ARCH_MIPSEL: archstr = "LM_ARCH_MIPSEL"; break;
+	case LM_ARCH_MIPSEL64: archstr = "LM_ARCH_MIPSEL64"; break;
+
+	case LM_ARCH_X86_16: archstr = "LM_ARCH_X86_16"; break;
+	case LM_ARCH_X86: archstr = "LM_ARCH_X86"; break;
+	case LM_ARCH_X64: archstr = "LM_ARCH_X64"; break;
+
+	case LM_ARCH_PPC32: archstr = "LM_ARCH_PPC32"; break;
+	case LM_ARCH_PPC64: archstr = "LM_ARCH_PPC64"; break;
+	case LM_ARCH_PPC64LE: archstr = "LM_ARCH_PPC64LE"; break;
+
+	case LM_ARCH_SPARC: archstr = "LM_ARCH_SPARC"; break;
+	case LM_ARCH_SPARC64: archstr = "LM_ARCH_SPARC64"; break;
+	case LM_ARCH_SPARCEL: archstr = "LM_ARCH_SPARCEL"; break;
+
+	case LM_ARCH_SYSZ: archstr = "LM_ARCH_SYSZ"; break;
+
+	case LM_ARCH_MAX: archstr = "LM_ARCH_MAX"; break;
+
+	default: archstr = "LM_ARCH_NONE"; break;
+	}
+
+	return PyUnicode_FromFormat("%s", archstr);
+}
+
+static PyTypeObject py_lm_arch_t = {
+	PyVarObject_HEAD_INIT(NULL, 0)
+	.tp_name = "libmem.lm_arch_t",
+	.tp_doc = "Stores a processor architecture",
+	.tp_basicsize = sizeof(py_lm_arch_obj),
+	.tp_itemsize = 0,
+	.tp_flags = Py_TPFLAGS_DEFAULT,
+	.tp_new = PyType_GenericNew,
+	.tp_str = py_lm_arch_str,
+	.tp_repr = py_lm_arch_str,
+	.tp_init = py_lm_arch_init
+};
+
+/****************************************/
+
 /* lm_process_t */
 typedef struct {
 	PyObject_HEAD
 	lm_process_t proc;
+	py_lm_arch_obj *arch;
 } py_lm_process_obj;
 
 static PyMemberDef py_lm_process_members[] = {
 	{ "pid", T_INT, offsetof(py_lm_process_obj, proc.pid), READONLY, "Process ID" },
 	{ "ppid", T_INT, offsetof(py_lm_process_obj, proc.ppid), READONLY, "Parent Process ID" },
+	{ "arch", T_OBJECT, offsetof(py_lm_process_obj, arch), READONLY, "Process Architecture" },
 	{ "bits", T_SIZE, offsetof(py_lm_process_obj, proc.bits), READONLY, "Process Bits" },
         { "start_time", T_ULONGLONG, offsetof(py_lm_process_obj, proc.start_time), READONLY, "Process Start Time" },
 	{ NULL }
 };
 
 PyObject *
 py_lm_process_get_path(PyObject *self, void *closure)
@@ -55,15 +143,24 @@
 	return PyUnicode_FromString(((py_lm_process_obj *)self)->proc.name);
 }
 
 PyObject *
 py_lm_process_str(PyObject *self)
 {
 	py_lm_process_obj *pyproc = (py_lm_process_obj *)self;
-	return PyUnicode_FromFormat("lm_process_t(pid = %d, ppid = %d, bits = %zu, start_time = %llu, path = \"%s\", name = \"%s\")", pyproc->proc.pid, pyproc->proc.ppid, pyproc->proc.bits, pyproc->proc.start_time, pyproc->proc.path, pyproc->proc.name);
+	PyObject *pyarchstr;
+	PyObject *pyfmtstr;
+
+	pyarchstr = PyObject_Str((PyObject *)pyproc->arch);
+
+	pyfmtstr = PyUnicode_FromFormat("lm_process_t(pid = %d, ppid = %d, arch = %s, bits = %zu, start_time = %llu, path = \"%s\", name = \"%s\")", pyproc->proc.pid, pyproc->proc.ppid, PyUnicode_AsUTF8(pyarchstr), pyproc->proc.bits, pyproc->proc.start_time, pyproc->proc.path, pyproc->proc.name);
+
+	Py_DECREF(pyarchstr);
+
+	return pyfmtstr;
 }
 
 static PyGetSetDef py_lm_process_accessors[] = {
 	{ "path", py_lm_process_get_path, NULL, NULL, NULL },
 	{ "name", py_lm_process_get_name, NULL, NULL, NULL },
 	{ NULL, NULL, NULL, NULL, NULL }
 };
@@ -88,14 +185,15 @@
 typedef struct {
 	PyObject_HEAD
 	lm_thread_t thread;
 } py_lm_thread_obj;
 
 static PyMemberDef py_lm_thread_members[] = {
 	{ "tid", T_INT, offsetof(py_lm_thread_obj, thread.tid), READONLY, "Thread ID" },
+	{ "owner_pid", T_INT, offsetof(py_lm_thread_obj, thread.owner_pid), READONLY, "Thread Owner PID" },
 	{ NULL }
 };
 
 PyObject *
 py_lm_thread_str(PyObject *self)
 {
 	py_lm_thread_obj *pythread = (py_lm_thread_obj *)self;
@@ -264,65 +362,66 @@
 };
 
 /****************************************/
 
 /* lm_page_t */
 typedef struct {
 	PyObject_HEAD
-	lm_page_t page;
+	lm_segment_t segment;
 	py_lm_prot_obj *prot;
-} py_lm_page_obj;
+} py_lm_segment_obj;
 
-static PyMemberDef py_lm_page_members[] = {
-	{ "base", T_SIZE, offsetof(py_lm_page_obj, page.base), READONLY, "Page Base Address" },
-	{ "end", T_SIZE, offsetof(py_lm_page_obj, page.end), READONLY, "Page End Address" },
-	{ "size", T_SIZE, offsetof(py_lm_page_obj, page.size), READONLY, "Page Size" },
-	{ "prot", T_OBJECT, offsetof(py_lm_page_obj, prot), READONLY, "Page Protection Flags" },
+static PyMemberDef py_lm_segment_members[] = {
+	{ "base", T_SIZE, offsetof(py_lm_segment_obj, segment.base), READONLY, "Segment Base Address" },
+	{ "end", T_SIZE, offsetof(py_lm_segment_obj, segment.end), READONLY, "Segment End Address" },
+	{ "size", T_SIZE, offsetof(py_lm_segment_obj, segment.size), READONLY, "Segment Size" },
+	{ "prot", T_OBJECT, offsetof(py_lm_segment_obj, prot), READONLY, "Segment Protection Flags" },
 	{ NULL }
 };
 
 PyObject *
-py_lm_page_str(PyObject *self)
+py_lm_segment_str(PyObject *self)
 {
-	py_lm_page_obj *pypage = (py_lm_page_obj *)self;
+	py_lm_segment_obj *pysegment = (py_lm_segment_obj *)self;
 	PyObject *pyprotstr;
 	const char *protstr;
 	PyObject *fmtstr;
 
-	pyprotstr = PyObject_Str((PyObject *)pypage->prot);
+	pyprotstr = PyObject_Str((PyObject *)pysegment->prot);
 	protstr = PyUnicode_AsUTF8(pyprotstr);
-	fmtstr = PyUnicode_FromFormat("lm_page_t(base = %p, end = %p, size = %p, prot = %s)", (void *)pypage->page.base, (void *)pypage->page.end, (void *)pypage->page.size, protstr);
+	fmtstr = PyUnicode_FromFormat("lm_segment_t(base = %p, end = %p, size = %p, prot = %s)", (void *)pysegment->segment.base, (void *)pysegment->segment.end, (void *)pysegment->segment.size, protstr);
 
 	Py_DECREF(pyprotstr); /* delete protection string object */
 
 	return fmtstr;
 }
 
-static PyTypeObject py_lm_page_t = {
+static PyTypeObject py_lm_segment_t = {
 	PyVarObject_HEAD_INIT(NULL, 0)
-	.tp_name = "libmem.lm_page_t",
-	.tp_doc = "Stores information about a page",
-	.tp_basicsize = sizeof(py_lm_page_obj),
+	.tp_name = "libmem.lm_segment_t",
+	.tp_doc = "Stores information about a segment",
+	.tp_basicsize = sizeof(py_lm_segment_obj),
 	.tp_itemsize = 0,
 	.tp_flags = Py_TPFLAGS_DEFAULT,
 	.tp_new = PyType_GenericNew,
-	.tp_members = py_lm_page_members,
-	.tp_str = py_lm_page_str,
-	.tp_repr = py_lm_page_str
+	.tp_members = py_lm_segment_members,
+	.tp_str = py_lm_segment_str,
+	.tp_repr = py_lm_segment_str
 };
 
 /****************************************/
 
 /* lm_inst_t */
 typedef struct {
 	PyObject_HEAD
 	lm_inst_t inst;
 } py_lm_inst_obj;
 
 static PyMemberDef py_lm_inst_members[] = {
+	{ "address", T_SIZE, offsetof(py_lm_inst_obj, inst.address), READONLY, "Instruction Address" },
 	{ "size", T_SIZE, offsetof(py_lm_inst_obj, inst.size), READONLY, "Instruction Size" },
 	{ NULL }
 };
 
 PyObject *
 py_lm_inst_get_mnemonic(PyObject *self, void *closure)
 {
```

### Comparing `libmem-5.0.0rc0/src/libmem.egg-info/PKG-INFO` & `libmem-5.0.0rc6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: libmem
-Version: 5.0.0rc0
-Summary: Advanced Game Hacking Library (Windows/Linux/FreeBSD)
-Home-page: https://github.com/rdbo/libmem
-Author: rdbo
-Project-URL: Documentation, https://github.com/rdbo/libmem/blob/master/docs/DOCS.md
-Project-URL: Bug Tracker, https://github.com/rdbo/libmem/issues
-Project-URL: Discord Server, https://discord.com/invite/Qw8jsPD99X
-Keywords: gamehacking memory process hooking detouring hacking winapi linux freebsd
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 ![libmem-logo](https://raw.githubusercontent.com/rdbo/libmem/master/LOGO.png)  
 ### Advanced Game Hacking Library (C/C++/Rust/Python) (Windows/Linux/FreeBSD)
 ### Made by rdbo
 #  
 
 ## Discord Server
 https://discord.com/invite/Qw8jsPD99X
@@ -131,14 +118,22 @@
 print(f"{code} : {inst.bytes}")
 
 print("[*] Disassembly:")
 inst = LM_Disassemble(bytearray(b"\x55"))
 print(f"{inst.bytes} : {inst.mnemonic} {inst.op_str}")
 ```
 
+## Unnoficial Bindings
+These bindings are done by the community/third-parties and are not affiliated with the libmem project or its author.
+
+Their code can have their own licenses as well, diverging from libmem's.
+
+- [Nim_Libmem](https://github.com/Hypnootika/Nim_Libmem)
+- [Crazymem (NodeJS)](https://github.com/karliky/Crazymem)
+
 ## CMake Usage (without installing)
 Add the following commands to your `CMakeLists.txt`.
 
 They will fetch `libmem-config.cmake` from the root of this repository, which will download libmem binaries for your system and include libmem in your CMake project.
 
 ```cmake
 include(FetchContent)
@@ -379,9 +374,7 @@
 Made with libmem:  
 - [AssaultCube Multihack](https://github.com/rdbo/AssaultCube-Multihack)  
 - [X-Inject](https://github.com/rdbo/x-inject)  
 - [DirectX9 BaseHook](https://github.com/rdbo/DX9-BaseHook)  
 - [DirectX11 BaseHook](https://github.com/rdbo/DX11-BaseHook)  
 - [OpenGL BaseHook](https://github.com/rdbo/GL-BaseHook)  
 - [Counter-Strike 1.6 BaseHook](https://github.com/rdbo/cstrike-basehook)  
-- [Crazymem - NodeJS Memory Library](https://github.com/karliky/Crazymem)  
-
```

### Comparing `libmem-5.0.0rc0/tests/test_mock.py` & `libmem-5.0.0rc6/tests/test_mock.py`

 * *Files identical despite different names*

### Comparing `libmem-5.0.0rc0/tests/tests.py` & `libmem-5.0.0rc6/tests/tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from libmem import *
 import ctypes
 import struct
+import time
+import os
 
 def separator():
     print("========================================")
 
 print("[*] libmem-py tests")
 
 separator()
@@ -23,15 +25,15 @@
 print("[*] Parent Process of Current Process")
 parent_proc = LM_GetProcessEx(curproc.ppid)
 print(parent_proc)
 
 separator()
 
 print("[*] Remote Process")
-proc = LM_FindProcess("test1")
+proc = LM_FindProcess("target")
 print(proc)
 
 separator()
 
 print(f"[*] Is Remote Process Alive? {'Yes' if LM_IsProcessAlive(proc) else 'No'}")
 
 separator()
@@ -77,64 +79,82 @@
 separator()
 
 mod = LM_FindModuleEx(proc, proc.path)
 print(f"[*] Remote Process Module: {mod}")
 
 separator()
 
-# TODO: Add tests for LM_LoadModule(Ex) and LM_UnloadModule(Ex)
+libpath = f"{os.path.dirname(os.path.realpath(__file__))}{os.sep}{os.pardir}{os.sep}{os.pardir}{os.sep}{os.pardir}{os.sep}build{os.sep}tests{os.sep}libtest.so"
+print(f"[*] Loadable Library Path: {libpath}")
+cur_loaded_mod = LM_LoadModule(libpath)
+print()
+print(f"[*] Loaded Module into Current Process: {cur_loaded_mod}")
 
-# separator()
+LM_UnloadModule(cur_loaded_mod)
+print("[*] Unloaded Module from Current Process")
+
+separator()
+
+loaded_mod = LM_LoadModuleEx(proc, libpath)
+print("[*] Loaded Module into Target Process: ", loaded_mod)
+
+LM_UnloadModuleEx(proc, loaded_mod)
+print("[*] Unloaded Module from Target Process")
+
+separator()
 
 print("[*] Symbol Enumeration")
 
 print("\n".join([str(sym) for sym in LM_EnumSymbols(curmod)[:5]]))
 
 separator()
 
 print("[*] Symbol Address Search")
 
 symaddr = LM_FindSymbolAddress(curmod, "Py_BytesMain")
 if symaddr == None:
     symaddr = LM_FindSymbolAddress(curmod, "_start_c")
-print(f"[*] Py_BytesMain Address: {symaddr}")
+print(f"[*] Py_BytesMain Address: {hex(symaddr)}")
 
 separator()
 
 mangled = "_Z15_LM_EnumSymbolsP11lm_module_tPFiP11lm_symbol_tPvES3_"
 demangled = LM_DemangleSymbol(mangled)
 print(f"[*] Demangled '{mangled}': {demangled}")
 
 separator()
 
 print("[*] Demangled Symbol Enumeration")
 
 print("\n".join([str(sym) for sym in LM_EnumSymbolsDemangled(curmod)[:5]]))
 
-# TODO: Add test for 'LM_FindSymbolAddressDemangled'
+separator()
 
-# separator()
+symaddr = LM_FindSymbolAddressDemangled(curmod, "Py_BytesMain")
+if symaddr == None:
+    symaddr = LM_FindSymbolAddressDemangled(curmod, "_start_c")
+print(f"[*] Py_BytesMain Address (Demangled): {hex(symaddr)}")
 
 separator()
 
-print("[*] Page Enumeration - Current Process")
-print("\n".join([str(page) for page in LM_EnumPages()[:5]]))
+print("[*] Segment Enumeration - Current Process")
+print("\n".join([str(segment) for segment in LM_EnumSegments()[:5]]))
 
 separator()
 
-print("[*] Page Enumeration - Remote Process")
-print("\n".join([str(page) for page in LM_EnumPagesEx(proc)[:5]]))
+print("[*] Segment Enumeration - Remote Process")
+print("\n".join([str(segment) for segment in LM_EnumSegmentsEx(proc)[:5]]))
 
 separator()
 
-print(f"[*] Page From Current Process Module: {LM_GetPage(symaddr)}")
+print(f"[*] Segment From Current Process Module: {LM_FindSegment(symaddr)}")
 
 separator()
 
-print(f"[*] Page From Remote Process Module: {LM_GetPageEx(proc, mod.base)}")
+print(f"[*] Segment From Remote Process Module: {LM_FindSegmentEx(proc, mod.base)}")
 
 separator()
 
 val = ctypes.c_int(10)
 val_addr = ctypes.addressof(val)
 rdbuf = LM_ReadMemory(val_addr, ctypes.sizeof(val))
 rdval = struct.unpack("@i", rdbuf)[0]
@@ -160,24 +180,24 @@
 
 # TODO: Add tests for 'LM_SetMemoryEx'
 # separator()
 
 print("[*] Changing Memory Protection - Current Process")
 old_prot = LM_ProtMemory(curmod.base, 0x1000, LM_PROT_XRW)
 print(f"[*] Old Memory Protection ({hex(curmod.base)}): {old_prot}")
-page = LM_GetPage(curmod.base)
-print(f"[*] Current Memory Protection ({hex(curmod.base)}): {page.prot}")
+segment = LM_FindSegment(curmod.base)
+print(f"[*] Current Memory Protection ({hex(curmod.base)}): {segment.prot}")
 
 separator()
 
 print("[*] Changing Memory Protection - Remote Process")
 old_prot = LM_ProtMemoryEx(proc, mod.base, 0x1000, LM_PROT_XRW)
 print(f"[*] Old Memory Protection ({hex(mod.base)}): {old_prot}")
-page = LM_GetPageEx(proc, mod.base)
-print(f"[*] Current Memory Protection ({hex(mod.base)}): {page.prot}")
+segment = LM_FindSegmentEx(proc, mod.base)
+print(f"[*] Current Memory Protection ({hex(mod.base)}): {segment.prot}")
 
 separator()
 
 alloc_size = 0x1000
 alloc = LM_AllocMemory(alloc_size, LM_PROT_XRW)
 print(f"[*] Allocated Memory - Current Process: {hex(alloc)}")
 LM_FreeMemory(alloc, alloc_size)
@@ -186,19 +206,22 @@
 
 alloc = LM_AllocMemoryEx(proc, alloc_size, LM_PROT_XRW)
 print(f"[*] Allocated Memory - Remote Process: {hex(alloc)}")
 LM_FreeMemoryEx(proc, alloc, alloc_size)
 
 separator()
 
-addr1 = LM_AllocMemory(4, LM_PROT_RW)
+addr0 = LM_AllocMemory(4, LM_PROT_RW)
+addr1 = LM_AllocMemory(8, LM_PROT_RW)
 addr2 = LM_AllocMemory(8, LM_PROT_RW)
 
-LM_WriteMemory(addr1, bytearray(b"\x10\x00\x00\x00"))
+LM_WriteMemory(addr0, bytearray(b"\x10\x00\x00\x00"))
+LM_WriteMemory(addr1, bytearray(addr0.to_bytes(8, byteorder="little")))
 LM_WriteMemory(addr2, bytearray(addr1.to_bytes(8, byteorder="little")))
+print("[*] Address 0: ", hex(addr0))
 print("[*] Address 1: ", hex(addr1))
 print("[*] Address 2: ", hex(addr2))
 
 deep_ptr = LM_DeepPointer(addr2, [0, 0])
 print("[*] Deep Pointer result: " + hex(deep_ptr))
 
 value = int.from_bytes(LM_ReadMemory(deep_ptr, 4), byteorder="little")
@@ -216,43 +239,61 @@
 pattern_scan = LM_PatternScan(bytearray(buf.value), "xxxx?x?x?x", scan_addr, scan_size)
 print(f"[*] Pattern Scan Match: {hex(pattern_scan)}")
 sig_scan = LM_SigScan("10 20 30 40 ?? ?? 70 80 ?? A0", scan_addr, scan_size)
 print(f"[*] Signature Scan Match: {hex(sig_scan)}")
 
 separator()
 
-# TODO: Add tests for 'LM_DataScanEx', 'LM_PatternScanEx', 'LM_SigScanEx'
-# separator()
+scan_alloc = LM_AllocMemoryEx(proc, 1024, LM_PROT_RW)
+print(f"[*] External Scan Alloc: {hex(scan_alloc)}")
+buf_addr = scan_alloc + 0x10
+LM_WriteMemoryEx(proc, buf_addr, bytearray(buf.value))
+print(f"[*] Externally Scanning For Buffer At: {hex(buf_addr)}")
+scan_addr = buf_addr - 0x10
+scan_size = 0x100
+data_scan = LM_DataScanEx(proc, bytearray(buf.value), scan_addr, scan_size)
+print(f"[*] Data Scan Match: {hex(data_scan)}")
+pattern_scan = LM_PatternScanEx(proc, bytearray(buf.value), "xxxx?x?x?x", scan_addr, scan_size)
+print(f"[*] Pattern Scan Match: {hex(pattern_scan)}")
+sig_scan = LM_SigScanEx(proc, "10 20 30 40 ?? ?? 70 80 ?? A0", scan_addr, scan_size)
+print(f"[*] Signature Scan Match: {hex(sig_scan)}")
 
 # TODO: Add tests for 'LM_HookCode' and 'LM_UnhookCode'
 # separator()
 
-# TODO: Add tests for 'LM_HookCodeEx' and 'LM_UnhookCodeEx'
-# separator()
+wait_message_addr = LM_FindSymbolAddress(mod, "wait_message")
+hk_wait_message_addr = LM_FindSymbolAddress(mod, "hk_wait_message")
+trampoline = LM_HookCodeEx(proc, wait_message_addr, hk_wait_message_addr)
+print(f"[*] External Hook Trampoline: {trampoline}")
+time.sleep(3)
+LM_UnhookCodeEx(proc, wait_message_addr, trampoline)
+print("[*] Unhooked External Function")
+
+separator()
 
 print("[*] Assemblying Instruction")
 inst = LM_Assemble("mov eax, ebx")
 print(inst)
 
 separator()
 
 print("[*] Assemblying Instructions")
-insts = LM_AssembleEx("push ebp; mov ebp, esp; mov esp, ebp; pop ebp; ret", 32, 0)
+insts = LM_AssembleEx("push ebp; mov ebp, esp; mov esp, ebp; pop ebp; ret", LM_ARCH_X86, 0)
 print(", ".join([hex(b) for b in insts]))
 
 separator()
 
 print("[*] Disassembly of PyBytesMain Instruction")
 inst = LM_Disassemble(symaddr)
 print(inst)
 
 separator()
 
 print("[*] Disassembly of PyBytesMain Instructions")
-insts = LM_DisassembleEx(symaddr, 32, 0x100, 5, symaddr)
+insts = LM_DisassembleEx(symaddr, LM_ARCH_X86, 0x100, 5, symaddr)
 print("\n".join([str(inst) for inst in insts]))
 
 separator()
 
 minlength = 0x5
 aligned_length = LM_CodeLength(symaddr, minlength)
 print(f"[*] Aligned Length for Minimum '{minlength}' Bytes is '{aligned_length}' Bytes (PyBytesMain)")
```

