# Comparing `tmp/aura_tools-0.8.tar.gz` & `tmp/aura_tools-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura_tools-0.8.tar", last modified: Wed May 29 12:29:20 2024, max compression
+gzip compressed data, was "aura_tools-0.9.tar", last modified: Wed May 29 12:33:55 2024, max compression
```

## Comparing `aura_tools-0.8.tar` & `aura_tools-0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.995993 aura_tools-0.8/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.8/LICENSE
--rw-rw-rw-   0        0        0      428 2024-05-29 12:29:20.995059 aura_tools-0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.964664 aura_tools-0.8/aura_tools/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.8/aura_tools/__init__.py
--rw-rw-rw-   0        0        0     4868 2024-05-29 12:26:52.000000 aura_tools-0.8/aura_tools/code_explanation_generator.py
--rw-rw-rw-   0        0        0     1554 2024-05-29 12:23:18.000000 aura_tools-0.8/aura_tools/count_functions.py
--rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.8/aura_tools/director_scanner.py
--rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.8/aura_tools/github_repository_downloader.py
--rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.8/aura_tools/java_function_extractor.py
--rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.8/aura_tools/json_file_util.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.980980 aura_tools-0.8/aura_tools/llm/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.8/aura_tools/llm/__init__.py
--rw-rw-rw-   0        0        0     3486 2024-05-29 12:03:32.000000 aura_tools-0.8/aura_tools/llm/baidu_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.986993 aura_tools-0.8/aura_tools/llm/base/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.8/aura_tools/llm/base/__init__.py
--rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.8/aura_tools/llm/base/llm_base_client.py
--rw-rw-rw-   0        0        0     2769 2024-05-29 11:45:24.000000 aura_tools-0.8/aura_tools/llm/tongyi_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.991088 aura_tools-0.8/aura_tools/process/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:54:58.000000 aura_tools-0.8/aura_tools/process/__init__.py
--rw-rw-rw-   0        0        0     2121 2024-05-29 11:57:29.000000 aura_tools-0.8/aura_tools/process/multi_process_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.993012 aura_tools-0.8/aura_tools.egg-info/
--rw-rw-rw-   0        0        0      428 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 12:29:20.996905 aura_tools-0.8/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-05-29 12:29:08.000000 aura_tools-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:33:55.588029 aura_tools-0.9/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.9/LICENSE
+-rw-rw-rw-   0        0        0      428 2024-05-29 12:33:55.585994 aura_tools-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 12:33:55.561125 aura_tools-0.9/aura_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.9/aura_tools/__init__.py
+-rw-rw-rw-   0        0        0     4945 2024-05-29 12:33:19.000000 aura_tools-0.9/aura_tools/code_explanation_generator.py
+-rw-rw-rw-   0        0        0     1554 2024-05-29 12:23:18.000000 aura_tools-0.9/aura_tools/count_functions.py
+-rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.9/aura_tools/director_scanner.py
+-rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.9/aura_tools/github_repository_downloader.py
+-rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.9/aura_tools/java_function_extractor.py
+-rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.9/aura_tools/json_file_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:33:55.574372 aura_tools-0.9/aura_tools/llm/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.9/aura_tools/llm/__init__.py
+-rw-rw-rw-   0        0        0     3486 2024-05-29 12:03:32.000000 aura_tools-0.9/aura_tools/llm/baidu_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:33:55.577823 aura_tools-0.9/aura_tools/llm/base/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.9/aura_tools/llm/base/__init__.py
+-rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.9/aura_tools/llm/base/llm_base_client.py
+-rw-rw-rw-   0        0        0     2769 2024-05-29 11:45:24.000000 aura_tools-0.9/aura_tools/llm/tongyi_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:33:55.581988 aura_tools-0.9/aura_tools/process/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:54:58.000000 aura_tools-0.9/aura_tools/process/__init__.py
+-rw-rw-rw-   0        0        0     2121 2024-05-29 11:57:29.000000 aura_tools-0.9/aura_tools/process/multi_process_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:33:55.583906 aura_tools-0.9/aura_tools.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-05-29 12:33:55.000000 aura_tools-0.9/aura_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2024-05-29 12:33:55.000000 aura_tools-0.9/aura_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:33:55.000000 aura_tools-0.9/aura_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-29 12:33:55.000000 aura_tools-0.9/aura_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 12:33:55.000000 aura_tools-0.9/aura_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:33:55.588029 aura_tools-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-29 12:33:42.000000 aura_tools-0.9/setup.py
```

### Comparing `aura_tools-0.8/aura_tools/code_explanation_generator.py` & `aura_tools-0.9/aura_tools/code_explanation_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,32 +71,32 @@
             print(f"Error: {e}")
             timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             self.error_file.append_json_line(f"{timestamp} Error: {e} , file = {file}")
 
     @staticmethod
     def download_and_scan(repo_url,target_dir='.'):
         """下载仓库并扫描Java文件"""
-        dir_path = GithubRepositoryDownloader(repo_url).download()
+        dir_path = GithubRepositoryDownloader(repo_url=repo_url,target_dir=target_dir).download()
         print(f"仓库已下载到: {dir_path}")
 
         scanner = DirectoryScanner(dir_path, filter_types=['.java'])
         all_files = scanner.scan_all()
         java_files = scanner.filter_files_by_type(all_files)
         return java_files
 
     def process_files(self, files_list):
         """处理文件列表"""
         file_total = len(files_list)
         for file_index, file in enumerate(files_list):
             print(f"正在处理第 {file_index + 1} 个文件,共 {file_total} 个文件 , file = {file}")
             self._process_file(file)
 
-    def run(self, repo_url):
+    def run(self, repo_url,target_dir='.'):
         """运行代码解释生成流程"""
-        java_files = self.download_and_scan(repo_url)
+        java_files = self.download_and_scan(repo_url=repo_url,target_dir=target_dir)
         self.process_files(java_files)
 
 if __name__ == '__main__':
     # 百度
     api_key = ""
     secret_key = ""
     client = BaiduAIClient(f"{api_key}|{secret_key}");
```

### Comparing `aura_tools-0.8/aura_tools/count_functions.py` & `aura_tools-0.9/aura_tools/count_functions.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools/director_scanner.py` & `aura_tools-0.9/aura_tools/director_scanner.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools/github_repository_downloader.py` & `aura_tools-0.9/aura_tools/github_repository_downloader.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools/java_function_extractor.py` & `aura_tools-0.9/aura_tools/java_function_extractor.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools/json_file_util.py` & `aura_tools-0.9/aura_tools/json_file_util.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools/llm/baidu_ai_client.py` & `aura_tools-0.9/aura_tools/llm/baidu_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools/llm/tongyi_ai_client.py` & `aura_tools-0.9/aura_tools/llm/tongyi_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools/process/multi_process_handler.py` & `aura_tools-0.9/aura_tools/process/multi_process_handler.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/aura_tools.egg-info/SOURCES.txt` & `aura_tools-0.9/aura_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aura_tools-0.8/setup.py` & `aura_tools-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aura_tools',  # 包名
-    version='0.8',  # 版本号
+    version='0.9',  # 版本号
     packages=find_packages(),  # 自动找到包目录
     install_requires=[  # 依赖包
         # 'some_package>=1.0',
     ],
     entry_points={  # 可选的命令行工具
         'console_scripts': [
             'my_command=my_project.some_module:main',
```

