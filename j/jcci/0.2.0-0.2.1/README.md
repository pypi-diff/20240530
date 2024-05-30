# Comparing `tmp/jcci-0.2.0.tar.gz` & `tmp/jcci-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.2.0.tar", last modified: Mon May 27 07:40:15 2024, max compression
+gzip compressed data, was "jcci-0.2.1.tar", last modified: Thu May 30 09:15:31 2024, max compression
```

## Comparing `jcci-0.2.0.tar` & `jcci-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.418904 jcci-0.2.0/
--rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    15416 2024-05-27 07:40:15.416900 jcci-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3679 2024-05-27 03:00:00.000000 jcci-0.2.0/README.md
--rw-rw-rw-   0        0        0     1612 2024-05-15 07:56:19.000000 jcci-0.2.0/README.pypi.md
--rw-rw-rw-   0        0        0      775 2024-05-27 07:39:38.000000 jcci-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 07:40:15.418904 jcci-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.379259 jcci-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.404902 jcci-0.2.0/src/jcci/
--rw-rw-rw-   0        0        0        0 2024-04-09 03:17:36.000000 jcci-0.2.0/src/jcci/__init__.py
--rw-rw-rw-   0        0        0    50225 2024-05-27 02:59:56.000000 jcci-0.2.0/src/jcci/analyze.py
--rw-rw-rw-   0        0        0      289 2024-05-06 05:41:58.000000 jcci-0.2.0/src/jcci/config.py
--rw-rw-rw-   0        0        0     1677 2024-05-15 07:56:19.000000 jcci-0.2.0/src/jcci/constant.py
--rw-rw-rw-   0        0        0     5531 2024-05-15 07:56:19.000000 jcci-0.2.0/src/jcci/database.py
--rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.2.0/src/jcci/diff_parse.py
--rw-rw-rw-   0        0        0     8521 2024-05-27 02:59:56.000000 jcci-0.2.0/src/jcci/graph.py
--rw-rw-rw-   0        0        0    62842 2024-05-27 03:00:00.000000 jcci-0.2.0/src/jcci/java_parse.py
--rw-rw-rw-   0        0        0     4528 2024-05-15 07:56:19.000000 jcci-0.2.0/src/jcci/mapper_parse.py
--rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.2.0/src/jcci/sql.py
-drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.415899 jcci-0.2.0/src/jcci.egg-info/
--rw-rw-rw-   0        0        0    15416 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.413901 jcci-0.2.0/test/
--rw-rw-rw-   0        0        0        0 2024-04-08 06:40:37.000000 jcci-0.2.0/test/test_case.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:15:31.140852 jcci-0.2.1/
+-rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    15416 2024-05-30 09:15:31.137853 jcci-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4103 2024-05-30 09:14:10.000000 jcci-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1612 2024-05-15 07:56:19.000000 jcci-0.2.1/README.pypi.md
+-rw-rw-rw-   0        0        0      775 2024-05-30 09:15:14.000000 jcci-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 09:15:31.140852 jcci-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 09:15:31.089850 jcci-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 09:15:31.123850 jcci-0.2.1/src/jcci/
+-rw-rw-rw-   0        0        0        0 2024-04-09 03:17:36.000000 jcci-0.2.1/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0    51772 2024-05-30 09:14:10.000000 jcci-0.2.1/src/jcci/analyze.py
+-rw-rw-rw-   0        0        0      484 2024-05-30 09:14:10.000000 jcci-0.2.1/src/jcci/config.py
+-rw-rw-rw-   0        0        0     1677 2024-05-15 07:56:19.000000 jcci-0.2.1/src/jcci/constant.py
+-rw-rw-rw-   0        0        0     5531 2024-05-15 07:56:19.000000 jcci-0.2.1/src/jcci/database.py
+-rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.2.1/src/jcci/diff_parse.py
+-rw-rw-rw-   0        0        0     7933 2024-05-29 06:00:01.000000 jcci-0.2.1/src/jcci/graph.py
+-rw-rw-rw-   0        0        0    62867 2024-05-30 09:14:10.000000 jcci-0.2.1/src/jcci/java_parse.py
+-rw-rw-rw-   0        0        0     4528 2024-05-15 07:56:19.000000 jcci-0.2.1/src/jcci/mapper_parse.py
+-rw-rw-rw-   0        0        0     2027 2024-05-30 09:14:09.000000 jcci-0.2.1/src/jcci/sql.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:15:31.135852 jcci-0.2.1/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0    15416 2024-05-30 09:15:30.000000 jcci-0.2.1/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-30 09:15:31.000000 jcci-0.2.1/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:15:30.000000 jcci-0.2.1/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-30 09:15:30.000000 jcci-0.2.1/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-30 09:15:30.000000 jcci-0.2.1/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 09:15:31.133851 jcci-0.2.1/test/
+-rw-rw-rw-   0        0        0        0 2024-04-08 06:40:37.000000 jcci-0.2.1/test/test_case.py
```

### Comparing `jcci-0.2.0/LICENSE` & `jcci-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.2.0/PKG-INFO` & `jcci-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.2.0
+Version: 0.2.1
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `jcci-0.2.0/README.md` & `jcci-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,25 +32,37 @@
 要求python >= 3.9 , sqlite3 >= 3.38
 
 ### 使用说明
 项目克隆下来后，新建python文件，引入jcci项目src目录下的jcci
 ```
 from path.to.jcci.src.jcci.analyze import JCCI
 
-# 同一分支不同commit比较
+# 同一分支不同commit分析
 commit_analyze = JCCI('git@xxxx.git', 'username1')
 commit_analyze.analyze_two_commit('master','commit_id1','commit_id2')
 
 # 分析一个类的方法影响, analyze_class_method方法最后参数为方法所在行数，不同方法行数用逗号分割，不填则分析完整类影响
 class_analyze = JCCI('git@xxxx.git', 'username1')
 class_analyze.analyze_class_method('master','commit_id1', 'package\src\main\java\ClassA.java', '20,81')
 
-# 不同分支比较
+# 不同分支分析
 branch_analyze = JCCI('git@xxxx.git', 'username1')
 branch_analyze.analyze_two_branch('branch_new','branch_old')
+
+# 多项目联合分析，上述三种方法都支持，以analyze_two_commit方法举例
+dependents = [
+    {
+        'git_url': 'git@xxxx.git',
+        'branch': 'master',  # default master when empty
+        'commit_id': 'HEAD'  # default HEAD when empty
+    }
+]
+commit_analyze = JCCI('git@xxxx.git', 'username1')
+commit_analyze.analyze_two_commit('master','commit_id1','commit_id2', dependents=dependents)
+
 ```
 #### 参数说明：
 * project_git_url - 项目git地址，代码使用本机git配置clone代码，确保本机git权限或通过用户名密码/token的方式拼接url来clone代码。示例：https://userName:password@github.com/xxx.git 或 https://token@github.com/xxx.git
 * username1 - 随便输入，为了避免并发分析同一项目导致结果错误，用户1分析项目A时，用户B需要等待，所以设置了该参数
 
 运行时，会将项目克隆到目录中，然后进行分析，生成后缀格式为.cci的文件，其中包含分析结果生成的关系图数据，下载[jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) ，选择分析结果的.cci文件，即可可通过视图显示。
```

### Comparing `jcci-0.2.0/README.pypi.md` & `jcci-0.2.1/README.pypi.md`

 * *Files identical despite different names*

### Comparing `jcci-0.2.0/pyproject.toml` & `jcci-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `jcci-0.2.0/src/jcci/analyze.py` & `jcci-0.2.1/src/jcci/analyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.DEBUG)
 
 
 class JCCI(object):
     def __init__(self, git_url, username):
         self.git_url = git_url
         self.username: str = username
-        # self.git_token = git_token
         self.branch_name: str = ''
         self.commit_or_branch_new: str = ''
         self.commit_or_branch_old: str = ''
         self.project_id: int = -1
         self.cci_filepath: str = ''
         self.project_name: str = ''
         self.file_path: str = ''
@@ -72,14 +71,30 @@
         # 占住项目分析
         logging.info('Start occupying project, and others can not analyze until released')
         occupy_filepath = os.path.join(self.file_path, 'Occupy.ing')
         with open(occupy_filepath, 'w') as ow:
             ow.write(f'Occupy by {self.username}')
         time.sleep(1)
 
+    def _clone_dependents_project(self, dependents):
+        for dependent in dependents:
+            dependent_git_url = dependent.get('git_url')
+            if not dependent_git_url:
+                continue
+            dependent_branch = dependent.get('branch', 'master')
+            dependent_commit_id = dependent.get('commit_id', 'HEAD')
+            dependent_project_name = dependent_git_url.split('/')[-1].split('.git')[0]
+            dependent_file_path = os.path.join(self.file_path, dependent_project_name)
+            if not os.path.exists(dependent_file_path):
+                logging.info(f'Cloning dependent project: {dependent_git_url}')
+                os.system(f'git clone -b {dependent_branch} {dependent_git_url} {dependent_file_path} && cd {dependent_file_path} && git reset --hard {dependent_commit_id}')
+            else:
+                os.system(f'cd {dependent_file_path} && git fetch --all && git checkout -b {dependent_branch} origin/{dependent_branch} && git reset --hard {dependent_commit_id}')
+                os.system(f'cd {dependent_file_path} && git checkout -b {dependent_branch} && git reset --hard {dependent_commit_id}')
+
     # Step 2
     def _get_diff_parse_map(self, filepath, branch, commit_first, commit_second):
         logging.info('Git pull project to HEAD')
         os.system(f'cd {filepath} && git checkout {branch} && git pull')
         time.sleep(1)
         logging.info(f'Git diff between {commit_first} and {commit_second}')
         diff_base = f'cd {self.file_path} && git diff {commit_second}..{commit_first} > diff_{commit_second}..{commit_first}.txt'
@@ -618,25 +633,27 @@
                 self._add_to_need_analyze_obj_list('java', package_class, None, None, commit_or_branch, class_entity)
                 class_node_id = self.view.create_node_category(class_name, 'entity', constant.NODE_TYPE_CLASS, constant.DIFF_TYPE_IMPACTED, '', self.file_path, '', '', {})
                 self.view.create_node_link(impacted_field_node_id, class_node_id)
 
     # Step 5.9
     def _handle_impacted_methods(self, impacted_methods: list, source_node_id):
         for impacted_method in impacted_methods:
-            is_api = impacted_method.get('is_api') == 'True'
-            node_extend_dict = impacted_method
-            node_extend_dict['is_api'] = is_api
+            node_extend_dict = {'is_api': False}
+            if impacted_method.get('is_api') == 'True':
+                node_extend_dict = {
+                    'is_api': True,
+                    'api_path': impacted_method['api_path']
+                }
             class_id = impacted_method['class_id']
             class_entity = self.sqlite.select_data(f'SELECT package_name, class_name, commit_or_branch, filepath FROM class WHERE class_id={class_id}')[0]
             class_name = class_entity['class_name']
             package_name = class_entity['package_name']
             package_class = f'{package_name}.{class_name}'
             commit_or_branch = class_entity['commit_or_branch']
             class_filepath = class_entity['filepath']
-            node_extend_dict['class_annotations'] = class_entity['annotations']
             method_name_param = f'{impacted_method["method_name"]}({",".join([param["parameter_type"] for param in json.loads(impacted_method["parameters"])])})'
             impacted_method_node_id = self.view.create_node_category(class_name, method_name_param, constant.NODE_TYPE_METHOD, constant.DIFF_TYPE_IMPACTED, impacted_method.get('body'), class_filepath, impacted_method.get('documentation'), impacted_method.get('body'), node_extend_dict)
             self.view.create_node_link(source_node_id, impacted_method_node_id)
             extend_dict = {'method_node_id': impacted_method_node_id, 'class_filepath': class_filepath}
             extend_dict.update(impacted_method)
             self._add_to_need_analyze_obj_list('java', package_class, None, self._get_method_param_string(impacted_method), commit_or_branch, extend_dict)
 
@@ -690,35 +707,39 @@
         try:
             logging.info(f'Analyze done, remove occupy, others can analyze now')
             os.remove(os.path.join(self.file_path, 'Occupy.ing'))
         finally:
             pass
         logging.info(f'Analyze done, spend: {t2 - self.t1}')
 
-    def analyze_two_branch(self, branch_first, branch_second):
+    def analyze_two_branch(self, branch_first, branch_second, **kwargs):
         logging.info('*' * 10 + 'Analyze start' + '*' * 10)
         self.commit_or_branch_new = branch_first
         self.commit_or_branch_old = branch_second
         self.branch_name = branch_first
         self.project_name = self.git_url.split('/')[-1].split('.git')[0]
         self.file_path = os.path.join(config.project_path, self.project_name)
         self.project_id = self.sqlite.add_project(self.project_name, self.git_url, self.branch_name, branch_first, branch_second)
         # 已有分析结果
         self.cci_filepath = os.path.join(self.file_path, f'{branch_second.replace("/", "#")}..{branch_first.replace("/", "#")}.cci')
         self._can_analyze(self.file_path, self.cci_filepath)
         # 无此项目, 先clone项目
         if not os.path.exists(self.file_path):
             logging.info(f'Cloning project: {self.git_url}')
             os.system(f'git clone -b {branch_first} {self.git_url} {self.file_path}')
+
+        dependents: list[dict] = kwargs.get('dependents', [])
+        self._clone_dependents_project(dependents)
+
         self._occupy_project()
         self.diff_parse_map = self._get_branch_diff_parse_map(self.file_path, branch_first, branch_second)
         self.xml_parse_results_new, self.xml_parse_results_old = self._parse_branch_project(self.file_path, branch_first, branch_second)
         self._start_analysis_diff_and_impact()
 
-    def analyze_two_commit(self, branch, commit_first, commit_second):
+    def analyze_two_commit(self, branch, commit_first, commit_second, **kwargs):
         logging.info('*' * 10 + 'Analyze start' + '*' * 10)
         self.branch_name = branch
         self.commit_or_branch_new = commit_first[0: 7] if len(commit_first) > 7 else commit_first
         self.commit_or_branch_old = commit_second[0: 7] if len(commit_second) > 7 else commit_second
 
         self.project_name = self.git_url.split('/')[-1].split('.git')[0]
         self.file_path = os.path.join(config.project_path, self.project_name)
@@ -729,22 +750,25 @@
         self._can_analyze(self.file_path, self.cci_filepath)
 
         # 无此项目, 先clone项目
         if not os.path.exists(self.file_path):
             logging.info(f'Cloning project: {self.git_url}')
             os.system(f'git clone -b {self.branch_name} {self.git_url} {self.file_path}')
 
+        dependents: list[dict] = kwargs.get('dependents', [])
+        self._clone_dependents_project(dependents)
+
         self._occupy_project()
         self.diff_parse_map = self._get_diff_parse_map(self.file_path, self.branch_name, self.commit_or_branch_new, self.commit_or_branch_old)
 
         self.xml_parse_results_new, self.xml_parse_results_old = self._parse_project(self.file_path, self.commit_or_branch_new, self.commit_or_branch_old)
 
         self._start_analysis_diff_and_impact()
 
-    def analyze_class_method(self, branch, commit_id, package_class, method_nums):
+    def analyze_class_method(self, branch, commit_id, package_class, method_nums, **kwargs):
         logging.info('*' * 10 + 'Analyze start' + '*' * 10)
         package_class = package_class.replace("\\", "/")
         self.branch_name = branch
         self.commit_or_branch_new = commit_id
         self.commit_or_branch_new = self.commit_or_branch_new[0: 7] if len(self.commit_or_branch_new) > 7 else self.commit_or_branch_new
         self.project_name = self.git_url.split('/')[-1].split('.git')[0]
         self.file_path = os.path.join(config.project_path, self.project_name)
@@ -755,14 +779,18 @@
         self.cci_filepath = os.path.join(self.file_path, cci_path)
         self._can_analyze(self.file_path, self.cci_filepath)
 
         # 无此项目, 先clone项目
         if not os.path.exists(self.file_path):
             logging.info(f'Cloning project: {self.git_url}')
             os.system(f'git clone -b {self.branch_name} {self.git_url} {self.file_path}')
+
+        dependents: list[dict] = kwargs.get('dependents', [])
+        self._clone_dependents_project(dependents)
+
         self._occupy_project()
 
         logging.info('Git pull project to HEAD')
         os.system(f'cd {self.file_path} && git checkout {branch} && git pull')
         time.sleep(1)
 
         if not method_nums:
```

### Comparing `jcci-0.2.0/src/jcci/constant.py` & `jcci-0.2.1/src/jcci/constant.py`

 * *Files identical despite different names*

### Comparing `jcci-0.2.0/src/jcci/database.py` & `jcci-0.2.1/src/jcci/database.py`

 * *Files identical despite different names*

### Comparing `jcci-0.2.0/src/jcci/diff_parse.py` & `jcci-0.2.1/src/jcci/diff_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.2.0/src/jcci/graph.py` & `jcci-0.2.1/src/jcci/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,18 +103,14 @@
             changed_node['label'] = {
                 'show': True,
                 'formatter': changed_node["name"].split("(")[0]
             }
             tooltip = f'{changed_node["name"].split("(")[0]}<br>[Changed]{changed_node.get("diff_content", "")}'
             if changed_node.get('is_api'):
                 tooltip = tooltip + f'<br>[API]{changed_node.get("api_path")}'
-            if changed_node.get("annotations"):
-                tooltip += f'<br>[annotations]{changed_node.get("annotations", "")}'
-            if changed_node.get("class_annotations"):
-                tooltip += f'<br>[class_annotations]{changed_node.get("class_annotations", "")}'
             changed_node['tooltip'] = {
                 'show': True,
                 'position': 'right',
                 'formatter': tooltip
             }
             all_node.append(changed_node)
         max_link_count = max([value for key, value in result.items()]) if result else 1
@@ -130,26 +126,21 @@
             level_node_index = level_node_list.index(impacted_node['id']) if impacted_node['id'] in level_node_list else 1
             impacted_node['x'] = 100 + ((canvas_width - 100) / max_link_count) * (path_level + 1)
             impacted_node['y'] = (canvas_height / len(count_node_result.get(str(path_level), [1]))) * level_node_index
             impacted_node['label'] = {
                 'show': True,
                 'formatter': impacted_node["name"].split("(")[0]
             }
-            tooltip = f'{impacted_node["name"].split("(")[0]}'
             if impacted_node.get('is_api'):
-                tooltip += f'<br>[API]{impacted_node.get("api_path")}'
-            if impacted_node.get("annotations"):
-                tooltip += f'<br>[annotations]{impacted_node.get("annotations", "")}'
-            if impacted_node.get("class_annotations"):
-                tooltip += f'<br>[class_annotations]{impacted_node.get("class_annotations", "")}'
-            impacted_node['tooltip'] = {
-                'show': True,
-                'position': 'right',
-                'formatter': tooltip
-            }
+                tooltip = f'{impacted_node["name"].split("(")[0]}<br>[API]{impacted_node.get("api_path")}'
+                impacted_node['tooltip'] = {
+                    'show': True,
+                    'position': 'right',
+                    'formatter': tooltip
+                }
             all_node.append(impacted_node)
         self.nodes = all_node
 
 if __name__ == '__main__':
     data = [{'source': '62', 'target': '61'}, {'source': '63', 'target': '64'}, {'source': '63', 'target': '65'}, {'source': '63', 'target': '66'}, {'source': '63', 'target': '67'}, {'source': '9', 'target': '8'}, {'source': '68', 'target': '25'}, {'source': '21', 'target': '18'}, {'source': '21', 'target': '19'}, {'source': '26', 'target': '25'}, {'source': '27', 'target': '25'}, {'source': '72', 'target': '5'}, {'source': '72', 'target': '8'}, {'source': '72', 'target': '9'}, {'source': '73', 'target': '18'}, {'source': '73', 'target': '19'}, {'source': '73', 'target': '20'}, {'source': '73', 'target': '21'}, {'source': '74', 'target': '17'}, {'source': '74', 'target': '54'}, {'source': '75', 'target': '76'}, {'source': '75', 'target': '3'}, {'source': '75', 'target': '77'}, {'source': '75', 'target': '5'}, {'source': '75', 'target': '78'}, {'source': '75', 'target': '79'}, {'source': '75', 'target': '6'}, {'source': '75', 'target': '80'}, {'source': '75', 'target': '8'}, {'source': '75', 'target': '9'}, {'source': '75', 'target': '81'}, {'source': '46', 'target': '47'}, {'source': '46', 'target': '60'}, {'source': '47', 'target': '61'}, {'source': '48', 'target': '47'}, {'source': '49', 'target': '46'}, {'source': '50', 'target': '46'}, {'source': '83', 'target': '17'}, {'source': '83', 'target': '18'}, {'source': '54', 'target': '17'}, {'source': '55', 'target': '18'}, {'source': '56', 'target': '55'}, {'source': '57', 'target': '55'}, {'source': '58', 'target': '56'}, {'source': '58', 'target': '57'}, {'source': '59', 'target': '54'}, {'source': '59', 'target': '55'}, {'source': '59', 'target': '56'}, {'source': '59', 'target': '57'}, {'source': '64', 'target': '66'}, {'source': '65', 'target': '64'}]
     bb = max_relationship_length(data)
```

### Comparing `jcci-0.2.0/src/jcci/java_parse.py` & `jcci-0.2.1/src/jcci/java_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,16 +920,16 @@
         import_list = self._parse_imports(tree_imports)
         import_map = {import_obj['import_path'].split('.')[-1]: import_obj['import_path'] for import_obj in import_list}
 
         # 处理 class 信息
         class_type = type(class_declaration).__name__.replace('Declaration', '')
         class_id, new_add = self._parse_class(class_declaration, filepath, package_name, import_list, commit_or_branch, parse_import_first)
         # 已经处理过了，返回
-        # if not new_add:
-        #     return
+        if not new_add and not config.reparse_class:
+            return
         # 导入import
         imports = [dict(import_obj, class_id=class_id, project_id=self.project_id) for import_obj in import_list]
         self.sqlite.update_data(f'DELETE FROM import WHERE class_id={class_id}')
         self.sqlite.insert_data('import', imports)
 
         # 处理 inner class
         inner_class_declarations = [inner_class for inner_class in class_declaration.body
```

### Comparing `jcci-0.2.0/src/jcci/mapper_parse.py` & `jcci-0.2.1/src/jcci/mapper_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.2.0/src/jcci/sql.py` & `jcci-0.2.1/src/jcci/sql.py`

 * *Files identical despite different names*

### Comparing `jcci-0.2.0/src/jcci.egg-info/PKG-INFO` & `jcci-0.2.1/src/jcci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.2.0
+Version: 0.2.1
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

