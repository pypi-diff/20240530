# Comparing `tmp/athina_logger-1.2.4.tar.gz` & `tmp/athina_logger-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina_logger-1.2.4.tar", max compression
+gzip compressed data, was "athina_logger-1.2.5.tar", max compression
```

## Comparing `athina_logger-1.2.4.tar` & `athina_logger-1.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.2.4/README.md
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.2.4/athina_logger/__init__.py
--rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.2.4/athina_logger/api_key.py
--rw-r--r--   0        0        0      626 2024-04-06 02:19:19.299377 athina_logger-1.2.4/athina_logger/athina_meta.py
--rw-r--r--   0        0        0      346 2024-04-11 21:50:15.997677 athina_logger-1.2.4/athina_logger/constants.py
--rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.2.4/athina_logger/exception/custom_exception.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.2.4/athina_logger/feedback/__init__.py
--rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.2.4/athina_logger/feedback/user_feedback.py
--rw-r--r--   0        0        0     4235 2024-04-06 02:19:19.299809 athina_logger-1.2.4/athina_logger/inference_logger.py
--rw-r--r--   0        0        0    14123 2024-04-19 09:54:02.373290 athina_logger-1.2.4/athina_logger/langchain_handler.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.2.4/athina_logger/log_stream_inference/__init__.py
--rw-r--r--   0        0        0     4943 2024-04-06 02:19:19.299987 athina_logger-1.2.4/athina_logger/log_stream_inference/log_stream_inference.py
--rw-r--r--   0        0        0     7678 2024-04-06 02:19:19.300143 athina_logger-1.2.4/athina_logger/log_stream_inference/openai_chat_completion_stream.py
--rw-r--r--   0        0        0     7004 2024-04-06 02:19:19.300276 athina_logger-1.2.4/athina_logger/log_stream_inference/openai_completion_stream.py
--rw-r--r--   0        0        0    10771 2024-04-06 02:19:19.300668 athina_logger-1.2.4/athina_logger/openai_wrapper.py
--rw-r--r--   0        0        0     1883 2024-03-31 23:05:11.799630 athina_logger-1.2.4/athina_logger/request_helper.py
--rw-r--r--   0        0        0        0 2024-03-31 22:30:00.376453 athina_logger-1.2.4/athina_logger/tracing/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 22:30:00.406928 athina_logger-1.2.4/athina_logger/tracing/callback/__init__.py
--rw-r--r--   0        0        0    22087 2024-04-22 12:30:48.413326 athina_logger-1.2.4/athina_logger/tracing/callback/langchain.py
--rw-r--r--   0        0        0      755 2024-03-31 22:30:00.403809 athina_logger-1.2.4/athina_logger/tracing/models.py
--rw-r--r--   0        0        0    14711 2024-04-22 12:30:48.413913 athina_logger-1.2.4/athina_logger/tracing/span.py
--rw-r--r--   0        0        0     7204 2024-04-22 12:30:48.414392 athina_logger-1.2.4/athina_logger/tracing/trace.py
--rw-r--r--   0        0        0      537 2024-04-22 12:30:48.414813 athina_logger-1.2.4/athina_logger/tracing/util.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.2.4/athina_logger/util/__init__.py
--rw-r--r--   0        0        0    10414 2024-03-31 22:30:00.357924 athina_logger-1.2.4/athina_logger/util/extract_model.py
--rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.2.4/athina_logger/util/token_count_helper.py
--rw-r--r--   0        0        0      465 2024-04-22 12:30:52.867104 athina_logger-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.2.5/athina_logger/__init__.py
+-rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.2.5/athina_logger/api_key.py
+-rw-r--r--   0        0        0      626 2024-04-06 02:19:19.299377 athina_logger-1.2.5/athina_logger/athina_meta.py
+-rw-r--r--   0        0        0      346 2024-05-30 19:03:58.790493 athina_logger-1.2.5/athina_logger/constants.py
+-rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.2.5/athina_logger/exception/custom_exception.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.2.5/athina_logger/feedback/__init__.py
+-rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.2.5/athina_logger/feedback/user_feedback.py
+-rw-r--r--   0        0        0     4235 2024-04-06 02:19:19.299809 athina_logger-1.2.5/athina_logger/inference_logger.py
+-rw-r--r--   0        0        0    14121 2024-05-30 19:12:42.495570 athina_logger-1.2.5/athina_logger/langchain_handler.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.2.5/athina_logger/log_stream_inference/__init__.py
+-rw-r--r--   0        0        0     4943 2024-04-06 02:19:19.299987 athina_logger-1.2.5/athina_logger/log_stream_inference/log_stream_inference.py
+-rw-r--r--   0        0        0     7678 2024-04-06 02:19:19.300143 athina_logger-1.2.5/athina_logger/log_stream_inference/openai_chat_completion_stream.py
+-rw-r--r--   0        0        0     7004 2024-04-06 02:19:19.300276 athina_logger-1.2.5/athina_logger/log_stream_inference/openai_completion_stream.py
+-rw-r--r--   0        0        0    10771 2024-04-06 02:19:19.300668 athina_logger-1.2.5/athina_logger/openai_wrapper.py
+-rw-r--r--   0        0        0     1883 2024-03-31 23:05:11.799630 athina_logger-1.2.5/athina_logger/request_helper.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.376453 athina_logger-1.2.5/athina_logger/tracing/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.406928 athina_logger-1.2.5/athina_logger/tracing/callback/__init__.py
+-rw-r--r--   0        0        0    22087 2024-04-22 12:30:48.413326 athina_logger-1.2.5/athina_logger/tracing/callback/langchain.py
+-rw-r--r--   0        0        0      755 2024-03-31 22:30:00.403809 athina_logger-1.2.5/athina_logger/tracing/models.py
+-rw-r--r--   0        0        0    14711 2024-04-22 12:30:48.413913 athina_logger-1.2.5/athina_logger/tracing/span.py
+-rw-r--r--   0        0        0     7204 2024-04-22 12:30:48.414392 athina_logger-1.2.5/athina_logger/tracing/trace.py
+-rw-r--r--   0        0        0      537 2024-04-22 12:30:48.414813 athina_logger-1.2.5/athina_logger/tracing/util.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.2.5/athina_logger/util/__init__.py
+-rw-r--r--   0        0        0    10414 2024-03-31 22:30:00.357924 athina_logger-1.2.5/athina_logger/util/extract_model.py
+-rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.2.5/athina_logger/util/token_count_helper.py
+-rw-r--r--   0        0        0      465 2024-05-30 19:12:42.495898 athina_logger-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.2.5/PKG-INFO
```

### Comparing `athina_logger-1.2.4/README.md` & `athina_logger-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/athina_meta.py` & `athina_logger-1.2.5/athina_logger/athina_meta.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/feedback/user_feedback.py` & `athina_logger-1.2.5/athina_logger/feedback/user_feedback.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/inference_logger.py` & `athina_logger-1.2.5/athina_logger/inference_logger.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/langchain_handler.py` & `athina_logger-1.2.5/athina_logger/langchain_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,18 +63,18 @@
         documents: Sequence[Document],
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
         try:
-            retrieved_documents_data = ''
+            retrieved_documents_data = []
             for document in documents:
                 page_content = document.page_content
-                retrieved_documents_data += page_content + '\n'
+                retrieved_documents_data.append(page_content)
             if self.global_context is None:
                 self.global_context = {}
             self.global_context['documents'] = retrieved_documents_data
         except Exception as e:
             exception_message = (
                 f"Error:\n"
                 f"service name: athina-logger\n"
```

### Comparing `athina_logger-1.2.4/athina_logger/log_stream_inference/log_stream_inference.py` & `athina_logger-1.2.5/athina_logger/log_stream_inference/log_stream_inference.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/log_stream_inference/openai_chat_completion_stream.py` & `athina_logger-1.2.5/athina_logger/log_stream_inference/openai_chat_completion_stream.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/log_stream_inference/openai_completion_stream.py` & `athina_logger-1.2.5/athina_logger/log_stream_inference/openai_completion_stream.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/openai_wrapper.py` & `athina_logger-1.2.5/athina_logger/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/request_helper.py` & `athina_logger-1.2.5/athina_logger/request_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/tracing/callback/langchain.py` & `athina_logger-1.2.5/athina_logger/tracing/callback/langchain.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/tracing/models.py` & `athina_logger-1.2.5/athina_logger/tracing/models.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/tracing/span.py` & `athina_logger-1.2.5/athina_logger/tracing/span.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/tracing/trace.py` & `athina_logger-1.2.5/athina_logger/tracing/trace.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/tracing/util.py` & `athina_logger-1.2.5/athina_logger/tracing/util.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/util/extract_model.py` & `athina_logger-1.2.5/athina_logger/util/extract_model.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/athina_logger/util/token_count_helper.py` & `athina_logger-1.2.5/athina_logger/util/token_count_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.4/PKG-INFO` & `athina_logger-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athina-logger
-Version: 1.2.4
+Version: 1.2.5
 Summary: 
 Author: Akshat Gupta
 Author-email: akshat@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

