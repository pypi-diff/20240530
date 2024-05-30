# Comparing `tmp/stance_llm-0.1.2.tar.gz` & `tmp/stance_llm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stance_llm-0.1.2.tar", max compression
+gzip compressed data, was "stance_llm-0.2.0.tar", max compression
```

## Comparing `stance_llm-0.1.2.tar` & `stance_llm-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1111 2024-05-21 09:34:20.112894 stance_llm-0.1.2/LICENSE
--rw-r--r--   0        0        0      893 2024-05-28 15:42:36.785870 stance_llm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      159 2024-05-28 15:33:30.070907 stance_llm-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-21 08:56:17.968717 stance_llm-0.1.2/src/stance_llm/__init__.py
--rw-r--r--   0        0        0    38960 2024-05-28 15:17:16.461482 stance_llm-0.1.2/src/stance_llm/base.py
--rw-r--r--   0        0        0    16415 2024-05-28 12:55:58.822898 stance_llm-0.1.2/src/stance_llm/process.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 stance_llm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-05-21 09:34:20.112894 stance_llm-0.2.0/LICENSE
+-rw-r--r--   0        0        0      879 2024-05-30 16:14:02.588214 stance_llm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13522 2024-05-30 16:14:02.588214 stance_llm-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 15:22:47.336745 stance_llm-0.2.0/src/stance_llm/__init__.py
+-rw-r--r--   0        0        0    38946 2024-05-30 16:01:03.647410 stance_llm-0.2.0/src/stance_llm/base.py
+-rw-r--r--   0        0        0    15654 2024-05-30 16:01:03.648434 stance_llm-0.2.0/src/stance_llm/process.py
+-rw-r--r--   0        0        0    14225 1970-01-01 00:00:00.000000 stance_llm-0.2.0/PKG-INFO
```

### Comparing `stance_llm-0.1.2/LICENSE` & `stance_llm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stance_llm-0.1.2/pyproject.toml` & `stance_llm-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "stance-llm"
-version = "0.1.2"
-description = "Classify stances of entities related to a statement in German text using large language models through guidance-llm"
+version = "0.2.0"
+description = "Classify stances of entities related to a statement in German text using large language models (LLMs)"
 authors = ["Mario Angst <mario.angst@uzh.ch>", "Viviane Walker <viviane.walker@uzh.ch>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/urban-sustainability-lab-zurich/stance-llm"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `stance_llm-0.1.2/src/stance_llm/base.py` & `stance_llm-0.2.0/src/stance_llm/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 from loguru import logger
 from typing_extensions import Self
 import re
 
-from guidance import models, gen, select, user, system, assistant, instruction
+from guidance import gen, select, user, assistant
 
 REGISTERED_LLM_CHAINS = {
     "sis": "summarize_irrelevant_stance",
     "s2is": "summarize_v2_irrelevant_stance",
     "s2": "summarize_v2",
     "is": "irrelevant_stance",
     "is2": "irrelevant_summarize_v2",
     "nise": "nested_irrelevant_summary_explicit",
-    "nis2e": "nested_irrelevant_summary_v2_explicit"
-    }
+    "nis2e": "nested_irrelevant_summary_v2_explicit",
+}
 
 ALLOWED_DUAL_LLM_CHAINS = ["is2"]
 
-CONSTRAINED_GRAMMAR_CHAINS = ["s2","is2"]
+CONSTRAINED_GRAMMAR_CHAINS = ["s2", "is2"]
 
 IRRELEVANCE_ANSWERS = {
-    "irrelevant": 'Bezieht keine Stellung',
-    "stance": 'Bezieht Stellung'
+    "irrelevant": "Bezieht keine Stellung",
+    "stance": "Bezieht Stellung",
 }
 IRRELEVANCE_ANSWERS2 = {
-    "irrelevant": 'Bezieht keine Haltung',
-    "stance": 'Bezieht eine Haltung'
+    "irrelevant": "Bezieht keine Haltung",
+    "stance": "Bezieht eine Haltung",
 }
 
-def construct_irrelevance_prompt(input_text,
-                                 entity,
-                                 statement):
+
+def construct_irrelevance_prompt(input_text, entity, statement):
     prompt = f"Analysiere den folgenden Text: {input_text}. Bezieht die Organisation {entity} Stellung zur folgenden Aussage: {statement}? Beziehe dich nur auf den Text. Antworte mit {IRRELEVANCE_ANSWERS['irrelevant']} oder {IRRELEVANCE_ANSWERS['stance']}"
-    return(prompt)
+    return prompt
+
+
+def construct_summary_prompt(input_text, entity):
+    prompt = f"Fasse die Position der Organisation {entity} im folgenden Text zusammen: \n {input_text}. Fasse dich kurz und starte deine Zusammenfassung mit: Die Organisation {entity}..."
+    return prompt
+
 
-def construct_summary_prompt(input_text,
-                             entity):
-    prompt = f'Fasse die Position der Organisation {entity} im folgenden Text zusammen: \n {input_text}. Fasse dich kurz und starte deine Zusammenfassung mit: Die Organisation {entity}...'
-    return(prompt)
-
-def construct_summary_statementspecific_prompt(input_text,
-                                               entity,
-                                               statement):
+def construct_summary_statementspecific_prompt(input_text, entity, statement):
     prompt = f'Fasse die Position der Organisation {entity} im folgenden Text in Bezug auf die Aussage "{statement}" zusammen: \n {input_text}. \n Fasse dich kurz und starte deine Zusammenfassung mit: Die Organisation {entity}...'
-    return(prompt)
+    return prompt
 
-def construct_general_stance_prompt(input_text,
-                                        entity):
+
+def construct_general_stance_prompt(input_text, entity):
     prompt = f"Analysiere den folgenden Text: {input_text}. Äussert die Organisation {entity} eine implizite oder explizite Haltung? Beziehe dich nur auf den Text. Antworte mit {IRRELEVANCE_ANSWERS2['irrelevant']} oder {IRRELEVANCE_ANSWERS2['stance']}"
-    return(prompt)
+    return prompt
+
 
-def construct_support_stance_prompt(input_text,
-                            entity,
-                            statement):
+def construct_support_stance_prompt(input_text, entity, statement):
     prompt = f"Analysiere den folgenden Text: {input_text}. Befürwortet die Organisation {entity} die Aussage: {statement}? Beziehe dich nur auf den Text. Antworte mit Ja oder Nein"
-    return(prompt)
+    return prompt
+
 
-def construct_opposition_stance_prompt(input_text,
-                            entity,
-                            statement):
+def construct_opposition_stance_prompt(input_text, entity, statement):
     prompt = f"Analysiere den folgenden Text: {input_text}. Lehnt die Organisation {entity} folgende die Aussage ab: {statement}? Beziehe dich nur auf den Text. Antworte mit Ja oder Nein"
-    return(prompt)
+    return prompt
+
 
 def get_registered_chains():
-    return(REGISTERED_LLM_CHAINS)
+    return REGISTERED_LLM_CHAINS
+
 
 def get_allowed_dual_llm_chains():
-    return(ALLOWED_DUAL_LLM_CHAINS)
+    return ALLOWED_DUAL_LLM_CHAINS
+
 
 class StanceClassification:
     """Class used for LLM-based classifications of stances by a specified entity in a text regarding a statement.
-    
+
     Attributes:
         entity (str): entity to classify stance of
         statement (str): statement to classify stance toward
         input_text (str): text to classify stance of entity in
-    
+
     Methods:
         # TODO
     """
 
-    def __init__(self,input_text,statement,entity):
+    def __init__(self, input_text, statement, entity):
         self.input_text = input_text
         self.statement = statement
         self.entity = entity
         self.stance = None
         self.meta = None
         self.masked_entity = entity
         self.masked_input_text = input_text
+
     def __str__(self):
-        return("The stance of entity {} towards the statement {} given text {} is {}".format(
-            self.entity,
-            self.statement,
-            self.input_text,
-            self.stance))
-    
-    def mask_entity(self, entity_mask:str)-> Self:
+        return "The stance of entity {} towards the statement {} given text {} is {}".format(
+            self.entity, self.statement, self.input_text, self.stance
+        )
+
+    def mask_entity(self, entity_mask: str) -> Self:
         """replaces the entity/actor within the entire prompt with a placeholder name like "Organisation X"
            Serves as a check for an actor bias
 
         Args:
             entity_mask (str): a string that will mask the original entity
         """
         self.masked_input_text = re.sub(self.entity, entity_mask, self.input_text)
         self.masked_entity = entity_mask
-        return(self)
+        return self
 
-    def summarize_irrelevant_stance_chain(self, llm, chat:bool,llm2=None, log=True) -> Self:
+    def summarize_irrelevant_stance_chain(
+        self, llm, chat: bool, llm2=None, log=True
+    ) -> Self:
         """prompt chain that:
            1. summarises text (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["summary"])
            2. classifies whether the detected actor has a stance in the summary related to the statement, or not (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["irrelevance"])
            3. if actor has a related stance: classify stance as opposition or support, not related stance: stance=irrelevant (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
 
         Args:
             self: StanceClassification class object, contains: entity, statement, input_text, stance
@@ -119,66 +119,77 @@
             log (bool, optional): To log or not. Defaults to True.
 
         Returns:
             StanceClassification class object with new class object attributes: meta and stance. The irrelevance, summary, and stance prompt texts are stored in a dictionary value at the key ["llms"] in a dictionary stored in the "meta" attribute of the StanceClassification object returned: e.g. meta["llms"]["irrelevance"].
         """
         if log:
             logger.info(f"Summarizing position of {self.entity}")
-        summary_prompt = construct_summary_prompt(input_text=self.masked_input_text,
-                                                  entity=self.masked_entity)
+        summary_prompt = construct_summary_prompt(
+            input_text=self.masked_input_text, entity=self.masked_entity
+        )
         if chat:
             with user():
                 summary = llm + summary_prompt
             with assistant():
                 summary += gen(name="summary", max_tokens=120)
-        if not chat: 
-                summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
+        if not chat:
+            summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
         if log:
-            logger.info(f"Basing classification on position summary: {summary['summary']}")
+            logger.info(
+                f"Basing classification on position summary: {summary['summary']}"
+            )
             logger.info("Checking irrelevance...")
-        irrelevance_prompt = construct_irrelevance_prompt(input_text=summary['summary'],
-                                                          entity=self.masked_entity,
-                                                          statement=self.statement)
+        irrelevance_prompt = construct_irrelevance_prompt(
+            input_text=summary["summary"],
+            entity=self.masked_entity,
+            statement=self.statement,
+        )
         if chat:
             with user():
                 irrelevance = llm + irrelevance_prompt
             with assistant():
-                irrelevance = irrelevance + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                irrelevance = irrelevance + select(
+                    list(IRRELEVANCE_ANSWERS.values()), name="answer"
+                )
         if not chat:
-            irrelevance = llm + irrelevance_prompt + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+            irrelevance = (
+                llm
+                + irrelevance_prompt
+                + select(list(IRRELEVANCE_ANSWERS.values()), name="answer")
+            )
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["irrelevant"]:
             self.stance = "irrelevant"
             stance = None
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["stance"]:
-            stance_prompt = construct_support_stance_prompt(input_text=summary['summary'],
-                                                    entity=self.masked_entity,
-                                                    statement=self.statement)
+            stance_prompt = construct_support_stance_prompt(
+                input_text=summary["summary"],
+                entity=self.masked_entity,
+                statement=self.statement,
+            )
             if chat:
                 with user():
                     stance = llm + stance_prompt
                 with assistant():
-                    stance = stance + select(['Ja','Nein'], name = 'answer')
+                    stance = stance + select(["Ja", "Nein"], name="answer")
             if not chat:
-                stance = llm + stance_prompt + select(['Ja','Nein'], name = 'answer')
+                stance = llm + stance_prompt + select(["Ja", "Nein"], name="answer")
             if stance["answer"] == "Ja":
                 self.stance = "support"
             if stance["answer"] == "Nein":
                 self.stance = "opposition"
         if log:
             logger.info(f"classified as {self.stance}")
         self.meta = {
-            "llms": {
-            "summary":summary,
-            "irrelevance":irrelevance,
-            "stance":stance
-            }
+            "llms": {"summary": summary, "irrelevance": irrelevance, "stance": stance}
         }
-        return(self)
-    
-    def summarize_v2_irrelevant_stance_chain(self, llm, chat:bool, llm2=None, log=True) -> Self:
+        return self
+
+    def summarize_v2_irrelevant_stance_chain(
+        self, llm, chat: bool, llm2=None, log=True
+    ) -> Self:
         """prompt chain that:
            1. summarises text in relation to the statement (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["summary"])
            2. classifies whether the detected actor has a stance in the summary related to the statement, or not (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["irrelevance"])
            3. if actor has a related stance: classify stance as opposition or support, if no related stance: stance=irrelevant (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
 
         Args:
             self: StanceClassification class object, contains: entity, statement, input_text, stance
@@ -189,67 +200,77 @@
 
         Returns:
             StanceClassification class object with new class object attributes: meta and stance. The irrelevance, summary, and stance prompt texts are stored in a dictionary value at the key ["llms"] in a dictionary stored in the "meta" attribute of the StanceClassification object returned: e.g. meta["llms"]["irrelevance"].
         """
 
         if log:
             logger.info(f"Summarizing position of {self.entity}")
-        summary_prompt = construct_summary_statementspecific_prompt(input_text=self.masked_input_text,
-                                                                    entity=self.masked_entity,
-                                                                    statement=self.statement)
+        summary_prompt = construct_summary_statementspecific_prompt(
+            input_text=self.masked_input_text,
+            entity=self.masked_entity,
+            statement=self.statement,
+        )
         if chat:
             with user():
                 summary = llm + summary_prompt
             with assistant():
                 summary += gen(name="summary", max_tokens=120)
-        if not chat: 
-                summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
+        if not chat:
+            summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
         if log:
-            logger.info(f"Basing classification on position summary: {summary['summary']}")
+            logger.info(
+                f"Basing classification on position summary: {summary['summary']}"
+            )
             logger.info("Checking irrelevance...")
-        irrelevance_prompt = construct_irrelevance_prompt(input_text=summary['summary'],
-                                                          entity=self.masked_entity,
-                                                          statement=self.statement)
+        irrelevance_prompt = construct_irrelevance_prompt(
+            input_text=summary["summary"],
+            entity=self.masked_entity,
+            statement=self.statement,
+        )
         if chat:
             with user():
                 irrelevance = llm + irrelevance_prompt
             with assistant():
-                irrelevance = irrelevance + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                irrelevance = irrelevance + select(
+                    list(IRRELEVANCE_ANSWERS.values()), name="answer"
+                )
         if not chat:
-            irrelevance = llm + irrelevance_prompt + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+            irrelevance = (
+                llm
+                + irrelevance_prompt
+                + select(list(IRRELEVANCE_ANSWERS.values()), name="answer")
+            )
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["irrelevant"]:
             self.stance = "irrelevant"
             stance = None
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["stance"]:
-            stance_prompt = construct_support_stance_prompt(input_text=summary['summary'],
-                                                    entity=self.masked_entity,
-                                                    statement=self.statement)
+            stance_prompt = construct_support_stance_prompt(
+                input_text=summary["summary"],
+                entity=self.masked_entity,
+                statement=self.statement,
+            )
             if chat:
                 with user():
                     stance = llm + stance_prompt
                 with assistant():
-                    stance = stance + select(['Ja','Nein'], name = 'answer')
+                    stance = stance + select(["Ja", "Nein"], name="answer")
             if not chat:
-                stance = llm + stance_prompt + select(['Ja','Nein'], name = 'answer')
+                stance = llm + stance_prompt + select(["Ja", "Nein"], name="answer")
             if stance["answer"] == "Ja":
                 self.stance = "support"
             if stance["answer"] == "Nein":
                 self.stance = "opposition"
         if log:
             logger.info(f"classified as {self.stance}")
         self.meta = {
-            "llms": {
-            "summary":summary,
-            "irrelevance":irrelevance,
-            "stance":stance
-            }
+            "llms": {"summary": summary, "irrelevance": irrelevance, "stance": stance}
         }
-        return(self)
-    
-    def summarize_v2_chain(self, llm, chat:bool, llm2=None, log=True)-> Self:
+        return self
+
+    def summarize_v2_chain(self, llm, chat: bool, llm2=None, log=True) -> Self:
         """prompt chain that:
            1. summarises text in relation to the statement (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["summary"])
            2. prompts llm directly to classify the detected actor's stance based on the summary, stance class labels to select from: irrelevant, opposition, support
 
         Args:
             self: StanceClassification class object, contains: entity, statement, input_text, stance
             llm: A guidance model backend from guidance.models
@@ -259,46 +280,69 @@
 
         Returns:
             StanceClassification class object with new class object attributes: meta and stance. The summary prompt text is stored in a dictionary value at the key ["llms"]["summary"] in a dictionary stored in the "meta" attribute of the StanceClassification object returned.
         """
 
         if log:
             logger.info(f"Summarizing position of {self.entity}")
-        summary_prompt = construct_summary_statementspecific_prompt(input_text=self.masked_input_text,
-                                                                    entity=self.masked_entity,
-                                                                    statement=self.statement)
+        summary_prompt = construct_summary_statementspecific_prompt(
+            input_text=self.masked_input_text,
+            entity=self.masked_entity,
+            statement=self.statement,
+        )
         if chat:
             with user():
                 summary = llm + summary_prompt
             with assistant():
-                summary += f"Die Organisation {self.masked_entity} " + select(["drückt keine Haltung aus dazu, dass",
-                                                                        "unterstützt, dass",
-                                                                        "lehnt ab, dass"], name="stance") + gen(name="summary", max_tokens=80)
-        if not chat: 
-                summary = llm + summary_prompt + f"Die Organisation {self.masked_entity} " + select(["drückt keine Haltung aus dazu, dass",
-                                                            "unterstützt, dass",
-                                                            "lehnt ab, dass"], 
-                                                            name="stance") + gen(name="summary", max_tokens=80)
-        if log:
-            logger.info(f"Basing classification on position summary: {self.entity} {summary['stance']} {summary['summary']}")
+                summary += (
+                    f"Die Organisation {self.masked_entity} "
+                    + select(
+                        [
+                            "drückt keine Haltung aus dazu, dass",
+                            "unterstützt, dass",
+                            "lehnt ab, dass",
+                        ],
+                        name="stance",
+                    )
+                    + gen(name="summary", max_tokens=80)
+                )
+        if not chat:
+            summary = (
+                llm
+                + summary_prompt
+                + f"Die Organisation {self.masked_entity} "
+                + select(
+                    [
+                        "drückt keine Haltung aus dazu, dass",
+                        "unterstützt, dass",
+                        "lehnt ab, dass",
+                    ],
+                    name="stance",
+                )
+                + gen(name="summary", max_tokens=80)
+            )
+        if log:
+            logger.info(
+                f"Basing classification on position summary: {self.entity} {summary['stance']} {summary['summary']}"
+            )
         if summary["stance"] == "drückt keine Haltung aus dazu, dass":
             self.stance = "irrelevant"
         if summary["stance"] == "unterstützt, dass":
             self.stance = "support"
         if summary["stance"] == "lehnt ab, dass":
             self.stance = "opposition"
         if log:
             logger.info(f"classified as {self.stance}")
         self.meta = {
             "llms": {
-            "summary":summary,
+                "summary": summary,
             }
         }
-        return(self)
-    
+        return self
+
     def irrelevant_summarize_v2_chain(self, llm, chat, llm2=None, log=True) -> Self:
         """prompt chain that:
            1. classifies whether the detected actor has a stance in the text related to the statement, or not (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["irrelevance"])
            2. if actor has a related stance: continue with 3., if not: stance=irrelevance (saved as a new class attribute called stance)
            3. summarises text in relation to the statement and prompts in the same prompt text/step for the stance classification for either opposition or support
 
         Args:
@@ -312,64 +356,93 @@
             StanceClassification class object with new class object attributes: meta and stance. The irrelevance and summary prompt texts are stored in a dictionary value at the key ["llms"] in a dictionary stored in the "meta" attribute of the StanceClassification object returned: e.g. meta["llms"]["irrelevance"].
         """
         if llm2 is None:
             llm2 = llm
         if log:
             logger.info(f"Summarizing position of {self.entity}")
             logger.info("Checking irrelevance...")
-        irrelevance_prompt = construct_irrelevance_prompt(input_text=self.masked_input_text,
-                                                          entity=self.masked_entity,
-                                                          statement=self.statement)
+        irrelevance_prompt = construct_irrelevance_prompt(
+            input_text=self.masked_input_text,
+            entity=self.masked_entity,
+            statement=self.statement,
+        )
         if chat:
             with user():
                 irrelevance = llm + irrelevance_prompt
             with assistant():
-                irrelevance = irrelevance + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                irrelevance = irrelevance + select(
+                    list(IRRELEVANCE_ANSWERS.values()), name="answer"
+                )
         if not chat:
-            irrelevance = llm + irrelevance_prompt + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+            irrelevance = (
+                llm
+                + irrelevance_prompt
+                + select(list(IRRELEVANCE_ANSWERS.values()), name="answer")
+            )
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["irrelevant"]:
             self.stance = "irrelevant"
             summary = None
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["stance"]:
-            summary_prompt = construct_summary_statementspecific_prompt(input_text=self.masked_input_text,
-                                                                        entity=self.masked_entity,
-                                                                        statement=self.statement)
+            summary_prompt = construct_summary_statementspecific_prompt(
+                input_text=self.masked_input_text,
+                entity=self.masked_entity,
+                statement=self.statement,
+            )
             if chat:
                 with user():
                     summary = llm2 + summary_prompt
                 with assistant():
-                    summary += f"Die Organisation {self.masked_entity} " + select(["drückt keine Haltung aus dazu, dass",
-                                                                            "unterstützt, dass",
-                                                                            "lehnt ab, dass"], name="stance") + gen(name="summary", 
-                                                                                                                    max_tokens=80)
-            if not chat: 
-                summary = llm2 + summary_prompt + f"Die Organisation {self.masked_entity} " + select(["drückt keine Haltung aus dazu, dass",
-                                                                                             "unterstützt, dass",
-                                                                                             "lehnt ab, dass"],
-                                                                                             name="stance") + gen(name="summary", 
-                                                                                                                  max_tokens=80)
+                    summary += (
+                        f"Die Organisation {self.masked_entity} "
+                        + select(
+                            [
+                                "drückt keine Haltung aus dazu, dass",
+                                "unterstützt, dass",
+                                "lehnt ab, dass",
+                            ],
+                            name="stance",
+                        )
+                        + gen(name="summary", max_tokens=80)
+                    )
+            if not chat:
+                summary = (
+                    llm2
+                    + summary_prompt
+                    + f"Die Organisation {self.masked_entity} "
+                    + select(
+                        [
+                            "drückt keine Haltung aus dazu, dass",
+                            "unterstützt, dass",
+                            "lehnt ab, dass",
+                        ],
+                        name="stance",
+                    )
+                    + gen(name="summary", max_tokens=80)
+                )
             if log:
-                logger.info(f"Basing classification on position summary: {self.entity} {summary['stance']} {summary['summary']}")
+                logger.info(
+                    f"Basing classification on position summary: {self.entity} {summary['stance']} {summary['summary']}"
+                )
             if summary["stance"] == "drückt keine Haltung aus dazu, dass":
                 self.stance = "irrelevant"
             if summary["stance"] == "unterstützt, dass":
                 self.stance = "support"
             if summary["stance"] == "lehnt ab, dass":
                 self.stance = "opposition"
         if log:
             logger.info(f"classified as {self.stance}")
         self.meta = {
             "llms": {
-            "summary":summary,
-            "irrelevance":irrelevance,
+                "summary": summary,
+                "irrelevance": irrelevance,
             }
         }
-        return(self)
-    
-    def irrelevant_stance_chain(self, llm, chat:bool, llm2=None, log=True) -> Self:
+        return self
+
+    def irrelevant_stance_chain(self, llm, chat: bool, llm2=None, log=True) -> Self:
         """prompt chain that:
            1. classifies whether the detected actor has a stance in the text related to the statement, or not (the irrelevance prompt text is stored in a dictionary value at the key ["llms"]["irrelevance"] in the "meta" attribute)
            2. if actor has a related stance: classify stance as support or not support, if no related stance: stance=irrelevant (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
            3. if the stance is not support: the stance=opposition (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
 
         Args:
             self: StanceClassification class object, contains: entity, statement, input_text, stance
@@ -377,57 +450,66 @@
             chat (bool): whether llm it is a chat llm or not
             llm2 (optional): A second guidance model backend from guidance.models. Defaults to None.
             log (bool, optional): To log or not. Defaults to True.
 
         Returns:
             StanceClassification class object with new class object attributes: meta and stance. The irrelevance and stance prompt texts are stored in a dictionary value at the key ["llms"] in a dictionary stored in the "meta" attribute of the StanceClassification object returned, e.g. meta["llms"]["stance"]
         """
-        
+
         if log:
-            logger.info(f"Analyzing position of {self.entity} regarding statement {self.statement}")
+            logger.info(
+                f"Analyzing position of {self.entity} regarding statement {self.statement}"
+            )
             logger.info("Checking irrelevance...")
-        irrelevance_prompt = construct_irrelevance_prompt(input_text=self.masked_input_text,
-                                                          entity=self.masked_entity,
-                                                          statement=self.statement)
+        irrelevance_prompt = construct_irrelevance_prompt(
+            input_text=self.masked_input_text,
+            entity=self.masked_entity,
+            statement=self.statement,
+        )
         if chat:
             with user():
                 irrelevance = llm + irrelevance_prompt
             with assistant():
-                irrelevance = irrelevance + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                irrelevance = irrelevance + select(
+                    list(IRRELEVANCE_ANSWERS.values()), name="answer"
+                )
         if not chat:
-            irrelevance = llm + irrelevance_prompt + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+            irrelevance = (
+                llm
+                + irrelevance_prompt
+                + select(list(IRRELEVANCE_ANSWERS.values()), name="answer")
+            )
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["irrelevant"]:
             self.stance = "irrelevant"
             stance = None
         if irrelevance["answer"] == IRRELEVANCE_ANSWERS["stance"]:
-            stance_prompt = construct_support_stance_prompt(input_text=self.masked_input_text,
-                                                    entity=self.masked_entity,
-                                                    statement=self.statement)
+            stance_prompt = construct_support_stance_prompt(
+                input_text=self.masked_input_text,
+                entity=self.masked_entity,
+                statement=self.statement,
+            )
             if chat:
                 with user():
                     stance = llm + stance_prompt
                 with assistant():
-                    stance = stance + select(['Ja','Nein'], name = 'answer')
+                    stance = stance + select(["Ja", "Nein"], name="answer")
             if not chat:
-                stance = llm + stance_prompt + select(['Ja','Nein'], name = 'answer')
+                stance = llm + stance_prompt + select(["Ja", "Nein"], name="answer")
             if stance["answer"] == "Ja":
                 self.stance = "support"
             if stance["answer"] == "Nein":
                 self.stance = "opposition"
         if log:
             logger.info(f"classified as {self.stance}")
-        self.meta = {
-            "llms": {
-            "irrelevance":irrelevance,
-            "stance":stance
-            }
-        }
-        return(self)
-    
-    def nested_irrelevant_summary_explicit(self, llm, chat:bool, llm2=None, log=True)-> Self:
+        self.meta = {"llms": {"irrelevance": irrelevance, "stance": stance}}
+        return self
+
+    def nested_irrelevant_summary_explicit(
+        self, llm, chat: bool, llm2=None, log=True
+    ) -> Self:
         """prompt chain that:
            1. checks if there is a (general) stance of the detected actor in the text, if not: stance=irrelevant (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["irrelevance_general"])
            2. checks whether the stance of the actor has a relation to the statement, or not, if not: stance=irrelevant (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["irrelevance"])
            3. summarises text (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["summary"])
            4. prompts llm explicitly, if the stance in the summary text is in support of the statement, if not: continue with 4., if yes: stance=support if actor has a related stance: classify stance as opposition or support (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
            5. prompts llm explicitly, if the stance in the summary text is in opposition of the statement, if not: stance=irrelevant, if yes: stance=opposition (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
 
@@ -440,101 +522,129 @@
 
         Returns:
             StanceClassification class object with new class object attributes: meta and stance. The irrelevance, summary, and stance prompt texts are stored in a dictionary value at the key ["llms"] in a dictionary stored in the "meta" attribute of the StanceClassification object returned: e.g. meta["llms"]["irrelevance"].
         """
         if log:
             logger.info(f"Analyzing if {self.entity} has position")
             logger.info("Checking potential stance...")
-        general_prompt = construct_general_stance_prompt(input_text=self.masked_input_text,
-                                                          entity=self.masked_entity)
+        general_prompt = construct_general_stance_prompt(
+            input_text=self.masked_input_text, entity=self.masked_entity
+        )
         if chat:
             with user():
                 irrelevance_general = llm + general_prompt
             with assistant():
-                irrelevance_general = irrelevance_general + select(list(IRRELEVANCE_ANSWERS2.values()), name='answer_general')
+                irrelevance_general = irrelevance_general + select(
+                    list(IRRELEVANCE_ANSWERS2.values()), name="answer_general"
+                )
         if not chat:
-            irrelevance_general = llm + general_prompt + select(list(IRRELEVANCE_ANSWERS2.values()), name='answer_general')
+            irrelevance_general = (
+                llm
+                + general_prompt
+                + select(list(IRRELEVANCE_ANSWERS2.values()), name="answer_general")
+            )
         if irrelevance_general["answer_general"] == IRRELEVANCE_ANSWERS2["irrelevant"]:
             self.stance = "irrelevant"
             stance = None
             summary = None
         if irrelevance_general["answer_general"] == IRRELEVANCE_ANSWERS2["stance"]:
             if log:
-                logger.info(f"Analyzing if {self.entity} supports statement {self.statement}")
+                logger.info(
+                    f"Analyzing if {self.entity} supports statement {self.statement}"
+                )
                 logger.info("Checking irrelevance...")
-            irrelevance_prompt = construct_irrelevance_prompt(input_text=self.masked_input_text,
-                                                          entity=self.masked_entity,
-                                                          statement=self.statement)
+            irrelevance_prompt = construct_irrelevance_prompt(
+                input_text=self.masked_input_text,
+                entity=self.masked_entity,
+                statement=self.statement,
+            )
             if chat:
                 with user():
                     irrelevance = llm + irrelevance_prompt
                 with assistant():
-                    irrelevance = irrelevance + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                    irrelevance = irrelevance + select(
+                        list(IRRELEVANCE_ANSWERS.values()), name="answer"
+                    )
             if not chat:
-                irrelevance = llm + irrelevance_prompt + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                irrelevance = (
+                    llm
+                    + irrelevance_prompt
+                    + select(list(IRRELEVANCE_ANSWERS.values()), name="answer")
+                )
             if irrelevance["answer"] == IRRELEVANCE_ANSWERS["irrelevant"]:
                 self.stance = "irrelevant"
                 stance = None
                 summary = None
             if irrelevance["answer"] == IRRELEVANCE_ANSWERS["stance"]:
                 if log:
                     logger.info(f"Summarizing position of {self.entity}")
-                summary_prompt = construct_summary_prompt(input_text=self.masked_input_text,
-                                                        entity=self.masked_entity)
+                summary_prompt = construct_summary_prompt(
+                    input_text=self.masked_input_text, entity=self.masked_entity
+                )
                 if chat:
                     with user():
                         summary = llm + summary_prompt
                     with assistant():
                         summary += gen(name="summary", max_tokens=120)
-                if not chat: 
-                        summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
+                if not chat:
+                    summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
                 if log:
-                    logger.info(f"Basing classification on position summary: {summary['summary']}")
+                    logger.info(
+                        f"Basing classification on position summary: {summary['summary']}"
+                    )
                     logger.info("Checking irrelevance...")
 
-                stance_prompt = construct_support_stance_prompt(input_text=summary['summary'],
-                                                        entity=self.masked_entity,
-                                                        statement=self.statement)
+                stance_prompt = construct_support_stance_prompt(
+                    input_text=summary["summary"],
+                    entity=self.masked_entity,
+                    statement=self.statement,
+                )
                 if chat:
                     with user():
                         stance = llm + stance_prompt
                     with assistant():
-                        stance = stance + select(['Ja','Nein'], name = 'answer')
+                        stance = stance + select(["Ja", "Nein"], name="answer")
                 if not chat:
-                    stance = llm + stance_prompt + select(['Ja','Nein'], name = 'answer')
+                    stance = llm + stance_prompt + select(["Ja", "Nein"], name="answer")
                 if stance["answer"] == "Ja":
                     self.stance = "support"
                 if stance["answer"] == "Nein":
-                    stance_prompt = construct_opposition_stance_prompt(input_text=summary['summary'],
-                                                            entity=self.masked_entity,
-                                                            statement=self.statement)
+                    stance_prompt = construct_opposition_stance_prompt(
+                        input_text=summary["summary"],
+                        entity=self.masked_entity,
+                        statement=self.statement,
+                    )
                     if chat:
                         with user():
                             stance = llm + stance_prompt
                         with assistant():
-                            stance = stance + select(['Ja','Nein'], name = 'answer')
+                            stance = stance + select(["Ja", "Nein"], name="answer")
                     if not chat:
-                        stance = llm + stance_prompt + select(['Ja','Nein'], name = 'answer')
+                        stance = (
+                            llm + stance_prompt + select(["Ja", "Nein"], name="answer")
+                        )
                     if stance["answer"] == "Ja":
                         self.stance = "opposition"
                     if stance["answer"] == "Nein":
-                        self.stance = "irrelevant"  
+                        self.stance = "irrelevant"
         if log:
             logger.info(f"classified as {self.stance}")
         self.meta = {
             "llms": {
-            "irrelevance_general":irrelevance_general,
-            "irrelevance":irrelevance,
-            "summary":summary,
-            "stance":stance
+                "irrelevance_general": irrelevance_general,
+                "irrelevance": irrelevance,
+                "summary": summary,
+                "stance": stance,
             }
         }
-        return(self)
-    
-    def nested_irrelevant_summary_v2_explicit(self, llm, chat:bool, llm2=None, log=True)-> Self:
+        return self
+
+    def nested_irrelevant_summary_v2_explicit(
+        self, llm, chat: bool, llm2=None, log=True
+    ) -> Self:
         """prompt chain that:
            1. checks if there is a (general) stance of the detected actor in the text, if not: stance=irrelevant (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["irrelevance_general"])
            2. checks whether the stance of the actor has a relation to the statement, or not, if not: stance=irrelevant (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["irrelevance"])
            3. summarises text in relation to the statement (stored in the "meta" attribute of the StanceClassification class object in a dictionary value at the key ["llms"]["summary"])
            4. prompts llm explicitly, if the stance in the summary text is in support of the statement, if not: continue with 4., if yes: stance=support if actor has a related stance: classify stance as opposition or support (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
            5. prompts llm explicitly, if the stance in the summary text is in opposition of the statement, if not: stance=irrelevant, if yes: stance=opposition (saves stance prompt in the "meta" attribute at the dictionary key ["llms"]["stance"] and the predicted stance separately in the class attribute "stance")
 
@@ -547,92 +657,119 @@
 
         Returns:
             StanceClassification class object with new class object attributes: meta and stance. The irrelevance, summary, and stance prompt texts are stored in a dictionary value at the key ["llms"] in the "meta" attribute of the returned StanceClassification object: e.g. meta["llms"]["irrelevance"].
         """
         if log:
             logger.info(f"Analyzing if {self.entity} has position")
             logger.info("Checking potential stance...")
-        general_prompt = construct_general_stance_prompt(input_text=self.masked_input_text,
-                                                          entity=self.masked_entity)
+        general_prompt = construct_general_stance_prompt(
+            input_text=self.masked_input_text, entity=self.masked_entity
+        )
         if chat:
             with user():
                 irrelevance_general = llm + general_prompt
             with assistant():
-                irrelevance_general = irrelevance_general + select(list(IRRELEVANCE_ANSWERS2.values()), name='answer_general')
+                irrelevance_general = irrelevance_general + select(
+                    list(IRRELEVANCE_ANSWERS2.values()), name="answer_general"
+                )
         if not chat:
-            irrelevance_general = llm + general_prompt + select(list(IRRELEVANCE_ANSWERS2.values()), name='answer_general')
+            irrelevance_general = (
+                llm
+                + general_prompt
+                + select(list(IRRELEVANCE_ANSWERS2.values()), name="answer_general")
+            )
         if irrelevance_general["answer_general"] == IRRELEVANCE_ANSWERS2["irrelevant"]:
             self.stance = "irrelevant"
             stance = None
             summary = None
         if irrelevance_general["answer_general"] == IRRELEVANCE_ANSWERS2["stance"]:
             if log:
-                logger.info(f"Analyzing if {self.entity} supports statement {self.statement}")
+                logger.info(
+                    f"Analyzing if {self.entity} supports statement {self.statement}"
+                )
                 logger.info("Checking irrelevance...")
-            irrelevance_prompt = construct_irrelevance_prompt(input_text=self.masked_input_text,
-                                                          entity=self.masked_entity,
-                                                          statement=self.statement)
+            irrelevance_prompt = construct_irrelevance_prompt(
+                input_text=self.masked_input_text,
+                entity=self.masked_entity,
+                statement=self.statement,
+            )
             if chat:
                 with user():
                     irrelevance = llm + irrelevance_prompt
                 with assistant():
-                    irrelevance = irrelevance + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                    irrelevance = irrelevance + select(
+                        list(IRRELEVANCE_ANSWERS.values()), name="answer"
+                    )
             if not chat:
-                irrelevance = llm + irrelevance_prompt + select(list(IRRELEVANCE_ANSWERS.values()), name='answer')
+                irrelevance = (
+                    llm
+                    + irrelevance_prompt
+                    + select(list(IRRELEVANCE_ANSWERS.values()), name="answer")
+                )
             if irrelevance["answer"] == IRRELEVANCE_ANSWERS["irrelevant"]:
                 self.stance = "irrelevant"
                 stance = None
                 summary = None
             if irrelevance["answer"] == IRRELEVANCE_ANSWERS["stance"]:
                 if log:
                     logger.info(f"Summarizing position of {self.entity}")
-                summary_prompt = construct_summary_statementspecific_prompt(input_text=self.masked_input_text,
-                                                                            entity=self.masked_entity,
-                                                                            statement=self.statement)
+                summary_prompt = construct_summary_statementspecific_prompt(
+                    input_text=self.masked_input_text,
+                    entity=self.masked_entity,
+                    statement=self.statement,
+                )
                 if chat:
                     with user():
                         summary = llm + summary_prompt
                     with assistant():
                         summary += gen(name="summary", max_tokens=120)
-                if not chat: 
-                        summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
+                if not chat:
+                    summary = llm + summary_prompt + gen(name="summary", max_tokens=80)
                 if log:
-                    logger.info(f"Basing classification on position summary: {summary['summary']}")
+                    logger.info(
+                        f"Basing classification on position summary: {summary['summary']}"
+                    )
                     logger.info("Checking irrelevance...")
-                stance_prompt = construct_support_stance_prompt(input_text=summary['summary'],
-                                                        entity=self.masked_entity,
-                                                        statement=self.statement)
+                stance_prompt = construct_support_stance_prompt(
+                    input_text=summary["summary"],
+                    entity=self.masked_entity,
+                    statement=self.statement,
+                )
                 if chat:
                     with user():
                         stance = llm + stance_prompt
                     with assistant():
-                        stance = stance + select(['Ja','Nein'], name = 'answer')
+                        stance = stance + select(["Ja", "Nein"], name="answer")
                 if not chat:
-                    stance = llm + stance_prompt + select(['Ja','Nein'], name = 'answer')
+                    stance = llm + stance_prompt + select(["Ja", "Nein"], name="answer")
                 if stance["answer"] == "Ja":
                     self.stance = "support"
                 if stance["answer"] == "Nein":
-                    stance_prompt = construct_opposition_stance_prompt(input_text=summary['summary'],
-                                                            entity=self.masked_entity,
-                                                            statement=self.statement)
+                    stance_prompt = construct_opposition_stance_prompt(
+                        input_text=summary["summary"],
+                        entity=self.masked_entity,
+                        statement=self.statement,
+                    )
                     if chat:
                         with user():
                             stance = llm + stance_prompt
                         with assistant():
-                            stance = stance + select(['Ja','Nein'], name = 'answer')
+                            stance = stance + select(["Ja", "Nein"], name="answer")
                     if not chat:
-                        stance = llm + stance_prompt + select(['Ja','Nein'], name = 'answer')
+                        stance = (
+                            llm + stance_prompt + select(["Ja", "Nein"], name="answer")
+                        )
                     if stance["answer"] == "Ja":
                         self.stance = "opposition"
                     if stance["answer"] == "Nein":
-                        self.stance = "irrelevant"  
+                        self.stance = "irrelevant"
         if log:
             logger.info(f"classified as {self.stance}")
         self.meta = {
             "llms": {
-            "irrelevance_general":irrelevance_general,
-            "irrelevance":irrelevance,
-            "summary":summary,
-            "stance":stance
+                "irrelevance_general": irrelevance_general,
+                "irrelevance": irrelevance,
+                "summary": summary,
+                "stance": stance,
             }
         }
-        return(self)
+        return self
```

### Comparing `stance_llm-0.1.2/src/stance_llm/process.py` & `stance_llm-0.2.0/src/stance_llm/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,261 +5,293 @@
 
 import srsly
 from tqdm import tqdm
 from sklearn.metrics import classification_report
 from loguru import logger
 from wonderwords import RandomWord
 
-from stance_llm.base import StanceClassification, get_registered_chains, get_allowed_dual_llm_chains
+from stance_llm.base import (
+    StanceClassification,
+    get_registered_chains,
+    get_allowed_dual_llm_chains,
+)
 
-def detect_stance(eg:dict, llm, chain_label:str, llm2=None, chat=True, entity_mask=None)-> Self:
+
+def detect_stance(
+    eg: dict, llm, chain_label: str, llm2=None, chat=True, entity_mask=None
+) -> Self:
     """Detect stance of an entity in a dictionary input
 
-    Expects a dictionary item with a "text" key containing text to classify, a key "org_text" 
-    containing a string for the organizational entity to detect stance for and a key "statement"
+    Expects a dictionary item with a "text" key containing text to classify, a key "ent_text"
+    containing a string matching the entity to detect stance for and a key "statement"
     containing the statement to evaluate the stance against
 
     Args:
-        eg: A dictionary item with a "text" key containing text to classify and a "org_text" key containing a string for the organizational entity to predict stance for and a key "statement" containing the statement to evaluate the stance against
+        eg: A dictionary item with a "text" key containing text to classify and a "ent_text" key containing a string matching the organizational entity to predict stance for and a key "statement" containing the statement to evaluate the stance against
         llm: A guidance model backend from guidance.models
         chain_label: A implemented llm chain. See stance_llm.base.get_registered_chains for list
-    
+
     Returns:
         A StanceClassification class object with a stance and meta data
     """
     chain_labels = get_registered_chains()
     if chain_label not in chain_labels:
-        raise NameError('Chain label is not registered')
+        raise NameError("Chain label is not registered")
     if llm2 is not None:
         allowed_dual_llm_labels = get_allowed_dual_llm_chains()
         if chain_label not in allowed_dual_llm_labels:
-            raise NameError(f"Prompt chain is not set up for using two llm backends. Allowed are {allowed_dual_llm_labels}")
-    entity = eg["org_text"]
+            raise NameError(
+                f"Prompt chain is not set up for using two llm backends. Allowed are {allowed_dual_llm_labels}"
+            )
+    entity = eg["ent_text"]
     text = eg["text"]
     statement = eg["statement"]
-    task = StanceClassification(
-        input_text=text,
-        statement=statement,
-        entity=entity)
+    task = StanceClassification(input_text=text, statement=statement, entity=entity)
     if entity_mask is not None:
         task = task.mask_entity(entity_mask=entity_mask)
     if chain_label == "sis":
-        classification = task.summarize_irrelevant_stance_chain(llm=llm,chat = chat,llm2=llm2)
+        classification = task.summarize_irrelevant_stance_chain(
+            llm=llm, chat=chat, llm2=llm2
+        )
     if chain_label == "is":
-        classification = task.irrelevant_stance_chain(llm=llm,chat = chat,llm2=llm2)
+        classification = task.irrelevant_stance_chain(llm=llm, chat=chat, llm2=llm2)
     if chain_label == "nise":
-        classification = task.nested_irrelevant_summary_explicit(llm=llm,chat = chat,llm2=llm2)
+        classification = task.nested_irrelevant_summary_explicit(
+            llm=llm, chat=chat, llm2=llm2
+        )
     if chain_label == "s2is":
-        classification = task.summarize_v2_irrelevant_stance_chain(llm=llm,chat = chat,llm2=llm2)
+        classification = task.summarize_v2_irrelevant_stance_chain(
+            llm=llm, chat=chat, llm2=llm2
+        )
     if chain_label == "s2":
-        classification = task.summarize_v2_chain(llm=llm,chat = chat,llm2=llm2)
+        classification = task.summarize_v2_chain(llm=llm, chat=chat, llm2=llm2)
     if chain_label == "is2":
-        classification = task.irrelevant_summarize_v2_chain(llm=llm, chat=chat,llm2=llm2)
+        classification = task.irrelevant_summarize_v2_chain(
+            llm=llm, chat=chat, llm2=llm2
+        )
     if chain_label == "nis2e":
-        classification = task.nested_irrelevant_summary_v2_explicit(llm=llm,chat = chat,llm2=llm2)
-    return(classification)
+        classification = task.nested_irrelevant_summary_v2_explicit(
+            llm=llm, chat=chat, llm2=llm2
+        )
+    return classification
+
 
-def make_export_folder(export_folder:str,
-                          model_used,
-                          chain_used:str,
-                          run_alias:str)-> str:
+def make_export_folder(
+    export_folder: str, model_used, chain_used: str, run_alias: str
+) -> str:
     """creates folder of format <export_folder/<chain_used>/<model_used>/<current date>/<run_alias>
 
     Args:
         export_folder: directory to which all outputs are saved
         model_used: llm model name
         chain_used: prompt chain (short name)
         run_alias: name of the classification run to be saved
     """
     today = str(date.today())
-    folder_path = os.path.join(export_folder,chain_used,model_used,today,run_alias)
+    folder_path = os.path.join(export_folder, chain_used, model_used, today, run_alias)
     if os.path.exists(folder_path):
-        return(folder_path)
+        return folder_path
     else:
         logger.info(f"Creating folder at {folder_path}")
         os.makedirs(folder_path)
-        return(folder_path)
+        return folder_path
+
 
 def get_prompt_texts_from_meta(classification: StanceClassification) -> dict:
     """pulls prompt texts from meta data and returns it
 
     Args:
         classification: StanceClassification class object, with predictions ideally
 
     Returns:
         dict: gets all the meta information - created during the stance classification with a prompt chain - and returns it as a string (instead of a nested dictionary)
     """
     if "llms" not in classification.meta:
-        return({})
+        return {}
     else:
         components = {}
         chain_components = classification.meta["llms"]
         for component_key in chain_components.keys():
-            components[component_key] = {"prompt_text":str(chain_components[component_key])}
-    return(components)
+            components[component_key] = {
+                "prompt_text": str(chain_components[component_key])
+            }
+    return components
 
 
 def process(
     egs,
     llm,
-    export_folder:str,
-    model_used:str,
-    chain_used:str,
+    export_folder: str,
+    model_used: str,
+    chain_used: str,
     true_stance_key=None,
     wait_time=5,
     stream_out=True,
-    id_key = None,
+    id_key=None,
     chat=True,
     llm2=None,
-    entity_mask=None):
+    entity_mask=None,
+):
     r_word = RandomWord()
     run_alias = "-".join(r_word.random_words(2))
     logger.info(f"Starting run {run_alias}")
     """serves like a main function that
      - sends data together with constructed prompts to the llm (detect_stance())
      - assigns run alias (specific name) and saves classifications together with prompt texts (get_prompt_texts_from_meta() & save_classifications_jsonl())
     
      # TODO
     Args:
-        egs: list of examples to classify as dictionaries with at least keys "text","org_text","statement" (see detect_stance())
+        egs: list of examples to classify as dictionaries with at least keys "text","ent_text","statement" (see detect_stance())
         llm: A guidance model backend from guidance.models
         export_folder: Folder for evaluation output.
         model_used: name of the currently employed llm
         chain_used: name of propt chain of the current execution
         true_stance_key: contains true stance. Defaults to None.
         wait_time: Wait time between two prompts sent to the llm. Defaults to 5.
         id_key = id of the instance. Defaults to None.
 
     Return:
         Returns the classifications (with text, statement, etc.) together with the extracted predicted stance ("pred_stance") from out of the StanceClassification class attribute "stance" as well as the prompt texts from the attribute "meta"
     
     """
     pred_egs = []
     for eg in tqdm(egs):
-        eg["stance_classification"] = detect_stance(eg,llm=llm,
-                                                    chain_label=chain_used,
-                                                    chat=chat,
-                                                    llm2=llm2,
-                                                    entity_mask=entity_mask)
+        eg["stance_classification"] = detect_stance(
+            eg,
+            llm=llm,
+            chain_label=chain_used,
+            chat=chat,
+            llm2=llm2,
+            entity_mask=entity_mask,
+        )
         eg["run_alias"] = run_alias
         eg["stance_pred"] = eg["stance_classification"].stance
         eg["meta"] = {
-            "prompt_history": get_prompt_texts_from_meta(classification=eg["stance_classification"])
+            "prompt_history": get_prompt_texts_from_meta(
+                classification=eg["stance_classification"]
+            )
         }
         if entity_mask is not None:
             eg["meta"] = eg["meta"] | {"entity_mask": entity_mask}
         pred_egs.append(eg)
         if stream_out:
             save_classifications_jsonl(
                 export_folder=export_folder,
                 egs_with_classifications=pred_egs,
                 model_used=model_used,
                 chain_used=chain_used,
                 run_alias=run_alias,
                 true_stance_key=true_stance_key,
-                id_key=id_key)
+                id_key=id_key,
+            )
         time.sleep(wait_time)
     if stream_out:
         save_run_meta_info_json(
-            export_folder=export_folder, 
+            export_folder=export_folder,
             model_used=model_used,
             chain_used=chain_used,
             run_alias=run_alias,
-            entity_mask = entity_mask)
+            entity_mask=entity_mask,
+        )
     logger.info(f"finished run {run_alias}")
-    return(pred_egs)
+    return pred_egs
+
 
 def evaluate(egs_with_preds):
     """creates and outputs evaluation metrics: for each stance class: precision, recall, f1, accuracy, and macro (precision, recall, F1, accuracy) and micro (precision, recall, F1, accuracy)
 
     Args:
         egs_with_preds: list of dictionaries containing predicted stances at a key "stance_pred" and true stances under at key "stance_true"
     """
     y_true = []
     y_pred = []
     for eg in egs_with_preds:
         y_pred.append(eg["stance_pred"])
         y_true.append(eg["stance_true"])
-    classes = ["support","opposition","irrelevant"]
+    classes = ["support", "opposition", "irrelevant"]
     logger.info("Creating evaluation report")
     eval_metrics = classification_report(
-        y_true,
-        y_pred,
-        labels=classes,
-        output_dict=True)
-    logger.info(f"----------- Evaluation metrics ------------ \n {eval_metrics} \n ------------------")
-    return(eval_metrics)
-
-def save_evaluations_json(export_folder:str,
-                          eval_metrics,
-                          chain_used:str,
-                          model_used:str,
-                          run_alias:str) -> None:
+        y_true, y_pred, labels=classes, output_dict=True
+    )
+    logger.info(
+        f"----------- Evaluation metrics ------------ \n {eval_metrics} \n ------------------"
+    )
+    return eval_metrics
+
+
+def save_evaluations_json(
+    export_folder: str, eval_metrics, chain_used: str, model_used: str, run_alias: str
+) -> None:
     """serializes metrics to metrics.json file at <export_folder/<chain_used>/<model_used>/<current date>/<run_alias>
 
     Args:
         export_folder: directory target for serialization
         eval_metrics: dictionary with evaluation metrics per stance class and macro and average (for each: precision ,recall, F1, accuracy)
         chain_used: prompt chain (short name)
         model_used: llm model name
         run_alias: name of the classification run to be saved
     """
-    export_folder_path = make_export_folder(export_folder=export_folder,
-                                            chain_used=chain_used,
-                                            model_used=model_used,
-                                            run_alias=run_alias)
-    out_dict = {
-        "run_alias": run_alias,
-        "metrics": eval_metrics
-    }
+    export_folder_path = make_export_folder(
+        export_folder=export_folder,
+        chain_used=chain_used,
+        model_used=model_used,
+        run_alias=run_alias,
+    )
+    out_dict = {"run_alias": run_alias, "metrics": eval_metrics}
     logger.info(f"Saving evaluation report to {str(export_folder_path)}")
-    srsly.write_json(os.path.join(export_folder_path,"metrics.json"),
-                     out_dict)
-    
-def save_run_meta_info_json(export_folder:str,
-                        chain_used:str,
-                        model_used:str,
-                        run_alias:str,
-                        entity_mask:str) -> None:
+    srsly.write_json(os.path.join(export_folder_path, "metrics.json"), out_dict)
+
+
+def save_run_meta_info_json(
+    export_folder: str,
+    chain_used: str,
+    model_used: str,
+    run_alias: str,
+    entity_mask: str,
+) -> None:
     """serializes run meta information to meta.json file at <export_folder/<chain_used>/<model_used>/<current date>/<run_alias>
 
     Args:
         export_folder: directory target for serialization
         chain_used: prompt chain (short name)
         model_used: llm model name
         run_alias: name of the classification run to be saved
         entity_mask: string used to mask the original entity string in the classified text, if any is given
 
     """
-    export_folder_path = make_export_folder(export_folder=export_folder,
-                                            chain_used=chain_used,
-                                            model_used=model_used,
-                                            run_alias=run_alias)
+    export_folder_path = make_export_folder(
+        export_folder=export_folder,
+        chain_used=chain_used,
+        model_used=model_used,
+        run_alias=run_alias,
+    )
     if entity_mask is not None:
         entity_masking = entity_mask
     else:
         entity_masking = "None"
     out_dict = {
         "run_alias": run_alias,
         "chain_used": chain_used,
         "model_used": model_used,
         "date_run": str(date.today()),
-        "entity_masking": entity_masking
+        "entity_masking": entity_masking,
     }
     logger.info(f"Saving run meta-information to {str(export_folder_path)}")
-    srsly.write_json(os.path.join(export_folder_path,"meta.json"),
-                     out_dict)
+    srsly.write_json(os.path.join(export_folder_path, "meta.json"), out_dict)
 
-def save_classifications_jsonl(export_folder:str,
-                               egs_with_classifications, 
-                               model_used:str, 
-                               chain_used:str,
-                               run_alias:str, 
-                               id_key = None,
-                               true_stance_key=None) -> None:
+
+def save_classifications_jsonl(
+    export_folder: str,
+    egs_with_classifications,
+    model_used: str,
+    chain_used: str,
+    run_alias: str,
+    id_key=None,
+    true_stance_key=None,
+) -> None:
     """serializes a list of stance classifications to JSONL in a classifications.jsonl file at <export_folder/<chain_used>/<model_used>/<current date>/<run_alias>
 
     Args:
         export_folder: directory target for serialization
         egs_with_classifications (list): List of stance classifications
         model_used: llm model name
         chain_used: prompt chain (short name)
@@ -268,101 +300,113 @@
         true_stance_key (optional): contains true stance. Defaults to None.
     """
     to_export = []
     for eg in egs_with_classifications:
         if "stance_classification" in eg.keys():
             export_dict = {
                 "text": eg["text"],
-                "org_text": eg["org_text"],
+                "ent_text": eg["ent_text"],
                 "statement": eg["statement"],
                 "stance_pred": eg["stance_classification"].stance,
                 "model_used": model_used,
                 "chain_used": chain_used,
                 "run_alias": run_alias,
-                "meta": eg["meta"]
-                }
+                "meta": eg["meta"],
+            }
             if id_key is not None:
                 export_dict = export_dict | {"id": eg[id_key]}
             if true_stance_key is not None:
                 export_dict = export_dict | {"stance_true": eg[true_stance_key]}
             to_export.append(export_dict)
-    export_subfolder = make_export_folder(export_folder=export_folder,
-                                          model_used=model_used,
-                                          chain_used=chain_used,
-                                          run_alias=run_alias)
-    filepath = os.path.join(export_subfolder,"classifications.jsonl")
-    srsly.write_jsonl(filepath,to_export)
+    export_subfolder = make_export_folder(
+        export_folder=export_folder,
+        model_used=model_used,
+        chain_used=chain_used,
+        run_alias=run_alias,
+    )
+    filepath = os.path.join(export_subfolder, "classifications.jsonl")
+    srsly.write_jsonl(filepath, to_export)
+
 
 def prepare_prodigy_egs(prodigy_egs, remove_flagged=True):
     """Helper to convert exports from prodigy to simpler list to pass to stance annotations tasks.
 
     Args:
         prodigy_egs: List of dicts exported from prodigy db
     """
     egs = []
     if remove_flagged:
-        logger.info("Removing flagged evaluation examples. To avoid this, set remove_flagged to False")
+        logger.info(
+            "Removing flagged evaluation examples. To avoid this, set remove_flagged to False"
+        )
     for eg in prodigy_egs:
-        refactored = { 
+        refactored = {
             "id": eg["par_id"],
             "text": eg["text"],
-            "org_text": eg["meta"]["org_text"],
+            "ent_text": eg["meta"]["ent_text"],
             "statement": eg["statement_de"],
-            "stance_true": eg["accept"][0]
+            "stance_true": eg["accept"][0],
         }
         if remove_flagged:
-            if 'flagged' in eg.keys():
-                if eg['flagged'] is not True:
-                    egs.append(refactored)
-            if 'flagged' not in eg.keys():
+            if "flagged" in eg.keys():
+                if eg["flagged"] is not True:
                     egs.append(refactored)
+            if "flagged" not in eg.keys():
+                egs.append(refactored)
         if remove_flagged is not True:
             egs.append(refactored)
-    return(egs)
+    return egs
+
 
-def process_evaluate(egs,
-               llm,
-               model_used:str,
-               chain_used:str,
-               chat=True,
-               wait_time=0.5,
-               export_folder="./evaluations",
-               llm2=None,
-               entity_mask=None):
+def process_evaluate(
+    egs,
+    llm,
+    model_used: str,
+    chain_used: str,
+    chat=True,
+    wait_time=0.5,
+    export_folder="./evaluations",
+    llm2=None,
+    entity_mask=None,
+):
     """Process a list of examples to via a llm backend, stream out results, evaluate against true values and save evaluations
 
     Args:
-        egs: A list of dictionary items with a "text" key containing text to classify, a "org_text" key containing a string for the organizational entity to predict stance for and a "stance_true" key containing a true stance to evaluate against
+        egs: A list of dictionary items with a "text" key containing text to classify, a "ent_text" key containing a string for the organizational entity to predict stance for and a "stance_true" key containing a true stance to evaluate against
         llm: A guidance model backend from guidance.models
         model_used: String giving label for model backend
         chain_used: An implemented llm chain. See stance_llm.base.get_registered_chains for list
         chat (bool, optional): Should a chat model variant be used? Defaults to True.
         wait_time (int): Wait time (in seconds) between two prompts sent to the llm. Defaults to 5.
         export_folder (str, optional): Folder for evaluation output. Defaults to "./evaluations".
     """
     preds = process(
-        egs = egs,
+        egs=egs,
         llm=llm,
         export_folder=export_folder,
         model_used=model_used,
         chain_used=chain_used,
         wait_time=wait_time,
         true_stance_key="stance_true",
         stream_out=True,
         chat=chat,
         llm2=llm2,
-        entity_mask=entity_mask
-        )
+        entity_mask=entity_mask,
+    )
     eval_metrics = evaluate(preds)
     run_alias = preds[0]["run_alias"]
     assert all([pred["run_alias"] == run_alias for pred in preds])
-    save_evaluations_json(export_folder=export_folder, 
-                          eval_metrics=eval_metrics,
-                          model_used=model_used,
-                          chain_used=chain_used,
-                          run_alias=run_alias)
-    save_run_meta_info_json(export_folder=export_folder, 
-                        model_used=model_used,
-                        chain_used=chain_used,
-                        run_alias=run_alias,
-                        entity_mask = entity_mask)
-    return(preds)
+    save_evaluations_json(
+        export_folder=export_folder,
+        eval_metrics=eval_metrics,
+        model_used=model_used,
+        chain_used=chain_used,
+        run_alias=run_alias,
+    )
+    save_run_meta_info_json(
+        export_folder=export_folder,
+        model_used=model_used,
+        chain_used=chain_used,
+        run_alias=run_alias,
+        entity_mask=entity_mask,
+    )
+    return preds
```

