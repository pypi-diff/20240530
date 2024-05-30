# Comparing `tmp/pie_modules-0.8.4.tar.gz` & `tmp/pie_modules-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pie_modules-0.8.4.tar", max compression
+gzip compressed data, was "pie_modules-0.9.0.tar", max compression
```

## Comparing `pie_modules-0.8.4.tar` & `pie_modules-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,48 @@
--rw-r--r--   0        0        0     1067 2023-12-11 19:23:08.138081 pie_modules-0.8.4/LICENSE
--rw-r--r--   0        0        0     4289 2023-12-11 19:23:08.138081 pie_modules-0.8.4/README.md
--rw-r--r--   0        0        0     1732 2023-12-11 19:23:20.238027 pie_modules-0.8.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-11 19:23:08.138081 pie_modules-0.8.4/src/pie_modules/__init__.py
--rw-r--r--   0        0        0      955 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/annotations.py
--rw-r--r--   0        0        0        0 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/document/__init__.py
--rw-r--r--   0        0        0      289 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/document/processing/__init__.py
--rw-r--r--   0        0        0     9777 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/document/processing/regex_partitioner.py
--rw-r--r--   0        0        0     4203 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/document/processing/relation_argument_sorter.py
--rw-r--r--   0        0        0     3674 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/document/processing/text_span_trimmer.py
--rw-r--r--   0        0        0    15624 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/document/processing/tokenization.py
--rw-r--r--   0        0        0     1555 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/documents.py
--rw-r--r--   0        0        0      277 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/metrics/__init__.py
--rw-r--r--   0        0        0     4599 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/metrics/span_length_collector.py
--rw-r--r--   0        0        0     5866 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/metrics/squad_f1.py
--rw-r--r--   0        0        0      353 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/__init__.py
--rw-r--r--   0        0        0        0 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/components/__init__.py
--rw-r--r--   0        0        0     7252 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/components/pooler.py
--rw-r--r--   0        0        0     2611 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/components/seq2seq_encoder.py
--rw-r--r--   0        0        0       39 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/interface.py
--rw-r--r--   0        0        0     6720 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/sequence_classification.py
--rw-r--r--   0        0        0     6521 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/simple_extractive_question_answering.py
--rw-r--r--   0        0        0     5827 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/simple_sequence_classification.py
--rw-r--r--   0        0        0     8793 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/models/token_classification_with_seq2seq_encoder_and_crf.py
--rw-r--r--   0        0        0      245 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/taskmodules/__init__.py
--rw-r--r--   0        0        0     9925 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/taskmodules/extractive_question_answering.py
--rw-r--r--   0        0        0    44738 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/taskmodules/re_text_classification_with_indices.py
--rw-r--r--   0        0        0    15278 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/taskmodules/token_classification.py
--rw-r--r--   0        0        0      772 2023-12-11 19:23:08.142081 pie_modules-0.8.4/src/pie_modules/utils.py
--rw-r--r--   0        0        0     5299 1970-01-01 00:00:00.000000 pie_modules-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-11 12:22:56.048548 pie_modules-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4534 2024-01-11 12:22:56.048548 pie_modules-0.9.0/README.md
+-rw-r--r--   0        0        0     1837 2024-01-11 12:23:07.720439 pie_modules-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/__init__.py
+-rw-r--r--   0        0        0     1494 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/annotations.py
+-rw-r--r--   0        0        0        0 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/document/__init__.py
+-rw-r--r--   0        0        0      289 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/document/processing/__init__.py
+-rw-r--r--   0        0        0     9777 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/document/processing/regex_partitioner.py
+-rw-r--r--   0        0        0     4203 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/document/processing/relation_argument_sorter.py
+-rw-r--r--   0        0        0     3674 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/document/processing/text_span_trimmer.py
+-rw-r--r--   0        0        0    15908 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/document/processing/tokenization.py
+-rw-r--r--   0        0        0     4040 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/documents.py
+-rw-r--r--   0        0        0      277 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/metrics/__init__.py
+-rw-r--r--   0        0        0     4599 2024-01-11 12:22:56.048548 pie_modules-0.9.0/src/pie_modules/metrics/span_length_collector.py
+-rw-r--r--   0        0        0     5916 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/metrics/squad_f1.py
+-rw-r--r--   0        0        0      406 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/__init__.py
+-rw-r--r--   0        0        0      134 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/base_models/__init__.py
+-rw-r--r--   0        0        0    19349 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/base_models/bart_as_pointer_network.py
+-rw-r--r--   0        0        0    24097 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/base_models/bart_with_decoder_position_ids.py
+-rw-r--r--   0        0        0        0 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/components/__init__.py
+-rw-r--r--   0        0        0    13208 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/components/pointer_head.py
+-rw-r--r--   0        0        0     7252 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/components/pooler.py
+-rw-r--r--   0        0        0     2611 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/components/seq2seq_encoder.py
+-rw-r--r--   0        0        0      305 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/interface.py
+-rw-r--r--   0        0        0     6720 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/sequence_classification.py
+-rw-r--r--   0        0        0     6521 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/simple_extractive_question_answering.py
+-rw-r--r--   0        0        0    14355 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/simple_generative.py
+-rw-r--r--   0        0        0     5827 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/simple_sequence_classification.py
+-rw-r--r--   0        0        0     8793 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/models/token_classification_with_seq2seq_encoder_and_crf.py
+-rw-r--r--   0        0        0      373 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/__init__.py
+-rw-r--r--   0        0        0      149 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/common/__init__.py
+-rw-r--r--   0        0        0     1009 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/common/interfaces.py
+-rw-r--r--   0        0        0     4834 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/common/mixins.py
+-rw-r--r--   0        0        0     1219 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/common/utils.py
+-rw-r--r--   0        0        0    10047 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/extractive_question_answering.py
+-rw-r--r--   0        0        0      342 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/metrics/__init__.py
+-rw-r--r--   0        0        0     4387 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/metrics/precision_recall_and_f1_for_labeled_annotations.py
+-rw-r--r--   0        0        0     6427 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/metrics/wrapped_layer_metrics_with_unbatch_and_decode_with_errors_function.py
+-rw-r--r--   0        0        0     1653 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/metrics/wrapped_metric_with_unbatch_function.py
+-rw-r--r--   0        0        0        0 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/pointer_network/__init__.py
+-rw-r--r--   0        0        0    10262 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/pointer_network/annotation_encoder_decoder.py
+-rw-r--r--   0        0        0     1898 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/pointer_network/logits_processor.py
+-rw-r--r--   0        0        0    35944 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/pointer_network_for_end2end_re.py
+-rw-r--r--   0        0        0    44738 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/re_text_classification_with_indices.py
+-rw-r--r--   0        0        0    18986 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/text_to_text.py
+-rw-r--r--   0        0        0    14977 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/taskmodules/token_classification.py
+-rw-r--r--   0        0        0      772 2024-01-11 12:22:56.052548 pie_modules-0.9.0/src/pie_modules/utils.py
+-rw-r--r--   0        0        0     5590 1970-01-01 00:00:00.000000 pie_modules-0.9.0/PKG-INFO
```

### Comparing `pie_modules-0.8.4/LICENSE` & `pie_modules-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/README.md` & `pie_modules-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,23 @@
 
 Available models:
 
 - [SimpleSequenceClassificationModel](src/pie_modules/models/simple_sequence_classification.py)
 - [SequenceClassificationModel](src/pie_modules/models/sequence_classification.py)
 - [TokenClassificationModelWithSeq2SeqEncoderAndCrf](src/pie_modules/models/token_classification_with_seq2seq_encoder_and_crf.py)
 - [SimpleExtractiveQuestionAnsweringModel](src/pie_modules/models/simple_extractive_question_answering.py)
+- [SimpleGenerativeModel](src/pie_modules/models/simple_generative.py)
 
 Available taskmodules:
 
 - [RETextClassificationWithIndicesTaskModule](src/pie_modules/taskmodules/re_text_classification_with_indices.py)
 - [TokenClassificationTaskModule](src/pie_modules/taskmodules/token_classification.py)
 - [ExtractiveQuestionAnsweringTaskModule](src/pie_modules/taskmodules/extractive_question_answering.py)
+- [TextToTextTaskModule](src/pie_modules/taskmodules/text_to_text.py)
+- [PointerNetworkTaskModuleForEnd2EndRE](src/pie_modules/taskmodules/pointer_network_for_end2end_re.py)
 
 Available metrics:
 
 - [SpanLengthCollector](src/pie_modules/metrics/span_length_collector.py)
 - [SQuADF1](src/pie_modules/metrics/squad_f1.py)
 
 ## Setup
```

#### html2text {}

```diff
@@ -9,36 +9,39 @@
 ChristophAlt/pytorch-ie). Available models: -
 [SimpleSequenceClassificationModel](src/pie_modules/models/
 simple_sequence_classification.py) - [SequenceClassificationModel](src/
 pie_modules/models/sequence_classification.py) -
 [TokenClassificationModelWithSeq2SeqEncoderAndCrf](src/pie_modules/models/
 token_classification_with_seq2seq_encoder_and_crf.py) -
 [SimpleExtractiveQuestionAnsweringModel](src/pie_modules/models/
-simple_extractive_question_answering.py) Available taskmodules: -
+simple_extractive_question_answering.py) - [SimpleGenerativeModel](src/
+pie_modules/models/simple_generative.py) Available taskmodules: -
 [RETextClassificationWithIndicesTaskModule](src/pie_modules/taskmodules/
 re_text_classification_with_indices.py) - [TokenClassificationTaskModule](src/
 pie_modules/taskmodules/token_classification.py) -
 [ExtractiveQuestionAnsweringTaskModule](src/pie_modules/taskmodules/
-extractive_question_answering.py) Available metrics: - [SpanLengthCollector]
-(src/pie_modules/metrics/span_length_collector.py) - [SQuADF1](src/pie_modules/
-metrics/squad_f1.py) ## Setup ```bash pip install pie-modules ``` To install
-the latest version from GitHub: ```bash pip install git+https://git@github.com/
-ArneBinder/pie-modules.git ``` ## Development ### Setup 1. This project is
-build with [Poetry](https://python-poetry.org/). See here for [installation
-instructions](https://python-poetry.org/docs/#installation). 2. Get the code
-and switch into the project directory: ```bash git clone https://github.com/
-ArneBinder/pie-modules cd pie-modules ``` 3. Create a virtual environment and
-install the dependencies: ```bash poetry install ``` Finally, to run any of the
-below commands, you need to activate the virtual environment: ```bash poetry
-shell ``` Note: You can also run commands in the virtual environment without
-activating it first: `poetry run `. ### Code Formatting, Linting and Static
-Type Checking ```bash pre-commit run -a ``` ### Testing run all tests with
-coverage: ```bash pytest --cov --cov-report term-missing ``` ### Releasing 1.
-Create the release branch: `git switch --create release main` 2. Increase the
-version: `poetry version
+extractive_question_answering.py) - [TextToTextTaskModule](src/pie_modules/
+taskmodules/text_to_text.py) - [PointerNetworkTaskModuleForEnd2EndRE](src/
+pie_modules/taskmodules/pointer_network_for_end2end_re.py) Available metrics: -
+[SpanLengthCollector](src/pie_modules/metrics/span_length_collector.py) -
+[SQuADF1](src/pie_modules/metrics/squad_f1.py) ## Setup ```bash pip install
+pie-modules ``` To install the latest version from GitHub: ```bash pip install
+git+https://git@github.com/ArneBinder/pie-modules.git ``` ## Development ###
+Setup 1. This project is build with [Poetry](https://python-poetry.org/). See
+here for [installation instructions](https://python-poetry.org/docs/
+#installation). 2. Get the code and switch into the project directory: ```bash
+git clone https://github.com/ArneBinder/pie-modules cd pie-modules ``` 3.
+Create a virtual environment and install the dependencies: ```bash poetry
+install ``` Finally, to run any of the below commands, you need to activate the
+virtual environment: ```bash poetry shell ``` Note: You can also run commands
+in the virtual environment without activating it first: `poetry run `. ### Code
+Formatting, Linting and Static Type Checking ```bash pre-commit run -a ``` ###
+Testing run all tests with coverage: ```bash pytest --cov --cov-report term-
+missing ``` ### Releasing 1. Create the release branch: `git switch --create
+release main` 2. Increase the version: `poetry version
 MINOR|MAJOR>`, e.g. `poetry version patch` for a patch release. If the release
 contains new features, or breaking changes, bump the minor version (this
 project has no main release yet). If the release contains only bugfixes, bump
 the patch version. See [Semantic Versioning](https://semver.org/) for more
 information. 3. Commit the changes: `git commit --message="release "
 pyproject.toml`, e.g. `git commit --message="release 0.13.0" pyproject.toml` 4.
 Push the changes to GitHub: `git push origin release` 5. Create a PR for that
```

### Comparing `pie_modules-0.8.4/pyproject.toml` & `pie_modules-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pie-modules"
-version = "0.8.4"
+version = "0.9.0"
 description = "Model and Taskmodule implementations for PyTorch-IE"
 authors = ["Arne Binder <arne.binder@dfki.de>"]
 readme = "README.md"
 homepage = "https://github.com/arnebinder/pie-modules"
 repository = "https://github.com/arnebinder/pie-modules"
 packages = [
     { include = "pie_modules", from = "src" },
@@ -20,25 +20,29 @@
 ]
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/arnebinder/pie-modules/issues"
 "Changelog" = "https://github.com/arnebinder/pie-modules/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pytorch-ie = ">=0.29.4,<0.30.0"
+pytorch-ie = ">=0.29.5,<0.30.0"
 pytorch-lightning = "^2.1.0"
 torchmetrics = "^1"
 pytorch-crf = ">=0.7.2"
+# because of BartModelWithDecoderPositionIds
+transformers = "^4.35.0"
 
 [tool.poetry.group.dev.dependencies]
 torch = {version = "^2.1.0+cpu", source = "pytorch"}
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.4.0"
 tabulate = "^0.9"
+# for rouge metric
+nltk = "^3.8.1"
 
 [[tool.poetry.source]]
 name = "pytorch"
 url = "https://download.pytorch.org/whl/cpu"
 priority = "explicit"
 
 [[tool.poetry.source]]
```

### Comparing `pie_modules-0.8.4/src/pie_modules/annotations.py` & `pie_modules-0.9.0/src/pie_modules/annotations.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 from typing import Optional
 
 from pytorch_ie.annotations import Span
 from pytorch_ie.core import Annotation
 
 
 @dataclasses.dataclass(eq=True, frozen=True)
-class Question(Annotation):
-    """A question about a context."""
-
+class AnnotationWithText(Annotation):
     text: str
 
+
+@dataclasses.dataclass(eq=True, frozen=True)
+class Question(AnnotationWithText):
+    """A question about a context."""
+
     def __str__(self) -> str:
         return self.text
 
 
 @dataclasses.dataclass(eq=True, frozen=True)
 class ExtractiveAnswer(Span):
     """An answer to a question."""
@@ -28,7 +31,22 @@
 
     def __str__(self) -> str:
         if not self.is_attached:
             return ""
         # we assume that the first target is the text
         context = self.named_targets["base"]
         return str(context[self.start : self.end])
+
+
+@dataclasses.dataclass(eq=True, frozen=True)
+class AbstractiveSummary(AnnotationWithText):
+    """An abstractive summary."""
+
+    score: Optional[float] = dataclasses.field(default=None, compare=False)
+
+
+@dataclasses.dataclass(eq=True, frozen=True)
+class GenerativeAnswer(AnnotationWithText):
+    """An answer to a question."""
+
+    score: Optional[float] = dataclasses.field(default=None, compare=False)
+    question: Optional[Question] = None
```

### Comparing `pie_modules-0.8.4/src/pie_modules/document/processing/regex_partitioner.py` & `pie_modules-0.9.0/src/pie_modules/document/processing/regex_partitioner.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/document/processing/relation_argument_sorter.py` & `pie_modules-0.9.0/src/pie_modules/document/processing/relation_argument_sorter.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/document/processing/text_span_trimmer.py` & `pie_modules-0.9.0/src/pie_modules/document/processing/text_span_trimmer.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/document/processing/tokenization.py` & `pie_modules-0.9.0/src/pie_modules/document/processing/tokenization.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,19 +339,22 @@
             )
             tokenized_document.metadata["tokenizer_encoding"] = batch_encoding
             result.append(tokenized_document)
 
     missed_annotations = defaultdict(set)
     if strict_span_conversion or verbose:
         for annotation_field in doc.annotation_fields():
-            current_missed_annotations = set(doc[annotation_field.name]) - set(
-                added_annotations[annotation_field.name]
-            )
-            if len(current_missed_annotations) > 0:
-                missed_annotations[annotation_field.name] = current_missed_annotations
+            # do not check the partition layer because the partitions are not required later on
+            # and entries get quite probably removed when windowing is applied, so this just pollutes the logs
+            if annotation_field.name != partition_layer:
+                current_missed_annotations = set(doc[annotation_field.name]) - set(
+                    added_annotations[annotation_field.name]
+                )
+                if len(current_missed_annotations) > 0:
+                    missed_annotations[annotation_field.name] = current_missed_annotations
 
     if len(missed_annotations) > 0:
         missed_annotations_simplified = {k: str(v) for k, v in missed_annotations.items()}
         if strict_span_conversion:
             raise ValueError(
                 f"could not convert all annotations from document with id={doc.id} to token based documents, "
                 f"but strict_span_conversion is True, so raise an error, "
```

### Comparing `pie_modules-0.8.4/src/pie_modules/metrics/span_length_collector.py` & `pie_modules-0.9.0/src/pie_modules/metrics/span_length_collector.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/metrics/squad_f1.py` & `pie_modules-0.9.0/src/pie_modules/metrics/squad_f1.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import string
 from collections import defaultdict
 from typing import Dict, List
 
 import pandas as pd
 from pytorch_ie.core import DocumentMetric
 
-from pie_modules.documents import ExtractiveQADocument
+from pie_modules.documents import TextDocumentWithQuestionsAndExtractiveAnswers
 
 logger = logging.getLogger(__name__)
 
 
 def prefix_keys(d: Dict[str, float], prefix: str) -> Dict[str, float]:
     return {f"{prefix}_{k}": v for k, v in d.items()}
 
@@ -38,15 +38,15 @@
     def reset(self):
         self.exact_scores = {}
         self.f1_scores = {}
         self.qas_id_to_has_answer = {}
         self.has_answer_qids = []
         self.no_answer_qids = []
 
-    def _update(self, document: ExtractiveQADocument):
+    def _update(self, document: TextDocumentWithQuestionsAndExtractiveAnswers):
         gold_answers_for_questions = defaultdict(list)
         predicted_answers_for_questions = defaultdict(list)
         for ann in document.answers:
             gold_answers_for_questions[ann.question].append(ann)
         for ann in document.answers.predictions:
             predicted_answers_for_questions[ann.question].append(ann)
```

### Comparing `pie_modules-0.8.4/src/pie_modules/models/components/pooler.py` & `pie_modules-0.9.0/src/pie_modules/models/components/pooler.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/models/components/seq2seq_encoder.py` & `pie_modules-0.9.0/src/pie_modules/models/components/seq2seq_encoder.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/models/sequence_classification.py` & `pie_modules-0.9.0/src/pie_modules/models/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/models/simple_extractive_question_answering.py` & `pie_modules-0.9.0/src/pie_modules/models/simple_extractive_question_answering.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/models/simple_sequence_classification.py` & `pie_modules-0.9.0/src/pie_modules/models/simple_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/models/token_classification_with_seq2seq_encoder_and_crf.py` & `pie_modules-0.9.0/src/pie_modules/models/token_classification_with_seq2seq_encoder_and_crf.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/taskmodules/extractive_question_answering.py` & `pie_modules-0.9.0/src/pie_modules/taskmodules/extractive_question_answering.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 from tokenizers import Encoding
 from transformers import AutoTokenizer, BatchEncoding, PreTrainedTokenizer
 from transformers.modeling_outputs import QuestionAnsweringModelOutput
 from typing_extensions import TypeAlias
 
 from pie_modules.annotations import ExtractiveAnswer, Question
 from pie_modules.document.processing import tokenize_document
-from pie_modules.documents import ExtractiveQADocument, TokenizedExtractiveQADocument
+from pie_modules.documents import (
+    TextDocumentWithQuestionsAndExtractiveAnswers,
+    TokenDocumentWithQuestionsAndExtractiveAnswers,
+)
 
 logger = logging.getLogger(__name__)
 
 
 DocumentType: TypeAlias = TextBasedDocument
 InputEncoding: TypeAlias = Union[Dict[str, Any], BatchEncoding]
 
@@ -25,15 +28,15 @@
 @dataclasses.dataclass
 class TargetEncoding:
     start_position: int
     end_position: int
 
 
 TaskEncodingType: TypeAlias = TaskEncoding[
-    ExtractiveQADocument,
+    TextDocumentWithQuestionsAndExtractiveAnswers,
     InputEncoding,
     TargetEncoding,
 ]
 
 TaskBatchEncoding: TypeAlias = Tuple[BatchEncoding, Optional[Dict[str, Any]]]
 ModelBatchOutput: TypeAlias = QuestionAnsweringModelOutput
 
@@ -63,15 +66,15 @@
         tokenizer_name_or_path: The name (Huggingface Hub identifier) or local path to a config of the tokenizer to use.
         max_length: The maximum length of the input sequence in means of tokens.
         answer_annotation: The name of the annotation layer for answers. Defaults to "answers".
         question_annotation: The name of the annotation layer for questions. Defaults to "questions".
         tokenize_kwargs: Additional keyword arguments for the tokenizer. Defaults to None.
     """
 
-    DOCUMENT_TYPE = ExtractiveQADocument
+    DOCUMENT_TYPE = TextDocumentWithQuestionsAndExtractiveAnswers
 
     def __init__(
         self,
         tokenizer_name_or_path: str,
         max_length: int,
         answer_annotation: str = "answers",
         question_annotation: str = "questions",
@@ -120,15 +123,15 @@
             tokenized_docs = tokenize_document(
                 document,
                 tokenizer=self.tokenizer,
                 text=question.text.strip(),
                 truncation="only_second",
                 max_length=self.max_length,
                 return_overflowing_tokens=True,
-                result_document_type=TokenizedExtractiveQADocument,
+                result_document_type=TokenDocumentWithQuestionsAndExtractiveAnswers,
                 strict_span_conversion=False,
                 verbose=False,
                 **self.tokenize_kwargs,
             )
             for doc in tokenized_docs:
                 inputs = self.tokenizer.convert_tokens_to_ids(list(doc.tokens))
                 task_encodings.append(
```

### Comparing `pie_modules-0.8.4/src/pie_modules/taskmodules/re_text_classification_with_indices.py` & `pie_modules-0.9.0/src/pie_modules/taskmodules/re_text_classification_with_indices.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/src/pie_modules/taskmodules/token_classification.py` & `pie_modules-0.9.0/src/pie_modules/taskmodules/token_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
         -> (InputEncoding, TargetEncoding) -> TaskEncoding
             -> ModelStepInputType -> ModelBatchOutput
         -> TaskOutput
     -> Document
 """
 
 import copy
-import dataclasses
 import logging
 from typing import (
     Any,
     Dict,
     Iterator,
     List,
     Optional,
@@ -21,36 +20,39 @@
     Tuple,
     Type,
     Union,
 )
 
 import torch
 import torch.nn.functional as F
-from pytorch_ie import AnnotationLayer, annotation_field
+from pytorch_ie import AnnotationLayer
 from pytorch_ie.annotations import LabeledSpan
 from pytorch_ie.core import TaskEncoding, TaskModule
 from pytorch_ie.documents import (
     TextDocument,
     TextDocumentWithLabeledSpans,
     TextDocumentWithLabeledSpansAndLabeledPartitions,
-    TokenBasedDocument,
 )
 from pytorch_ie.models.transformer_token_classification import (
     ModelOutputType,
     ModelStepInputType,
 )
 from pytorch_ie.utils.span import bio_tags_to_spans
 from tokenizers import Encoding
 from transformers import AutoTokenizer
 from typing_extensions import TypeAlias
 
 from pie_modules.document.processing import (
     token_based_document_to_text_based,
     tokenize_document,
 )
+from pie_modules.documents import (
+    TokenDocumentWithLabeledSpans,
+    TokenDocumentWithLabeledSpansAndLabeledPartitions,
+)
 
 DocumentType: TypeAlias = TextDocument
 
 InputEncodingType: TypeAlias = Encoding
 TargetEncodingType: TypeAlias = Sequence[int]
 TaskEncodingType: TypeAlias = TaskEncoding[
     DocumentType,
@@ -67,24 +69,14 @@
     ModelOutputType,
     TaskOutputType,
 ]
 
 logger = logging.getLogger(__name__)
 
 
-@dataclasses.dataclass
-class TokenDocumentWithLabeledSpans(TokenBasedDocument):
-    labeled_spans: AnnotationLayer[LabeledSpan] = annotation_field(target="tokens")
-
-
-@dataclasses.dataclass
-class TokenDocumentWithLabeledSpansAndLabeledPartitions(TokenDocumentWithLabeledSpans):
-    labeled_partitions: AnnotationLayer[LabeledSpan] = annotation_field(target="tokens")
-
-
 @TaskModule.register()
 class TokenClassificationTaskModule(TaskModuleType):
     """Taskmodule for span prediction (e.g. NER) as token classification.
 
     This taskmodule expects the input documents to be of TextBasedDocument with an annotation layer of
     labeled spans (e.g. TextDocumentWithLabeledSpans). The text is tokenized using the provided tokenizer and
     the labels are converted to BIO tags.
```

### Comparing `pie_modules-0.8.4/src/pie_modules/utils.py` & `pie_modules-0.9.0/src/pie_modules/utils.py`

 * *Files identical despite different names*

### Comparing `pie_modules-0.8.4/PKG-INFO` & `pie_modules-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pie-modules
-Version: 0.8.4
+Version: 0.9.0
 Summary: Model and Taskmodule implementations for PyTorch-IE
 Home-page: https://github.com/arnebinder/pie-modules
 Author: Arne Binder
 Author-email: arne.binder@dfki.de
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: pytorch-crf (>=0.7.2)
-Requires-Dist: pytorch-ie (>=0.29.4,<0.30.0)
+Requires-Dist: pytorch-ie (>=0.29.5,<0.30.0)
 Requires-Dist: pytorch-lightning (>=2.1.0,<3.0.0)
 Requires-Dist: torchmetrics (>=1,<2)
+Requires-Dist: transformers (>=4.35.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/arnebinder/pie-modules/issues
 Project-URL: Changelog, https://github.com/arnebinder/pie-modules/releases
 Project-URL: Repository, https://github.com/arnebinder/pie-modules
 Description-Content-Type: text/markdown
 
 # pie-modules
 
@@ -38,20 +39,23 @@
 
 Available models:
 
 - [SimpleSequenceClassificationModel](src/pie_modules/models/simple_sequence_classification.py)
 - [SequenceClassificationModel](src/pie_modules/models/sequence_classification.py)
 - [TokenClassificationModelWithSeq2SeqEncoderAndCrf](src/pie_modules/models/token_classification_with_seq2seq_encoder_and_crf.py)
 - [SimpleExtractiveQuestionAnsweringModel](src/pie_modules/models/simple_extractive_question_answering.py)
+- [SimpleGenerativeModel](src/pie_modules/models/simple_generative.py)
 
 Available taskmodules:
 
 - [RETextClassificationWithIndicesTaskModule](src/pie_modules/taskmodules/re_text_classification_with_indices.py)
 - [TokenClassificationTaskModule](src/pie_modules/taskmodules/token_classification.py)
 - [ExtractiveQuestionAnsweringTaskModule](src/pie_modules/taskmodules/extractive_question_answering.py)
+- [TextToTextTaskModule](src/pie_modules/taskmodules/text_to_text.py)
+- [PointerNetworkTaskModuleForEnd2EndRE](src/pie_modules/taskmodules/pointer_network_for_end2end_re.py)
 
 Available metrics:
 
 - [SpanLengthCollector](src/pie_modules/metrics/span_length_collector.py)
 - [SQuADF1](src/pie_modules/metrics/squad_f1.py)
 
 ## Setup
```

#### html2text {}

```diff
@@ -1,57 +1,61 @@
-Metadata-Version: 2.1 Name: pie-modules Version: 0.8.4 Summary: Model and
+Metadata-Version: 2.1 Name: pie-modules Version: 0.9.0 Summary: Model and
 Taskmodule implementations for PyTorch-IE Home-page: https://github.com/
 arnebinder/pie-modules Author: Arne Binder Author-email: arne.binder@dfki.de
 Requires-Python: >=3.9,<4.0 Classifier: Framework :: Pytest Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Requires-Dist: pytorch-
-crf (>=0.7.2) Requires-Dist: pytorch-ie (>=0.29.4,<0.30.0) Requires-Dist:
+crf (>=0.7.2) Requires-Dist: pytorch-ie (>=0.29.5,<0.30.0) Requires-Dist:
 pytorch-lightning (>=2.1.0,<3.0.0) Requires-Dist: torchmetrics (>=1,<2)
-Project-URL: Bug Tracker, https://github.com/arnebinder/pie-modules/issues
-Project-URL: Changelog, https://github.com/arnebinder/pie-modules/releases
-Project-URL: Repository, https://github.com/arnebinder/pie-modules Description-
-Content-Type: text/markdown # pie-modules _[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_P_y_T_o_r_c_h_-_I_E_]
+Requires-Dist: transformers (>=4.35.0,<5.0.0) Project-URL: Bug Tracker, https:/
+/github.com/arnebinder/pie-modules/issues Project-URL: Changelog, https://
+github.com/arnebinder/pie-modules/releases Project-URL: Repository, https://
+github.com/arnebinder/pie-modules Description-Content-Type: text/markdown #
+pie-modules _[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_P_y_T_o_r_c_h_-_I_E_]
 [![PyPI](https://img.shields.io/pypi/v/pie-modules.svg)][pypi status] [![Tests]
 (https://github.com/arnebinder/pie-modules/workflows/Tests/badge.svg)][tests]
 [![Codecov](https://codecov.io/gh/arnebinder/pie-modules/branch/main/graph/
 badge.svg)][codecov] [![pre-commit](https://img.shields.io/badge/pre--commit-
 enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit] [![Black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)][black] Model-,
 taskmodule-, and metric-implementations for [PyTorch-IE](https://github.com/
 ChristophAlt/pytorch-ie). Available models: -
 [SimpleSequenceClassificationModel](src/pie_modules/models/
 simple_sequence_classification.py) - [SequenceClassificationModel](src/
 pie_modules/models/sequence_classification.py) -
 [TokenClassificationModelWithSeq2SeqEncoderAndCrf](src/pie_modules/models/
 token_classification_with_seq2seq_encoder_and_crf.py) -
 [SimpleExtractiveQuestionAnsweringModel](src/pie_modules/models/
-simple_extractive_question_answering.py) Available taskmodules: -
+simple_extractive_question_answering.py) - [SimpleGenerativeModel](src/
+pie_modules/models/simple_generative.py) Available taskmodules: -
 [RETextClassificationWithIndicesTaskModule](src/pie_modules/taskmodules/
 re_text_classification_with_indices.py) - [TokenClassificationTaskModule](src/
 pie_modules/taskmodules/token_classification.py) -
 [ExtractiveQuestionAnsweringTaskModule](src/pie_modules/taskmodules/
-extractive_question_answering.py) Available metrics: - [SpanLengthCollector]
-(src/pie_modules/metrics/span_length_collector.py) - [SQuADF1](src/pie_modules/
-metrics/squad_f1.py) ## Setup ```bash pip install pie-modules ``` To install
-the latest version from GitHub: ```bash pip install git+https://git@github.com/
-ArneBinder/pie-modules.git ``` ## Development ### Setup 1. This project is
-build with [Poetry](https://python-poetry.org/). See here for [installation
-instructions](https://python-poetry.org/docs/#installation). 2. Get the code
-and switch into the project directory: ```bash git clone https://github.com/
-ArneBinder/pie-modules cd pie-modules ``` 3. Create a virtual environment and
-install the dependencies: ```bash poetry install ``` Finally, to run any of the
-below commands, you need to activate the virtual environment: ```bash poetry
-shell ``` Note: You can also run commands in the virtual environment without
-activating it first: `poetry run `. ### Code Formatting, Linting and Static
-Type Checking ```bash pre-commit run -a ``` ### Testing run all tests with
-coverage: ```bash pytest --cov --cov-report term-missing ``` ### Releasing 1.
-Create the release branch: `git switch --create release main` 2. Increase the
-version: `poetry version
+extractive_question_answering.py) - [TextToTextTaskModule](src/pie_modules/
+taskmodules/text_to_text.py) - [PointerNetworkTaskModuleForEnd2EndRE](src/
+pie_modules/taskmodules/pointer_network_for_end2end_re.py) Available metrics: -
+[SpanLengthCollector](src/pie_modules/metrics/span_length_collector.py) -
+[SQuADF1](src/pie_modules/metrics/squad_f1.py) ## Setup ```bash pip install
+pie-modules ``` To install the latest version from GitHub: ```bash pip install
+git+https://git@github.com/ArneBinder/pie-modules.git ``` ## Development ###
+Setup 1. This project is build with [Poetry](https://python-poetry.org/). See
+here for [installation instructions](https://python-poetry.org/docs/
+#installation). 2. Get the code and switch into the project directory: ```bash
+git clone https://github.com/ArneBinder/pie-modules cd pie-modules ``` 3.
+Create a virtual environment and install the dependencies: ```bash poetry
+install ``` Finally, to run any of the below commands, you need to activate the
+virtual environment: ```bash poetry shell ``` Note: You can also run commands
+in the virtual environment without activating it first: `poetry run `. ### Code
+Formatting, Linting and Static Type Checking ```bash pre-commit run -a ``` ###
+Testing run all tests with coverage: ```bash pytest --cov --cov-report term-
+missing ``` ### Releasing 1. Create the release branch: `git switch --create
+release main` 2. Increase the version: `poetry version
 MINOR|MAJOR>`, e.g. `poetry version patch` for a patch release. If the release
 contains new features, or breaking changes, bump the minor version (this
 project has no main release yet). If the release contains only bugfixes, bump
 the patch version. See [Semantic Versioning](https://semver.org/) for more
 information. 3. Commit the changes: `git commit --message="release "
 pyproject.toml`, e.g. `git commit --message="release 0.13.0" pyproject.toml` 4.
 Push the changes to GitHub: `git push origin release` 5. Create a PR for that
```

