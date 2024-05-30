# Comparing `tmp/botshop-0.0.43.tar.gz` & `tmp/botshop-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botshop-0.0.43.tar", last modified: Fri Mar  8 22:02:23 2024, max compression
+gzip compressed data, was "botshop-0.0.44.tar", last modified: Thu May 30 21:32:45 2024, max compression
```

## Comparing `botshop-0.0.43.tar` & `botshop-0.0.44.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-03-08 22:02:23.091332 botshop-0.0.43/
--rw-r--r--   0 freddy.snijder   (501) staff       (20)    11357 2024-02-05 21:24:27.000000 botshop-0.0.43/LICENSE
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      643 2024-03-08 22:02:23.091153 botshop-0.0.43/PKG-INFO
--rw-r--r--   0 freddy.snijder   (501) staff       (20)       91 2024-02-05 21:24:27.000000 botshop-0.0.43/README.md
-drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-03-08 22:02:23.089457 botshop-0.0.43/botshop/
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      302 2024-02-05 21:24:27.000000 botshop-0.0.43/botshop/__init__.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)     3961 2024-02-11 00:39:09.000000 botshop-0.0.43/botshop/conversation_engine.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)     4474 2024-02-05 21:36:40.000000 botshop-0.0.43/botshop/io_processor.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)     1211 2024-02-05 21:24:27.000000 botshop-0.0.43/botshop/model_evaluator.py
-drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-03-08 22:02:23.090693 botshop-0.0.43/botshop/pytorch/
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      173 2024-02-05 21:24:27.000000 botshop-0.0.43/botshop/pytorch/__init__.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      312 2024-02-05 21:24:27.000000 botshop-0.0.43/botshop/pytorch/conversation_engine.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      212 2024-02-05 21:24:27.000000 botshop-0.0.43/botshop/pytorch/sample_and_rank.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)     1369 2024-02-10 23:03:36.000000 botshop-0.0.43/botshop/pytorch/utils.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)     1840 2024-02-05 21:24:27.000000 botshop-0.0.43/botshop/sample_and_rank.py
--rw-r--r--   0 freddy.snijder   (501) staff       (20)     9766 2024-03-08 22:00:15.000000 botshop-0.0.43/botshop/simple_bot.py
-drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-03-08 22:02:23.090971 botshop-0.0.43/botshop.egg-info/
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      643 2024-03-08 22:02:23.000000 botshop-0.0.43/botshop.egg-info/PKG-INFO
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      458 2024-03-08 22:02:23.000000 botshop-0.0.43/botshop.egg-info/SOURCES.txt
--rw-r--r--   0 freddy.snijder   (501) staff       (20)        1 2024-03-08 22:02:23.000000 botshop-0.0.43/botshop.egg-info/dependency_links.txt
--rw-r--r--   0 freddy.snijder   (501) staff       (20)       26 2024-03-08 22:02:23.000000 botshop-0.0.43/botshop.egg-info/requires.txt
--rw-r--r--   0 freddy.snijder   (501) staff       (20)        8 2024-03-08 22:02:23.000000 botshop-0.0.43/botshop.egg-info/top_level.txt
--rw-r--r--   0 freddy.snijder   (501) staff       (20)       38 2024-03-08 22:02:23.091368 botshop-0.0.43/setup.cfg
--rw-r--r--   0 freddy.snijder   (501) staff       (20)      813 2024-03-08 22:01:01.000000 botshop-0.0.43/setup.py
+drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-05-30 21:32:45.922978 botshop-0.0.44/
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)    11357 2024-02-05 21:24:27.000000 botshop-0.0.44/LICENSE
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      643 2024-05-30 21:32:45.922763 botshop-0.0.44/PKG-INFO
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)       91 2024-02-05 21:24:27.000000 botshop-0.0.44/README.md
+drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-05-30 21:32:45.920912 botshop-0.0.44/botshop/
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      302 2024-02-05 21:24:27.000000 botshop-0.0.44/botshop/__init__.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)     3961 2024-02-11 00:39:09.000000 botshop-0.0.44/botshop/conversation_engine.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)     4474 2024-02-05 21:36:40.000000 botshop-0.0.44/botshop/io_processor.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)     1211 2024-02-05 21:24:27.000000 botshop-0.0.44/botshop/model_evaluator.py
+drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-05-30 21:32:45.922182 botshop-0.0.44/botshop/pytorch/
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      173 2024-02-05 21:24:27.000000 botshop-0.0.44/botshop/pytorch/__init__.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      312 2024-02-05 21:24:27.000000 botshop-0.0.44/botshop/pytorch/conversation_engine.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      212 2024-02-05 21:24:27.000000 botshop-0.0.44/botshop/pytorch/sample_and_rank.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)     1369 2024-02-10 23:03:36.000000 botshop-0.0.44/botshop/pytorch/utils.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)     1840 2024-02-05 21:24:27.000000 botshop-0.0.44/botshop/sample_and_rank.py
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)     9969 2024-05-30 21:29:04.000000 botshop-0.0.44/botshop/simple_bot.py
+drwxr-xr-x   0 freddy.snijder   (501) staff       (20)        0 2024-05-30 21:32:45.922473 botshop-0.0.44/botshop.egg-info/
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      643 2024-05-30 21:32:45.000000 botshop-0.0.44/botshop.egg-info/PKG-INFO
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      458 2024-05-30 21:32:45.000000 botshop-0.0.44/botshop.egg-info/SOURCES.txt
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)        1 2024-05-30 21:32:45.000000 botshop-0.0.44/botshop.egg-info/dependency_links.txt
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)       26 2024-05-30 21:32:45.000000 botshop-0.0.44/botshop.egg-info/requires.txt
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)        8 2024-05-30 21:32:45.000000 botshop-0.0.44/botshop.egg-info/top_level.txt
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)       38 2024-05-30 21:32:45.923017 botshop-0.0.44/setup.cfg
+-rw-r--r--   0 freddy.snijder   (501) staff       (20)      813 2024-05-30 21:29:24.000000 botshop-0.0.44/setup.py
```

### Comparing `botshop-0.0.43/LICENSE` & `botshop-0.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `botshop-0.0.43/PKG-INFO` & `botshop-0.0.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botshop
-Version: 0.0.43
+Version: 0.0.44
 Summary: Framework for chatbot model inference, optimized for neural conversation models.
 Home-page: https://github.com/nuhame/botshop
 Author: Freddy Snijder
 Author-email: botshop@visionscapers.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `botshop-0.0.43/botshop/conversation_engine.py` & `botshop-0.0.44/botshop/conversation_engine.py`

 * *Files identical despite different names*

### Comparing `botshop-0.0.43/botshop/io_processor.py` & `botshop-0.0.44/botshop/io_processor.py`

 * *Files identical despite different names*

### Comparing `botshop-0.0.43/botshop/model_evaluator.py` & `botshop-0.0.44/botshop/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `botshop-0.0.43/botshop/pytorch/utils.py` & `botshop-0.0.44/botshop/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `botshop-0.0.43/botshop/sample_and_rank.py` & `botshop-0.0.44/botshop/sample_and_rank.py`

 * *Files identical despite different names*

### Comparing `botshop-0.0.43/botshop/simple_bot.py` & `botshop-0.0.44/botshop/simple_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,23 +160,28 @@
         bot_chat = None
         other_outputs = None
         if system_message is None:  # No command executed
             self._chats.append(user_chat)
             self._is_user.append(True)
             self._actor_name.append(user_name)
 
+            generation_exception = None
             try:
                 bot_chat, scores, other_outputs = self._respond()
             except UnableToGenerateValidResponse as e:
                 system_message = f"Bot {self._bot_name} was unable to generate a valid response. " \
                                  f"Your chat is not recorded."
+                generation_exception = e
             except Exception as e:
                 system_message = f"An unexpected exception occurred, bot {self._bot_name} was " \
                                  f"unable to generate a response. Your chat is not recorded."
-                log_exception(self._log, "system_message", e)
+                generation_exception = e
+
+            if generation_exception is not None:
+                log_exception(self._log, "Response generation failed", generation_exception)
 
             if system_message is None:  # No exception occurred
                 if self._conversation_start:
                     self._conversation_start = False
 
                 self._chats.append(bot_chat)
                 self._is_user.append(False)
```

### Comparing `botshop-0.0.43/botshop.egg-info/PKG-INFO` & `botshop-0.0.44/botshop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botshop
-Version: 0.0.43
+Version: 0.0.44
 Summary: Framework for chatbot model inference, optimized for neural conversation models.
 Home-page: https://github.com/nuhame/botshop
 Author: Freddy Snijder
 Author-email: botshop@visionscapers.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `botshop-0.0.43/setup.py` & `botshop-0.0.44/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="botshop",
-    version="0.0.43",
+    version="0.0.44",
     author="Freddy Snijder",
     author_email="botshop@visionscapers.com",
     description="Framework for chatbot model inference, optimized for neural conversation models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nuhame/botshop",
     packages=setuptools.find_packages(),
```

