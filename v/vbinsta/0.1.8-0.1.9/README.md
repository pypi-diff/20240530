# Comparing `tmp/vbinsta-0.1.8.tar.gz` & `tmp/vbinsta-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbinsta-0.1.8.tar", max compression
+gzip compressed data, was "vbinsta-0.1.9.tar", max compression
```

## Comparing `vbinsta-0.1.8.tar` & `vbinsta-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.8/README.md
--rw-r--r--   0        0        0      368 2024-05-26 09:16:08.297506 vbinsta-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.8/vbinsta/__init__.py
--rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.8/vbinsta/__main__.py
--rw-r--r--   0        0        0     1236 2024-05-25 15:57:02.621318 vbinsta-0.1.8/vbinsta/choice_option.py
--rw-r--r--   0        0        0     3587 2024-05-26 08:00:21.497913 vbinsta-0.1.8/vbinsta/function_gpt.py
--rw-r--r--   0        0        0     3390 2024-05-26 09:15:55.005376 vbinsta-0.1.8/vbinsta/functions.py
--rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.8/vbinsta/main.py
--rw-r--r--   0        0        0     4178 2024-05-25 17:25:25.115487 vbinsta-0.1.8/vbinsta/token_cost_calculations.py
--rw-r--r--   0        0        0     2400 2024-05-26 09:16:02.221404 vbinsta-0.1.8/vbinsta/upload.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.9/README.md
+-rw-r--r--   0        0        0      368 2024-05-28 07:36:46.707226 vbinsta-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.9/vbinsta/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.9/vbinsta/__main__.py
+-rw-r--r--   0        0        0     1236 2024-05-25 15:57:02.621318 vbinsta-0.1.9/vbinsta/choice_option.py
+-rw-r--r--   0        0        0     3587 2024-05-26 08:00:21.497913 vbinsta-0.1.9/vbinsta/function_gpt.py
+-rw-r--r--   0        0        0     3390 2024-05-28 07:07:00.901559 vbinsta-0.1.9/vbinsta/functions.py
+-rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.9/vbinsta/main.py
+-rw-r--r--   0        0        0     4178 2024-05-25 17:25:25.115487 vbinsta-0.1.9/vbinsta/token_cost_calculations.py
+-rw-r--r--   0        0        0     2569 2024-05-28 07:36:50.491850 vbinsta-0.1.9/vbinsta/upload.py
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.9/PKG-INFO
```

### Comparing `vbinsta-0.1.8/vbinsta/choice_option.py` & `vbinsta-0.1.9/vbinsta/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.8/vbinsta/function_gpt.py` & `vbinsta-0.1.9/vbinsta/function_gpt.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.8/vbinsta/functions.py` & `vbinsta-0.1.9/vbinsta/functions.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.8/vbinsta/token_cost_calculations.py` & `vbinsta-0.1.9/vbinsta/token_cost_calculations.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.8/vbinsta/upload.py` & `vbinsta-0.1.9/vbinsta/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 from instagrapi import Client
 from rich.console import Console
 import os
 from .functions import login, upload_single_image, upload_carousel
 from .function_gpt import process_images
 from .choice_option import ChoiceOption
-from .functions import resize_images
+# from .functions import resize_images
 
 
 USERNAME = os.getenv('INSTA_USERNAME')
 PASSWORD = os.getenv('INSTA_PASSWORD')
 
 SESSION_FILE = os.path.expanduser("~/.vbinsta_session.json")
 
@@ -25,14 +25,15 @@
 )
 @click.option(
     "-p",
     "--prompt",
     cls=ChoiceOption,
     type=click.Choice(
         [
+            "Analyse this image it contains a physics problem, describe the problem and discuss the solution approach, in caption format for insta in simple text, don't format for web page",
             "Analyse this image and write an instagram caption with few hashtags, keep it under 1500 characters and conceptual.",
             "prompt",
         ],
         case_sensitive=False),
     prompt=True,
     default=1,
     show_default=True,
@@ -63,15 +64,15 @@
         print(f"An error occurred: {e}")
         return
 
     if prompt == "prompt":
         prompt = click.prompt("Enter the prompt: ")
 
     caption = process_images(
-        resize_images(image, (800, 800)),
+        image[0],
         prompt,
         model,
         os.getenv('OPENAI_API_KEY'),
         1500
     )
     # Verify if the login was successful
     if client.user_id:
```

