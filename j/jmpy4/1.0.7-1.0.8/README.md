# Comparing `tmp/jmpy4-1.0.7.tar.gz` & `tmp/jmpy4-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmpy4-1.0.7.tar", last modified: Tue May 28 12:41:20 2024, max compression
+gzip compressed data, was "jmpy4-1.0.8.tar", last modified: Wed May 29 12:36:09 2024, max compression
```

## Comparing `jmpy4-1.0.7.tar` & `jmpy4-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 12:41:20.377620 jmpy4-1.0.7/
--rw-rw-rw-   0        0        0     1096 2020-12-29 07:22:13.000000 jmpy4-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       61 2020-12-29 07:22:13.000000 jmpy4-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      779 2024-05-28 12:41:20.373605 jmpy4-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      421 2024-05-28 12:35:09.000000 jmpy4-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 12:41:20.327608 jmpy4-1.0.7/jmpy/
--rw-rw-rw-   0        0        0      109 2020-12-29 07:22:13.000000 jmpy4-1.0.7/jmpy/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-05-28 12:36:19.000000 jmpy4-1.0.7/jmpy/cmdline.py
--rw-rw-rw-   0        0        0     6402 2024-05-28 12:37:25.000000 jmpy4-1.0.7/jmpy/encrypt_py.py
--rw-rw-rw-   0        0        0      531 2020-12-29 07:22:13.000000 jmpy4-1.0.7/jmpy/log.py
-drwxrwxrwx   0        0        0        0 2024-05-28 12:41:20.368609 jmpy4-1.0.7/jmpy4.egg-info/
--rw-rw-rw-   0        0        0      779 2024-05-28 12:41:20.000000 jmpy4-1.0.7/jmpy4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-28 12:41:20.000000 jmpy4-1.0.7/jmpy4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 12:41:20.000000 jmpy4-1.0.7/jmpy4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-28 12:41:20.000000 jmpy4-1.0.7/jmpy4.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 12:41:20.000000 jmpy4-1.0.7/jmpy4.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-28 12:41:20.000000 jmpy4-1.0.7/jmpy4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 12:41:20.378605 jmpy4-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1139 2024-05-28 12:33:39.000000 jmpy4-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 12:41:20.361607 jmpy4-1.0.7/tests/
--rw-rw-rw-   0        0        0      402 2024-05-28 12:35:31.000000 jmpy4-1.0.7/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.723052 jmpy4-1.0.8/
+-rw-rw-rw-   0        0        0     1103 2024-05-28 13:12:38.000000 jmpy4-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       61 2020-12-29 07:22:13.000000 jmpy4-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      929 2024-05-29 12:36:09.717048 jmpy4-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2024-05-29 09:12:59.000000 jmpy4-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.652050 jmpy4-1.0.8/jmpy/
+-rw-rw-rw-   0        0        0      109 2020-12-29 07:22:13.000000 jmpy4-1.0.8/jmpy/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-05-28 14:16:29.000000 jmpy4-1.0.8/jmpy/cmdline.py
+-rw-rw-rw-   0        0        0     6756 2024-05-29 12:35:09.000000 jmpy4-1.0.8/jmpy/encrypt_py.py
+-rw-rw-rw-   0        0        0      531 2020-12-29 07:22:13.000000 jmpy4-1.0.8/jmpy/log.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.711048 jmpy4-1.0.8/jmpy4.egg-info/
+-rw-rw-rw-   0        0        0      929 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 12:36:09.000000 jmpy4-1.0.8/jmpy4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:36:09.724048 jmpy4-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2024-05-29 09:22:53.000000 jmpy4-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:36:09.701047 jmpy4-1.0.8/tests/
+-rw-rw-rw-   0        0        0      402 2024-05-29 12:16:32.000000 jmpy4-1.0.8/tests/test.py
```

### Comparing `jmpy4-1.0.7/LICENSE` & `jmpy4-1.0.8/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 MIT License
 
 Modifications:
 
-Copyright (c) 2020 Boris <boris@bzkj.tech>
+Copyright (c) 2024 Shenny <shenny520@outlook.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jmpy4-1.0.7/PKG-INFO` & `jmpy4-1.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: jmpy4
-Version: 1.0.7
+Version: 1.0.8
 Summary: python代码一键加密
 Home-page: https://github.com/shenny520/jmpy-plus.git
 Author: Shenny
 Author-email: shenny520@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Cython==0.29.20
+Requires-Dist: Cython==3.0.0
 
 # jmpy
 
 ![](https://img.shields.io/badge/python-3.0-brightgreen)
 
 ## 简介
 
 将python代码一键加密为so或pyd。支持单个文件加密，整个项目加密。
 
 Fork from: https://github.com/Boris-code/jmpy.git
+
 支持多进程，修复 bug
 
 ## 安装
 
     pip install jmpy4
 
 ## 使用方法
 
-    jmpy -i "xxx project dir" [-o output dir]
+    jmpy -i "xxx project dir" [-o output dir] -w 8
 
 加密后的文件默认存储在 dist/project_name/ 下
+
+## Tips
+
+加密过程会产生如下警告，不影响使用，可以忽略
+
+    'build\bdist.win-amd64' does not exist -- can't clean it
```

### Comparing `jmpy4-1.0.7/jmpy/cmdline.py` & `jmpy4-1.0.8/jmpy/cmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 "ignore_files=",
                 "except_main_file=",
                 "worker="
             ],
         )
         input_file_path = output_file_path = ignore_files = ""
         except_main_file = 1
-        worker_num = 1
+        worker_num = 4
 
         for name, value in options:
             if name in ("-h", "--help"):
                 print(usage.__doc__)
                 sys.exit()
 
             elif name in ("-i", "--input_file_path"):
```

### Comparing `jmpy4-1.0.7/jmpy/encrypt_py.py` & `jmpy4-1.0.8/jmpy/encrypt_py.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         shutil.rmtree(self.name)
 
 
 def search(content, regexs):
     content = content.replace('\\', '/')
+    regexs = regexs.replace('\\', '/')
     if isinstance(regexs, str):
         return re.search(regexs, content)
 
     for regex in regexs:
         if re.search(regex, content):
             return True
 
@@ -114,39 +115,47 @@
 
         _files.append(file)
 
     return _files
 
 
 def _encrypt_py(py_file):
-    with TemporaryDirectory() as td:
-        try:
-            dir_name = os.path.dirname(os.path.abspath(py_file))
-            file_name = os.path.basename(py_file)
-
-            os.chdir(dir_name)
-
-            logger.debug("正在加密 {}".format(file_name))
-
+    try:
+        dir_name = os.path.dirname(os.path.abspath(py_file))
+        file_name = os.path.basename(py_file)
+        os.chdir(dir_name)
+        logger.debug("正在加密 {}".format(file_name))
+        with TemporaryDirectory() as td:
             setup(
-                ext_modules=cythonize([file_name], quiet=True, language_level=3),
-                script_args=["build_ext", "-t", td, "--inplace"],
+                ext_modules=cythonize([py_file], quiet=True, language_level=3),
+                script_args=["build_ext", "-t", td, "--inplace", "clean", "--all"],
             )
-            logger.debug("加密成功 {}".format(file_name))
-            return py_file
-        except Exception as e:
-            logger.exception("加密失败 {} , error {}".format(py_file, e))
-            temp_c = py_file.replace(".py", ".c")
-            if os.path.exists(temp_c):
-                os.remove(temp_c)
+        logger.debug("加密成功 {}".format(file_name))
+        return py_file
+    except Exception as e:
+        logger.exception("加密失败 {} , error {}".format(py_file, e))
+        temp_c = py_file.replace(".py", ".c")
+        if os.path.exists(temp_c):
+            os.remove(temp_c)
 
 
 def encrypt_py(py_files: list, worker_num: int = 1):
-    with Pool(worker_num) as pool:
-        return pool.map(_encrypt_py, py_files)
+    total = len(py_files)
+    complete = 0
+
+    def show_progress(*args):
+        nonlocal complete
+        complete += 1
+        print('*' * 20, f'【{complete}/{total}】', '*' * 20)
+
+    pool = Pool(worker_num)
+    results = [pool.apply_async(_encrypt_py, args=(file,), callback=show_progress) for file in py_files]
+    pool.close()
+    pool.join()
+    return [res.get() for res in results if res.get() is not None]
 
 
 def delete_files(files_path):
     """
     @summary: 删除文件
     ---------
     @param files_path: 文件路径 py 及 c 文件
@@ -159,15 +168,15 @@
             os.remove(file)  # py文件
             os.remove(file.replace(".py", ".c"))  # c文件
 
     except Exception as e:
         pass
 
 
-def rename_excrypted_file(output_file_path):
+def rename_encrypted_file(output_file_path):
     files = walk_file(output_file_path)
     for file in files:
         if file.endswith(".pyd") or file.endswith(".so"):
             new_filename = re.sub("(.*)\..*\.(.*)", r"\1.\2", file)
             os.rename(file, new_filename)
 
 
@@ -207,14 +216,14 @@
     py_files = get_py_files(files, ignore_files)
 
     # 过滤掉不需要加密的文件
     need_encrypted_py = filter_cannot_encrypted_py(py_files, except_main_file)
 
     encrypted_py = encrypt_py(need_encrypted_py, worker_num)
     delete_files(encrypted_py)
-    rename_excrypted_file(output_file_path)
+    rename_encrypted_file(output_file_path)
 
     logger.debug(
         "加密完成 total_count={}, success_count={}, 生成到 {}".format(
             len(need_encrypted_py), len(encrypted_py), output_file_path
         )
     )
```

### Comparing `jmpy4-1.0.7/jmpy/log.py` & `jmpy4-1.0.8/jmpy/log.py`

 * *Files identical despite different names*

### Comparing `jmpy4-1.0.7/jmpy4.egg-info/PKG-INFO` & `jmpy4-1.0.8/jmpy4.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: jmpy4
-Version: 1.0.7
+Version: 1.0.8
 Summary: python代码一键加密
 Home-page: https://github.com/shenny520/jmpy-plus.git
 Author: Shenny
 Author-email: shenny520@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Cython==0.29.20
+Requires-Dist: Cython==3.0.0
 
 # jmpy
 
 ![](https://img.shields.io/badge/python-3.0-brightgreen)
 
 ## 简介
 
 将python代码一键加密为so或pyd。支持单个文件加密，整个项目加密。
 
 Fork from: https://github.com/Boris-code/jmpy.git
+
 支持多进程，修复 bug
 
 ## 安装
 
     pip install jmpy4
 
 ## 使用方法
 
-    jmpy -i "xxx project dir" [-o output dir]
+    jmpy -i "xxx project dir" [-o output dir] -w 8
 
 加密后的文件默认存储在 dist/project_name/ 下
+
+## Tips
+
+加密过程会产生如下警告，不影响使用，可以忽略
+
+    'build\bdist.win-amd64' does not exist -- can't clean it
```

### Comparing `jmpy4-1.0.7/setup.py` & `jmpy4-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     version=version,
     author="Shenny",
     license="MIT",
     author_email="shenny520@outlook.com",
     description="python代码一键加密",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["Cython==0.29.20"],
+    install_requires=["Cython==3.0.0"],
     entry_points={"console_scripts": ["jmpy = jmpy.cmdline:execute"]},
     url="https://github.com/shenny520/jmpy-plus.git",
     packages=packages,
     include_package_data=True,
     classifiers=["Programming Language :: Python :: 3"],
 )
```

