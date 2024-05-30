# Comparing `tmp/akasha-terminal-0.8.8.tar.gz` & `tmp/akasha-terminal-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akasha-terminal-0.8.8.tar", last modified: Tue Jan 16 03:06:34 2024, max compression
+gzip compressed data, was "akasha-terminal-0.8.9.tar", last modified: Mon Jan 22 08:02:31 2024, max compression
```

## Comparing `akasha-terminal-0.8.8.tar` & `akasha-terminal-0.8.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.729382 akasha-terminal-0.8.8/
--rw-rw-rw-   0        0        0     1088 2023-12-08 03:18:31.000000 akasha-terminal-0.8.8/License
--rw-rw-rw-   0        0        0    41672 2024-01-16 03:06:34.728382 akasha-terminal-0.8.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.705382 akasha-terminal-0.8.8/akasha/
--rw-rw-rw-   0        0        0       23 2023-12-08 07:41:35.000000 akasha-terminal-0.8.8/akasha/__init__.py
--rw-rw-rw-   0        0        0    30169 2024-01-16 03:05:54.000000 akasha-terminal-0.8.8/akasha/akasha.py
--rw-rw-rw-   0        0        0    24305 2024-01-16 03:05:54.000000 akasha-terminal-0.8.8/akasha/db.py
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.708390 akasha-terminal-0.8.8/akasha/eval/
--rw-rw-rw-   0        0        0       44 2023-12-11 03:26:11.000000 akasha-terminal-0.8.8/akasha/eval/__init__.py
--rw-rw-rw-   0        0        0    50191 2024-01-16 03:05:54.000000 akasha-terminal-0.8.8/akasha/eval/eval.py
--rw-rw-rw-   0        0        0     3591 2023-12-11 08:00:30.000000 akasha-terminal-0.8.8/akasha/eval/scores.py
--rw-rw-rw-   0        0        0     3448 2023-12-11 03:26:11.000000 akasha-terminal-0.8.8/akasha/format.py
--rw-rw-rw-   0        0        0    18083 2024-01-16 03:05:54.000000 akasha-terminal-0.8.8/akasha/helper.py
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.713381 akasha-terminal-0.8.8/akasha/interface/
--rw-rw-rw-   0        0        0     5041 2023-12-27 06:34:40.000000 akasha-terminal-0.8.8/akasha/interface/cot_page.py
--rw-rw-rw-   0        0        0     3935 2023-12-27 06:35:00.000000 akasha-terminal-0.8.8/akasha/interface/res_page.py
--rw-rw-rw-   0        0        0     9571 2023-12-27 06:35:32.000000 akasha-terminal-0.8.8/akasha/interface/setting.py
--rw-rw-rw-   0        0        0     4713 2023-12-27 06:35:55.000000 akasha-terminal-0.8.8/akasha/interface/sum_page.py
--rw-rw-rw-   0        0        0     1546 2023-12-11 03:26:11.000000 akasha-terminal-0.8.8/akasha/interface/upload_file.py
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.715382 akasha-terminal-0.8.8/akasha/models/
--rw-rw-rw-   0        0        0     7580 2024-01-15 06:04:28.000000 akasha-terminal-0.8.8/akasha/models/hf.py
--rw-rw-rw-   0        0        0     8589 2024-01-15 06:04:28.000000 akasha-terminal-0.8.8/akasha/models/llama2.py
--rw-rw-rw-   0        0        0    16270 2024-01-15 06:04:28.000000 akasha-terminal-0.8.8/akasha/prompts.py
--rw-rw-rw-   0        0        0    27894 2024-01-15 06:04:28.000000 akasha-terminal-0.8.8/akasha/search.py
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.717382 akasha-terminal-0.8.8/akasha/summary/
--rw-rw-rw-   0        0        0       24 2023-12-08 07:41:35.000000 akasha-terminal-0.8.8/akasha/summary/__init__.py
--rw-rw-rw-   0        0        0    13935 2023-12-27 06:30:55.000000 akasha-terminal-0.8.8/akasha/summary/summary.py
--rw-rw-rw-   0        0        0     7010 2023-12-27 06:36:24.000000 akasha-terminal-0.8.8/akasha/ui.py
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.723382 akasha-terminal-0.8.8/akasha_terminal.egg-info/
--rw-rw-rw-   0        0        0    41672 2024-01-16 03:06:34.000000 akasha-terminal-0.8.8/akasha_terminal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2024-01-16 03:06:34.000000 akasha-terminal-0.8.8/akasha_terminal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-16 03:06:34.000000 akasha-terminal-0.8.8/akasha_terminal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-01-16 03:06:34.000000 akasha-terminal-0.8.8/akasha_terminal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      377 2024-01-16 03:06:34.000000 akasha-terminal-0.8.8/akasha_terminal.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-16 03:06:34.000000 akasha-terminal-0.8.8/akasha_terminal.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.724380 akasha-terminal-0.8.8/cli/
--rw-rw-rw-   0        0        0    14205 2023-12-27 06:30:55.000000 akasha-terminal-0.8.8/cli/glue.py
--rw-rw-rw-   0        0        0       42 2024-01-16 03:06:34.729382 akasha-terminal-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     1596 2024-01-16 03:05:54.000000 akasha-terminal-0.8.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-16 03:06:34.727381 akasha-terminal-0.8.8/tests/
--rw-rw-rw-   0        0        0     5183 2023-12-27 07:56:15.000000 akasha-terminal-0.8.8/tests/test_akasha.py
--rw-rw-rw-   0        0        0     2520 2024-01-15 06:20:40.000000 akasha-terminal-0.8.8/tests/test_eval.py
--rw-rw-rw-   0        0        0     1074 2023-12-27 06:59:33.000000 akasha-terminal-0.8.8/tests/test_summary.py
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.540812 akasha-terminal-0.8.9/
+-rw-rw-rw-   0        0        0     1088 2023-12-08 03:18:31.000000 akasha-terminal-0.8.9/License
+-rw-rw-rw-   0        0        0    42483 2024-01-22 08:02:31.540812 akasha-terminal-0.8.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.378814 akasha-terminal-0.8.9/akasha/
+-rw-rw-rw-   0        0        0       23 2023-12-08 07:41:35.000000 akasha-terminal-0.8.9/akasha/__init__.py
+-rw-rw-rw-   0        0        0    30127 2024-01-22 04:02:53.000000 akasha-terminal-0.8.9/akasha/akasha.py
+-rw-rw-rw-   0        0        0    24305 2024-01-16 03:05:54.000000 akasha-terminal-0.8.9/akasha/db.py
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.392814 akasha-terminal-0.8.9/akasha/eval/
+-rw-rw-rw-   0        0        0       44 2023-12-11 03:26:11.000000 akasha-terminal-0.8.9/akasha/eval/__init__.py
+-rw-rw-rw-   0        0        0    57620 2024-01-22 04:02:53.000000 akasha-terminal-0.8.9/akasha/eval/eval.py
+-rw-rw-rw-   0        0        0     3591 2023-12-11 08:00:30.000000 akasha-terminal-0.8.9/akasha/eval/scores.py
+-rw-rw-rw-   0        0        0     3448 2023-12-11 03:26:11.000000 akasha-terminal-0.8.9/akasha/format.py
+-rw-rw-rw-   0        0        0    18083 2024-01-16 03:05:54.000000 akasha-terminal-0.8.9/akasha/helper.py
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.446813 akasha-terminal-0.8.9/akasha/interface/
+-rw-rw-rw-   0        0        0     5041 2023-12-27 06:34:40.000000 akasha-terminal-0.8.9/akasha/interface/cot_page.py
+-rw-rw-rw-   0        0        0     3935 2023-12-27 06:35:00.000000 akasha-terminal-0.8.9/akasha/interface/res_page.py
+-rw-rw-rw-   0        0        0     9571 2023-12-27 06:35:32.000000 akasha-terminal-0.8.9/akasha/interface/setting.py
+-rw-rw-rw-   0        0        0     4713 2023-12-27 06:35:55.000000 akasha-terminal-0.8.9/akasha/interface/sum_page.py
+-rw-rw-rw-   0        0        0     1546 2023-12-11 03:26:11.000000 akasha-terminal-0.8.9/akasha/interface/upload_file.py
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.459813 akasha-terminal-0.8.9/akasha/models/
+-rw-rw-rw-   0        0        0     7580 2024-01-15 06:04:28.000000 akasha-terminal-0.8.9/akasha/models/hf.py
+-rw-rw-rw-   0        0        0     8589 2024-01-15 06:04:28.000000 akasha-terminal-0.8.9/akasha/models/llama2.py
+-rw-rw-rw-   0        0        0    17668 2024-01-22 04:02:53.000000 akasha-terminal-0.8.9/akasha/prompts.py
+-rw-rw-rw-   0        0        0    27894 2024-01-15 06:04:28.000000 akasha-terminal-0.8.9/akasha/search.py
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.481814 akasha-terminal-0.8.9/akasha/summary/
+-rw-rw-rw-   0        0        0       24 2023-12-08 07:41:35.000000 akasha-terminal-0.8.9/akasha/summary/__init__.py
+-rw-rw-rw-   0        0        0    13935 2023-12-27 06:30:55.000000 akasha-terminal-0.8.9/akasha/summary/summary.py
+-rw-rw-rw-   0        0        0     7010 2023-12-27 06:36:24.000000 akasha-terminal-0.8.9/akasha/ui.py
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.507813 akasha-terminal-0.8.9/akasha_terminal.egg-info/
+-rw-rw-rw-   0        0        0    42483 2024-01-22 08:02:31.000000 akasha-terminal-0.8.9/akasha_terminal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-01-22 08:02:31.000000 akasha-terminal-0.8.9/akasha_terminal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-22 08:02:31.000000 akasha-terminal-0.8.9/akasha_terminal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-01-22 08:02:31.000000 akasha-terminal-0.8.9/akasha_terminal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      377 2024-01-22 08:02:31.000000 akasha-terminal-0.8.9/akasha_terminal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-01-22 08:02:31.000000 akasha-terminal-0.8.9/akasha_terminal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.514813 akasha-terminal-0.8.9/cli/
+-rw-rw-rw-   0        0        0    14205 2023-12-27 06:30:55.000000 akasha-terminal-0.8.9/cli/glue.py
+-rw-rw-rw-   0        0        0       42 2024-01-22 08:02:31.541813 akasha-terminal-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     1596 2024-01-22 04:02:53.000000 akasha-terminal-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-22 08:02:31.538813 akasha-terminal-0.8.9/tests/
+-rw-rw-rw-   0        0        0     5183 2023-12-27 07:56:15.000000 akasha-terminal-0.8.9/tests/test_akasha.py
+-rw-rw-rw-   0        0        0     2520 2024-01-15 06:20:40.000000 akasha-terminal-0.8.9/tests/test_eval.py
+-rw-rw-rw-   0        0        0     1074 2023-12-27 06:59:33.000000 akasha-terminal-0.8.9/tests/test_summary.py
```

### Comparing `akasha-terminal-0.8.8/License` & `akasha-terminal-0.8.9/License`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/PKG-INFO` & `akasha-terminal-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: akasha-terminal
-Version: 0.8.8
+Version: 0.8.9
 Summary: document QA package using langchain and chromadb
 Home-page: https://github.com/iii-org/akasha
 Author: chih chuan chang
 Author-email: ccchang@iii.org.tw
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: License
 
 # akasha
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![pypi package : 0.8.8](https://img.shields.io/badge/pypi%20package-0.8.7-blue)](https://pypi.org/project/akasha-terminal/)
+[![pypi package : 0.8.9](https://img.shields.io/badge/pypi%20package-0.8.7-blue)](https://pypi.org/project/akasha-terminal/)
 [![python version : 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 ![GitLab CI](https://img.shields.io/badge/gitlab%20ci-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white)
 
 <br/>
 
 Akasha simplifies document-based Question Answering (QA) by harnessing the power of Large Language Models to accurately answer your queries while searching through your provided documents.
 
@@ -694,14 +694,35 @@
 
 eva.auto_create_questionset(doc_path="doc/mic/", question_num=10, output_file_path="questionset/mic_irre.txt")
 
 bert_score, rouge, llm_score = eva.auto_evaluation(questionset_path="questionset/mic_irre.txt", doc_path="doc/mic/", question_style = "essay", record_exp="exp_mic_auto_evaluation",topK=3,search_type="svm")
 
 ```
 
+<br/>
+<br/>
+
+
+## assign certain topic of questionset
+If you want to generate certain topic of question, you can use **create_topic_questionset** function, it will use the topic input to find related texts in the documents
+ and generate question set.
+
+
+```python
+
+import akasha.eval as eval
+
+eva = eval.Model_Eval(search_type='merge', question_type = "irrelevant", model="openai:gpt-3.5-turbo", record_exp="exp_mic_auto_questionset")
+
+eva.create_topic_questionset(doc_path="doc/mic/", topic= "工業4.0", question_num=3, output_file_path="questionset/mic_topic_irre.txt")
+
+bert_score, rouge, llm_score = eva.auto_evaluation(questionset_path="questionset/mic_topic_irre.txt", doc_path="doc/mic/", question_style = "essay", record_exp="exp_mic_auto_evaluation",topK=3,search_type="svm")
+
+```
+
 
 <br/>
 <br/>
 <br/>
 <br/>
```

### Comparing `akasha-terminal-0.8.8/akasha/akasha.py` & `akasha-terminal-0.8.9/akasha/akasha.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,15 +561,14 @@
             )
             metrics = format.handle_metrics(self.doc_length,
                                             end_time - start_time,
                                             self.doc_tokens)
             table = format.handle_table(prompt, self.docs, self.response)
             aiido_upload(self.record_exp, params, metrics, table)
 
-        del self.db
         return self.response
 
     def chain_of_thought(self, doc_path: Union[List[str], str],
                          prompt_list: list, **kwargs) -> list:
         """input the documents directory path and question, will first store the documents
         into vectors db (chromadb), then search similar documents based on the prompt question.
         llm model will use these documents to generate the response of the question.
@@ -682,15 +681,14 @@
                 self.language,
             )
             metrics = format.handle_metrics(self.doc_length,
                                             end_time - start_time,
                                             self.doc_tokens)
             aiido_upload(self.record_exp, params, metrics, table)
 
-        del self.db
         return self.response
 
     def ask_whole_file(self, file_path: str, prompt: str, **kwargs) -> str:
         """input the documents directory path and question, will first store the documents
         into vectors db (chromadb), then search similar documents based on the prompt question.
         llm model will use these documents to generate the response of the question.
```

### Comparing `akasha-terminal-0.8.8/akasha/db.py` & `akasha-terminal-0.8.9/akasha/db.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/eval/eval.py` & `akasha-terminal-0.8.9/akasha/eval/eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -460,15 +460,15 @@
                                                    self.doc_tokens)
             params["doc_range"] = doc_range
             akasha.aiido_upload(self.record_exp, params, metrics, table)
 
         self._add_result_log(timestamp, end_time - start_time)
 
         self._save_questionset(timestamp, output_file_path)
-        del self.db
+
         return self.question, self.answer
 
     def _eval_get_res_fact(self, question: Union[str, list], answer: str,
                            timestamp: str) -> dict:
         """generate fact resposne from the question, can evaluate with reference answer
 
         Args:
@@ -800,15 +800,14 @@
                                                    self.doc_tokens)
             params["doc_range"] = doc_range
             akasha.aiido_upload(self.record_exp, params, metrics, table)
 
         self._add_result_log(timestamp, end_time - start_time)
 
         self._save_questionset(timestamp, output_file_path)
-        del self.db
         return self.question, self.answer
 
     def auto_evaluation(
         self,
         questionset_file: str,
         doc_path: Union[List[str], str],
         eval_model: str = "openai:gpt-3.5-turbo",
@@ -919,15 +918,15 @@
                 metrics = akasha.format.handle_metrics(self.doc_length,
                                                        end_time - start_time,
                                                        self.doc_tokens)
                 metrics["avg_bert"] = avg_bert
                 metrics["avg_rouge"] = avg_rouge
                 metrics["avg_llm_score"] = avg_llm_score
                 akasha.aiido_upload(self.record_exp, params, metrics, table)
-            del self.db
+
             return avg_bert, avg_rouge, avg_llm_score, self.doc_tokens
 
         else:
             self.logs[timestamp]["correct_rate"] = (
                 self.score["correct_count"] / self.question_num)
             if self.record_exp != "":
                 params = akasha.format.handle_params(
@@ -941,15 +940,15 @@
                 )
                 metrics = akasha.format.handle_metrics(self.doc_length,
                                                        end_time - start_time,
                                                        self.doc_tokens)
                 metrics["correct_rate"] = (self.score["correct_count"] /
                                            self.question_num)
                 akasha.aiido_upload(self.record_exp, params, metrics, table)
-            del self.db
+
             return self.logs[timestamp]["correct_rate"], self.doc_tokens
 
     def optimum_combination(
         self,
         questionset_flie: str,
         doc_path: Union[List[str], str],
         embeddings_list: list = ["openai:text-embedding-ada-002"],
@@ -1083,22 +1082,198 @@
         format_time = "time spend: " + "{:.3f}".format(end_time - start_time)
         print(format_time)
 
         if self.question_type.lower() == "essay":
             return bs_combination, rs_combination, ls_combination
         return bs_combination, bc_combination
 
+    def create_topic_questionset(
+        self,
+        doc_path: Union[List[str], str],
+        topic: str,
+        question_num: int = 10,
+        choice_num: int = 4,
+        output_file_path: str = "",
+        **kwargs,
+    ) -> (list, list):
+        """similar to auto_create_questionset, but it will use the topic to find the related documents and create questionset.
+            Args:
+                **doc_path (str)**: documents directory path\n
+                **topic (str)**: the topic of the questionset\n
+                **question_num (int, optional)**: number of questions you want to create. Defaults to 10.\n
+                **choice_num (int, optional)**: the number of choices for each single choice question, only use it if question_type is "single_choice".
+            Defaults to 4.\n
+                **output_file_path (str, optional)**: the path of output question set txt file, if not assign, use doc_path+datetime as the file name.
+                **kwargs**: the arguments you set in the initial of the class, you can change it here. Include:\n
+                question_style, question_type, embeddings, chunk_size, model, verbose, topK, threshold, language , search_type, record_exp,
+                system_prompt, max_doc_len, temperature.
+            Raises:
+                Exception: _description_
+
+            Returns:
+                (question_list:list, answer_list:list): the question and answer list that generated by llm model
+        """
+        ## set class variables ##
+        self._set_model(**kwargs)
+        self._change_variables(**kwargs)
+        self.doc_path = doc_path
+        self.question_num = question_num
+
+        if check_sum_type(self.question_type, self.question_style, "related"):
+            return [], []
+
+        ## check db ##
+        if self.use_chroma:
+            self.db, db_path_names = akasha.db.get_db_from_chromadb(
+                self.doc_path, self.embeddings)
+        else:
+            self.db, db_path_names = akasha.db.processMultiDB(
+                self.doc_path, self.verbose, self.embeddings_obj,
+                self.embeddings, self.chunk_size, self.ignore_check)
+        if not self._check_db():
+            return [], []
+
+        ## set local variables ##
+        doc_range = (
+            1999 + self.chunk_size
+        ) // self.chunk_size  # doc_range is determine by the chunk size, so the select documents won't be too short to having trouble genereating a question
+        vis_doc_range = set()
+        self.doc_tokens, self.doc_length = 0, 0
+        self.question, self.answer, self.docs = [], [], []
+        table = {}
+
+        ## add logs ##
+        timestamp = datetime.datetime.now().strftime("%Y/%m/%d, %H:%M:%S")
+        self.timestamp_list.append(timestamp)
+        start_time = time.time()
+        self._add_basic_log(timestamp, "related_questionset")
+        self.logs[timestamp]["doc_range"] = doc_range
+        self.logs[timestamp]["question_num"] = question_num
+        self.logs[timestamp]["question_type"] = self.question_type
+        self.logs[timestamp]["question_style"] = self.question_style
+        self.logs[timestamp]["choice_num"] = choice_num
+        self.logs[timestamp]["topic"] = topic
+
+        ## search related documents ##
+        self.docs, docs_len, docs_token = akasha.search.get_docs(
+            self.db,
+            self.embeddings_obj,
+            topic,
+            99,
+            self.threshold,
+            self.language,
+            self.search_type,
+            self.verbose,
+            self.model_obj,
+            999999,
+            self.logs[timestamp],
+        )
+
+        texts = [doc.page_content for doc in self.docs]
+        metadata = [doc.metadata for doc in self.docs]
+        print(texts)
+        doc_range = min(doc_range, len(texts))
+
+        progress = tqdm(total=question_num,
+                        desc=f"Create Q({self.question_type})")
+        regenerate_limit = question_num
+        ### random select a range of documents from the documents , and use llm model to generate a question and answer pair ###
+        for i in range(question_num):
+            progress.update(1)
+
+            random_index = akasha.helper.get_non_repeat_rand_int(
+                vis_doc_range,
+                len(texts) - doc_range, doc_range)
+
+            doc_text = "\n".join(texts[random_index:random_index + doc_range])
+            docs = [
+                Document(page_content=texts[k], metadata=metadata[k])
+                for k in range(random_index, random_index + doc_range)
+            ]
+
+            try:
+                q_prompt = akasha.prompts.format_create_question_prompt(
+                    doc_text, self.question_type, self.question_style, topic)
+
+                response = akasha.helper.call_model(self.model_obj, q_prompt)
+                response = akasha.helper.sim_to_trad(
+                    response
+                )  # transform simplified chinese to traditional chinese
+                if not self._process_response(response, doc_text, choice_num):
+                    raise Exception("Question Format Error")
+
+                self.doc_length += akasha.helper.get_docs_length(
+                    self.language, docs)
+                self.doc_tokens += self.model_obj.get_num_tokens(doc_text)
+                self.docs.extend(docs)
+
+            except:
+                if regenerate_limit > 0:
+                    regenerate_limit -= 1
+                    i -= 1
+                    progress.update(-1)
+                    print(
+                        "Question Format Error while generating questions. Regenerate\n"
+                    )
+                    continue
+                else:
+                    print(
+                        "Question Format Error while generating questions. Stop\n"
+                    )
+                    break
+
+            new_table = akasha.format.handle_table(self.question[-1], docs,
+                                                   self.answer[-1])
+            for key in new_table:
+                if key not in table:
+                    table[key] = []
+                table[key].append(new_table[key])
+
+        progress.close()  # end running llm progress bar
+
+        end_time = time.time()
+
+        ### record logs ###
+        if self.record_exp != "":
+            params = akasha.format.handle_params(
+                self.model,
+                self.embeddings,
+                self.chunk_size,
+                self.search_type_str,
+                self.topK,
+                self.threshold,
+                self.language,
+            )
+            metrics = akasha.format.handle_metrics(self.doc_length,
+                                                   end_time - start_time,
+                                                   self.doc_tokens)
+            params["doc_range"] = doc_range
+            akasha.aiido_upload(self.record_exp, params, metrics, table)
+
+        self._add_result_log(timestamp, end_time - start_time)
+
+        self._save_questionset(timestamp, output_file_path)
+
+        return self.question, self.answer
+
 
 ### sub func###
-def check_sum_type(question_type: str, question_style: str) -> bool:
+def check_sum_type(question_type: str,
+                   question_style: str,
+                   func: str = "auto") -> bool:
     ## check question_type and question_style, summary can not be used in single_choice question_type ##
+    if func != "auto" and question_type.lower() in [
+            'compare', 'comparison', 'comparisons', '比較', 'compared'
+    ]:
+        print("compare can not be used in related_questionset\n\n")
+        return True
     if question_type.lower() in [
             "summary", "sum", "summarization", "summarize", "summaries", "摘要"
     ] and question_style.lower() == "single_choice":
-        print("summary can not be used in single_choice question_type")
+        print("summary can not be used in single_choice question_type\n\n")
 
         return True
 
     return False
 
 
 def check_essay_system_prompt(question_style: str, language: str,
```

### Comparing `akasha-terminal-0.8.8/akasha/eval/scores.py` & `akasha-terminal-0.8.9/akasha/eval/scores.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/format.py` & `akasha-terminal-0.8.9/akasha/format.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/helper.py` & `akasha-terminal-0.8.9/akasha/helper.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/interface/cot_page.py` & `akasha-terminal-0.8.9/akasha/interface/cot_page.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/interface/res_page.py` & `akasha-terminal-0.8.9/akasha/interface/res_page.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/interface/setting.py` & `akasha-terminal-0.8.9/akasha/interface/setting.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/interface/sum_page.py` & `akasha-terminal-0.8.9/akasha/interface/sum_page.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/interface/upload_file.py` & `akasha-terminal-0.8.9/akasha/interface/upload_file.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/models/hf.py` & `akasha-terminal-0.8.9/akasha/models/hf.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/models/llama2.py` & `akasha-terminal-0.8.9/akasha/models/llama2.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/prompts.py` & `akasha-terminal-0.8.9/akasha/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,16 @@
                 st_cor + correct_ans + end_cor + "\n\n")
 
     return q_prompt
 
 
 def format_create_question_prompt(doc_text: str,
                                   question_type: str = "fact",
-                                  question_style: str = "essay") -> str:
+                                  question_style: str = "essay",
+                                  topic: str = "") -> str:
     """prompts for auto generate question from document
 
     Args:
         **doc_text (str)**: texts from documents\n
         **question_type (str)**: question type, can be "single choice", "essay"\n
 
     Returns:
@@ -146,50 +147,55 @@
     question_style = question_style.lower()
     if question_style not in [
             "essay", "問答", "essay question", "essay_question"
     ]:
         qt = "少於100字的"
 
     if question_type in ["fact", "facts", "factoid", "factoids", "事實"]:
-        q_prompt = fact_question_prompt(qt)
+        q_prompt = fact_question_prompt(qt, topic)
     elif question_type in [
             "summary", "sum", "summarization", "summarize", "summaries", "摘要"
     ]:
         q_prompt = summary_question_prompt(qt)
     elif question_type in ["irre", "irrelevant", "irrelevance", "無關"]:
-        q_prompt = irre_question_prompt(qt)
+        q_prompt = irre_question_prompt(qt, topic)
 
     # end_prompt = "<End Document>\n"
     end_prompt = "<結束文件>\n"
     # generate question prompt = generate_question_prompt(Document)
     q_prompt = q_prompt + doc_text + end_prompt
 
     return q_prompt
 
 
-def fact_question_prompt(qt: str = "") -> str:
+def fact_question_prompt(qt: str = "", topic: str = "") -> str:
     """prompt for generate fact question"""
 
-    fact_prompt = f"人類：您是一位教師，正在為測驗準備問題。\n請基於文件只生成一個問題和一個{qt}答案，問題應該詳細並且明確基於文件中的訊息，但不要使用\'根據文件中的訊息\'等詞語取代想詢問的問題內容。"
+    if topic != "":
+        topic = f"相關{topic}的"
+
+    fact_prompt = f"人類：您是一位教師，正在為測驗準備問題。\n請基於文件只生成一個{topic}問題和一個{qt}答案，問題應該詳細並且明確基於文件中的訊息，但不要使用\'根據文件中的訊息\'等詞語取代想詢問的問題內容。"
     format_prompt = "\n\n示例格式：\n<開始文件>\n...\n<結束文件>\n問題：問題在這里\n答案：答案在這里\n\n。開始吧！"
     return (sys_s + fact_prompt + format_prompt + sys_e + "<開始文件>\n")
 
 
 def summary_question_prompt(qt: str = "") -> str:
     """prompt for generate summary question"""
 
     sum_prompt = "人類： 請根據以下文件進行摘要，並將摘要放在 \"答案\"後面."
     format_prompt = "\n\n示例格式：\n<開始文件>\n...\n<結束文件>\n答案：摘要在這裡\n\n。開始吧！"
     return (sys_s + sum_prompt + format_prompt + sys_e + "<開始文件>\n")
 
 
-def irre_question_prompt(qt: str = "") -> str:
+def irre_question_prompt(qt: str = "", topic: str = "") -> str:
     """prompt for generate irrelevant question"""
+    if topic != "":
+        topic = f"和{topic}"
 
-    irre_prompt = f"人類：我想測試語言模型根據文件回答的可靠性。\n請只生成一個名詞或領域與文件內容相關，但文件內容中不存在的問題。這代表說，詢問任何人這個問題與文件，都無法回答該問題。問題應該詳細但不要使用\'根據文件中的訊息\'等詞語取代想詢問的問題內容。根據這個問題和文件，生成一個{qt}回答"
+    irre_prompt = f"人類：我想測試語言模型根據文件回答的可靠性。\n請只生成一個名詞或領域與文件內容{topic}相關，但文件內容中不存在的問題。這代表說，詢問任何人這個問題與文件，都無法回答該問題。問題應該詳細但不要使用\'根據文件中的訊息\'等詞語取代想詢問的問題內容。根據這個問題和文件，生成一個{qt}回答"
     format_prompt = "\n\n示例格式：\n<開始文件>\n...\n<結束文件>\n問題：問題在這里\n答案：答案在這里\n\n。開始吧！"
     return (sys_s + irre_prompt + format_prompt + sys_e + "<開始文件>\n")
 
 
 def compare_question_prompt(question_style: str, topic: str, nouns: str,
                             used_texts: str):
     """prompt for generate compare question"""
@@ -335,21 +341,47 @@
         ]:
             self.type = "str"
 
     def __str__(self):
         return f"\t{self.name}: {self.type}  // {self.description}"
 
 
+def XML_formatter(schemas: Union[list, OutputSchema]):
+    """generate prompt for generate XML format, input list of OutputSchema, which include every key and value you want to generate in JSON format"""
+
+    if isinstance(schemas, OutputSchema):
+        schemas = [schemas]
+
+    schema_str = "\n".join([sche.__str__() for sche in schemas])
+    XML_FORMAT_INSTRUCTIONS = f"""The output should be formatted as a XML file.
+    1. Output should conform to the tags below. 
+    2. If tags are not given, make them on your own.
+    3. Remember to always open and close all the tags.
+
+    As an example, for the tags ["foo", "bar", "baz"]:
+    1. String "<foo>\n   <bar>\n      <baz></baz>\n   </bar>\n</foo>" is a well-formatted instance of the schema. 
+    2. String "<foo>\n   <bar>\n   </foo>" is a badly-formatted instance.
+    3. String "<foo>\n   <tag>\n   </tag>\n</foo>" is a badly-formatted instance.
+
+    Here are the output tags:
+    ```
+    {schema_str}
+    ```"""
+
+    return XML_FORMAT_INSTRUCTIONS
+
+
 def JSON_formatter(schemas: Union[list, OutputSchema]):
     """generate prompt for generate JSON format, input list of OutputSchema, which include every key and value you want to generate in JSON format"""
 
     if isinstance(schemas, OutputSchema):
         schemas = [schemas]
 
     schema_str = "\n".join([sche.__str__() for sche in schemas])
+
     format_instruct = f"""The output should be formatted as a JSON instance that conforms to the JSON schema below:
     {{
     {schema_str}
     }}\n
     """
     return format_instruct
 
@@ -375,7 +407,11 @@
 
     format_instruct = f"""The output should be formatted as a JSON instance that conforms to the JSON schema below:
     {{
     {schema_str}
     }}\n
     """
     return format_instruct
+
+
+from langchain.output_parsers import ResponseSchema, StructuredOutputParser
+from langchain.output_parsers import XMLOutputParser
```

### Comparing `akasha-terminal-0.8.8/akasha/search.py` & `akasha-terminal-0.8.9/akasha/search.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/summary/summary.py` & `akasha-terminal-0.8.9/akasha/summary/summary.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha/ui.py` & `akasha-terminal-0.8.9/akasha/ui.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/akasha_terminal.egg-info/PKG-INFO` & `akasha-terminal-0.8.9/akasha_terminal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: akasha-terminal
-Version: 0.8.8
+Version: 0.8.9
 Summary: document QA package using langchain and chromadb
 Home-page: https://github.com/iii-org/akasha
 Author: chih chuan chang
 Author-email: ccchang@iii.org.tw
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: License
 
 # akasha
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![pypi package : 0.8.8](https://img.shields.io/badge/pypi%20package-0.8.7-blue)](https://pypi.org/project/akasha-terminal/)
+[![pypi package : 0.8.9](https://img.shields.io/badge/pypi%20package-0.8.7-blue)](https://pypi.org/project/akasha-terminal/)
 [![python version : 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 ![GitLab CI](https://img.shields.io/badge/gitlab%20ci-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white)
 
 <br/>
 
 Akasha simplifies document-based Question Answering (QA) by harnessing the power of Large Language Models to accurately answer your queries while searching through your provided documents.
 
@@ -694,14 +694,35 @@
 
 eva.auto_create_questionset(doc_path="doc/mic/", question_num=10, output_file_path="questionset/mic_irre.txt")
 
 bert_score, rouge, llm_score = eva.auto_evaluation(questionset_path="questionset/mic_irre.txt", doc_path="doc/mic/", question_style = "essay", record_exp="exp_mic_auto_evaluation",topK=3,search_type="svm")
 
 ```
 
+<br/>
+<br/>
+
+
+## assign certain topic of questionset
+If you want to generate certain topic of question, you can use **create_topic_questionset** function, it will use the topic input to find related texts in the documents
+ and generate question set.
+
+
+```python
+
+import akasha.eval as eval
+
+eva = eval.Model_Eval(search_type='merge', question_type = "irrelevant", model="openai:gpt-3.5-turbo", record_exp="exp_mic_auto_questionset")
+
+eva.create_topic_questionset(doc_path="doc/mic/", topic= "工業4.0", question_num=3, output_file_path="questionset/mic_topic_irre.txt")
+
+bert_score, rouge, llm_score = eva.auto_evaluation(questionset_path="questionset/mic_topic_irre.txt", doc_path="doc/mic/", question_style = "essay", record_exp="exp_mic_auto_evaluation",topK=3,search_type="svm")
+
+```
+
 
 <br/>
 <br/>
 <br/>
 <br/>
```

### Comparing `akasha-terminal-0.8.8/akasha_terminal.egg-info/SOURCES.txt` & `akasha-terminal-0.8.9/akasha_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/cli/glue.py` & `akasha-terminal-0.8.9/cli/glue.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/setup.py` & `akasha-terminal-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 if platform.system() == "Windows":
     install_requires.append("opencc==1.1.1")
 else:
     install_requires.append('opencc==1.1.6')
 
 setup(
     name="akasha-terminal",
-    version="0.8.8",
+    version="0.8.9",
     description="document QA package using langchain and chromadb",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="chih chuan chang",
     url="https://github.com/iii-org/akasha",
     author_email="ccchang@iii.org.tw",
     install_requires=install_requires,
```

### Comparing `akasha-terminal-0.8.8/tests/test_akasha.py` & `akasha-terminal-0.8.9/tests/test_akasha.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/tests/test_eval.py` & `akasha-terminal-0.8.9/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `akasha-terminal-0.8.8/tests/test_summary.py` & `akasha-terminal-0.8.9/tests/test_summary.py`

 * *Files identical despite different names*

