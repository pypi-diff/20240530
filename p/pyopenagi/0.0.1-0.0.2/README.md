# Comparing `tmp/pyopenagi-0.0.1-py3-none-any.whl.zip` & `tmp/pyopenagi-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 73927 bytes, number of entries: 48
+Zip file size: 73962 bytes, number of entries: 48
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 src/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 src/agents/__init__.py
 -rw-r--r--  2.0 unx     3753 b- defN 20-Feb-02 00:00 src/agents/agent_factory.py
 -rw-r--r--  2.0 unx     4356 b- defN 20-Feb-02 00:00 src/agents/agent_process.py
 -rw-r--r--  2.0 unx     5247 b- defN 20-Feb-02 00:00 src/agents/base.py
 -rw-r--r--  2.0 unx     1015 b- defN 20-Feb-02 00:00 src/agents/agent_config/AcademicAgent.json
 -rw-r--r--  2.0 unx     1022 b- defN 20-Feb-02 00:00 src/agents/agent_config/CreationAgent.json
@@ -39,12 +39,12 @@
 -rw-r--r--  2.0 unx     5173 b- defN 20-Feb-02 00:00 src/tools/online/trip_advisor/restaurant.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 src/utils/__init__.py
 -rw-r--r--  2.0 unx      535 b- defN 20-Feb-02 00:00 src/utils/compressor.py
 -rw-r--r--  2.0 unx     3131 b- defN 20-Feb-02 00:00 src/utils/logger.py
 -rw-r--r--  2.0 unx      438 b- defN 20-Feb-02 00:00 src/utils/message.py
 -rw-r--r--  2.0 unx     2768 b- defN 20-Feb-02 00:00 src/utils/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 src/utils/commands/top.py
-?rw-r--r--  2.0 unx     6797 b- defN 20-Feb-02 00:00 pyopenagi-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyopenagi-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 pyopenagi-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     4337 b- defN 20-Feb-02 00:00 pyopenagi-0.0.1.dist-info/RECORD
-48 files, 200294 bytes uncompressed, 66903 bytes compressed:  66.6%
+?rw-r--r--  2.0 unx     6902 b- defN 20-Feb-02 00:00 pyopenagi-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyopenagi-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 pyopenagi-0.0.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     4337 b- defN 20-Feb-02 00:00 pyopenagi-0.0.2.dist-info/RECORD
+48 files, 200399 bytes uncompressed, 66938 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -126,20 +126,20 @@
 
 Filename: src/utils/utils.py
 Comment: 
 
 Filename: src/utils/commands/top.py
 Comment: 
 
-Filename: pyopenagi-0.0.1.dist-info/METADATA
+Filename: pyopenagi-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pyopenagi-0.0.1.dist-info/WHEEL
+Filename: pyopenagi-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyopenagi-0.0.1.dist-info/licenses/LICENSE
+Filename: pyopenagi-0.0.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pyopenagi-0.0.1.dist-info/RECORD
+Filename: pyopenagi-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyopenagi-0.0.1.dist-info/METADATA` & `pyopenagi-0.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyopenagi
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenAGI: Package for AI Agent Creation
 Project-URL: Homepage, https://github.com/agiresearch/OpenAGI
 Project-URL: Repository, https://github.com/agiresearch/OpenAGI.git
 Project-URL: Tools Docs, https://github.com/agiresearch/OpenAGI/tools.md
 Author-email: Kai Mei <marknju2018@gmail.com>, Yongfeng Zhang <yongfeng@email.com>
 Maintainer-email: Kai Mei <marknju2018@gmail.com>, Yongfeng Zhang <yongfeng@email.com>, Balaji Rama <balajirw10@gmail.com>
 License: MIT License
@@ -50,14 +50,16 @@
 Requires-Dist: llama-index-core==0.10.36
 Requires-Dist: llama-index-embeddings-huggingface==0.2.0
 Requires-Dist: llama-index-readers-file==0.1.22
 Requires-Dist: llama-index-vector-stores-chroma==0.1.8
 Requires-Dist: numpy==1.26.4
 Requires-Dist: ollama==0.1.7
 Requires-Dist: openai==1.20.0
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.24.0
+Requires-Dist: opentelemetry-proto==1.24.0
 Requires-Dist: pandas==2.2.2
 Requires-Dist: pre-commit==3.7.0
 Requires-Dist: protobuf==5.26.1
 Requires-Dist: pydantic==2.7.0
 Requires-Dist: pympler==1.0.1
 Requires-Dist: pytest==8.1.1
 Requires-Dist: python-dotenv==1.0.0
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pyopenagi Version: 0.0.1 Summary: OpenAGI: Package
+Metadata-Version: 2.3 Name: pyopenagi Version: 0.0.2 Summary: OpenAGI: Package
 for AI Agent Creation Project-URL: Homepage, https://github.com/agiresearch/
 OpenAGI Project-URL: Repository, https://github.com/agiresearch/OpenAGI.git
 Project-URL: Tools Docs, https://github.com/agiresearch/OpenAGI/tools.md
 Author-email: Kai Mei
 gmail.com>, Yongfeng Zhang
 email.com> Maintainer-email: Kai Mei
 gmail.com>, Yongfeng Zhang
@@ -32,38 +32,39 @@
 Requires-Python: >=3.7 Requires-Dist: chromadb==0.4.23 Requires-Dist:
 click==8.1.7 Requires-Dist: google-api-python-client==2.123.0 Requires-Dist:
 googlemaps==4.10.0 Requires-Dist: langchain-community==0.0.33 Requires-Dist:
 langchain-core==0.1.43 Requires-Dist: llama-index-core==0.10.36 Requires-Dist:
 llama-index-embeddings-huggingface==0.2.0 Requires-Dist: llama-index-readers-
 file==0.1.22 Requires-Dist: llama-index-vector-stores-chroma==0.1.8 Requires-
 Dist: numpy==1.26.4 Requires-Dist: ollama==0.1.7 Requires-Dist: openai==1.20.0
-Requires-Dist: pandas==2.2.2 Requires-Dist: pre-commit==3.7.0 Requires-Dist:
-protobuf==5.26.1 Requires-Dist: pydantic==2.7.0 Requires-Dist: pympler==1.0.1
-Requires-Dist: pytest==8.1.1 Requires-Dist: python-dotenv==1.0.0 Requires-Dist:
-requests==2.31.0 Requires-Dist: torch==2.0.1 Requires-Dist:
-transformers==4.38.1 Requires-Dist: wikipedia==1.4.0 Requires-Dist:
-wolframalpha==5.0.0 Description-Content-Type: text/markdown # OpenAGI: Package
-for AI Agent Creation _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_a_p_e_r_-_P_D_F_-_r_e_d_][![Code
-License](https://img.shields.io/badge/Code%20License-MIT-green.svg)](https://
-github.com/agiresearch/OpenAGI/blob/main/LICENSE) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_C_o_m_m_u_n_i_t_y_-_D_i_s_c_o_r_d_-_8_A_2_B_E_2_]## âï¸ 1. Getting Started ### 1.1
-Installation #### (1) use OpenAGI in AIOS 1. follow [AIOS](https://github.com/
-agiresearch/AIOS) instruction to install the virtual environment 2. Allow your
-code to be able to see 'openagi' ``` $ pip install -e . ``` #### (2) use
-OpenAGI alone 1. set up virtual environment and install the required packages
-using pip ```bash conda create -n OpenAGI python=3.11 source activate OpenAGI
-cd OpenAGI pip install -r requirements.txt ``` 2. Allow your code to be able to
-see 'openagi' ``` $ pip install -e . ``` ### 1.2 Usage If you use external tool
-APIs in your agents, you can follow instructions of setting up tools in [How to
-setup external tools](./tools.md). You can also create .env file from the
-.env.example file, and then use dotenv to load the environment variables using
-.env file into your application's environment at runtime. ```bash cp
-.env.example .env ``` ## 2. Contributing Run tests: Add your test code into the
-tests/ directory if any, then run test via pytest ``` cd openagi pytest -
-v tests ``` sample output ```
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.24.0 Requires-Dist:
+opentelemetry-proto==1.24.0 Requires-Dist: pandas==2.2.2 Requires-Dist: pre-
+commit==3.7.0 Requires-Dist: protobuf==5.26.1 Requires-Dist: pydantic==2.7.0
+Requires-Dist: pympler==1.0.1 Requires-Dist: pytest==8.1.1 Requires-Dist:
+python-dotenv==1.0.0 Requires-Dist: requests==2.31.0 Requires-Dist:
+torch==2.0.1 Requires-Dist: transformers==4.38.1 Requires-Dist:
+wikipedia==1.4.0 Requires-Dist: wolframalpha==5.0.0 Description-Content-Type:
+text/markdown # OpenAGI: Package for AI Agent Creation _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_P_a_p_e_r_-_P_D_F_-_r_e_d_][![Code License](https://img.shields.io/badge/
+Code%20License-MIT-green.svg)](https://github.com/agiresearch/OpenAGI/blob/
+main/LICENSE) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_m_m_u_n_i_t_y_-_D_i_s_c_o_r_d_-_8_A_2_B_E_2_]## âï¸
+1. Getting Started ### 1.1 Installation #### (1) use OpenAGI in AIOS 1. follow
+[AIOS](https://github.com/agiresearch/AIOS) instruction to install the virtual
+environment 2. Allow your code to be able to see 'openagi' ``` $ pip install -
+e . ``` #### (2) use OpenAGI alone 1. set up virtual environment and install
+the required packages using pip ```bash conda create -n OpenAGI python=3.11
+source activate OpenAGI cd OpenAGI pip install -r requirements.txt ``` 2. Allow
+your code to be able to see 'openagi' ``` $ pip install -e . ``` ### 1.2 Usage
+If you use external tool APIs in your agents, you can follow instructions of
+setting up tools in [How to setup external tools](./tools.md). You can also
+create .env file from the .env.example file, and then use dotenv to load the
+environment variables using .env file into your application's environment at
+runtime. ```bash cp .env.example .env ``` ## 2. Contributing Run tests: Add
+your test code into the tests/ directory if any, then run test via pytest ```
+cd openagi pytest -v tests ``` sample output ```
 =============================================================================================================================
 test session starts
 ==============================================================================================================================
 platform darwin -- Python 3.11.9, pytest-8.1.1, pluggy-1.5.0 -- "" cachedir:
 .pytest_cache rootdir: "" plugins: anyio-4.3.0 collected 2 items tests/
 test_agent_creation.py::test_agent_creation PASSED [ 50%] tests/test_tools.py::
 test_currency_converter_api PASSED [100%] ``` ## ðï¸ 3. Research Please
```

## Comparing `pyopenagi-0.0.1.dist-info/licenses/LICENSE` & `pyopenagi-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pyopenagi-0.0.1.dist-info/RECORD` & `pyopenagi-0.0.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -38,11 +38,11 @@
 src/tools/online/trip_advisor/restaurant.py,sha256=TrjQQy0ytDhkY12miwosga1uRsTbPmSpAwkZGt7FyXo,5173
 src/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/utils/compressor.py,sha256=NYRfF6rGrDLLpJ9xLl7jLmlxKtQCpIEHOZK1dfeJ6io,535
 src/utils/logger.py,sha256=6ZKCFmj5YWi4dtaE2MceaCwCwq1fSceWevty1G6Tf4I,3131
 src/utils/message.py,sha256=PgkyPK8nJ-YS6X3rWkcdQzvbUmm7o3fMkKA2GPgDOB4,438
 src/utils/utils.py,sha256=HoV36lH_hLgjwntC4cI3Oib7Ck5CWRLT7u4xRiLS3mA,2768
 src/utils/commands/top.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pyopenagi-0.0.1.dist-info/METADATA,sha256=ca4QCmoA0ye7Jw3BgpkQY2x6t2T6QAE2SZyqmNgf81Q,6797
-pyopenagi-0.0.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-pyopenagi-0.0.1.dist-info/licenses/LICENSE,sha256=3EChpr20TyTBu8pP5_xFuNPlyDcPQ8F6n2R-VjJoaRg,1069
-pyopenagi-0.0.1.dist-info/RECORD,,
+pyopenagi-0.0.2.dist-info/METADATA,sha256=kV9YeWlVDHeUi7OtvikUenPCeX4bmeJcXty_1XI20xY,6902
+pyopenagi-0.0.2.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+pyopenagi-0.0.2.dist-info/licenses/LICENSE,sha256=3EChpr20TyTBu8pP5_xFuNPlyDcPQ8F6n2R-VjJoaRg,1069
+pyopenagi-0.0.2.dist-info/RECORD,,
```

