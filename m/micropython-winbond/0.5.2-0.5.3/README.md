# Comparing `tmp/micropython-winbond-0.5.2.tar.gz` & `tmp/micropython-winbond-0.5.3.tar.gz`

## Comparing `micropython-winbond-0.5.2.tar` & `micropython-winbond-0.5.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2023-11-16 16:35:07.000000 micropython-winbond-0.5.2/micropython_winbond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-16 16:35:00.000000 micropython-winbond-0.5.2/winbond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-16 16:35:06.000000 micropython-winbond-0.5.2/winbond/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14681 2023-11-16 16:35:00.000000 micropython-winbond-0.5.2/winbond/winbond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-30 09:54:13.000000 micropython-winbond-0.5.3/micropython_winbond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 09:54:05.000000 micropython-winbond-0.5.3/winbond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 09:54:12.000000 micropython-winbond-0.5.3/winbond/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-05-30 09:54:05.000000 micropython-winbond-0.5.3/winbond/winbond.py
```

### Comparing `micropython-winbond-0.5.2/micropython_winbond.egg-info/PKG-INFO` & `micropython-winbond-0.5.3/micropython_winbond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-winbond
-Version: 0.5.2
+Version: 0.5.3
 Summary: Simple MicroPython Winbond library
 Home-page: https://github.com/brainelectronics/micropython-winbond
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-winbond/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-winbond
```

### Comparing `micropython-winbond-0.5.2/winbond/winbond.py` & `micropython-winbond-0.5.3/winbond/winbond.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,16 +168,16 @@
         self._capacity = int(2**cap)
 
         if not (mf and mem_type and cap):  # something is 0x00
             raise OSError("device not responding, check wiring. ({}, {}, {})".
                           format(hex(mf), hex(mem_type), hex(cap)))
         if mf != 0xEF or mem_type not in [0x40, 0x60, 0x70]:
             # Winbond manufacturer, Q25 series memory (tested 0x40 only)
-            print(f"Warning manufacturer ({hex(mf)}) or memory type"
-                  f"({hex(mem_type)}) not tested.")
+            print(f"""Warning manufacturer ({hex(mf)}) or memory type
+                      ({hex(mem_type)}) not tested.""")
 
         self._manufacturer = mf
         self._mem_type = mem_type
         self._device_type = mem_type << 8 | cap
 
     def get_size(self) -> int:
         """
```

