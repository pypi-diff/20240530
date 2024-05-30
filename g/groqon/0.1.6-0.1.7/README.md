# Comparing `tmp/groqon-0.1.6.tar.gz` & `tmp/groqon-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqon-0.1.6.tar", max compression
+gzip compressed data, was "groqon-0.1.7.tar", max compression
```

## Comparing `groqon-0.1.6.tar` & `groqon-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,17 @@
--rw-r--r--   0        0        0     3396 2024-04-26 11:47:58.504342 groqon-0.1.6/README.md
--rw-r--r--   0        0        0      112 2024-04-25 19:21:55.434929 groqon-0.1.6/groqon/__init__.py
--rw-r--r--   0        0        0     2904 2024-05-21 09:51:27.256884 groqon-0.1.6/groqon/element_selectors.py
--rw-r--r--   0        0        0     8280 2024-05-21 09:51:27.257884 groqon-0.1.6/groqon/groq.py
--rw-r--r--   0        0        0      229 2024-05-21 09:51:27.257884 groqon-0.1.6/groqon/groq_config.py
--rw-r--r--   0        0        0     8048 2024-05-21 09:51:27.258884 groqon-0.1.6/groqon/groq_utils.py
--rw-r--r--   0        0        0      930 2024-05-21 09:51:27.258884 groqon-0.1.6/groqon/parsing.py
--rw-r--r--   0        0        0      446 2024-05-21 09:57:18.225062 groqon-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3800 1970-01-01 00:00:00.000000 groqon-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3492 2024-05-22 13:47:15.279707 groqon-0.1.7/README.md
+-rw-r--r--   0        0        0      270 2024-05-29 18:38:37.047706 groqon-0.1.7/groqon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:28.521416 groqon-0.1.7/groqon/async_api/__init__.py
+-rw-r--r--   0        0        0    21996 2024-05-30 07:01:41.156774 groqon-0.1.7/groqon/async_api/agroq.py
+-rw-r--r--   0        0        0     8365 2024-05-29 18:39:08.757118 groqon-0.1.7/groqon/async_api/agroq_utils.py
+-rw-r--r--   0        0        0       53 2024-05-22 13:13:35.662297 groqon-0.1.7/groqon/async_api/experimental/__init__.py
+-rw-r--r--   0        0        0     1275 2024-05-22 13:22:45.285100 groqon-0.1.7/groqon/async_api/experimental/mock_api.py
+-rw-r--r--   0        0        0     3419 2024-05-30 06:27:02.736663 groqon-0.1.7/groqon/element_selectors.py
+-rw-r--r--   0        0        0     1573 2024-05-29 18:38:37.094694 groqon-0.1.7/groqon/groq_config.py
+-rw-r--r--   0        0        0     1098 2024-05-29 18:38:37.068701 groqon-0.1.7/groqon/logger.py
+-rw-r--r--   0        0        0     2292 2024-05-29 18:38:37.118688 groqon-0.1.7/groqon/parsing.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:37.983678 groqon-0.1.7/groqon/sync_api/__init__.py
+-rw-r--r--   0        0        0     8887 2024-05-22 13:50:34.888728 groqon-0.1.7/groqon/sync_api/groq.py
+-rw-r--r--   0        0        0     6976 2024-05-22 17:23:19.949054 groqon-0.1.7/groqon/sync_api/groq_utils.py
+-rw-r--r--   0        0        0      154 2024-05-29 18:38:37.067701 groqon-0.1.7/groqon/utils.py
+-rw-r--r--   0        0        0      468 2024-05-29 18:40:49.831833 groqon-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3889 1970-01-01 00:00:00.000000 groqon-0.1.7/PKG-INFO
```

### Comparing `groqon-0.1.6/README.md` & `groqon-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,23 +70,24 @@
                         'what is the purpose of life?'\
                         'why everyone hates meg griffin?'
 
 options:
   -h, --help            show this help message and exit
   --model MODEL         Available models are gemma-7b llama3-70b llama3-8b mixtral-8x7b
   --cookie_file COOKIE_FILE
-  --headless            set true to not see the browser
+  --headless            set true to not see the browser, e.g --headless True/False
   --save_output         set true to save the groq output with its query name.json
   --output_dir OUTPUT_DIR
                         Path to save the output file. Defaults to current working directory.
+  --reset_cookies       Deletes the old cookies, need to login again
 ```
 
 ## TODO (Need Help)
 
-* [x] Set System Prompt
+* [ ] Set System Prompt
 * [ ] Keep updated
 * [ ] Add something
 * [ ] Use Better parser
 * [ ] Use color for better Visual / Rich text formatting
 * [ ] Add logger
 * [ ] Multiround chat
```

### Comparing `groqon-0.1.6/groqon/element_selectors.py` & `groqon-0.1.7/groqon/element_selectors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 CLEAR_CHAT_BUTTON = r"body > main > div > div.flex.flex-col.md\:flex-col.md\:relative.w-full.max-w-\[900px\].bg-background.z-10.gap-2.md\:gap-6 > div > button.inline-flex.items-center.justify-center.whitespace-nowrap.rounded-md.text-sm.font-medium.ring-offset-background.transition-colors.focus-visible\:outline-none.disabled\:pointer-events-none.disabled\:opacity-50.underline-offset-4.h-10.p-0.text-muted-foreground.dark\:text-\[\#BCBCBC\].hover\:text-primaryaccent.dark\:hover\:text-primaryaccent.hover\:no-underline"
-DROPDOWN_BUTTON = r"body > header > div.flex-1.flex.items-center.justify-center.md\:col-span-4.md\:col-start-2 > div > button.flex.h-10.w-full.items-center.justify-between.border.border-input.bg-background.py-2.text-sm.ring-offset-background.placeholder\:text-muted-foreground.focus\:outline-none.focus\:ring-ring.focus\:ring-offset-2.disabled\:cursor-not-allowed.disabled\:opacity-50.\[\&\>span\]\:line-clamp-1.ml-auto.max-w-\[160px\].sm\:max-w-\[190px\].rounded-none.border-none.overflow-hidden.px-2.sm\:px-3.focus\:ring-0"
+MODEL_DROPDOWN_SELECTOR = r"body > header > div.flex-1.flex.items-center.justify-center.md\:col-span-4.md\:col-start-2 > div > button"
 QUERY_SELECTOR = "div.break-words"
 RESPONSE_SELECTOR = "div.text-base"
 PROMPT_SETTER_SELETOR = r"body > header > div.flex-1.flex.items-center.justify-center.md\:col-span-4.md\:col-start-2 > div > button.flex.gap-1.items-center.ml-1.px-2.sm\:px-3"
 PROMPT_TEXTAREA_SELECTOR = r"#radix-\:r3\: > textarea"
 END_TEXT_SELECTOR = r"body > main > div > div.flex.flex-col.md\:flex-col.md\:relative.w-full.max-w-\[900px\].bg-background.z-10.gap-2.md\:gap-6 > div > button.block.lg\:hidden > div > div"
 QUERY_INPUT_SELECTOR = "#chat"
+CHAT_INPUT_SELECTOR = "#chat"
+
 QUERY_SUBMIT_SELECTOR = ".self-end"
 
 PROFILE_BUTTON_SELECTOR = r"#radix-\:r3\:"
-ADVANCED_SETTING_SELECTOR =r"#radix-\:rf\:"
+ADVANCED_SETTING_SELECTOR = r"#radix-\:rf\:"
 SYSTEM_PROMPT_BUTTON = r"button.py-1\.5:nth-child(1)"
 SYSTEM_PROMPT_TEXTAREA = r"textarea.w-full:nth-child(2)"
 PROMPT_SAVE_BUTTON_SELECTOR = r"html.__variable_b1da2a.__variable_aaf875.dark body.fixed.!inset-0.flex.flex-col.font-montserrat.selection:bg-selection.bg-background.text-foreground div#radix-:rl:.fixed.left-[50%].top-[50%].z-50.grid.max-w-xl.translate-x-[-50%].translate-y-[-50%].gap-4.border.bg-background.p-6.shadow-lg.duration-200.data-[state=open]:animate-in.data-[state=closed]:animate-out.data-[state=closed]:fade-out-0.data-[state=open]:fade-in-0.data-[state=closed]:zoom-out-95.data-[state=open]:zoom-in-95.data-[state=closed]:slide-out-to-left-1/2.data-[state=closed]:slide-out-to-top-[48%].data-[state=open]:slide-in-from-left-1/2.data-[state=open]:slide-in-from-top-[48%].sm:rounded-lg.w-full.h-full.md:max-w-[455px].md:h-auto div div.flex.items-center button.inline-flex.items-center.justify-center.whitespace-nowrap.rounded-md.text-sm.font-medium.ring-offset-background.transition-colors.focus-visible:outline-none.disabled:pointer-events-none.disabled:opacity-50.hover:bg-gray-600.dark:hover:bg-slate-200.h-10.px-4.py-2.ml-3.text-background.bg-foreground.dark:text-black.dark:bg-white"
+COPY_BUTTON_SELECTOR = r"body > main > div > div.grow.w-full.overflow-auto.mt-2.flex.flex-col.md\:flex-col > div.flex.flex-col.\[word-break\:break-word\].mb-6 > div.flex.flex-col.font-normal.text-base.border-l.border-mutedaccent.px-5 > div.flex.flex-row.align-center.items-center.gap-4.pt-4 > div:nth-child(1) > svg"
+MODEL_NAME_SELECTOR = r"body > header > div.flex-1.flex.items-center.justify-center.md\:col-span-4.md\:col-start-2 > div > button > p"
+
+SIGNIN_BUTTON_SELECTOR = r"body > footer > div.grid.grid-cols-3.items-end.pb-2 > div.flex.flex-col.items-start.px-6 > button.inline-flex.items-center.whitespace-nowrap.rounded-md.text-sm.font-medium.ring-offset-background.transition-colors.focus-visible\:outline-none.disabled\:pointer-events-none.disabled\:opacity-50.text-primary.underline-offset-4.h-10.justify-start.p-0.hover\:text-primaryaccent.hover\:no-underline"
```

### Comparing `groqon-0.1.6/groqon/groq.py` & `groqon-0.1.7/groqon/sync_api/groq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import argparse
 import json
 import os
 from contextlib import contextmanager
+from pathlib import Path
 
-from playwright.sync_api import Page, sync_playwright
 from playwright._impl._errors import TimeoutError
-from .groq_config import modelindex
+from playwright.sync_api import Page, sync_playwright
+
+from ..element_selectors import (
+    END_TEXT_SELECTOR,
+    QUERY_INPUT_SELECTOR,
+    QUERY_SUBMIT_SELECTOR,
+)
+from ..groq_config import modelindex, URL, GROQ_COOKIE_FILE
 from .groq_utils import (
     check_element_and_get_text,
     clear_chat,
     file_exists,
     get_content_text,
     get_cookie,
     get_query_text,
     save_cookie,
     select_model,
     set_system_prompt,
 )
-from pathlib import Path
-from .element_selectors import(
-    END_TEXT_SELECTOR,
-    QUERY_INPUT_SELECTOR,
-    QUERY_SUBMIT_SELECTOR
-)
 
 
-URL = "https://groq.com/"
-
 @contextmanager
 def groq_context(
-    cookie_file: str = "groq_cookie.json",
+    cookie_file: str = GROQ_COOKIE_FILE,
     model: str = "llama3-8b",
     headless: bool = False,
     system_prompt: str = None,
+    reset_cookies=False
 ) -> Page:
     """
     Context manager for creating a Groq context.
 
     Args:
         cookie_file (str, optional): The path to the cookie file. Defaults to 'groq_cookie.json'.
         model (str, optional): The model to use. Defaults to 'llama3-70b'.
@@ -47,14 +47,17 @@
         Page: The page object for interacting with the browser.
 
     Raises:
         None
     """
 
     url = URL
+    
+    if reset_cookies:
+        os.remove(GROQ_COOKIE_FILE)
 
     if file_exists(cookie_file):
         cookie = get_cookie(cookie_file)
     else:
         headless = False
         cookie = None
 
@@ -65,15 +68,15 @@
 
         if cookie:
             context.add_cookies(cookie)
             print("Cookie loaded!!!")
         else:
             print(
                 "Cookie not loaded!!!",
-                "You have 120 seconds to login to groq.com, Make it quick!!! HEADLESS is set to False",
+                "You have 120 seconds to login to groq.com, Make it quick!!! HEADLESS is set to False, just a one time thing.",
             )
 
         page.goto(url, timeout=60_000) #wait_until="networkidle")
 
         if not cookie:
             page.wait_for_timeout(1000 * 120)  # 120 sec to login
 
@@ -87,14 +90,15 @@
             set_system_prompt(page, system_prompt=system_prompt)
             
         try:
             yield page
         finally:
             # Save cookie
             save_cookie(context.cookies(), cookie_file)
+            page.close()
             browser.close()
             print("Browser closed!!!")
 
 
 def get_groq_response(
     page: Page, query: str, save_output: bool = False, save_dir: str = os.getcwd()
 ) -> dict:
@@ -152,21 +156,22 @@
             json.dump(output_dict, f)
 
     return output_dict
 
 
 def groq(
     query_list: list[str],
-    cookie_file: str = "groq_cookie.json",
+    cookie_file: str = GROQ_COOKIE_FILE,
     model: str = "llama3-70b",
     headless: bool = False,
     save_output: bool = True,
     save_dir: str = os.getcwd(),
     system_prompt: str = None,
     print_output=True,
+    reset_cookies=False
 ) -> list[dict]:
     """
     Executes a list of Groq queries and returns a list of dictionaries containing the query, response, and token/s value.
 
     Args:
         query_list (list[str]): A list of Groq queries to execute.
         cookie_file (str, optional): The path to the cookie file. Defaults to 'groq_cookie.json'.
@@ -185,28 +190,30 @@
         query_list = [query_list]
 
     with groq_context(
         cookie_file=cookie_file,
         model=model,
         headless=headless,
         system_prompt=system_prompt,
+        reset_cookies=reset_cookies
     ) as page:
         response_list = []
         for query in query_list:
             response = get_groq_response(
                 page, query, save_output=save_output, save_dir=save_dir
             )
             response_list.append(response)
 
             if print_output:
                 print("Query", ":", response.get("query", None))
                 print("Response", ":", response.get("response", None))
                 print("token/s", ":", response.get("token/s", None))
         return response_list
 
+                
 
 def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "queries",
         nargs="+",
         help="one or more quoted string like 'what is the purpose of life?' 'why everyone hates meg griffin?'",
@@ -215,43 +222,61 @@
         "--model",
         default="llama3-70b",
         help=f"Available models are {' '.join(modelindex.keys())}",
     )
     parser.add_argument(
         "--cookie_file",
         type=str,
-        default="groq_cookie.json",
+        default=GROQ_COOKIE_FILE,
         help="looks in current directory by default for groq_cookie.json. If not found, You will have to login when the browswer opens under 120 seconds. It's one time thing",
     )
     parser.add_argument(
         "--system_prompt",
         type=str,
         help="System prompt to be given to the llm model. Its like 'you are samuel l jackson as my assistant'. Default is None.",
     )
     parser.add_argument(
-        "--headless", action="store_true", help="set true to not see the browser"
+        "--headless", 
+        type=str,
+        default='True',
+        help="set true to not see the browser"
     )
     parser.add_argument(
         "--save_output",
         action="store_true",
         help="set true to save the groq output with its query name.json",
     )
     parser.add_argument(
         "--output_dir",
         default=os.getcwd(),
         help="Path to save the output file. Defaults to current working directory.",
     )
 
+    parser.add_argument(
+        "--reset_cookies",
+        action="store_true", 
+        help="deletes the old cookie , need to login again"    
+    )
+
     args = parser.parse_args()
+    def check_headless(x):
+        if x.lower().strip() == "true":
+            return True
+        else:
+            return False
+
 
+    headless = check_headless(args.headless)
+    
     groq(
         cookie_file=args.cookie_file,
         model=args.model,
-        headless=args.headless,
+        headless=headless,
         query_list=args.queries,
         save_output=args.save_output,
         save_dir=args.output_dir,
         system_prompt=args.system_prompt,
         print_output=True,
+        reset_cookie=args.reset_cookies
     )
```

### Comparing `groqon-0.1.6/groqon/groq_utils.py` & `groqon-0.1.7/groqon/sync_api/groq_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import json
 import re
 from html import unescape
 from pathlib import Path
+from tqdm import tqdm
+import time
 
 from playwright.sync_api import Page
 from typing import Any
-from .groq_config import modelindex
-
-from .element_selectors import(
+from ..groq_config import modelindex
+from ..parsing import extract_to_markdown
+from ..element_selectors import(
     CLEAR_CHAT_BUTTON, 
-    DROPDOWN_BUTTON, 
+    MODEL_DROPDOWN_SELECTOR, 
     QUERY_SELECTOR, 
     RESPONSE_SELECTOR, 
     PROMPT_SETTER_SELETOR, 
     SYSTEM_PROMPT_TEXTAREA, 
     PROMPT_SAVE_BUTTON_SELECTOR, 
     PROFILE_BUTTON_SELECTOR,
     ADVANCED_SETTING_SELECTOR,
@@ -65,15 +67,15 @@
     Description:
         This function clicks on the dropdown button on the page, finds the index of the model_choice
         in the modelindex list, and then presses the ArrowDown key that many times. Finally, it presses
         the Enter key to select the model. If an error occurs during the process, it prints an error message.
     """
     try:
         # dropdown_button
-        page.locator(DROPDOWN_BUTTON).click()
+        page.locator(MODEL_DROPDOWN_SELECTOR).click()
 
         downpress = list(modelindex.keys()).index(model_choice)
 
         for _ in range(downpress):
             page.keyboard.press("ArrowDown")
         page.keyboard.press("Enter")
 
@@ -220,47 +222,11 @@
     Returns:
         None
     """
     with open(filename, "w") as output:
         json.dump(cookie, output)
 
 
-def extract_to_markdown(html_source: str) -> str:
-    """
-    Extracts markdown content from the given HTML source.
-
-    Args:
-        html_source (str): The HTML source code from which to extract markdown content.
 
-    Returns:
-        str: The extracted markdown content from the HTML source.
-    """
-    output = []
-    in_table = False
-    code_block = []
-    for line in html_source.split("\n"):
-        line = line.strip()
-        if line.startswith("<pre>"):
-            
-            output.append("```\n")
-            code_block = []
-        elif line.startswith("</pre>"):
-            code_block.append(line.replace("</pre>", ""))
-            code = unescape("\n".join(code_block))
-            output.append(code + "\n")
-            output.append("```\n\n")
-            code_block = []
-        elif line.startswith("<table"):
-            table_lines = [line]
-            in_table = True
-        elif in_table and line.startswith("</table>"):
-            table_lines.append(line)
-            table = "\n".join(table_lines)
-            output.append(table + "\n\n")
-            in_table = False
-        elif in_table:
-            table_lines.append(line)
-        else:
-            text = re.sub(r"<[^>]+>", "", line)
-            if text:
-                output.append(text + "\n")
-    return "".join(output).strip().strip(r"\n")
+def show_progress_bar(seconds):
+    for _ in tqdm(range(seconds), unit='s', bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt} [{elapsed}<{remaining}]"):
+        time.sleep(1)
```

### Comparing `groqon-0.1.6/PKG-INFO` & `groqon-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: groqon
-Version: 0.1.6
+Version: 0.1.7
 Summary: Use Groq.com as llm
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: playwright (>=1.44.0,<2.0.0)
+Requires-Dist: playwright (==1.44.0)
 Description-Content-Type: text/markdown
 
 # GROQ without API : GroqOn
 
 This projects uses playwright to Access [GROQ](https://www.groq.com) using python
 
 ## Inspiration(Story)
@@ -83,23 +83,24 @@
                         'what is the purpose of life?'\
                         'why everyone hates meg griffin?'
 
 options:
   -h, --help            show this help message and exit
   --model MODEL         Available models are gemma-7b llama3-70b llama3-8b mixtral-8x7b
   --cookie_file COOKIE_FILE
-  --headless            set true to not see the browser
+  --headless            set true to not see the browser, e.g --headless True/False
   --save_output         set true to save the groq output with its query name.json
   --output_dir OUTPUT_DIR
                         Path to save the output file. Defaults to current working directory.
+  --reset_cookies       Deletes the old cookies, need to login again
 ```
 
 ## TODO (Need Help)
 
-* [x] Set System Prompt
+* [ ] Set System Prompt
 * [ ] Keep updated
 * [ ] Add something
 * [ ] Use Better parser
 * [ ] Use color for better Visual / Rich text formatting
 * [ ] Add logger
 * [ ] Multiround chat
```

