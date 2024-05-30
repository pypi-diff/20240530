# Comparing `tmp/besser_bot_framework-1.2.1.tar.gz` & `tmp/besser_bot_framework-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besser_bot_framework-1.2.1.tar", last modified: Wed May  8 12:13:01 2024, max compression
+gzip compressed data, was "besser_bot_framework-1.2.2.tar", last modified: Thu May 30 12:55:40 2024, max compression
```

## Comparing `besser_bot_framework-1.2.1.tar` & `besser_bot_framework-1.2.2.tar`

### file list

```diff
@@ -1,105 +1,114 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.452528 besser_bot_framework-1.2.1/
--rw-rw-rw-   0        0        0     1090 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     3204 2024-05-08 12:13:01.452528 besser_bot_framework-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1849 2024-01-22 15:17:03.000000 besser_bot_framework-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.361421 besser_bot_framework-1.2.1/besser/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.362421 besser_bot_framework-1.2.1/besser/bot/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.370420 besser_bot_framework-1.2.1/besser/bot/core/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/core/__init__.py
--rw-rw-rw-   0        0        0    20671 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.374424 besser_bot_framework-1.2.1/besser/bot/core/entity/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/core/entity/__init__.py
--rw-rw-rw-   0        0        0     3098 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/entity/entity.py
--rw-rw-rw-   0        0        0      820 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/entity/entity_entry.py
--rw-rw-rw-   0        0        0     3855 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/core/file.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.378423 besser_bot_framework-1.2.1/besser/bot/core/intent/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/core/intent/__init__.py
--rw-rw-rw-   0        0        0     4815 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/core/intent/intent.py
--rw-rw-rw-   0        0        0     1187 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/intent/intent_parameter.py
--rw-rw-rw-   0        0        0     1077 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/property.py
--rw-rw-rw-   0        0        0     6585 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/session.py
--rw-rw-rw-   0        0        0    18203 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/state.py
--rw-rw-rw-   0        0        0     5258 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/transition.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.380421 besser_bot_framework-1.2.1/besser/bot/db/
--rw-rw-rw-   0        0        0     1648 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/db/__init__.py
--rw-rw-rw-   0        0        0    10274 2024-05-08 12:10:29.000000 besser_bot_framework-1.2.1/besser/bot/db/monitoring_db.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.383421 besser_bot_framework-1.2.1/besser/bot/exceptions/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/exceptions/__init__.py
--rw-rw-rw-   0        0        0     4814 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.384421 besser_bot_framework-1.2.1/besser/bot/library/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.387421 besser_bot_framework-1.2.1/besser/bot/library/entity/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/entity/__init__.py
--rw-rw-rw-   0        0        0     1423 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/library/entity/base_entities.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.390422 besser_bot_framework-1.2.1/besser/bot/library/event/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/event/__init__.py
--rw-rw-rw-   0        0        0     2729 2024-02-06 10:51:26.000000 besser_bot_framework-1.2.1/besser/bot/library/event/event_library.py
--rw-rw-rw-   0        0        0      315 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/library/event/event_template.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.394422 besser_bot_framework-1.2.1/besser/bot/library/intent/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/intent/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/library/intent/intent_classifier_configuration_library.py
--rw-rw-rw-   0        0        0      239 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/library/intent/intent_library.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.397425 besser_bot_framework-1.2.1/besser/bot/library/state/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/state/__init__.py
--rw-rw-rw-   0        0        0      756 2024-02-19 15:24:24.000000 besser_bot_framework-1.2.1/besser/bot/library/state/state_library.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.400422 besser_bot_framework-1.2.1/besser/bot/nlp/
--rw-rw-rw-   0        0        0     5328 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.408422 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier.py
--rw-rw-rw-   0        0        0     6907 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py
--rw-rw-rw-   0        0        0     2896 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py
--rw-rw-rw-   0        0        0    12208 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/llm_intent_classifier.py
--rw-rw-rw-   0        0        0     7722 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/simple_intent_classifier.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.414455 besser_bot_framework-1.2.1/besser/bot/nlp/ner/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.419429 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/__init__.py
--rw-rw-rw-   0        0        0      226 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/any.py
--rw-rw-rw-   0        0        0     7050 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/datetime.py
--rw-rw-rw-   0        0        0      975 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/number.py
--rw-rw-rw-   0        0        0      786 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/matched_parameter.py
--rw-rw-rw-   0        0        0     1576 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner.py
--rw-rw-rw-   0        0        0     1891 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner_prediction.py
--rw-rw-rw-   0        0        0    10536 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/simple_ner.py
--rw-rw-rw-   0        0        0     7010 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/nlp_engine.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.422447 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      909 2023-12-10 20:05:59.000000 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/pipelines.py
--rw-rw-rw-   0        0        0     2787 2023-12-12 13:27:54.000000 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/text_preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.427527 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/
--rw-rw-rw-   0        0        0        0 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/__init__.py
--rw-rw-rw-   0        0        0     2294 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/api_speech2text.py
--rw-rw-rw-   0        0        0     2302 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/hf_speech2text.py
--rw-rw-rw-   0        0        0     1255 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/speech2text.py
--rw-rw-rw-   0        0        0     1234 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.430527 besser_bot_framework-1.2.1/besser/bot/platforms/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/platforms/__init__.py
--rw-rw-rw-   0        0        0     3790 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/payload.py
--rw-rw-rw-   0        0        0     1787 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.433528 besser_bot_framework-1.2.1/besser/bot/platforms/telegram/
--rw-rw-rw-   0        0        0      364 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/platforms/telegram/__init__.py
--rw-rw-rw-   0        0        0    11876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/telegram/telegram_platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.437531 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/
--rw-rw-rw-   0        0        0     1546 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/__init__.py
--rw-rw-rw-   0        0        0      793 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/message.py
--rw-rw-rw-   0        0        0    11100 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/streamlit_ui.py
--rw-rw-rw-   0        0        0    10093 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/websocket_platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.439531 besser_bot_framework-1.2.1/besser/bot/test/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.443527 besser_bot_framework-1.2.1/besser/bot/test/examples/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/__init__.py
--rw-rw-rw-   0        0        0     1876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/greetings_bot.py
--rw-rw-rw-   0        0        0     3303 2024-05-08 07:50:07.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/telegram_bot.py
--rw-rw-rw-   0        0        0     2075 2024-05-07 11:25:10.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/weather_bot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.451529 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/
--rw-rw-rw-   0        0        0     3204 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2919 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      431 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      454 2024-05-08 12:12:35.000000 besser_bot_framework-1.2.1/requirements.txt
--rw-rw-rw-   0        0        0      704 2024-05-08 12:13:01.454527 besser_bot_framework-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.440761 besser_bot_framework-1.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3203 2024-05-30 12:55:40.439717 besser_bot_framework-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1849 2024-01-22 15:17:03.000000 besser_bot_framework-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.330245 besser_bot_framework-1.2.2/besser/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.331244 besser_bot_framework-1.2.2/besser/bot/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.339896 besser_bot_framework-1.2.2/besser/bot/core/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/core/__init__.py
+-rw-rw-rw-   0        0        0    20671 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/core/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.343897 besser_bot_framework-1.2.2/besser/bot/core/entity/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/core/entity/__init__.py
+-rw-rw-rw-   0        0        0     3098 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/core/entity/entity.py
+-rw-rw-rw-   0        0        0      820 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/core/entity/entity_entry.py
+-rw-rw-rw-   0        0        0     3855 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/core/file.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.347898 besser_bot_framework-1.2.2/besser/bot/core/intent/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/core/intent/__init__.py
+-rw-rw-rw-   0        0        0     4815 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/core/intent/intent.py
+-rw-rw-rw-   0        0        0     1187 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/core/intent/intent_parameter.py
+-rw-rw-rw-   0        0        0     1077 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/core/property.py
+-rw-rw-rw-   0        0        0     6585 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/core/session.py
+-rw-rw-rw-   0        0        0    18203 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/core/state.py
+-rw-rw-rw-   0        0        0     5258 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/core/transition.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.350049 besser_bot_framework-1.2.2/besser/bot/db/
+-rw-rw-rw-   0        0        0     1648 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/db/__init__.py
+-rw-rw-rw-   0        0        0    10274 2024-05-08 12:10:29.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_db.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.361048 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/
+-rw-rw-rw-   0        0        0        0 2024-05-06 15:04:46.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/__init__.py
+-rw-rw-rw-   0        0        0     2118 2024-05-06 18:55:53.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/db_connection.py
+-rw-rw-rw-   0        0        0     3984 2024-05-07 19:47:18.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/flow_graph.py
+-rw-rw-rw-   0        0        0     2416 2024-05-07 20:00:19.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/home.py
+-rw-rw-rw-   0        0        0     1310 2024-05-07 20:02:35.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/monitoring_ui.py
+-rw-rw-rw-   0        0        0      368 2024-05-07 20:02:42.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/sidebar.py
+-rw-rw-rw-   0        0        0      942 2024-05-07 19:38:53.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/table_overview.py
+-rw-rw-rw-   0        0        0     3089 2024-05-06 14:43:29.000000 besser_bot_framework-1.2.2/besser/bot/db/monitoring_ui/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.364198 besser_bot_framework-1.2.2/besser/bot/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     4814 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.365713 besser_bot_framework-1.2.2/besser/bot/library/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/library/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.367727 besser_bot_framework-1.2.2/besser/bot/library/entity/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/library/entity/__init__.py
+-rw-rw-rw-   0        0        0     1423 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/library/entity/base_entities.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.371773 besser_bot_framework-1.2.2/besser/bot/library/event/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/library/event/__init__.py
+-rw-rw-rw-   0        0        0     2729 2024-02-06 10:51:26.000000 besser_bot_framework-1.2.2/besser/bot/library/event/event_library.py
+-rw-rw-rw-   0        0        0      315 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/library/event/event_template.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.375755 besser_bot_framework-1.2.2/besser/bot/library/intent/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/library/intent/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/library/intent/intent_classifier_configuration_library.py
+-rw-rw-rw-   0        0        0      239 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/library/intent/intent_library.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.377792 besser_bot_framework-1.2.2/besser/bot/library/state/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/library/state/__init__.py
+-rw-rw-rw-   0        0        0      756 2024-02-19 15:24:24.000000 besser_bot_framework-1.2.2/besser/bot/library/state/state_library.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.381943 besser_bot_framework-1.2.2/besser/bot/nlp/
+-rw-rw-rw-   0        0        0     5328 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.389950 besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/intent_classifier.py
+-rw-rw-rw-   0        0        0     6476 2024-05-30 12:11:35.000000 besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py
+-rw-rw-rw-   0        0        0     2896 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py
+-rw-rw-rw-   0        0        0    12208 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/llm_intent_classifier.py
+-rw-rw-rw-   0        0        0     7426 2024-05-30 12:31:45.000000 besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/simple_intent_classifier.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.397553 besser_bot_framework-1.2.2/besser/bot/nlp/ner/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.402583 besser_bot_framework-1.2.2/besser/bot/nlp/ner/base/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/base/__init__.py
+-rw-rw-rw-   0        0        0      226 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/base/any.py
+-rw-rw-rw-   0        0        0     7050 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/base/datetime.py
+-rw-rw-rw-   0        0        0      975 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/base/number.py
+-rw-rw-rw-   0        0        0      786 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/matched_parameter.py
+-rw-rw-rw-   0        0        0     1576 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/ner.py
+-rw-rw-rw-   0        0        0     1891 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/ner_prediction.py
+-rw-rw-rw-   0        0        0    10536 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/nlp/ner/simple_ner.py
+-rw-rw-rw-   0        0        0     7089 2024-05-30 12:24:21.000000 besser_bot_framework-1.2.2/besser/bot/nlp/nlp_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.406344 besser_bot_framework-1.2.2/besser/bot/nlp/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/nlp/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-12-10 20:05:59.000000 besser_bot_framework-1.2.2/besser/bot/nlp/preprocessing/pipelines.py
+-rw-rw-rw-   0        0        0     2787 2023-12-12 13:27:54.000000 besser_bot_framework-1.2.2/besser/bot/nlp/preprocessing/text_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.412086 besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/
+-rw-rw-rw-   0        0        0        0 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/__init__.py
+-rw-rw-rw-   0        0        0     2294 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/api_speech2text.py
+-rw-rw-rw-   0        0        0     2302 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/hf_speech2text.py
+-rw-rw-rw-   0        0        0     1255 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/speech2text.py
+-rw-rw-rw-   0        0        0     1234 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.2/besser/bot/nlp/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.416124 besser_bot_framework-1.2.2/besser/bot/platforms/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/platforms/__init__.py
+-rw-rw-rw-   0        0        0     3790 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/platforms/payload.py
+-rw-rw-rw-   0        0        0     1787 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/platforms/platform.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.418087 besser_bot_framework-1.2.2/besser/bot/platforms/telegram/
+-rw-rw-rw-   0        0        0      364 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.2/besser/bot/platforms/telegram/__init__.py
+-rw-rw-rw-   0        0        0    11876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/platforms/telegram/telegram_platform.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.424085 besser_bot_framework-1.2.2/besser/bot/platforms/websocket/
+-rw-rw-rw-   0        0        0     1546 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.2/besser/bot/platforms/websocket/__init__.py
+-rw-rw-rw-   0        0        0      793 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/platforms/websocket/message.py
+-rw-rw-rw-   0        0        0    11100 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/platforms/websocket/streamlit_ui.py
+-rw-rw-rw-   0        0        0    10093 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.2/besser/bot/platforms/websocket/websocket_platform.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.425085 besser_bot_framework-1.2.2/besser/bot/test/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.430715 besser_bot_framework-1.2.2/besser/bot/test/examples/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.2/besser/bot/test/examples/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-05-30 11:56:22.000000 besser_bot_framework-1.2.2/besser/bot/test/examples/greetings_bot.py
+-rw-rw-rw-   0        0        0     3303 2024-05-08 07:50:07.000000 besser_bot_framework-1.2.2/besser/bot/test/examples/telegram_bot.py
+-rw-rw-rw-   0        0        0     2075 2024-05-30 09:26:17.000000 besser_bot_framework-1.2.2/besser/bot/test/examples/weather_bot.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:40.438715 besser_bot_framework-1.2.2/besser_bot_framework.egg-info/
+-rw-rw-rw-   0        0        0     3203 2024-05-30 12:55:40.000000 besser_bot_framework-1.2.2/besser_bot_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3249 2024-05-30 12:55:40.000000 besser_bot_framework-1.2.2/besser_bot_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:55:40.000000 besser_bot_framework-1.2.2/besser_bot_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      430 2024-05-30 12:55:40.000000 besser_bot_framework-1.2.2/besser_bot_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 12:55:40.000000 besser_bot_framework-1.2.2/besser_bot_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      453 2024-05-30 12:55:00.000000 besser_bot_framework-1.2.2/requirements.txt
+-rw-rw-rw-   0        0        0      704 2024-05-30 12:55:40.441884 besser_bot_framework-1.2.2/setup.cfg
```

### Comparing `besser_bot_framework-1.2.1/LICENSE` & `besser_bot_framework-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/PKG-INFO` & `besser_bot_framework-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: besser-bot-framework
-Version: 1.2.1
+Version: 1.2.2
 Summary: BESSER Bot Framework (BBF)
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besserbot-framework.readthedocs.io/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER-Bot-Framework
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER-Bot-Framework/issues
 Keywords: bot,framework,chatbot,state-machine,nlp
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audio-recorder-streamlit==0.0.8
 Requires-Dist: dateparser==1.1.8
-Requires-Dist: keras==2.14.0
+Requires-Dist: keras==3.3.3
 Requires-Dist: librosa==0.10.1
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.26.1
 Requires-Dist: openai==1.8.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: plotly==5.18.0
 Requires-Dist: psycopg2-binary==2.9.9
@@ -25,15 +25,15 @@
 Requires-Dist: replicate==0.23.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: snowballstemmer==2.2.0
 Requires-Dist: spacy==3.7.2
 Requires-Dist: SpeechRecognition==3.10.0
 Requires-Dist: sqlalchemy==2.0.29
 Requires-Dist: streamlit==1.27.2
-Requires-Dist: tensorflow==2.14.0
+Requires-Dist: tensorflow==2.16.1
 Requires-Dist: text2num==2.5.0
 Requires-Dist: transformers==4.37.0
 Requires-Dist: websocket-client==1.6.4
 Requires-Dist: websockets==11.0.3
 
 # BESSER Bot Framework
```

### Comparing `besser_bot_framework-1.2.1/README.md` & `besser_bot_framework-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/bot.py` & `besser_bot_framework-1.2.2/besser/bot/core/bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/entity/entity.py` & `besser_bot_framework-1.2.2/besser/bot/core/entity/entity.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/entity/entity_entry.py` & `besser_bot_framework-1.2.2/besser/bot/core/entity/entity_entry.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/file.py` & `besser_bot_framework-1.2.2/besser/bot/core/file.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/intent/intent.py` & `besser_bot_framework-1.2.2/besser/bot/core/intent/intent.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/intent/intent_parameter.py` & `besser_bot_framework-1.2.2/besser/bot/core/intent/intent_parameter.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/property.py` & `besser_bot_framework-1.2.2/besser/bot/core/property.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/session.py` & `besser_bot_framework-1.2.2/besser/bot/core/session.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/state.py` & `besser_bot_framework-1.2.2/besser/bot/core/state.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/core/transition.py` & `besser_bot_framework-1.2.2/besser/bot/core/transition.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/db/__init__.py` & `besser_bot_framework-1.2.2/besser/bot/db/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/db/monitoring_db.py` & `besser_bot_framework-1.2.2/besser/bot/db/monitoring_db.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/exceptions/exceptions.py` & `besser_bot_framework-1.2.2/besser/bot/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/library/entity/base_entities.py` & `besser_bot_framework-1.2.2/besser/bot/library/entity/base_entities.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/library/event/event_library.py` & `besser_bot_framework-1.2.2/besser/bot/library/event/event_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/library/intent/intent_classifier_configuration_library.py` & `besser_bot_framework-1.2.2/besser/bot/library/intent/intent_classifier_configuration_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/library/state/state_library.py` & `besser_bot_framework-1.2.2/besser/bot/library/state/state_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/__init__.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,27 @@
     The Simple Intent Classifier Configuration class.
 
     It allows the customization of a
     :class:`~besser.bot.nlp.intent_classifier.simple_intent_classifier.SimpleIntentClassifier`.
 
     Args:
         num_words (int): Max num of words to keep in the index of words
-        lower (bool): whether to transform the sentences to lowercase or not
-        oov_token (str): Token for the out of vocabulary words
         num_epochs (int): Number of epochs to be run during training
         embedding_dim (int): Number of embedding dimensions to be used when embedding the words
         input_max_num_tokens (int): Max length for the vector representing a sentence
         discard_oov_sentences (bool): whether to automatically assign zero probabilities to sentences with all tokens
             being oov ones or not
         check_exact_prediction_match (bool): Whether to check for exact match between the sentence to predict and one of
             the training sentences or not
         activation_last_layer (str): The activation function of the last layer
         activation_hidden_layers (str): The activation function of the hidden layers
         lr (float): Learning rate for the optimizer
 
     Attributes:
         num_words (int): Max num of words to keep in the index of words
-        lower (bool): whether to transform the sentences to lowercase or not
-        oov_token (str): Token for the out of vocabulary words
         num_epochs (int): Number of epochs to be run during training
         embedding_dim (int): Number of embedding dimensions to be used when embedding the words
         input_max_num_tokens (int): Max length for the vector representing a sentence
         discard_oov_sentences (bool): whether to automatically assign zero probabilities to sentences with all tokens
             being oov ones or not
         check_exact_prediction_match (bool): Whether to check for exact match between the sentence to predict and one of
             the training sentences or not
@@ -53,29 +49,25 @@
         lr (float): Learning rate for the optimizer
 
     """
 
     def __init__(
             self,
             num_words: int = 1000,
-            lower: bool = True,
-            oov_token: str = '<OOV>',
             num_epochs: int = 300,
             embedding_dim: int = 128,
             input_max_num_tokens: int = 15,
             discard_oov_sentences: bool = True,
             check_exact_prediction_match: bool = True,
             activation_last_layer: str = 'sigmoid',
             activation_hidden_layers: str = 'tanh',
             lr: float = 0.001,
     ):
         super().__init__()
         self.num_words: int = num_words
-        self.lower: bool = lower
-        self.oov_token: str = oov_token
         self.num_epochs: int = num_epochs
         self.embedding_dim: int = embedding_dim
         self.input_max_num_tokens: int = input_max_num_tokens
         self.discard_oov_sentences: bool = discard_oov_sentences
         self.check_exact_prediction_match: bool = check_exact_prediction_match
         self.activation_last_layer: str = activation_last_layer
         self.activation_hidden_layers: str = activation_hidden_layers
```

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/llm_intent_classifier.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/llm_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/simple_intent_classifier.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/intent_classifier/simple_intent_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,60 @@
-import os
 from typing import TYPE_CHECKING
 
-import keras
 import numpy as np
 from keras import Sequential
-from keras.layers import Dense, Embedding, GlobalAveragePooling1D
-from keras.losses import SparseCategoricalCrossentropy
-from keras.preprocessing.text import Tokenizer
-from keras.utils import pad_sequences
+from keras.src.layers import TextVectorization, Dense, Embedding, GlobalAveragePooling1D
+from keras.src.losses import SparseCategoricalCrossentropy
+from keras.src.optimizers import Adam
+from keras.src.utils import pad_sequences
 
 from besser.bot.core.intent.intent import Intent
 from besser.bot.nlp.intent_classifier.intent_classifier import IntentClassifier
 from besser.bot.nlp.intent_classifier.intent_classifier_prediction import IntentClassifierPrediction
 from besser.bot.nlp.ner.ner_prediction import NERPrediction
 from besser.bot.nlp.preprocessing.text_preprocessing import process_text
 
 if TYPE_CHECKING:
     from besser.bot.core.state import State
     from besser.bot.nlp.nlp_engine import NLPEngine
 
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
-
 
 class SimpleIntentClassifier(IntentClassifier):
     """A Simple Intent Classifier.
 
     It works using a simple Keras Neural Network (the prediction model) for text classification.
 
     Args:
         nlp_engine (NLPEngine): the NLPEngine that handles the NLP processes of the bot
         state (State): the state the intent classifier belongs to
 
     Attributes:
-        _tokenizer (`Tokenizer <https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/text/Tokenizer>`_):
+        _tokenizer (`TextVectorization <https://www.tensorflow.org/api_docs/python/tf/keras/layers/TextVectorization>`_):
             The intent classifier tokenizer
         _model (`Sequential <https://www.tensorflow.org/api_docs/python/tf/keras/Sequential>`_):
             The intent classifier language model
 
     See Also:
         :class:`~besser.bot.nlp.intent_classifier.intent_classifier_configuration.SimpleIntentClassifierConfiguration`.
     """
 
     def __init__(
             self,
             nlp_engine: 'NLPEngine',
             state: 'State'
     ):
         super().__init__(nlp_engine, state)
-        self._tokenizer: Tokenizer = Tokenizer(
-            num_words=self._state.ic_config.num_words,
-            lower=self._state.ic_config.lower,
-            oov_token=self._state.ic_config.oov_token
+        self._tokenizer = TextVectorization(
+            max_tokens=self._state.ic_config.num_words,
+            standardize='lower_and_strip_punctuation',
+            output_sequence_length=self._state.ic_config.input_max_num_tokens
         )
         self._model: Sequential = Sequential([
             Embedding(input_dim=self._state.ic_config.num_words,
-                      output_dim=self._state.ic_config.embedding_dim,
-                      input_length=self._state.ic_config.input_max_num_tokens),
+                      output_dim=self._state.ic_config.embedding_dim),
             GlobalAveragePooling1D(),
             Dense(24, activation=self._state.ic_config.activation_hidden_layers),
             Dense(24, activation=self._state.ic_config.activation_hidden_layers),
             Dense(len(self._state.intents), activation=self._state.ic_config.activation_last_layer)
         ])
         self.__total_training_sentences: list[str] = []
         """All the processed training sentences of all intents of the intent classifier's state."""
@@ -81,25 +76,21 @@
                 intent.processed_training_sentences
             )
             self.__total_labels_training_sentences.extend(
                 [index_intent for _ in range(len(intent.processed_training_sentences))]
             )
             self.__intent_label_mapping[index_intent] = intent
 
-        self._tokenizer.fit_on_texts(self.__total_training_sentences)
-        self.__total_training_sequences = pad_sequences(
-            self._tokenizer.texts_to_sequences(self.__total_training_sentences),
-            maxlen=self._state.ic_config.input_max_num_tokens,
-            padding='post',
-            truncating='post'
+        self._tokenizer.adapt(self.__total_training_sentences)
+        self.__total_training_sequences = self._tokenizer(
+            self.__total_training_sentences,
         )
-
         self._model.compile(
             loss=SparseCategoricalCrossentropy(),
-            optimizer=keras.optimizers.Adam(learning_rate=self._state.ic_config.lr),
+            optimizer=Adam(learning_rate=self._state.ic_config.lr),
             metrics=['accuracy']
         )
 
         history = self._model.fit(
             np.array(self.__total_training_sequences),
             np.array(self.__total_labels_training_sentences),
             epochs=self._state.ic_config.num_epochs, verbose=0
@@ -110,15 +101,15 @@
         intent_classifier_results: list[IntentClassifierPrediction] = []
 
         # We try to replace all potential entity value with the corresponding entity name
         ner_prediction: NERPrediction = self._state.bot.nlp_engine.ner.predict(self._state, message)
         for (ner_sentence, intents) in ner_prediction.ner_sentences.items():
             # DOUBLE STEMMING AVOIDED
             sentences = [ner_sentence]
-            sequences = self._tokenizer.texts_to_sequences(sentences)
+            sequences = self._tokenizer(sentences)
             padded = pad_sequences(
                 sequences,
                 maxlen=self._state.ic_config.input_max_num_tokens,
                 padding='post',
                 truncating='post'
             )
             run_full_prediction: bool = True
```

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/datetime.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/ner/base/datetime.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/number.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/ner/base/number.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/ner/matched_parameter.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/ner/matched_parameter.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/ner/ner.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner_prediction.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/ner/ner_prediction.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/ner/simple_ner.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/ner/simple_ner.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/nlp_engine.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/nlp_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'  # Hide Tensorflow logs
+
 import logging
 from typing import Any, TYPE_CHECKING
 
 from besser.bot import nlp
 from besser.bot.core.property import Property
 from besser.bot.core.session import Session
 from besser.bot.nlp.intent_classifier.intent_classifier import IntentClassifier
```

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/pipelines.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/preprocessing/pipelines.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/text_preprocessing.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/preprocessing/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/api_speech2text.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/api_speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/hf_speech2text.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/hf_speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/speech2text.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/speech2text/speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/nlp/utils.py` & `besser_bot_framework-1.2.2/besser/bot/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/platforms/payload.py` & `besser_bot_framework-1.2.2/besser/bot/platforms/payload.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/platforms/platform.py` & `besser_bot_framework-1.2.2/besser/bot/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/platforms/telegram/telegram_platform.py` & `besser_bot_framework-1.2.2/besser/bot/platforms/telegram/telegram_platform.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/__init__.py` & `besser_bot_framework-1.2.2/besser/bot/platforms/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/message.py` & `besser_bot_framework-1.2.2/besser/bot/platforms/websocket/message.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/streamlit_ui.py` & `besser_bot_framework-1.2.2/besser/bot/platforms/websocket/streamlit_ui.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/websocket_platform.py` & `besser_bot_framework-1.2.2/besser/bot/platforms/websocket/websocket_platform.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/test/examples/greetings_bot.py` & `besser_bot_framework-1.2.2/besser/bot/test/examples/greetings_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/test/examples/telegram_bot.py` & `besser_bot_framework-1.2.2/besser/bot/test/examples/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser/bot/test/examples/weather_bot.py` & `besser_bot_framework-1.2.2/besser/bot/test/examples/weather_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.1/besser_bot_framework.egg-info/PKG-INFO` & `besser_bot_framework-1.2.2/besser_bot_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: besser-bot-framework
-Version: 1.2.1
+Version: 1.2.2
 Summary: BESSER Bot Framework (BBF)
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besserbot-framework.readthedocs.io/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER-Bot-Framework
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER-Bot-Framework/issues
 Keywords: bot,framework,chatbot,state-machine,nlp
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audio-recorder-streamlit==0.0.8
 Requires-Dist: dateparser==1.1.8
-Requires-Dist: keras==2.14.0
+Requires-Dist: keras==3.3.3
 Requires-Dist: librosa==0.10.1
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.26.1
 Requires-Dist: openai==1.8.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: plotly==5.18.0
 Requires-Dist: psycopg2-binary==2.9.9
@@ -25,15 +25,15 @@
 Requires-Dist: replicate==0.23.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: snowballstemmer==2.2.0
 Requires-Dist: spacy==3.7.2
 Requires-Dist: SpeechRecognition==3.10.0
 Requires-Dist: sqlalchemy==2.0.29
 Requires-Dist: streamlit==1.27.2
-Requires-Dist: tensorflow==2.14.0
+Requires-Dist: tensorflow==2.16.1
 Requires-Dist: text2num==2.5.0
 Requires-Dist: transformers==4.37.0
 Requires-Dist: websocket-client==1.6.4
 Requires-Dist: websockets==11.0.3
 
 # BESSER Bot Framework
```

### Comparing `besser_bot_framework-1.2.1/besser_bot_framework.egg-info/SOURCES.txt` & `besser_bot_framework-1.2.2/besser_bot_framework.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 besser/bot/core/entity/entity.py
 besser/bot/core/entity/entity_entry.py
 besser/bot/core/intent/__init__.py
 besser/bot/core/intent/intent.py
 besser/bot/core/intent/intent_parameter.py
 besser/bot/db/__init__.py
 besser/bot/db/monitoring_db.py
+besser/bot/db/monitoring_ui/__init__.py
+besser/bot/db/monitoring_ui/db_connection.py
+besser/bot/db/monitoring_ui/flow_graph.py
+besser/bot/db/monitoring_ui/home.py
+besser/bot/db/monitoring_ui/monitoring_ui.py
+besser/bot/db/monitoring_ui/sidebar.py
+besser/bot/db/monitoring_ui/table_overview.py
+besser/bot/db/monitoring_ui/utils.py
 besser/bot/exceptions/__init__.py
 besser/bot/exceptions/exceptions.py
 besser/bot/library/__init__.py
 besser/bot/library/entity/__init__.py
 besser/bot/library/entity/base_entities.py
 besser/bot/library/event/__init__.py
 besser/bot/library/event/event_library.py
```

### Comparing `besser_bot_framework-1.2.1/setup.cfg` & `besser_bot_framework-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6573 7365 722d 626f 742d 6672   = besser-bot-fr
 00000020: 616d 6577 6f72 6b0d 0a76 6572 7369 6f6e  amework..version
-00000030: 203d 2031 2e32 2e31 0d0a 6175 7468 6f72   = 1.2.1..author
+00000030: 203d 2031 2e32 2e32 0d0a 6175 7468 6f72   = 1.2.2..author
 00000040: 203d 204c 7578 656d 626f 7572 6720 496e   = Luxembourg In
 00000050: 7374 6974 7574 6520 6f66 2053 6369 656e  stitute of Scien
 00000060: 6365 2061 6e64 2054 6563 686e 6f6c 6f67  ce and Technolog
 00000070: 790d 0a64 6573 6372 6970 7469 6f6e 203d  y..description =
 00000080: 2042 4553 5345 5220 426f 7420 4672 616d   BESSER Bot Fram
 00000090: 6577 6f72 6b20 2842 4246 290d 0a6c 6f6e  ework (BBF)..lon
 000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

