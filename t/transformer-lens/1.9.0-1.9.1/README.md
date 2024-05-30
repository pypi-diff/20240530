# Comparing `tmp/transformer_lens-1.9.0.tar.gz` & `tmp/transformer_lens-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_lens-1.9.0.tar", max compression
+gzip compressed data, was "transformer_lens-1.9.1.tar", max compression
```

## Comparing `transformer_lens-1.9.0.tar` & `transformer_lens-1.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-10-22 15:42:35.365259 transformer_lens-1.9.0/LICENSE
--rw-r--r--   0        0        0    10494 2023-10-22 15:42:35.365259 transformer_lens-1.9.0/README.md
--rw-r--r--   0        0        0     5303 2023-10-22 15:43:49.194926 transformer_lens-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    47142 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/ActivationCache.py
--rw-r--r--   0        0        0     9536 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/FactoredMatrix.py
--rw-r--r--   0        0        0    15634 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/HookedEncoder.py
--rw-r--r--   0        0        0   109011 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/HookedTransformer.py
--rw-r--r--   0        0        0    14413 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/HookedTransformerConfig.py
--rw-r--r--   0        0        0     5985 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/SVDInterpreter.py
--rw-r--r--   0        0        0      951 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/__init__.py
--rw-r--r--   0        0        0    49393 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/components.py
--rw-r--r--   0        0        0    12838 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/evals.py
--rw-r--r--   0        0        0    11887 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/head_detector.py
--rw-r--r--   0        0        0    21910 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/hook_points.py
--rw-r--r--   0        0        0    65834 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/loading_from_pretrained.py
--rw-r--r--   0        0        0     4353 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/past_key_value_caching.py
--rw-r--r--   0        0        0    32941 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/patching.py
--rw-r--r--   0        0        0     5510 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/train.py
--rw-r--r--   0        0        0        0 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/utilities/__init__.py
--rw-r--r--   0        0        0     2449 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/utilities/devices.py
--rw-r--r--   0        0        0    45679 2023-10-22 15:42:35.465262 transformer_lens-1.9.0/transformer_lens/utils.py
--rw-r--r--   0        0        0    13120 1970-01-01 00:00:00.000000 transformer_lens-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-10-26 13:30:21.036057 transformer_lens-1.9.1/LICENSE
+-rw-r--r--   0        0        0    10034 2023-10-26 13:30:21.036057 transformer_lens-1.9.1/README.md
+-rw-r--r--   0        0        0     5303 2023-10-26 13:31:45.686558 transformer_lens-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    47142 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/ActivationCache.py
+-rw-r--r--   0        0        0     9536 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/FactoredMatrix.py
+-rw-r--r--   0        0        0    15634 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/HookedEncoder.py
+-rw-r--r--   0        0        0   109011 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/HookedTransformer.py
+-rw-r--r--   0        0        0    14413 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/HookedTransformerConfig.py
+-rw-r--r--   0        0        0     5985 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/SVDInterpreter.py
+-rw-r--r--   0        0        0      951 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/__init__.py
+-rw-r--r--   0        0        0    49393 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/components.py
+-rw-r--r--   0        0        0    12838 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/evals.py
+-rw-r--r--   0        0        0    11887 2023-10-26 13:30:21.184061 transformer_lens-1.9.1/transformer_lens/head_detector.py
+-rw-r--r--   0        0        0    21910 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/hook_points.py
+-rw-r--r--   0        0        0    65834 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/loading_from_pretrained.py
+-rw-r--r--   0        0        0     4353 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/past_key_value_caching.py
+-rw-r--r--   0        0        0    32941 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/patching.py
+-rw-r--r--   0        0        0     5510 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/train.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/utilities/__init__.py
+-rw-r--r--   0        0        0     2449 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/utilities/devices.py
+-rw-r--r--   0        0        0    45679 2023-10-26 13:30:21.188062 transformer_lens-1.9.1/transformer_lens/utils.py
+-rw-r--r--   0        0        0    12660 1970-01-01 00:00:00.000000 transformer_lens-1.9.1/PKG-INFO
```

### Comparing `transformer_lens-1.9.0/LICENSE` & `transformer_lens-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/README.md` & `transformer_lens-1.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,106 +1,184 @@
 # TransformerLens
 
-![TransformerLens](assets/rm_transformer_lens_logo.png)
-
 <!-- Status Icons -->
 [![Pypi](https://img.shields.io/pypi/v/transformer-lens?color=blue)](https://pypi.org/project/transformer-lens/)
-![Pepy Total Downlods](https://img.shields.io/pepy/dt/transformer_lens?color=blue) ![PyPI -
-License](https://img.shields.io/pypi/l/transformer_lens?color=blue)
-[![Release CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml)
-[![Tests CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml) [![Docs CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml)
+![Pypi Total Downloads](https://img.shields.io/pepy/dt/transformer_lens?color=blue) ![PyPI -
+License](https://img.shields.io/pypi/l/transformer_lens?color=blue) [![Release
+CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml)
+[![Tests
+CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml)
+[![Docs
+CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml)
+
+A Library for Mechanistic Interpretability of Generative Language Models.
+
+[![Read the Docs
+Here](https://img.shields.io/badge/-Read%20the%20Docs%20Here-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white&link=https://neelnanda-io.github.io/TransformerLens/)](https://neelnanda-io.github.io/TransformerLens/)
+
+This is a library for doing [mechanistic
+interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The
+goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms
+the model learned during training from its weights.
+
+TransformerLens lets you load in 50+ different open source language models, and exposes the internal
+activations of the model to you. You can cache any internal activation in the model, and add in
+functions to edit, remove or replace these activations as the model runs.
 
-This library is maintained by **Joseph Bloom** and was created by **[Neel Nanda](https://neelnanda.io)**
+~~ [OCTOBER SURVEY HERE](https://forms.gle/bw7U3PfioacDtFmT8) ~~
 
-## [Read the Docs Here](https://neelnanda-io.github.io/TransformerLens/)
+## Quick Start
 
-## Installation
+### Install
 
-Install: `pip install transformer_lens`
+```shell
+pip install transformer_lens
+```
+
+### Use
 
 ```python
 import transformer_lens
 
 # Load a model (eg GPT-2 Small)
 model = transformer_lens.HookedTransformer.from_pretrained("gpt2-small")
 
 # Run the model and get logits and activations
 logits, activations = model.run_with_cache("Hello World")
 ```
 
 ## Key Tutorials
 
-### [Introduction to the Library and Mech Interp](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp)
-
-### [Demo of Main TransformerLens Features](https://neelnanda.io/transformer-lens-demo)
-
-## A Library for Mechanistic Interpretability of Generative Language Models
-
-This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this!
-
-TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make _my_ experience of doing research easier and more fun, hopefully this transfers to you!
+* [Introduction to the Library and Mech
+  Interp](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp)
+* [Demo of Main TransformerLens Features](https://neelnanda.io/transformer-lens-demo)
 
 ## Gallery
 
 Research done involving TransformerLens:
 
-- [Progress Measures for Grokking via Mechanistic Interpretability](https://arxiv.org/abs/2301.05217) (ICLR Spotlight, 2023) by Neel Nanda, Lawrence Chan, Tom Lieberum, Jess Smith, Jacob Steinhardt
-- [Finding Neurons in a Haystack: Case Studies with Sparse Probing](https://arxiv.org/abs/2305.01610) by Wes Gurnee, Neel Nanda, Matthew Pauly, Katherine Harvey, Dmitrii Troitskii, Dimitris Bertsimas
-- [Towards Automated Circuit Discovery for Mechanistic Interpretability](https://arxiv.org/abs/2304.14997) by Arthur Conmy, Augustine N. Mavor-Parker, Aengus Lynch, Stefan Heimersheim, Adrià Garriga-Alonso
-- [Actually, Othello-GPT Has A Linear Emergent World Representation](https://neelnanda.io/othello) by Neel Nanda
-- [A circuit for Python docstrings in a 4-layer attention-only transformer](https://www.alignmentforum.org/posts/u6KXXmKFbXfWzoAXn/a-circuit-for-python-docstrings-in-a-4-layer-attention-only) by Stefan Heimersheim and Jett Janiak
-- [A Toy Model of Universality](https://arxiv.org/abs/2302.03025) (ICML, 2023) by Bilal Chughtai, Lawrence Chan, Neel Nanda
-- [N2G: A Scalable Approach for Quantifying Interpretable Neuron Representations in Large Language Models](https://openreview.net/forum?id=ZB6bK6MTYq) (2023, ICLR Workshop RTML) by Alex Foote, Neel Nanda, Esben Kran, Ioannis Konstas, Fazl Barez
-- [Eliciting Latent Predictions from Transformers with the Tuned Lens](https://arxiv.org/abs/2303.08112) by Nora Belrose, Zach Furman, Logan Smith, Danny Halawi, Igor Ostrovsky, Lev McKinney, Stella Biderman, Jacob Steinhardt
+<!-- If you change this also change docs/source/content/gallery.md -->
+* [Progress Measures for Grokking via Mechanistic
+  Interpretability](https://arxiv.org/abs/2301.05217) (ICLR Spotlight, 2023) by Neel Nanda, Lawrence
+  Chan, Tom Lieberum, Jess Smith, Jacob Steinhardt
+* [Finding Neurons in a Haystack: Case Studies with Sparse
+  Probing](https://arxiv.org/abs/2305.01610) by Wes Gurnee, Neel Nanda, Matthew Pauly, Katherine
+  Harvey, Dmitrii Troitskii, Dimitris Bertsimas
+* [Towards Automated Circuit Discovery for Mechanistic
+  Interpretability](https://arxiv.org/abs/2304.14997) by Arthur Conmy, Augustine N. Mavor-Parker,
+  Aengus Lynch, Stefan Heimersheim, Adrià Garriga-Alonso
+* [Actually, Othello-GPT Has A Linear Emergent World Representation](https://neelnanda.io/othello)
+  by Neel Nanda
+* [A circuit for Python docstrings in a 4-layer attention-only
+  transformer](https://www.alignmentforum.org/posts/u6KXXmKFbXfWzoAXn/a-circuit-for-python-docstrings-in-a-4-layer-attention-only)
+  by Stefan Heimersheim and Jett Janiak
+* [A Toy Model of Universality](https://arxiv.org/abs/2302.03025) (ICML, 2023) by Bilal Chughtai,
+  Lawrence Chan, Neel Nanda
+* [N2G: A Scalable Approach for Quantifying Interpretable Neuron Representations in Large Language
+  Models](https://openreview.net/forum?id=ZB6bK6MTYq) (2023, ICLR Workshop RTML) by Alex Foote, Neel
+  Nanda, Esben Kran, Ioannis Konstas, Fazl Barez
+* [Eliciting Latent Predictions from Transformers with the Tuned
+  Lens](https://arxiv.org/abs/2303.08112) by Nora Belrose, Zach Furman, Logan Smith, Danny Halawi,
+  Igor Ostrovsky, Lev McKinney, Stella Biderman, Jacob Steinhardt
 
 User contributed examples of the library being used in action:
 
-- [Induction Heads Phase Change Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb): A partial replication of [In-Context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) from Connor Kissane
-- [Decision Transformer Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of scripts for training decision transformers which uses transformer lens to view intermediate activations, perform attribution and ablations. A write up of the initial work can be found [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
+* [Induction Heads Phase Change
+  Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb):
+  A partial replication of [In-Context Learning and Induction
+  Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html)
+  from Connor Kissane
+* [Decision Transformer
+  Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of
+  scripts for training decision transformers which uses transformer lens to view intermediate
+  activations, perform attribution and ablations. A write up of the initial work can be found
+  [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
 
-Check out [our demos folder](https://github.com/neelnanda-io/TransformerLens/tree/main/demos) for more examples of TransformerLens in practice
+Check out [our demos folder](https://github.com/neelnanda-io/TransformerLens/tree/main/demos) for
+more examples of TransformerLens in practice
 
 ## Getting Started in Mechanistic Interpretability
 
-Mechanistic interpretability is a very young and small field, and there are a _lot_ of open problems. This means there's both a lot of low-hanging fruit, and that the bar for entry is low - if you would like to help, please try working on one! The standard answer to "why has no one done this yet" is just that there aren't enough people! Key resources:
-
-- [A Guide to Getting Started in Mechanistic Interpretability](https://neelnanda.io/getting-started)
-- [ARENA Mechanistic Interpretability Tutorials](https://arena-ch1-transformers.streamlit.app/) from Callum McDougall. A comprehensive practical introduction to mech interp, written in TransformerLens - full of snippets to copy and they come with exercises and solutions! Notable tutorials:
-  - [Coding GPT-2 from scratch](https://arena-ch1-transformers.streamlit.app/[1.1]_Transformer_from_Scratch), with accompanying video tutorial from me ([1](https://neelnanda.io/transformer-tutorial) [2](https://neelnanda.io/transformer-tutorial-2)) - a good introduction to transformers
-  - [Introduction to Mech Interp and TransformerLens](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp): An introduction to TransformerLens and mech interp via studying induction heads. Covers the foundational concepts of the library
-  - [Indirect Object Identification](https://arena-ch1-transformers.streamlit.app/[1.3]_Indirect_Object_Identification): a replication of interpretability in the wild, that covers standard techniques in mech interp such as [direct logit attribution](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=disz2gTx-jooAcR0a5r8e7LZ), [activation patching and path patching](https://www.lesswrong.com/posts/xh85KbTFhbCz7taD4/how-to-think-about-activation-patching)
-- [Mech Interp Paper Reading List](https://neelnanda.io/paper-list)
-- [200 Concrete Open Problems in Mechanistic Interpretability](https://neelnanda.io/concrete-open-problems)
-- [A Comprehensive Mechanistic Interpretability Explainer](https://neelnanda.io/glossary): To look up all the jargon and unfamiliar terms you're going to come across!
-- [Neel Nanda's Youtube channel](https://www.youtube.com/channel/UCBMJ0D-omcRay8dh4QT0doQ): A range of mech interp video content, including [paper walkthroughs](https://www.youtube.com/watch?v=KV5gbOmHbjU&list=PL7m7hLIqA0hpsJYYhlt1WbHHgdfRLM2eY&index=1), and [walkthroughs of doing research](https://www.youtube.com/watch?v=yo4QvDn-vsU&list=PL7m7hLIqA0hr4dVOgjNwP2zjQGVHKeB7T)
+Mechanistic interpretability is a very young and small field, and there are a _lot_ of open
+problems. This means there's both a lot of low-hanging fruit, and that the bar for entry is low - if
+you would like to help, please try working on one! The standard answer to "why has no one done this
+yet" is just that there aren't enough people! Key resources:
+
+* [A Guide to Getting Started in Mechanistic Interpretability](https://neelnanda.io/getting-started)
+* [ARENA Mechanistic Interpretability Tutorials](https://arena-ch1-transformers.streamlit.app/) from
+  Callum McDougall. A comprehensive practical introduction to mech interp, written in
+  TransformerLens - full of snippets to copy and they come with exercises and solutions! Notable
+  tutorials:
+  * [Coding GPT-2 from
+    scratch](https://arena-ch1-transformers.streamlit.app/[1.1]_Transformer_from_Scratch), with
+    accompanying video tutorial from me ([1](https://neelnanda.io/transformer-tutorial)
+    [2](https://neelnanda.io/transformer-tutorial-2)) - a good introduction to transformers
+  * [Introduction to Mech Interp and
+    TransformerLens](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp): An
+    introduction to TransformerLens and mech interp via studying induction heads. Covers the
+    foundational concepts of the library
+  * [Indirect Object
+    Identification](https://arena-ch1-transformers.streamlit.app/[1.3]_Indirect_Object_Identification):
+    a replication of interpretability in the wild, that covers standard techniques in mech interp
+    such as [direct logit
+    attribution](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=disz2gTx-jooAcR0a5r8e7LZ),
+    [activation patching and path
+    patching](https://www.lesswrong.com/posts/xh85KbTFhbCz7taD4/how-to-think-about-activation-patching)
+* [Mech Interp Paper Reading List](https://neelnanda.io/paper-list)
+* [200 Concrete Open Problems in Mechanistic
+  Interpretability](https://neelnanda.io/concrete-open-problems)
+* [A Comprehensive Mechanistic Interpretability Explainer](https://neelnanda.io/glossary): To look
+  up all the jargon and unfamiliar terms you're going to come across!
+* [Neel Nanda's Youtube channel](https://www.youtube.com/channel/UCBMJ0D-omcRay8dh4QT0doQ): A range
+  of mech interp video content, including [paper
+  walkthroughs](https://www.youtube.com/watch?v=KV5gbOmHbjU&list=PL7m7hLIqA0hpsJYYhlt1WbHHgdfRLM2eY&index=1),
+  and [walkthroughs of doing
+  research](https://www.youtube.com/watch?v=yo4QvDn-vsU&list=PL7m7hLIqA0hr4dVOgjNwP2zjQGVHKeB7T)
 
 ## Support & Community
 
-If you have issues, questions, feature requests or bug reports, please search the issues to check if it's already been answered, and if not please raise an issue!
-
-You're also welcome to join the open source mech interp community on [Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA)! Please use issues for concrete discussions about the package, and Slack for higher bandwidth discussions about eg supporting important new use cases, or if you want to make substantial contributions to the library and want a maintainer's opinion. We'd also love for you to come and share your projects on the Slack!
-
-We're particularly excited to support grad students and professional researchers using TransformerLens for their work, please have a low bar for reaching out if there's ways we could better support your use case!
-
-## Background
+[![Contributing
+Guide](https://img.shields.io/badge/-Contributing%20Guide-blue?style=for-the-badge&logo=GitHub&logoColor=white)](https://neelnanda-io.github.io/TransformerLens/content/contributing.html)
 
-I (Neel Nanda) used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook!
+If you have issues, questions, feature requests or bug reports, please search the issues to check if
+it's already been answered, and if not please raise an issue!
 
-The core features were heavily inspired by the interface to [Anthropic's excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson Elhage and Chris Olah for building Garcon and showing me the value of good infrastructure for enabling exploratory research!
+You're also welcome to join the open source mech interp community on
+[Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA).
+Please use issues for concrete discussions about the package, and Slack for higher bandwidth
+discussions about eg supporting important new use cases, or if you want to make substantial
+contributions to the library and want a maintainer's opinion. We'd also love for you to come and
+share your projects on the Slack!
+
+## Credits
+
+This library was created by **[Neel Nanda](https://neelnanda.io)** and is maintained by **Joseph
+Bloom**.
+
+The core features of TransformerLens were heavily inspired by the interface to [Anthropic's
+excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson
+Elhage and Chris Olah for building Garcon and showing the value of good infrastructure for enabling
+exploratory research!
+
+### Creator's Note (Neel Nanda)
+
+I (Neel Nanda) used to work for the [Anthropic interpretability team](transformer-circuits.pub), and
+I wrote this library because after I left and tried doing independent research, I got extremely
+frustrated by the state of open source tooling. There's a lot of excellent infrastructure like
+HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals
+and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get
+into the field even if you don't work at an industry org with real infrastructure! One of the great
+things about mechanistic interpretability is that you don't need large models or tons of compute.
+There are lots of important open problems that can be solved with a small model in a Colab notebook!
 
-
-## Contributing
-
-See https://neelnanda-io.github.io/TransformerLens/content/contributing.html
-
-## Citation
+### Citation
 
 Please cite this library as:
 
 ```BibTeX
 @misc{nanda2022transformerlens,
     title = {TransformerLens},
     author = {Neel Nanda and Joseph Bloom},
     year = {2022},
     howpublished = {\url{https://github.com/neelnanda-io/TransformerLens}},
 }
-```
+```
```

### Comparing `transformer_lens-1.9.0/pyproject.toml` & `transformer_lens-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformer-lens"
-version = "v1.9.0" # This is automatically set by the CD pipeline on release
+version = "v1.9.1" # This is automatically set by the CD pipeline on release
 description = "An implementation of transformers tailored for mechanistic interpretability."
 authors = ["Neel Nanda <77788841+neelnanda-io@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "transformer_lens"}]
 
 [tool.poetry.scripts]
@@ -33,26 +33,26 @@
 # it doesn't work with Poetry. This is a known bug - the workaround is to place them manually here
 # (from the one wheel that did correctly list them). This was broken in 2.0.1 and the fix wasn't
 # made for 2.1.0, however Meta are aware of the issue and once it is fixed (and the torch version
 # requirement bumped) this should be removed. Note also the python version is used to specify that
 # this is only added where v2 torch is installed (as per the torch version requirement above).
 # https://github.com/pytorch/pytorch/issues/100974
 # https://github.com/python-poetry/poetry/issues/7902#issuecomment-1583078794
-nvidia-cuda-nvrtc-cu12 = { version = "==12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-cuda-runtime-cu12 = { version = "==12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-cuda-cupti-cu12 = { version = "==12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-cudnn-cu12 = { version = "==8.9.2.26", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-cublas-cu12 = { version = "==12.1.3.1", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-cufft-cu12 = { version = "==11.0.2.54", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-curand-cu12 = { version = "==10.3.2.106", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-cusolver-cu12 = { version = "==11.4.5.107", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-cusparse-cu12 = { version = "==12.1.0.106", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-nccl-cu12 = { version = "==2.18.1", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-nvidia-nvtx-cu12 = { version = "==12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
-triton = { version = "==2.1.0", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cuda-nvrtc-cu12 = { version = ">=12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cuda-runtime-cu12 = { version = ">=12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cuda-cupti-cu12 = { version = ">=12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cudnn-cu12 = { version = ">=8.9.2.26", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cublas-cu12 = { version = ">=12.1.3.1", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cufft-cu12 = { version = ">=11.0.2.54", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-curand-cu12 = { version = ">=10.3.2.106", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cusolver-cu12 = { version = ">=11.4.5.107", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-cusparse-cu12 = { version = ">=12.1.0.106", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-nccl-cu12 = { version = ">=2.18.1", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+nvidia-nvtx-cu12 = { version = ">=12.1.105", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
+triton = { version = ">=2.1.0", markers = "platform_system == 'Linux' and platform_machine == 'x86_64'" }
 # End PyTorch 2.1.0 Bug Fix
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 pytest-cov = ">=4.0.0"
 mypy = ">=0.991"
 jupyter = ">=1.0.0"
```

### Comparing `transformer_lens-1.9.0/transformer_lens/ActivationCache.py` & `transformer_lens-1.9.1/transformer_lens/ActivationCache.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/FactoredMatrix.py` & `transformer_lens-1.9.1/transformer_lens/FactoredMatrix.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/HookedEncoder.py` & `transformer_lens-1.9.1/transformer_lens/HookedEncoder.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/HookedTransformer.py` & `transformer_lens-1.9.1/transformer_lens/HookedTransformer.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/HookedTransformerConfig.py` & `transformer_lens-1.9.1/transformer_lens/HookedTransformerConfig.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/SVDInterpreter.py` & `transformer_lens-1.9.1/transformer_lens/SVDInterpreter.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/__init__.py` & `transformer_lens-1.9.1/transformer_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/components.py` & `transformer_lens-1.9.1/transformer_lens/components.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/evals.py` & `transformer_lens-1.9.1/transformer_lens/evals.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/head_detector.py` & `transformer_lens-1.9.1/transformer_lens/head_detector.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/hook_points.py` & `transformer_lens-1.9.1/transformer_lens/hook_points.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/loading_from_pretrained.py` & `transformer_lens-1.9.1/transformer_lens/loading_from_pretrained.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/past_key_value_caching.py` & `transformer_lens-1.9.1/transformer_lens/past_key_value_caching.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/patching.py` & `transformer_lens-1.9.1/transformer_lens/patching.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/train.py` & `transformer_lens-1.9.1/transformer_lens/train.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/utilities/devices.py` & `transformer_lens-1.9.1/transformer_lens/utilities/devices.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/transformer_lens/utils.py` & `transformer_lens-1.9.1/transformer_lens/utils.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.9.0/PKG-INFO` & `transformer_lens-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformer-lens
-Version: 1.9.0
+Version: 1.9.1
 Summary: An implementation of transformers tailored for mechanistic interpretability.
 License: MIT
 Author: Neel Nanda
 Author-email: 77788841+neelnanda-io@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,134 +17,213 @@
 Requires-Dist: datasets (>=2.7.1)
 Requires-Dist: einops (>=0.6.0)
 Requires-Dist: fancy-einsum (>=0.0.3)
 Requires-Dist: jaxtyping (>=0.2.11)
 Requires-Dist: numpy (>=1.20,<1.25) ; python_version >= "3.8" and python_version < "3.9"
 Requires-Dist: numpy (>=1.24) ; python_version >= "3.9" and python_version < "3.12"
 Requires-Dist: numpy (>=1.26) ; python_version >= "3.12" and python_version < "3.13"
-Requires-Dist: nvidia-cublas-cu12 (==12.1.3.1) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-cuda-cupti-cu12 (==12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-cuda-nvrtc-cu12 (==12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-cuda-runtime-cu12 (==12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-cudnn-cu12 (==8.9.2.26) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-cufft-cu12 (==11.0.2.54) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-curand-cu12 (==10.3.2.106) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-cusolver-cu12 (==11.4.5.107) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-cusparse-cu12 (==12.1.0.106) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-nccl-cu12 (==2.18.1) ; platform_system == "Linux" and platform_machine == "x86_64"
-Requires-Dist: nvidia-nvtx-cu12 (==12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cublas-cu12 (>=12.1.3.1) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cuda-cupti-cu12 (>=12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cuda-nvrtc-cu12 (>=12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cuda-runtime-cu12 (>=12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cudnn-cu12 (>=8.9.2.26) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cufft-cu12 (>=11.0.2.54) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-curand-cu12 (>=10.3.2.106) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cusolver-cu12 (>=11.4.5.107) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-cusparse-cu12 (>=12.1.0.106) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-nccl-cu12 (>=2.18.1) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: nvidia-nvtx-cu12 (>=12.1.105) ; platform_system == "Linux" and platform_machine == "x86_64"
 Requires-Dist: pandas (>=1.1.5)
 Requires-Dist: rich (>=12.6.0)
 Requires-Dist: torch (>=1.10)
 Requires-Dist: tqdm (>=4.64.1)
 Requires-Dist: transformers (>=4.25.1)
-Requires-Dist: triton (==2.1.0) ; platform_system == "Linux" and platform_machine == "x86_64"
+Requires-Dist: triton (>=2.1.0) ; platform_system == "Linux" and platform_machine == "x86_64"
 Requires-Dist: typing-extensions
 Requires-Dist: wandb (>=0.13.5)
 Description-Content-Type: text/markdown
 
 # TransformerLens
 
-![TransformerLens](assets/rm_transformer_lens_logo.png)
-
 <!-- Status Icons -->
 [![Pypi](https://img.shields.io/pypi/v/transformer-lens?color=blue)](https://pypi.org/project/transformer-lens/)
-![Pepy Total Downlods](https://img.shields.io/pepy/dt/transformer_lens?color=blue) ![PyPI -
-License](https://img.shields.io/pypi/l/transformer_lens?color=blue)
-[![Release CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml)
-[![Tests CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml) [![Docs CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml)
+![Pypi Total Downloads](https://img.shields.io/pepy/dt/transformer_lens?color=blue) ![PyPI -
+License](https://img.shields.io/pypi/l/transformer_lens?color=blue) [![Release
+CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/release.yml)
+[![Tests
+CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/checks.yml)
+[![Docs
+CD](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/neelnanda-io/TransformerLens/actions/workflows/gh-pages.yml)
+
+A Library for Mechanistic Interpretability of Generative Language Models.
+
+[![Read the Docs
+Here](https://img.shields.io/badge/-Read%20the%20Docs%20Here-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white&link=https://neelnanda-io.github.io/TransformerLens/)](https://neelnanda-io.github.io/TransformerLens/)
+
+This is a library for doing [mechanistic
+interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The
+goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms
+the model learned during training from its weights.
+
+TransformerLens lets you load in 50+ different open source language models, and exposes the internal
+activations of the model to you. You can cache any internal activation in the model, and add in
+functions to edit, remove or replace these activations as the model runs.
 
-This library is maintained by **Joseph Bloom** and was created by **[Neel Nanda](https://neelnanda.io)**
+~~ [OCTOBER SURVEY HERE](https://forms.gle/bw7U3PfioacDtFmT8) ~~
 
-## [Read the Docs Here](https://neelnanda-io.github.io/TransformerLens/)
+## Quick Start
 
-## Installation
+### Install
 
-Install: `pip install transformer_lens`
+```shell
+pip install transformer_lens
+```
+
+### Use
 
 ```python
 import transformer_lens
 
 # Load a model (eg GPT-2 Small)
 model = transformer_lens.HookedTransformer.from_pretrained("gpt2-small")
 
 # Run the model and get logits and activations
 logits, activations = model.run_with_cache("Hello World")
 ```
 
 ## Key Tutorials
 
-### [Introduction to the Library and Mech Interp](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp)
-
-### [Demo of Main TransformerLens Features](https://neelnanda.io/transformer-lens-demo)
-
-## A Library for Mechanistic Interpretability of Generative Language Models
-
-This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this!
-
-TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make _my_ experience of doing research easier and more fun, hopefully this transfers to you!
+* [Introduction to the Library and Mech
+  Interp](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp)
+* [Demo of Main TransformerLens Features](https://neelnanda.io/transformer-lens-demo)
 
 ## Gallery
 
 Research done involving TransformerLens:
 
-- [Progress Measures for Grokking via Mechanistic Interpretability](https://arxiv.org/abs/2301.05217) (ICLR Spotlight, 2023) by Neel Nanda, Lawrence Chan, Tom Lieberum, Jess Smith, Jacob Steinhardt
-- [Finding Neurons in a Haystack: Case Studies with Sparse Probing](https://arxiv.org/abs/2305.01610) by Wes Gurnee, Neel Nanda, Matthew Pauly, Katherine Harvey, Dmitrii Troitskii, Dimitris Bertsimas
-- [Towards Automated Circuit Discovery for Mechanistic Interpretability](https://arxiv.org/abs/2304.14997) by Arthur Conmy, Augustine N. Mavor-Parker, Aengus Lynch, Stefan Heimersheim, Adrià Garriga-Alonso
-- [Actually, Othello-GPT Has A Linear Emergent World Representation](https://neelnanda.io/othello) by Neel Nanda
-- [A circuit for Python docstrings in a 4-layer attention-only transformer](https://www.alignmentforum.org/posts/u6KXXmKFbXfWzoAXn/a-circuit-for-python-docstrings-in-a-4-layer-attention-only) by Stefan Heimersheim and Jett Janiak
-- [A Toy Model of Universality](https://arxiv.org/abs/2302.03025) (ICML, 2023) by Bilal Chughtai, Lawrence Chan, Neel Nanda
-- [N2G: A Scalable Approach for Quantifying Interpretable Neuron Representations in Large Language Models](https://openreview.net/forum?id=ZB6bK6MTYq) (2023, ICLR Workshop RTML) by Alex Foote, Neel Nanda, Esben Kran, Ioannis Konstas, Fazl Barez
-- [Eliciting Latent Predictions from Transformers with the Tuned Lens](https://arxiv.org/abs/2303.08112) by Nora Belrose, Zach Furman, Logan Smith, Danny Halawi, Igor Ostrovsky, Lev McKinney, Stella Biderman, Jacob Steinhardt
+<!-- If you change this also change docs/source/content/gallery.md -->
+* [Progress Measures for Grokking via Mechanistic
+  Interpretability](https://arxiv.org/abs/2301.05217) (ICLR Spotlight, 2023) by Neel Nanda, Lawrence
+  Chan, Tom Lieberum, Jess Smith, Jacob Steinhardt
+* [Finding Neurons in a Haystack: Case Studies with Sparse
+  Probing](https://arxiv.org/abs/2305.01610) by Wes Gurnee, Neel Nanda, Matthew Pauly, Katherine
+  Harvey, Dmitrii Troitskii, Dimitris Bertsimas
+* [Towards Automated Circuit Discovery for Mechanistic
+  Interpretability](https://arxiv.org/abs/2304.14997) by Arthur Conmy, Augustine N. Mavor-Parker,
+  Aengus Lynch, Stefan Heimersheim, Adrià Garriga-Alonso
+* [Actually, Othello-GPT Has A Linear Emergent World Representation](https://neelnanda.io/othello)
+  by Neel Nanda
+* [A circuit for Python docstrings in a 4-layer attention-only
+  transformer](https://www.alignmentforum.org/posts/u6KXXmKFbXfWzoAXn/a-circuit-for-python-docstrings-in-a-4-layer-attention-only)
+  by Stefan Heimersheim and Jett Janiak
+* [A Toy Model of Universality](https://arxiv.org/abs/2302.03025) (ICML, 2023) by Bilal Chughtai,
+  Lawrence Chan, Neel Nanda
+* [N2G: A Scalable Approach for Quantifying Interpretable Neuron Representations in Large Language
+  Models](https://openreview.net/forum?id=ZB6bK6MTYq) (2023, ICLR Workshop RTML) by Alex Foote, Neel
+  Nanda, Esben Kran, Ioannis Konstas, Fazl Barez
+* [Eliciting Latent Predictions from Transformers with the Tuned
+  Lens](https://arxiv.org/abs/2303.08112) by Nora Belrose, Zach Furman, Logan Smith, Danny Halawi,
+  Igor Ostrovsky, Lev McKinney, Stella Biderman, Jacob Steinhardt
 
 User contributed examples of the library being used in action:
 
-- [Induction Heads Phase Change Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb): A partial replication of [In-Context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) from Connor Kissane
-- [Decision Transformer Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of scripts for training decision transformers which uses transformer lens to view intermediate activations, perform attribution and ablations. A write up of the initial work can be found [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
+* [Induction Heads Phase Change
+  Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb):
+  A partial replication of [In-Context Learning and Induction
+  Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html)
+  from Connor Kissane
+* [Decision Transformer
+  Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of
+  scripts for training decision transformers which uses transformer lens to view intermediate
+  activations, perform attribution and ablations. A write up of the initial work can be found
+  [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
 
-Check out [our demos folder](https://github.com/neelnanda-io/TransformerLens/tree/main/demos) for more examples of TransformerLens in practice
+Check out [our demos folder](https://github.com/neelnanda-io/TransformerLens/tree/main/demos) for
+more examples of TransformerLens in practice
 
 ## Getting Started in Mechanistic Interpretability
 
-Mechanistic interpretability is a very young and small field, and there are a _lot_ of open problems. This means there's both a lot of low-hanging fruit, and that the bar for entry is low - if you would like to help, please try working on one! The standard answer to "why has no one done this yet" is just that there aren't enough people! Key resources:
-
-- [A Guide to Getting Started in Mechanistic Interpretability](https://neelnanda.io/getting-started)
-- [ARENA Mechanistic Interpretability Tutorials](https://arena-ch1-transformers.streamlit.app/) from Callum McDougall. A comprehensive practical introduction to mech interp, written in TransformerLens - full of snippets to copy and they come with exercises and solutions! Notable tutorials:
-  - [Coding GPT-2 from scratch](https://arena-ch1-transformers.streamlit.app/[1.1]_Transformer_from_Scratch), with accompanying video tutorial from me ([1](https://neelnanda.io/transformer-tutorial) [2](https://neelnanda.io/transformer-tutorial-2)) - a good introduction to transformers
-  - [Introduction to Mech Interp and TransformerLens](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp): An introduction to TransformerLens and mech interp via studying induction heads. Covers the foundational concepts of the library
-  - [Indirect Object Identification](https://arena-ch1-transformers.streamlit.app/[1.3]_Indirect_Object_Identification): a replication of interpretability in the wild, that covers standard techniques in mech interp such as [direct logit attribution](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=disz2gTx-jooAcR0a5r8e7LZ), [activation patching and path patching](https://www.lesswrong.com/posts/xh85KbTFhbCz7taD4/how-to-think-about-activation-patching)
-- [Mech Interp Paper Reading List](https://neelnanda.io/paper-list)
-- [200 Concrete Open Problems in Mechanistic Interpretability](https://neelnanda.io/concrete-open-problems)
-- [A Comprehensive Mechanistic Interpretability Explainer](https://neelnanda.io/glossary): To look up all the jargon and unfamiliar terms you're going to come across!
-- [Neel Nanda's Youtube channel](https://www.youtube.com/channel/UCBMJ0D-omcRay8dh4QT0doQ): A range of mech interp video content, including [paper walkthroughs](https://www.youtube.com/watch?v=KV5gbOmHbjU&list=PL7m7hLIqA0hpsJYYhlt1WbHHgdfRLM2eY&index=1), and [walkthroughs of doing research](https://www.youtube.com/watch?v=yo4QvDn-vsU&list=PL7m7hLIqA0hr4dVOgjNwP2zjQGVHKeB7T)
+Mechanistic interpretability is a very young and small field, and there are a _lot_ of open
+problems. This means there's both a lot of low-hanging fruit, and that the bar for entry is low - if
+you would like to help, please try working on one! The standard answer to "why has no one done this
+yet" is just that there aren't enough people! Key resources:
+
+* [A Guide to Getting Started in Mechanistic Interpretability](https://neelnanda.io/getting-started)
+* [ARENA Mechanistic Interpretability Tutorials](https://arena-ch1-transformers.streamlit.app/) from
+  Callum McDougall. A comprehensive practical introduction to mech interp, written in
+  TransformerLens - full of snippets to copy and they come with exercises and solutions! Notable
+  tutorials:
+  * [Coding GPT-2 from
+    scratch](https://arena-ch1-transformers.streamlit.app/[1.1]_Transformer_from_Scratch), with
+    accompanying video tutorial from me ([1](https://neelnanda.io/transformer-tutorial)
+    [2](https://neelnanda.io/transformer-tutorial-2)) - a good introduction to transformers
+  * [Introduction to Mech Interp and
+    TransformerLens](https://arena-ch1-transformers.streamlit.app/[1.2]_Intro_to_Mech_Interp): An
+    introduction to TransformerLens and mech interp via studying induction heads. Covers the
+    foundational concepts of the library
+  * [Indirect Object
+    Identification](https://arena-ch1-transformers.streamlit.app/[1.3]_Indirect_Object_Identification):
+    a replication of interpretability in the wild, that covers standard techniques in mech interp
+    such as [direct logit
+    attribution](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=disz2gTx-jooAcR0a5r8e7LZ),
+    [activation patching and path
+    patching](https://www.lesswrong.com/posts/xh85KbTFhbCz7taD4/how-to-think-about-activation-patching)
+* [Mech Interp Paper Reading List](https://neelnanda.io/paper-list)
+* [200 Concrete Open Problems in Mechanistic
+  Interpretability](https://neelnanda.io/concrete-open-problems)
+* [A Comprehensive Mechanistic Interpretability Explainer](https://neelnanda.io/glossary): To look
+  up all the jargon and unfamiliar terms you're going to come across!
+* [Neel Nanda's Youtube channel](https://www.youtube.com/channel/UCBMJ0D-omcRay8dh4QT0doQ): A range
+  of mech interp video content, including [paper
+  walkthroughs](https://www.youtube.com/watch?v=KV5gbOmHbjU&list=PL7m7hLIqA0hpsJYYhlt1WbHHgdfRLM2eY&index=1),
+  and [walkthroughs of doing
+  research](https://www.youtube.com/watch?v=yo4QvDn-vsU&list=PL7m7hLIqA0hr4dVOgjNwP2zjQGVHKeB7T)
 
 ## Support & Community
 
-If you have issues, questions, feature requests or bug reports, please search the issues to check if it's already been answered, and if not please raise an issue!
-
-You're also welcome to join the open source mech interp community on [Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA)! Please use issues for concrete discussions about the package, and Slack for higher bandwidth discussions about eg supporting important new use cases, or if you want to make substantial contributions to the library and want a maintainer's opinion. We'd also love for you to come and share your projects on the Slack!
-
-We're particularly excited to support grad students and professional researchers using TransformerLens for their work, please have a low bar for reaching out if there's ways we could better support your use case!
-
-## Background
+[![Contributing
+Guide](https://img.shields.io/badge/-Contributing%20Guide-blue?style=for-the-badge&logo=GitHub&logoColor=white)](https://neelnanda-io.github.io/TransformerLens/content/contributing.html)
 
-I (Neel Nanda) used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook!
+If you have issues, questions, feature requests or bug reports, please search the issues to check if
+it's already been answered, and if not please raise an issue!
 
-The core features were heavily inspired by the interface to [Anthropic's excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson Elhage and Chris Olah for building Garcon and showing me the value of good infrastructure for enabling exploratory research!
+You're also welcome to join the open source mech interp community on
+[Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA).
+Please use issues for concrete discussions about the package, and Slack for higher bandwidth
+discussions about eg supporting important new use cases, or if you want to make substantial
+contributions to the library and want a maintainer's opinion. We'd also love for you to come and
+share your projects on the Slack!
+
+## Credits
+
+This library was created by **[Neel Nanda](https://neelnanda.io)** and is maintained by **Joseph
+Bloom**.
+
+The core features of TransformerLens were heavily inspired by the interface to [Anthropic's
+excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson
+Elhage and Chris Olah for building Garcon and showing the value of good infrastructure for enabling
+exploratory research!
+
+### Creator's Note (Neel Nanda)
+
+I (Neel Nanda) used to work for the [Anthropic interpretability team](transformer-circuits.pub), and
+I wrote this library because after I left and tried doing independent research, I got extremely
+frustrated by the state of open source tooling. There's a lot of excellent infrastructure like
+HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals
+and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get
+into the field even if you don't work at an industry org with real infrastructure! One of the great
+things about mechanistic interpretability is that you don't need large models or tons of compute.
+There are lots of important open problems that can be solved with a small model in a Colab notebook!
 
-
-## Contributing
-
-See https://neelnanda-io.github.io/TransformerLens/content/contributing.html
-
-## Citation
+### Citation
 
 Please cite this library as:
 
 ```BibTeX
 @misc{nanda2022transformerlens,
     title = {TransformerLens},
     author = {Neel Nanda and Joseph Bloom},
     year = {2022},
     howpublished = {\url{https://github.com/neelnanda-io/TransformerLens}},
 }
 ```
+
```

