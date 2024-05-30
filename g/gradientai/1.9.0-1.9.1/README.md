# Comparing `tmp/gradientai-1.9.0.tar.gz` & `tmp/gradientai-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradientai-1.9.0.tar", max compression
+gzip compressed data, was "gradientai-1.9.1.tar", max compression
```

## Comparing `gradientai-1.9.0.tar` & `gradientai-1.9.1.tar`

### file list

```diff
@@ -1,339 +1,339 @@
--rw-r--r--   0        0        0      384 2024-01-02 22:48:19.948017 gradientai-1.9.0/README.md
--rw-r--r--   0        0        0      873 2024-01-26 22:46:41.832392 gradientai-1.9.0/gradientai/__init__.py
--rw-r--r--   0        0        0     2237 2024-01-26 22:46:41.832503 gradientai-1.9.0/gradientai/__init__.pyi
--rw-r--r--   0        0        0     2686 2024-01-26 22:46:41.832628 gradientai-1.9.0/gradientai/_base_model.py
--rw-r--r--   0        0        0     3984 2024-01-02 22:48:19.948502 gradientai-1.9.0/gradientai/_embeddings_model.py
--rw-r--r--   0        0        0    16178 2024-04-03 23:04:21.105909 gradientai-1.9.0/gradientai/_gradient.py
--rw-r--r--   0        0        0     2333 2024-04-03 00:11:07.185923 gradientai-1.9.0/gradientai/_model.py
--rw-r--r--   0        0        0     3510 2023-10-24 19:44:32.688189 gradientai-1.9.0/gradientai/_model_adapter.py
--rw-r--r--   0        0        0     1748 2024-04-03 23:04:21.106074 gradientai-1.9.0/gradientai/_rag.py
--rw-r--r--   0        0        0     2497 2024-04-02 16:51:03.746721 gradientai-1.9.0/gradientai/_types.py
--rw-r--r--   0        0        0      730 2024-01-02 22:48:19.948773 gradientai-1.9.0/gradientai/helpers/asyncio_threads.py
--rw-r--r--   0        0        0     2155 2023-09-11 18:57:16.856296 gradientai-1.9.0/gradientai/helpers/env_manager.py
--rw-r--r--   0        0        0        0 2024-04-02 21:06:10.508888 gradientai-1.9.0/gradientai/openapi/__init__.py
--rw-r--r--   0        0        0    11944 2024-04-02 23:02:40.025793 gradientai-1.9.0/gradientai/openapi/client/__init__.py
--rw-r--r--   0        0        0      363 2024-04-02 23:02:40.025926 gradientai-1.9.0/gradientai/openapi/client/api/__init__.py
--rw-r--r--   0        0        0    59385 2024-04-02 21:06:10.436752 gradientai-1.9.0/gradientai/openapi/client/api/blocks_api.py
--rw-r--r--   0        0        0    15138 2024-04-02 21:06:10.456255 gradientai-1.9.0/gradientai/openapi/client/api/embeddings_api.py
--rw-r--r--   0        0        0     8147 2024-04-02 21:06:10.464141 gradientai-1.9.0/gradientai/openapi/client/api/files_api.py
--rw-r--r--   0        0        0    43721 2024-04-02 21:06:10.473572 gradientai-1.9.0/gradientai/openapi/client/api/models_api.py
--rw-r--r--   0        0        0    16242 2024-04-02 23:02:40.026264 gradientai-1.9.0/gradientai/openapi/client/api/rag_api.py
--rw-r--r--   0        0        0    30160 2024-04-02 21:06:10.517186 gradientai-1.9.0/gradientai/openapi/client/api_client.py
--rw-r--r--   0        0        0      844 2024-04-02 21:06:10.519343 gradientai-1.9.0/gradientai/openapi/client/api_response.py
--rw-r--r--   0        0        0    14896 2024-04-02 21:06:10.495099 gradientai-1.9.0/gradientai/openapi/client/configuration.py
--rw-r--r--   0        0        0     1259 2024-04-02 23:02:40.026440 gradientai-1.9.0/gradientai/openapi/client/docs/AddFilesToRagCollectionBodyParams.md
--rw-r--r--   0        0        0     1101 2024-04-02 23:02:40.026527 gradientai-1.9.0/gradientai/openapi/client/docs/AddFilesToRagCollectionError.md
--rw-r--r--   0        0        0     1294 2024-04-02 21:06:08.817381 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md
--rw-r--r--   0        0        0     1275 2024-04-02 21:06:08.859982 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md
--rw-r--r--   0        0        0      989 2024-04-02 21:06:08.888938 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentError.md
--rw-r--r--   0        0        0     1017 2024-04-02 21:06:09.017017 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md
--rw-r--r--   0        0        0      935 2024-04-02 21:06:09.077859 gradientai-1.9.0/gradientai/openapi/client/docs/BaseModel.md
--rw-r--r--   0        0        0    23913 2024-04-02 21:06:10.452912 gradientai-1.9.0/gradientai/openapi/client/docs/BlocksApi.md
--rw-r--r--   0        0        0     2065 2024-04-02 21:06:09.106119 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParams.md
--rw-r--r--   0        0        0     1226 2024-04-02 21:06:09.173646 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md
--rw-r--r--   0        0        0     1153 2024-04-02 21:06:09.300783 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md
--rw-r--r--   0        0        0     1069 2024-04-02 21:06:09.338931 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelError.md
--rw-r--r--   0        0        0     1146 2024-04-02 21:06:09.380345 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md
--rw-r--r--   0        0        0     1161 2024-04-02 21:06:09.414975 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md
--rw-r--r--   0        0        0     1080 2024-04-02 21:06:09.450202 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md
--rw-r--r--   0        0        0     1224 2024-04-02 21:06:09.525750 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md
--rw-r--r--   0        0        0     1161 2024-04-02 21:06:09.547399 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md
--rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.569264 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md
--rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.585117 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md
--rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.601035 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md
--rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.613596 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md
--rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.630346 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md
--rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.652113 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md
--rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.675322 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md
--rw-r--r--   0        0        0     1243 2024-04-02 21:06:09.694265 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md
--rw-r--r--   0        0        0     1394 2024-04-02 21:06:09.713760 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md
--rw-r--r--   0        0        0     1019 2024-04-02 21:06:09.728650 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelSuccess.md
--rw-r--r--   0        0        0     1172 2024-04-02 21:06:09.749173 gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionBodyParams.md
--rw-r--r--   0        0        0     1100 2024-04-02 21:06:09.763865 gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionError.md
--rw-r--r--   0        0        0     1135 2024-04-02 21:06:09.782221 gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionSuccess.md
--rw-r--r--   0        0        0     1195 2024-04-02 21:06:09.799851 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParams.md
--rw-r--r--   0        0        0     1622 2024-04-02 21:06:09.808092 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md
--rw-r--r--   0        0        0     1565 2024-04-02 21:06:09.814804 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md
--rw-r--r--   0        0        0     1550 2024-04-02 21:06:09.823247 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md
--rw-r--r--   0        0        0     1219 2024-04-02 21:06:09.830872 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md
--rw-r--r--   0        0        0      924 2024-04-02 21:06:09.838966 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelError.md
--rw-r--r--   0        0        0      945 2024-04-02 21:06:09.847442 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelSuccess.md
--rw-r--r--   0        0        0     1254 2024-04-02 23:02:40.026608 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionBodyParams.md
--rw-r--r--   0        0        0     1271 2024-04-02 23:02:40.026699 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionBodyParamsFilesInner.md
--rw-r--r--   0        0        0     1035 2024-04-02 23:02:40.026778 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionError.md
--rw-r--r--   0        0        0     1056 2024-04-02 23:02:40.026848 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionSuccess.md
--rw-r--r--   0        0        0      924 2024-04-02 21:06:09.922306 gradientai-1.9.0/gradientai/openapi/client/docs/DeleteModelError.md
--rw-r--r--   0        0        0     5995 2024-04-02 21:06:10.460915 gradientai-1.9.0/gradientai/openapi/client/docs/EmbeddingsApi.md
--rw-r--r--   0        0        0     1218 2024-04-02 21:06:09.930543 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParams.md
--rw-r--r--   0        0        0     1235 2024-04-02 21:06:09.942847 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md
--rw-r--r--   0        0        0      950 2024-04-02 21:06:09.951498 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityError.md
--rw-r--r--   0        0        0     1052 2024-04-02 21:06:09.958892 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccess.md
--rw-r--r--   0        0        0     1105 2024-04-02 21:06:09.968200 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md
--rw-r--r--   0        0        0      911 2024-04-02 21:06:09.974240 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfError.md
--rw-r--r--   0        0        0     1050 2024-04-02 21:06:09.980697 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccess.md
--rw-r--r--   0        0        0     1462 2024-04-02 21:06:09.989400 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md
--rw-r--r--   0        0        0     1262 2024-04-02 21:06:09.999431 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md
--rw-r--r--   0        0        0     1380 2024-04-02 21:06:10.006871 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md
--rw-r--r--   0        0        0     1598 2024-04-02 21:06:10.015894 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md
--rw-r--r--   0        0        0     1646 2024-04-02 21:06:10.022832 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md
--rw-r--r--   0        0        0     1326 2024-04-02 21:06:10.029202 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md
--rw-r--r--   0        0        0     2801 2024-04-02 21:06:10.469329 gradientai-1.9.0/gradientai/openapi/client/docs/FilesApi.md
--rw-r--r--   0        0        0     1109 2024-04-02 21:06:10.036440 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParams.md
--rw-r--r--   0        0        0     1452 2024-04-02 21:06:10.042021 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md
--rw-r--r--   0        0        0     1496 2024-04-02 21:06:10.048829 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md
--rw-r--r--   0        0        0     1256 2024-04-02 21:06:10.057143 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md
--rw-r--r--   0        0        0     1562 2024-04-02 21:06:10.064934 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md
--rw-r--r--   0        0        0     1076 2024-04-02 21:06:10.072608 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelError.md
--rw-r--r--   0        0        0     1061 2024-04-02 21:06:10.078529 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md
--rw-r--r--   0        0        0     1074 2024-04-02 21:06:10.085792 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md
--rw-r--r--   0        0        0     1033 2024-04-02 21:06:10.092123 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelSuccess.md
--rw-r--r--   0        0        0     1127 2024-04-02 21:06:10.101646 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md
--rw-r--r--   0        0        0     1177 2024-04-02 21:06:10.134519 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md
--rw-r--r--   0        0        0     1290 2024-04-02 21:06:10.146161 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md
--rw-r--r--   0        0        0     1290 2024-04-02 21:06:10.154510 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md
--rw-r--r--   0        0        0      963 2024-04-02 21:06:10.162634 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerError.md
--rw-r--r--   0        0        0     1097 2024-04-02 21:06:10.169665 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccess.md
--rw-r--r--   0        0        0     1235 2024-04-02 21:06:10.176849 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md
--rw-r--r--   0        0        0     1359 2024-04-02 21:06:10.183918 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md
--rw-r--r--   0        0        0     1159 2024-04-02 21:06:10.192220 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md
--rw-r--r--   0        0        0     1229 2024-04-02 21:06:10.199299 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md
--rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.209914 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingError.md
--rw-r--r--   0        0        0     1119 2024-04-02 21:06:10.219023 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md
--rw-r--r--   0        0        0     1273 2024-04-02 21:06:10.225005 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md
--rw-r--r--   0        0        0     1061 2024-04-02 21:06:10.230449 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionError.md
--rw-r--r--   0        0        0     1197 2024-04-02 21:06:10.238093 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccess.md
--rw-r--r--   0        0        0     1195 2024-04-02 21:06:10.243126 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf.md
--rw-r--r--   0        0        0     1289 2024-04-02 21:06:10.248549 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1.md
--rw-r--r--   0        0        0     1261 2024-04-02 21:06:10.254570 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1Result.md
--rw-r--r--   0        0        0      885 2024-04-02 21:06:10.260434 gradientai-1.9.0/gradientai/openapi/client/docs/GetModelError.md
--rw-r--r--   0        0        0     1034 2024-04-02 21:06:10.266339 gradientai-1.9.0/gradientai/openapi/client/docs/GetModelSuccess.md
--rw-r--r--   0        0        0      963 2024-04-02 21:06:10.273428 gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsError.md
--rw-r--r--   0        0        0     1093 2024-04-02 21:06:10.278509 gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md
--rw-r--r--   0        0        0     1280 2024-04-02 21:06:10.286179 gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md
--rw-r--r--   0        0        0      911 2024-04-02 21:06:10.291565 gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsError.md
--rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.297535 gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccess.md
--rw-r--r--   0        0        0     1281 2024-04-02 21:06:10.303477 gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md
--rw-r--r--   0        0        0      988 2024-04-02 21:06:10.309052 gradientai-1.9.0/gradientai/openapi/client/docs/ModelAdapter.md
--rw-r--r--   0        0        0    17156 2024-04-02 21:06:10.478620 gradientai-1.9.0/gradientai/openapi/client/docs/ModelsApi.md
--rw-r--r--   0        0        0     1258 2024-04-02 21:06:10.313692 gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md
--rw-r--r--   0        0        0     1028 2024-04-02 21:06:10.319260 gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentError.md
--rw-r--r--   0        0        0     1068 2024-04-02 21:06:10.325029 gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md
--rw-r--r--   0        0        0     6299 2024-04-02 23:02:40.027022 gradientai-1.9.0/gradientai/openapi/client/docs/RAGApi.md
--rw-r--r--   0        0        0     1347 2024-04-02 21:06:10.331891 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md
--rw-r--r--   0        0        0     1286 2024-04-02 21:06:10.337363 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md
--rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.343168 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentError.md
--rw-r--r--   0        0        0     1028 2024-04-02 21:06:10.348221 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md
--rw-r--r--   0        0        0      911 2024-04-02 21:06:10.356695 gradientai-1.9.0/gradientai/openapi/client/docs/UploadFileError.md
--rw-r--r--   0        0        0      932 2024-04-02 21:06:10.363682 gradientai-1.9.0/gradientai/openapi/client/docs/UploadFileSuccess.md
--rw-r--r--   0        0        0     5323 2024-04-02 21:06:10.512625 gradientai-1.9.0/gradientai/openapi/client/exceptions.py
--rw-r--r--   0        0        0    11009 2024-04-02 23:02:40.027183 gradientai-1.9.0/gradientai/openapi/client/models/__init__.py
--rw-r--r--   0        0        0     3166 2024-04-03 23:04:21.106342 gradientai-1.9.0/gradientai/openapi/client/models/add_files_to_rag_collection_body_params.py
--rw-r--r--   0        0        0     2557 2024-04-02 23:02:40.027355 gradientai-1.9.0/gradientai/openapi/client/models/add_files_to_rag_collection_error.py
--rw-r--r--   0        0        0     3617 2024-04-02 21:06:08.792526 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params.py
--rw-r--r--   0        0        0     3053 2024-04-02 21:06:08.847811 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py
--rw-r--r--   0        0        0     2501 2024-04-02 21:06:08.872357 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_error.py
--rw-r--r--   0        0        0     2799 2024-04-02 21:06:08.904229 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_success.py
--rw-r--r--   0        0        0     3400 2024-04-02 21:06:09.034106 gradientai-1.9.0/gradientai/openapi/client/models/base_model.py
--rw-r--r--   0        0        0     6500 2024-04-02 21:06:09.090984 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params.py
--rw-r--r--   0        0        0     3043 2024-04-02 21:06:09.144530 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_guidance.py
--rw-r--r--   0        0        0     2680 2024-04-02 21:06:09.246459 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_rag.py
--rw-r--r--   0        0        0    13624 2024-04-02 21:06:09.326952 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error.py
--rw-r--r--   0        0        0     3793 2024-04-02 21:06:09.357221 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of.py
--rw-r--r--   0        0        0     3887 2024-04-02 21:06:09.397688 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1.py
--rw-r--r--   0        0        0     2885 2024-04-02 21:06:09.433031 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of10.py
--rw-r--r--   0        0        0     3347 2024-04-02 21:06:09.509206 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py
--rw-r--r--   0        0        0     3361 2024-04-02 21:06:09.534327 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of2.py
--rw-r--r--   0        0        0     2849 2024-04-02 21:06:09.557641 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of3.py
--rw-r--r--   0        0        0     2891 2024-04-02 21:06:09.576512 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of4.py
--rw-r--r--   0        0        0     2875 2024-04-02 21:06:09.591719 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of5.py
--rw-r--r--   0        0        0     2887 2024-04-02 21:06:09.606721 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of6.py
--rw-r--r--   0        0        0     2869 2024-04-02 21:06:09.620763 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of7.py
--rw-r--r--   0        0        0     2875 2024-04-02 21:06:09.640394 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of8.py
--rw-r--r--   0        0        0     2877 2024-04-02 21:06:09.666604 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of9.py
--rw-r--r--   0        0        0     3281 2024-04-02 21:06:09.686784 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload.py
--rw-r--r--   0        0        0     2700 2024-04-02 21:06:09.705656 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py
--rw-r--r--   0        0        0     2665 2024-04-02 21:06:09.722372 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_success.py
--rw-r--r--   0        0        0     2619 2024-04-02 21:06:09.739180 gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_body_params.py
--rw-r--r--   0        0        0     2565 2024-04-02 21:06:09.755475 gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_error.py
--rw-r--r--   0        0        0     2640 2024-04-02 21:06:09.770734 gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_success.py
--rw-r--r--   0        0        0     3807 2024-04-02 21:06:09.790028 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params.py
--rw-r--r--   0        0        0     4559 2024-04-02 21:06:09.803767 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py
--rw-r--r--   0        0        0     3018 2024-04-02 21:06:09.811376 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
--rw-r--r--   0        0        0     3165 2024-04-02 21:06:09.819303 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py
--rw-r--r--   0        0        0     2836 2024-04-02 21:06:09.826269 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_model.py
--rw-r--r--   0        0        0     2461 2024-04-02 21:06:09.834119 gradientai-1.9.0/gradientai/openapi/client/models/create_model_error.py
--rw-r--r--   0        0        0     2457 2024-04-02 21:06:09.842823 gradientai-1.9.0/gradientai/openapi/client/models/create_model_success.py
--rw-r--r--   0        0        0     3788 2024-04-02 23:02:40.027441 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_body_params.py
--rw-r--r--   0        0        0     2727 2024-04-02 23:02:40.027522 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_body_params_files_inner.py
--rw-r--r--   0        0        0     2525 2024-04-02 23:02:40.027595 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_error.py
--rw-r--r--   0        0        0     2521 2024-04-02 23:02:40.027660 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_success.py
--rw-r--r--   0        0        0     2461 2024-04-02 21:06:09.918218 gradientai-1.9.0/gradientai/openapi/client/models/delete_model_error.py
--rw-r--r--   0        0        0     3456 2024-04-02 21:06:09.926059 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params.py
--rw-r--r--   0        0        0     3228 2024-04-02 21:06:09.936371 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py
--rw-r--r--   0        0        0     2477 2024-04-02 21:06:09.946388 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_error.py
--rw-r--r--   0        0        0     3136 2024-04-02 21:06:09.955137 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success.py
--rw-r--r--   0        0        0     5870 2024-04-02 21:06:09.964168 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success_entity_value.py
--rw-r--r--   0        0        0     2453 2024-04-02 21:06:09.971377 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_error.py
--rw-r--r--   0        0        0     3365 2024-04-02 21:06:09.976832 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success.py
--rw-r--r--   0        0        0     4761 2024-04-02 21:06:09.985105 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py
--rw-r--r--   0        0        0     2937 2024-04-02 21:06:09.995158 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py
--rw-r--r--   0        0        0     3397 2024-04-02 21:06:10.003745 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py
--rw-r--r--   0        0        0     3774 2024-04-02 21:06:10.009350 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
--rw-r--r--   0        0        0     3545 2024-04-02 21:06:10.019368 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
--rw-r--r--   0        0        0     3065 2024-04-02 21:06:10.025975 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py
--rw-r--r--   0        0        0     3075 2024-04-02 21:06:10.032424 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params.py
--rw-r--r--   0        0        0     4023 2024-04-02 21:06:10.039042 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py
--rw-r--r--   0        0        0     3056 2024-04-02 21:06:10.044989 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
--rw-r--r--   0        0        0     5780 2024-04-02 21:06:10.053458 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py
--rw-r--r--   0        0        0     3137 2024-04-02 21:06:10.061882 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
--rw-r--r--   0        0        0    10150 2024-04-02 21:06:10.068980 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error.py
--rw-r--r--   0        0        0     2881 2024-04-02 21:06:10.075247 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of.py
--rw-r--r--   0        0        0     2851 2024-04-02 21:06:10.081189 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py
--rw-r--r--   0        0        0     2748 2024-04-02 21:06:10.088300 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_success.py
--rw-r--r--   0        0        0     2993 2024-04-02 21:06:10.098254 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params.py
--rw-r--r--   0        0        0     6307 2024-04-02 21:06:10.105052 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source.py
--rw-r--r--   0        0        0     3023 2024-04-02 21:06:10.138849 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py
--rw-r--r--   0        0        0     2959 2024-04-02 21:06:10.149368 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py
--rw-r--r--   0        0        0     2485 2024-04-02 21:06:10.157233 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_error.py
--rw-r--r--   0        0        0     3047 2024-04-02 21:06:10.165942 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success.py
--rw-r--r--   0        0        0     3197 2024-04-02 21:06:10.173414 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context.py
--rw-r--r--   0        0        0     2831 2024-04-02 21:06:10.179649 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py
--rw-r--r--   0        0        0     3137 2024-04-02 21:06:10.188248 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params.py
--rw-r--r--   0        0        0     2629 2024-04-02 21:06:10.194657 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py
--rw-r--r--   0        0        0     2509 2024-04-02 21:06:10.205377 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_error.py
--rw-r--r--   0        0        0     3124 2024-04-02 21:06:10.214647 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success.py
--rw-r--r--   0        0        0     2802 2024-04-02 21:06:10.221585 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py
--rw-r--r--   0        0        0     2541 2024-04-02 21:06:10.227642 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_error.py
--rw-r--r--   0        0        0     6225 2024-04-02 21:06:10.233896 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success.py
--rw-r--r--   0        0        0     3230 2024-04-02 21:06:10.240370 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of.py
--rw-r--r--   0        0        0     3331 2024-04-02 21:06:10.245238 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of1.py
--rw-r--r--   0        0        0     2620 2024-04-02 21:06:10.251490 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of1_result.py
--rw-r--r--   0        0        0     2437 2024-04-02 21:06:10.256772 gradientai-1.9.0/gradientai/openapi/client/models/get_model_error.py
--rw-r--r--   0        0        0     3226 2024-04-02 21:06:10.262685 gradientai-1.9.0/gradientai/openapi/client/models/get_model_success.py
--rw-r--r--   0        0        0     2485 2024-04-02 21:06:10.269520 gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_error.py
--rw-r--r--   0        0        0     3198 2024-04-02 21:06:10.275832 gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success.py
--rw-r--r--   0        0        0     2877 2024-04-02 21:06:10.281153 gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py
--rw-r--r--   0        0        0     2453 2024-04-02 21:06:10.288818 gradientai-1.9.0/gradientai/openapi/client/models/list_models_error.py
--rw-r--r--   0        0        0     2988 2024-04-02 21:06:10.294142 gradientai-1.9.0/gradientai/openapi/client/models/list_models_success.py
--rw-r--r--   0        0        0     6222 2024-04-02 21:06:10.300547 gradientai-1.9.0/gradientai/openapi/client/models/list_models_success_models_inner.py
--rw-r--r--   0        0        0     3202 2024-04-02 21:06:10.306093 gradientai-1.9.0/gradientai/openapi/client/models/model_adapter.py
--rw-r--r--   0        0        0     2910 2024-04-02 21:06:10.311164 gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_body_params.py
--rw-r--r--   0        0        0     2525 2024-04-02 21:06:10.316119 gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_error.py
--rw-r--r--   0        0        0     2625 2024-04-02 21:06:10.322296 gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_success.py
--rw-r--r--   0        0        0     4281 2024-04-02 21:06:10.327645 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params.py
--rw-r--r--   0        0        0     2771 2024-04-02 21:06:10.334291 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py
--rw-r--r--   0        0        0     2509 2024-04-02 21:06:10.339705 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_error.py
--rw-r--r--   0        0        0     2525 2024-04-02 21:06:10.345591 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_success.py
--rw-r--r--   0        0        0     2453 2024-04-02 21:06:10.353564 gradientai-1.9.0/gradientai/openapi/client/models/upload_file_error.py
--rw-r--r--   0        0        0     2449 2024-04-02 21:06:10.360525 gradientai-1.9.0/gradientai/openapi/client/models/upload_file_success.py
--rw-r--r--   0        0        0    12904 2024-04-02 21:06:10.522227 gradientai-1.9.0/gradientai/openapi/client/rest.py
--rw-r--r--   0        0        0        0 2024-04-02 21:06:10.513888 gradientai-1.9.0/gradientai/openapi/client/test/__init__.py
--rw-r--r--   0        0        0     2273 2024-04-02 23:02:40.027750 gradientai-1.9.0/gradientai/openapi/client/test/test_add_files_to_rag_collection_body_params.py
--rw-r--r--   0        0        0     1745 2024-04-02 23:02:40.027813 gradientai-1.9.0/gradientai/openapi/client/test/test_add_files_to_rag_collection_error.py
--rw-r--r--   0        0        0     2004 2024-04-02 21:06:08.808961 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py
--rw-r--r--   0        0        0     1960 2024-04-02 21:06:08.854945 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py
--rw-r--r--   0        0        0     1655 2024-04-02 21:06:08.881571 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_error.py
--rw-r--r--   0        0        0     1697 2024-04-02 21:06:08.967099 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_success.py
--rw-r--r--   0        0        0     2039 2024-04-02 21:06:09.063993 gradientai-1.9.0/gradientai/openapi/client/test/test_base_model.py
--rw-r--r--   0        0        0     1980 2024-04-02 21:06:10.439861 gradientai-1.9.0/gradientai/openapi/client/test/test_blocks_api.py
--rw-r--r--   0        0        0     2280 2024-04-02 21:06:09.099603 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params.py
--rw-r--r--   0        0        0     1930 2024-04-02 21:06:09.164507 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py
--rw-r--r--   0        0        0     1731 2024-04-02 21:06:09.292954 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_rag.py
--rw-r--r--   0        0        0     2177 2024-04-02 21:06:09.333291 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error.py
--rw-r--r--   0        0        0     2591 2024-04-02 21:06:09.371930 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of.py
--rw-r--r--   0        0        0     2257 2024-04-02 21:06:09.406401 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1.py
--rw-r--r--   0        0        0     1802 2024-04-02 21:06:09.441943 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of10.py
--rw-r--r--   0        0        0     1812 2024-04-02 21:06:09.518575 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py
--rw-r--r--   0        0        0     2271 2024-04-02 21:06:09.542666 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of2.py
--rw-r--r--   0        0        0     1762 2024-04-02 21:06:09.564892 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of3.py
--rw-r--r--   0        0        0     1804 2024-04-02 21:06:09.581061 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of4.py
--rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.598195 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of5.py
--rw-r--r--   0        0        0     1800 2024-04-02 21:06:09.610916 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of6.py
--rw-r--r--   0        0        0     1782 2024-04-02 21:06:09.625548 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of7.py
--rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.648082 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of8.py
--rw-r--r--   0        0        0     1790 2024-04-02 21:06:09.671711 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of9.py
--rw-r--r--   0        0        0     2235 2024-04-02 21:06:09.691977 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py
--rw-r--r--   0        0        0     1999 2024-04-02 21:06:09.710627 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py
--rw-r--r--   0        0        0     1732 2024-04-02 21:06:09.725385 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_success.py
--rw-r--r--   0        0        0     1815 2024-04-02 21:06:09.747060 gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_body_params.py
--rw-r--r--   0        0        0     1753 2024-04-02 21:06:09.758952 gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_error.py
--rw-r--r--   0        0        0     1795 2024-04-02 21:06:09.778352 gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_success.py
--rw-r--r--   0        0        0     2659 2024-04-02 21:06:09.796918 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params.py
--rw-r--r--   0        0        0     2349 2024-04-02 21:06:09.806264 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py
--rw-r--r--   0        0        0     2121 2024-04-02 21:06:09.813285 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
--rw-r--r--   0        0        0     2106 2024-04-02 21:06:09.821729 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py
--rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.828921 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_model.py
--rw-r--r--   0        0        0     1595 2024-04-02 21:06:09.836385 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_error.py
--rw-r--r--   0        0        0     1609 2024-04-02 21:06:09.845646 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_success.py
--rw-r--r--   0        0        0     2087 2024-04-02 23:02:40.027879 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_body_params.py
--rw-r--r--   0        0        0     1926 2024-04-02 23:02:40.027954 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_body_params_files_inner.py
--rw-r--r--   0        0        0     1693 2024-04-02 23:02:40.028029 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_error.py
--rw-r--r--   0        0        0     1707 2024-04-02 23:02:40.028100 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_success.py
--rw-r--r--   0        0        0     1595 2024-04-02 21:06:09.920600 gradientai-1.9.0/gradientai/openapi/client/test/test_delete_model_error.py
--rw-r--r--   0        0        0     1087 2024-04-02 21:06:10.458193 gradientai-1.9.0/gradientai/openapi/client/test/test_embeddings_api.py
--rw-r--r--   0        0        0     2242 2024-04-02 21:06:09.928651 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params.py
--rw-r--r--   0        0        0     1857 2024-04-02 21:06:09.940584 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py
--rw-r--r--   0        0        0     1619 2024-04-02 21:06:09.949460 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_error.py
--rw-r--r--   0        0        0     1747 2024-04-02 21:06:09.957081 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success.py
--rw-r--r--   0        0        0     1718 2024-04-02 21:06:09.966737 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py
--rw-r--r--   0        0        0     1583 2024-04-02 21:06:09.973033 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_error.py
--rw-r--r--   0        0        0     5829 2024-04-02 21:06:09.979063 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success.py
--rw-r--r--   0        0        0     5055 2024-04-02 21:06:09.987342 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py
--rw-r--r--   0        0        0     1938 2024-04-02 21:06:09.997669 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py
--rw-r--r--   0        0        0     3256 2024-04-02 21:06:10.005551 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py
--rw-r--r--   0        0        0     2800 2024-04-02 21:06:10.010890 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
--rw-r--r--   0        0        0     2291 2024-04-02 21:06:10.021591 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
--rw-r--r--   0        0        0     2066 2024-04-02 21:06:10.027698 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py
--rw-r--r--   0        0        0      876 2024-04-02 21:06:10.466006 gradientai-1.9.0/gradientai/openapi/client/test/test_files_api.py
--rw-r--r--   0        0        0     2583 2024-04-02 21:06:10.034445 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params.py
--rw-r--r--   0        0        0     2070 2024-04-02 21:06:10.040640 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py
--rw-r--r--   0        0        0     2047 2024-04-02 21:06:10.047326 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
--rw-r--r--   0        0        0     1844 2024-04-02 21:06:10.055514 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py
--rw-r--r--   0        0        0     2108 2024-04-02 21:06:10.063530 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
--rw-r--r--   0        0        0     2183 2024-04-02 21:06:10.071132 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error.py
--rw-r--r--   0        0        0     1792 2024-04-02 21:06:10.077033 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py
--rw-r--r--   0        0        0     1766 2024-04-02 21:06:10.084327 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py
--rw-r--r--   0        0        0     1748 2024-04-02 21:06:10.090376 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_success.py
--rw-r--r--   0        0        0     1758 2024-04-02 21:06:10.100215 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params.py
--rw-r--r--   0        0        0     1899 2024-04-02 21:06:10.125636 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source.py
--rw-r--r--   0        0        0     1904 2024-04-02 21:06:10.144238 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py
--rw-r--r--   0        0        0     1910 2024-04-02 21:06:10.152562 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py
--rw-r--r--   0        0        0     1631 2024-04-02 21:06:10.159600 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_error.py
--rw-r--r--   0        0        0     2101 2024-04-02 21:06:10.167754 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success.py
--rw-r--r--   0        0        0     2299 2024-04-02 21:06:10.175433 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py
--rw-r--r--   0        0        0     2018 2024-04-02 21:06:10.182073 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py
--rw-r--r--   0        0        0     2123 2024-04-02 21:06:10.190615 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params.py
--rw-r--r--   0        0        0     1861 2024-04-02 21:06:10.197672 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py
--rw-r--r--   0        0        0     1667 2024-04-02 21:06:10.207994 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_error.py
--rw-r--r--   0        0        0     2299 2024-04-02 21:06:10.217113 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success.py
--rw-r--r--   0        0        0     2026 2024-04-02 21:06:10.223798 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py
--rw-r--r--   0        0        0     1717 2024-04-02 21:06:10.229190 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_error.py
--rw-r--r--   0        0        0     2126 2024-04-02 21:06:10.236708 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success.py
--rw-r--r--   0        0        0     1882 2024-04-02 21:06:10.241895 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of.py
--rw-r--r--   0        0        0     2202 2024-04-02 21:06:10.246805 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1.py
--rw-r--r--   0        0        0     1883 2024-04-02 21:06:10.253414 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1_result.py
--rw-r--r--   0        0        0     1559 2024-04-02 21:06:10.258844 gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_error.py
--rw-r--r--   0        0        0     2193 2024-04-02 21:06:10.264578 gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_success.py
--rw-r--r--   0        0        0     1631 2024-04-02 21:06:10.272082 gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_error.py
--rw-r--r--   0        0        0     2101 2024-04-02 21:06:10.277361 gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success.py
--rw-r--r--   0        0        0     1923 2024-04-02 21:06:10.284407 gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py
--rw-r--r--   0        0        0     1583 2024-04-02 21:06:10.290426 gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_error.py
--rw-r--r--   0        0        0     1695 2024-04-02 21:06:10.296286 gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success.py
--rw-r--r--   0        0        0     2579 2024-04-02 21:06:10.302172 gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success_models_inner.py
--rw-r--r--   0        0        0     2155 2024-04-02 21:06:10.307900 gradientai-1.9.0/gradientai/openapi/client/test/test_model_adapter.py
--rw-r--r--   0        0        0     1568 2024-04-02 21:06:10.475138 gradientai-1.9.0/gradientai/openapi/client/test/test_models_api.py
--rw-r--r--   0        0        0     1844 2024-04-02 21:06:10.312637 gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_body_params.py
--rw-r--r--   0        0        0     1691 2024-04-02 21:06:10.317720 gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_error.py
--rw-r--r--   0        0        0     1743 2024-04-02 21:06:10.323929 gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_success.py
--rw-r--r--   0        0        0     1066 2024-04-02 23:02:40.028172 gradientai-1.9.0/gradientai/openapi/client/test/test_rag_api.py
--rw-r--r--   0        0        0     2044 2024-04-02 21:06:10.329773 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params.py
--rw-r--r--   0        0        0     1954 2024-04-02 21:06:10.336161 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py
--rw-r--r--   0        0        0     1667 2024-04-02 21:06:10.341321 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_error.py
--rw-r--r--   0        0        0     1691 2024-04-02 21:06:10.347050 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_success.py
--rw-r--r--   0        0        0     1583 2024-04-02 21:06:10.355366 gradientai-1.9.0/gradientai/openapi/client/test/test_upload_file_error.py
--rw-r--r--   0        0        0     1597 2024-04-02 21:06:10.362354 gradientai-1.9.0/gradientai/openapi/client/test/test_upload_file_success.py
--rw-r--r--   0        0        0    22901 2024-04-02 23:02:40.028355 gradientai-1.9.0/gradientai/openapi/client_README.md
--rw-r--r--   0        0        0        0 2023-08-31 18:54:00.559055 gradientai-1.9.0/gradientai/py.typed
--rw-r--r--   0        0        0      210 2023-10-24 19:44:32.690293 gradientai-1.9.0/gradientai/pydantic_models/types.py
--rw-r--r--   0        0        0     1761 2024-04-05 00:24:39.981741 gradientai-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 gradientai-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      384 2024-01-02 22:48:19.948017 gradientai-1.9.1/README.md
+-rw-r--r--   0        0        0      873 2024-01-26 22:46:41.832392 gradientai-1.9.1/gradientai/__init__.py
+-rw-r--r--   0        0        0     2237 2024-01-26 22:46:41.832503 gradientai-1.9.1/gradientai/__init__.pyi
+-rw-r--r--   0        0        0     2686 2024-01-26 22:46:41.832628 gradientai-1.9.1/gradientai/_base_model.py
+-rw-r--r--   0        0        0     3984 2024-01-02 22:48:19.948502 gradientai-1.9.1/gradientai/_embeddings_model.py
+-rw-r--r--   0        0        0    16549 2024-04-05 19:44:39.852479 gradientai-1.9.1/gradientai/_gradient.py
+-rw-r--r--   0        0        0     2333 2024-04-03 00:11:07.185923 gradientai-1.9.1/gradientai/_model.py
+-rw-r--r--   0        0        0     3510 2023-10-24 19:44:32.688189 gradientai-1.9.1/gradientai/_model_adapter.py
+-rw-r--r--   0        0        0     1751 2024-04-05 19:44:39.852694 gradientai-1.9.1/gradientai/_rag.py
+-rw-r--r--   0        0        0     2497 2024-04-02 16:51:03.746721 gradientai-1.9.1/gradientai/_types.py
+-rw-r--r--   0        0        0      730 2024-01-02 22:48:19.948773 gradientai-1.9.1/gradientai/helpers/asyncio_threads.py
+-rw-r--r--   0        0        0     2155 2023-09-11 18:57:16.856296 gradientai-1.9.1/gradientai/helpers/env_manager.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:06:10.508888 gradientai-1.9.1/gradientai/openapi/__init__.py
+-rw-r--r--   0        0        0    11944 2024-04-02 23:02:40.025793 gradientai-1.9.1/gradientai/openapi/client/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-02 23:02:40.025926 gradientai-1.9.1/gradientai/openapi/client/api/__init__.py
+-rw-r--r--   0        0        0    59385 2024-04-02 21:06:10.436752 gradientai-1.9.1/gradientai/openapi/client/api/blocks_api.py
+-rw-r--r--   0        0        0    15138 2024-04-02 21:06:10.456255 gradientai-1.9.1/gradientai/openapi/client/api/embeddings_api.py
+-rw-r--r--   0        0        0     8147 2024-04-02 21:06:10.464141 gradientai-1.9.1/gradientai/openapi/client/api/files_api.py
+-rw-r--r--   0        0        0    43721 2024-04-02 21:06:10.473572 gradientai-1.9.1/gradientai/openapi/client/api/models_api.py
+-rw-r--r--   0        0        0    16242 2024-04-02 23:02:40.026264 gradientai-1.9.1/gradientai/openapi/client/api/rag_api.py
+-rw-r--r--   0        0        0    30160 2024-04-02 21:06:10.517186 gradientai-1.9.1/gradientai/openapi/client/api_client.py
+-rw-r--r--   0        0        0      844 2024-04-02 21:06:10.519343 gradientai-1.9.1/gradientai/openapi/client/api_response.py
+-rw-r--r--   0        0        0    14896 2024-04-02 21:06:10.495099 gradientai-1.9.1/gradientai/openapi/client/configuration.py
+-rw-r--r--   0        0        0     1259 2024-04-02 23:02:40.026440 gradientai-1.9.1/gradientai/openapi/client/docs/AddFilesToRagCollectionBodyParams.md
+-rw-r--r--   0        0        0     1101 2024-04-02 23:02:40.026527 gradientai-1.9.1/gradientai/openapi/client/docs/AddFilesToRagCollectionError.md
+-rw-r--r--   0        0        0     1294 2024-04-02 21:06:08.817381 gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md
+-rw-r--r--   0        0        0     1275 2024-04-02 21:06:08.859982 gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md
+-rw-r--r--   0        0        0      989 2024-04-02 21:06:08.888938 gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentError.md
+-rw-r--r--   0        0        0     1017 2024-04-02 21:06:09.017017 gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md
+-rw-r--r--   0        0        0      935 2024-04-02 21:06:09.077859 gradientai-1.9.1/gradientai/openapi/client/docs/BaseModel.md
+-rw-r--r--   0        0        0    23913 2024-04-02 21:06:10.452912 gradientai-1.9.1/gradientai/openapi/client/docs/BlocksApi.md
+-rw-r--r--   0        0        0     2065 2024-04-02 21:06:09.106119 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelBodyParams.md
+-rw-r--r--   0        0        0     1226 2024-04-02 21:06:09.173646 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md
+-rw-r--r--   0        0        0     1153 2024-04-02 21:06:09.300783 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md
+-rw-r--r--   0        0        0     1069 2024-04-02 21:06:09.338931 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelError.md
+-rw-r--r--   0        0        0     1146 2024-04-02 21:06:09.380345 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md
+-rw-r--r--   0        0        0     1161 2024-04-02 21:06:09.414975 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md
+-rw-r--r--   0        0        0     1080 2024-04-02 21:06:09.450202 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md
+-rw-r--r--   0        0        0     1224 2024-04-02 21:06:09.525750 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md
+-rw-r--r--   0        0        0     1161 2024-04-02 21:06:09.547399 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.569264 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.585117 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.601035 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.613596 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.630346 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.652113 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.675322 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md
+-rw-r--r--   0        0        0     1243 2024-04-02 21:06:09.694265 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md
+-rw-r--r--   0        0        0     1394 2024-04-02 21:06:09.713760 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md
+-rw-r--r--   0        0        0     1019 2024-04-02 21:06:09.728650 gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelSuccess.md
+-rw-r--r--   0        0        0     1172 2024-04-02 21:06:09.749173 gradientai-1.9.1/gradientai/openapi/client/docs/CreateAudioTranscriptionBodyParams.md
+-rw-r--r--   0        0        0     1100 2024-04-02 21:06:09.763865 gradientai-1.9.1/gradientai/openapi/client/docs/CreateAudioTranscriptionError.md
+-rw-r--r--   0        0        0     1135 2024-04-02 21:06:09.782221 gradientai-1.9.1/gradientai/openapi/client/docs/CreateAudioTranscriptionSuccess.md
+-rw-r--r--   0        0        0     1195 2024-04-02 21:06:09.799851 gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParams.md
+-rw-r--r--   0        0        0     1622 2024-04-02 21:06:09.808092 gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md
+-rw-r--r--   0        0        0     1565 2024-04-02 21:06:09.814804 gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md
+-rw-r--r--   0        0        0     1550 2024-04-02 21:06:09.823247 gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md
+-rw-r--r--   0        0        0     1219 2024-04-02 21:06:09.830872 gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md
+-rw-r--r--   0        0        0      924 2024-04-02 21:06:09.838966 gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelError.md
+-rw-r--r--   0        0        0      945 2024-04-02 21:06:09.847442 gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelSuccess.md
+-rw-r--r--   0        0        0     1254 2024-04-02 23:02:40.026608 gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionBodyParams.md
+-rw-r--r--   0        0        0     1271 2024-04-02 23:02:40.026699 gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionBodyParamsFilesInner.md
+-rw-r--r--   0        0        0     1035 2024-04-02 23:02:40.026778 gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionError.md
+-rw-r--r--   0        0        0     1056 2024-04-02 23:02:40.026848 gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionSuccess.md
+-rw-r--r--   0        0        0      924 2024-04-02 21:06:09.922306 gradientai-1.9.1/gradientai/openapi/client/docs/DeleteModelError.md
+-rw-r--r--   0        0        0     5995 2024-04-02 21:06:10.460915 gradientai-1.9.1/gradientai/openapi/client/docs/EmbeddingsApi.md
+-rw-r--r--   0        0        0     1218 2024-04-02 21:06:09.930543 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntityBodyParams.md
+-rw-r--r--   0        0        0     1235 2024-04-02 21:06:09.942847 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md
+-rw-r--r--   0        0        0      950 2024-04-02 21:06:09.951498 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntityError.md
+-rw-r--r--   0        0        0     1052 2024-04-02 21:06:09.958892 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntitySuccess.md
+-rw-r--r--   0        0        0     1105 2024-04-02 21:06:09.968200 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md
+-rw-r--r--   0        0        0      911 2024-04-02 21:06:09.974240 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfError.md
+-rw-r--r--   0        0        0     1050 2024-04-02 21:06:09.980697 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccess.md
+-rw-r--r--   0        0        0     1462 2024-04-02 21:06:09.989400 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md
+-rw-r--r--   0        0        0     1262 2024-04-02 21:06:09.999431 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md
+-rw-r--r--   0        0        0     1380 2024-04-02 21:06:10.006871 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md
+-rw-r--r--   0        0        0     1598 2024-04-02 21:06:10.015894 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md
+-rw-r--r--   0        0        0     1646 2024-04-02 21:06:10.022832 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md
+-rw-r--r--   0        0        0     1326 2024-04-02 21:06:10.029202 gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md
+-rw-r--r--   0        0        0     2801 2024-04-02 21:06:10.469329 gradientai-1.9.1/gradientai/openapi/client/docs/FilesApi.md
+-rw-r--r--   0        0        0     1109 2024-04-02 21:06:10.036440 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParams.md
+-rw-r--r--   0        0        0     1452 2024-04-02 21:06:10.042021 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md
+-rw-r--r--   0        0        0     1496 2024-04-02 21:06:10.048829 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md
+-rw-r--r--   0        0        0     1256 2024-04-02 21:06:10.057143 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md
+-rw-r--r--   0        0        0     1562 2024-04-02 21:06:10.064934 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md
+-rw-r--r--   0        0        0     1076 2024-04-02 21:06:10.072608 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelError.md
+-rw-r--r--   0        0        0     1061 2024-04-02 21:06:10.078529 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md
+-rw-r--r--   0        0        0     1074 2024-04-02 21:06:10.085792 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md
+-rw-r--r--   0        0        0     1033 2024-04-02 21:06:10.092123 gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelSuccess.md
+-rw-r--r--   0        0        0     1127 2024-04-02 21:06:10.101646 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md
+-rw-r--r--   0        0        0     1177 2024-04-02 21:06:10.134519 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md
+-rw-r--r--   0        0        0     1290 2024-04-02 21:06:10.146161 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md
+-rw-r--r--   0        0        0     1290 2024-04-02 21:06:10.154510 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md
+-rw-r--r--   0        0        0      963 2024-04-02 21:06:10.162634 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerError.md
+-rw-r--r--   0        0        0     1097 2024-04-02 21:06:10.169665 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerSuccess.md
+-rw-r--r--   0        0        0     1235 2024-04-02 21:06:10.176849 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md
+-rw-r--r--   0        0        0     1359 2024-04-02 21:06:10.183918 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md
+-rw-r--r--   0        0        0     1159 2024-04-02 21:06:10.192220 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md
+-rw-r--r--   0        0        0     1229 2024-04-02 21:06:10.199299 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md
+-rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.209914 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingError.md
+-rw-r--r--   0        0        0     1119 2024-04-02 21:06:10.219023 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md
+-rw-r--r--   0        0        0     1273 2024-04-02 21:06:10.225005 gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md
+-rw-r--r--   0        0        0     1061 2024-04-02 21:06:10.230449 gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionError.md
+-rw-r--r--   0        0        0     1197 2024-04-02 21:06:10.238093 gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccess.md
+-rw-r--r--   0        0        0     1195 2024-04-02 21:06:10.243126 gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf.md
+-rw-r--r--   0        0        0     1289 2024-04-02 21:06:10.248549 gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1.md
+-rw-r--r--   0        0        0     1261 2024-04-02 21:06:10.254570 gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1Result.md
+-rw-r--r--   0        0        0      885 2024-04-02 21:06:10.260434 gradientai-1.9.1/gradientai/openapi/client/docs/GetModelError.md
+-rw-r--r--   0        0        0     1034 2024-04-02 21:06:10.266339 gradientai-1.9.1/gradientai/openapi/client/docs/GetModelSuccess.md
+-rw-r--r--   0        0        0      963 2024-04-02 21:06:10.273428 gradientai-1.9.1/gradientai/openapi/client/docs/ListEmbeddingsError.md
+-rw-r--r--   0        0        0     1093 2024-04-02 21:06:10.278509 gradientai-1.9.1/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md
+-rw-r--r--   0        0        0     1280 2024-04-02 21:06:10.286179 gradientai-1.9.1/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md
+-rw-r--r--   0        0        0      911 2024-04-02 21:06:10.291565 gradientai-1.9.1/gradientai/openapi/client/docs/ListModelsError.md
+-rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.297535 gradientai-1.9.1/gradientai/openapi/client/docs/ListModelsSuccess.md
+-rw-r--r--   0        0        0     1281 2024-04-02 21:06:10.303477 gradientai-1.9.1/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md
+-rw-r--r--   0        0        0      988 2024-04-02 21:06:10.309052 gradientai-1.9.1/gradientai/openapi/client/docs/ModelAdapter.md
+-rw-r--r--   0        0        0    17156 2024-04-02 21:06:10.478620 gradientai-1.9.1/gradientai/openapi/client/docs/ModelsApi.md
+-rw-r--r--   0        0        0     1258 2024-04-02 21:06:10.313692 gradientai-1.9.1/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md
+-rw-r--r--   0        0        0     1028 2024-04-02 21:06:10.319260 gradientai-1.9.1/gradientai/openapi/client/docs/PersonalizeDocumentError.md
+-rw-r--r--   0        0        0     1068 2024-04-02 21:06:10.325029 gradientai-1.9.1/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md
+-rw-r--r--   0        0        0     6299 2024-04-02 23:02:40.027022 gradientai-1.9.1/gradientai/openapi/client/docs/RAGApi.md
+-rw-r--r--   0        0        0     1347 2024-04-02 21:06:10.331891 gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md
+-rw-r--r--   0        0        0     1286 2024-04-02 21:06:10.337363 gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md
+-rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.343168 gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentError.md
+-rw-r--r--   0        0        0     1028 2024-04-02 21:06:10.348221 gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md
+-rw-r--r--   0        0        0      911 2024-04-02 21:06:10.356695 gradientai-1.9.1/gradientai/openapi/client/docs/UploadFileError.md
+-rw-r--r--   0        0        0      932 2024-04-02 21:06:10.363682 gradientai-1.9.1/gradientai/openapi/client/docs/UploadFileSuccess.md
+-rw-r--r--   0        0        0     5323 2024-04-02 21:06:10.512625 gradientai-1.9.1/gradientai/openapi/client/exceptions.py
+-rw-r--r--   0        0        0    11009 2024-04-02 23:02:40.027183 gradientai-1.9.1/gradientai/openapi/client/models/__init__.py
+-rw-r--r--   0        0        0     3166 2024-04-03 23:04:21.106342 gradientai-1.9.1/gradientai/openapi/client/models/add_files_to_rag_collection_body_params.py
+-rw-r--r--   0        0        0     2557 2024-04-02 23:02:40.027355 gradientai-1.9.1/gradientai/openapi/client/models/add_files_to_rag_collection_error.py
+-rw-r--r--   0        0        0     3617 2024-04-02 21:06:08.792526 gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_body_params.py
+-rw-r--r--   0        0        0     3053 2024-04-02 21:06:08.847811 gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py
+-rw-r--r--   0        0        0     2501 2024-04-02 21:06:08.872357 gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_error.py
+-rw-r--r--   0        0        0     2799 2024-04-02 21:06:08.904229 gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_success.py
+-rw-r--r--   0        0        0     3400 2024-04-02 21:06:09.034106 gradientai-1.9.1/gradientai/openapi/client/models/base_model.py
+-rw-r--r--   0        0        0     6500 2024-04-02 21:06:09.090984 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_body_params.py
+-rw-r--r--   0        0        0     3043 2024-04-02 21:06:09.144530 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_body_params_guidance.py
+-rw-r--r--   0        0        0     2680 2024-04-02 21:06:09.246459 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_body_params_rag.py
+-rw-r--r--   0        0        0    13624 2024-04-02 21:06:09.326952 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error.py
+-rw-r--r--   0        0        0     3793 2024-04-02 21:06:09.357221 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of.py
+-rw-r--r--   0        0        0     3887 2024-04-02 21:06:09.397688 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of1.py
+-rw-r--r--   0        0        0     2885 2024-04-02 21:06:09.433031 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of10.py
+-rw-r--r--   0        0        0     3347 2024-04-02 21:06:09.509206 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py
+-rw-r--r--   0        0        0     3361 2024-04-02 21:06:09.534327 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of2.py
+-rw-r--r--   0        0        0     2849 2024-04-02 21:06:09.557641 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of3.py
+-rw-r--r--   0        0        0     2891 2024-04-02 21:06:09.576512 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of4.py
+-rw-r--r--   0        0        0     2875 2024-04-02 21:06:09.591719 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of5.py
+-rw-r--r--   0        0        0     2887 2024-04-02 21:06:09.606721 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of6.py
+-rw-r--r--   0        0        0     2869 2024-04-02 21:06:09.620763 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of7.py
+-rw-r--r--   0        0        0     2875 2024-04-02 21:06:09.640394 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of8.py
+-rw-r--r--   0        0        0     2877 2024-04-02 21:06:09.666604 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of9.py
+-rw-r--r--   0        0        0     3281 2024-04-02 21:06:09.686784 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of_payload.py
+-rw-r--r--   0        0        0     2700 2024-04-02 21:06:09.705656 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py
+-rw-r--r--   0        0        0     2665 2024-04-02 21:06:09.722372 gradientai-1.9.1/gradientai/openapi/client/models/complete_model_success.py
+-rw-r--r--   0        0        0     2619 2024-04-02 21:06:09.739180 gradientai-1.9.1/gradientai/openapi/client/models/create_audio_transcription_body_params.py
+-rw-r--r--   0        0        0     2565 2024-04-02 21:06:09.755475 gradientai-1.9.1/gradientai/openapi/client/models/create_audio_transcription_error.py
+-rw-r--r--   0        0        0     2640 2024-04-02 21:06:09.770734 gradientai-1.9.1/gradientai/openapi/client/models/create_audio_transcription_success.py
+-rw-r--r--   0        0        0     3807 2024-04-02 21:06:09.790028 gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params.py
+-rw-r--r--   0        0        0     4559 2024-04-02 21:06:09.803767 gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py
+-rw-r--r--   0        0        0     3018 2024-04-02 21:06:09.811376 gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
+-rw-r--r--   0        0        0     3165 2024-04-02 21:06:09.819303 gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py
+-rw-r--r--   0        0        0     2836 2024-04-02 21:06:09.826269 gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_model.py
+-rw-r--r--   0        0        0     2461 2024-04-02 21:06:09.834119 gradientai-1.9.1/gradientai/openapi/client/models/create_model_error.py
+-rw-r--r--   0        0        0     2457 2024-04-02 21:06:09.842823 gradientai-1.9.1/gradientai/openapi/client/models/create_model_success.py
+-rw-r--r--   0        0        0     3788 2024-04-02 23:02:40.027441 gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_body_params.py
+-rw-r--r--   0        0        0     2727 2024-04-02 23:02:40.027522 gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_body_params_files_inner.py
+-rw-r--r--   0        0        0     2525 2024-04-02 23:02:40.027595 gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_error.py
+-rw-r--r--   0        0        0     2521 2024-04-02 23:02:40.027660 gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_success.py
+-rw-r--r--   0        0        0     2461 2024-04-02 21:06:09.918218 gradientai-1.9.1/gradientai/openapi/client/models/delete_model_error.py
+-rw-r--r--   0        0        0     3456 2024-04-02 21:06:09.926059 gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_body_params.py
+-rw-r--r--   0        0        0     3228 2024-04-02 21:06:09.936371 gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py
+-rw-r--r--   0        0        0     2477 2024-04-02 21:06:09.946388 gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_error.py
+-rw-r--r--   0        0        0     3136 2024-04-02 21:06:09.955137 gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_success.py
+-rw-r--r--   0        0        0     5870 2024-04-02 21:06:09.964168 gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_success_entity_value.py
+-rw-r--r--   0        0        0     2453 2024-04-02 21:06:09.971377 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_error.py
+-rw-r--r--   0        0        0     3365 2024-04-02 21:06:09.976832 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success.py
+-rw-r--r--   0        0        0     4761 2024-04-02 21:06:09.985105 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py
+-rw-r--r--   0        0        0     2937 2024-04-02 21:06:09.995158 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py
+-rw-r--r--   0        0        0     3397 2024-04-02 21:06:10.003745 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py
+-rw-r--r--   0        0        0     3774 2024-04-02 21:06:10.009350 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
+-rw-r--r--   0        0        0     3545 2024-04-02 21:06:10.019368 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
+-rw-r--r--   0        0        0     3065 2024-04-02 21:06:10.025975 gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py
+-rw-r--r--   0        0        0     3075 2024-04-02 21:06:10.032424 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params.py
+-rw-r--r--   0        0        0     4023 2024-04-02 21:06:10.039042 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py
+-rw-r--r--   0        0        0     3056 2024-04-02 21:06:10.044989 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
+-rw-r--r--   0        0        0     5780 2024-04-02 21:06:10.053458 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py
+-rw-r--r--   0        0        0     3137 2024-04-02 21:06:10.061882 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
+-rw-r--r--   0        0        0    10150 2024-04-02 21:06:10.068980 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_error.py
+-rw-r--r--   0        0        0     2881 2024-04-02 21:06:10.075247 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_error_one_of.py
+-rw-r--r--   0        0        0     2851 2024-04-02 21:06:10.081189 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py
+-rw-r--r--   0        0        0     2748 2024-04-02 21:06:10.088300 gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_success.py
+-rw-r--r--   0        0        0     2993 2024-04-02 21:06:10.098254 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params.py
+-rw-r--r--   0        0        0     6307 2024-04-02 21:06:10.105052 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params_source.py
+-rw-r--r--   0        0        0     3023 2024-04-02 21:06:10.138849 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py
+-rw-r--r--   0        0        0     2959 2024-04-02 21:06:10.149368 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py
+-rw-r--r--   0        0        0     2485 2024-04-02 21:06:10.157233 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_error.py
+-rw-r--r--   0        0        0     3047 2024-04-02 21:06:10.165942 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_success.py
+-rw-r--r--   0        0        0     3197 2024-04-02 21:06:10.173414 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_success_rag_context.py
+-rw-r--r--   0        0        0     2831 2024-04-02 21:06:10.179649 gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py
+-rw-r--r--   0        0        0     3137 2024-04-02 21:06:10.188248 gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_body_params.py
+-rw-r--r--   0        0        0     2629 2024-04-02 21:06:10.194657 gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py
+-rw-r--r--   0        0        0     2509 2024-04-02 21:06:10.205377 gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_error.py
+-rw-r--r--   0        0        0     3124 2024-04-02 21:06:10.214647 gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_success.py
+-rw-r--r--   0        0        0     2802 2024-04-02 21:06:10.221585 gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py
+-rw-r--r--   0        0        0     2541 2024-04-02 21:06:10.227642 gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_error.py
+-rw-r--r--   0        0        0     6225 2024-04-02 21:06:10.233896 gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success.py
+-rw-r--r--   0        0        0     3230 2024-04-02 21:06:10.240370 gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success_one_of.py
+-rw-r--r--   0        0        0     3331 2024-04-02 21:06:10.245238 gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success_one_of1.py
+-rw-r--r--   0        0        0     2620 2024-04-02 21:06:10.251490 gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success_one_of1_result.py
+-rw-r--r--   0        0        0     2437 2024-04-02 21:06:10.256772 gradientai-1.9.1/gradientai/openapi/client/models/get_model_error.py
+-rw-r--r--   0        0        0     3226 2024-04-02 21:06:10.262685 gradientai-1.9.1/gradientai/openapi/client/models/get_model_success.py
+-rw-r--r--   0        0        0     2485 2024-04-02 21:06:10.269520 gradientai-1.9.1/gradientai/openapi/client/models/list_embeddings_error.py
+-rw-r--r--   0        0        0     3198 2024-04-02 21:06:10.275832 gradientai-1.9.1/gradientai/openapi/client/models/list_embeddings_success.py
+-rw-r--r--   0        0        0     2877 2024-04-02 21:06:10.281153 gradientai-1.9.1/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py
+-rw-r--r--   0        0        0     2453 2024-04-02 21:06:10.288818 gradientai-1.9.1/gradientai/openapi/client/models/list_models_error.py
+-rw-r--r--   0        0        0     2988 2024-04-02 21:06:10.294142 gradientai-1.9.1/gradientai/openapi/client/models/list_models_success.py
+-rw-r--r--   0        0        0     6222 2024-04-02 21:06:10.300547 gradientai-1.9.1/gradientai/openapi/client/models/list_models_success_models_inner.py
+-rw-r--r--   0        0        0     3202 2024-04-02 21:06:10.306093 gradientai-1.9.1/gradientai/openapi/client/models/model_adapter.py
+-rw-r--r--   0        0        0     2910 2024-04-02 21:06:10.311164 gradientai-1.9.1/gradientai/openapi/client/models/personalize_document_body_params.py
+-rw-r--r--   0        0        0     2525 2024-04-02 21:06:10.316119 gradientai-1.9.1/gradientai/openapi/client/models/personalize_document_error.py
+-rw-r--r--   0        0        0     2625 2024-04-02 21:06:10.322296 gradientai-1.9.1/gradientai/openapi/client/models/personalize_document_success.py
+-rw-r--r--   0        0        0     4281 2024-04-02 21:06:10.327645 gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_body_params.py
+-rw-r--r--   0        0        0     2771 2024-04-02 21:06:10.334291 gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py
+-rw-r--r--   0        0        0     2509 2024-04-02 21:06:10.339705 gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_error.py
+-rw-r--r--   0        0        0     2525 2024-04-02 21:06:10.345591 gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_success.py
+-rw-r--r--   0        0        0     2453 2024-04-02 21:06:10.353564 gradientai-1.9.1/gradientai/openapi/client/models/upload_file_error.py
+-rw-r--r--   0        0        0     2449 2024-04-02 21:06:10.360525 gradientai-1.9.1/gradientai/openapi/client/models/upload_file_success.py
+-rw-r--r--   0        0        0    12904 2024-04-02 21:06:10.522227 gradientai-1.9.1/gradientai/openapi/client/rest.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:06:10.513888 gradientai-1.9.1/gradientai/openapi/client/test/__init__.py
+-rw-r--r--   0        0        0     2273 2024-04-02 23:02:40.027750 gradientai-1.9.1/gradientai/openapi/client/test/test_add_files_to_rag_collection_body_params.py
+-rw-r--r--   0        0        0     1745 2024-04-02 23:02:40.027813 gradientai-1.9.1/gradientai/openapi/client/test/test_add_files_to_rag_collection_error.py
+-rw-r--r--   0        0        0     2004 2024-04-02 21:06:08.808961 gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py
+-rw-r--r--   0        0        0     1960 2024-04-02 21:06:08.854945 gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py
+-rw-r--r--   0        0        0     1655 2024-04-02 21:06:08.881571 gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_error.py
+-rw-r--r--   0        0        0     1697 2024-04-02 21:06:08.967099 gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_success.py
+-rw-r--r--   0        0        0     2039 2024-04-02 21:06:09.063993 gradientai-1.9.1/gradientai/openapi/client/test/test_base_model.py
+-rw-r--r--   0        0        0     1980 2024-04-02 21:06:10.439861 gradientai-1.9.1/gradientai/openapi/client/test/test_blocks_api.py
+-rw-r--r--   0        0        0     2280 2024-04-02 21:06:09.099603 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_body_params.py
+-rw-r--r--   0        0        0     1930 2024-04-02 21:06:09.164507 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py
+-rw-r--r--   0        0        0     1731 2024-04-02 21:06:09.292954 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_body_params_rag.py
+-rw-r--r--   0        0        0     2177 2024-04-02 21:06:09.333291 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error.py
+-rw-r--r--   0        0        0     2591 2024-04-02 21:06:09.371930 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of.py
+-rw-r--r--   0        0        0     2257 2024-04-02 21:06:09.406401 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of1.py
+-rw-r--r--   0        0        0     1802 2024-04-02 21:06:09.441943 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of10.py
+-rw-r--r--   0        0        0     1812 2024-04-02 21:06:09.518575 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py
+-rw-r--r--   0        0        0     2271 2024-04-02 21:06:09.542666 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of2.py
+-rw-r--r--   0        0        0     1762 2024-04-02 21:06:09.564892 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of3.py
+-rw-r--r--   0        0        0     1804 2024-04-02 21:06:09.581061 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of4.py
+-rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.598195 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of5.py
+-rw-r--r--   0        0        0     1800 2024-04-02 21:06:09.610916 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of6.py
+-rw-r--r--   0        0        0     1782 2024-04-02 21:06:09.625548 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of7.py
+-rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.648082 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of8.py
+-rw-r--r--   0        0        0     1790 2024-04-02 21:06:09.671711 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of9.py
+-rw-r--r--   0        0        0     2235 2024-04-02 21:06:09.691977 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py
+-rw-r--r--   0        0        0     1999 2024-04-02 21:06:09.710627 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py
+-rw-r--r--   0        0        0     1732 2024-04-02 21:06:09.725385 gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_success.py
+-rw-r--r--   0        0        0     1815 2024-04-02 21:06:09.747060 gradientai-1.9.1/gradientai/openapi/client/test/test_create_audio_transcription_body_params.py
+-rw-r--r--   0        0        0     1753 2024-04-02 21:06:09.758952 gradientai-1.9.1/gradientai/openapi/client/test/test_create_audio_transcription_error.py
+-rw-r--r--   0        0        0     1795 2024-04-02 21:06:09.778352 gradientai-1.9.1/gradientai/openapi/client/test/test_create_audio_transcription_success.py
+-rw-r--r--   0        0        0     2659 2024-04-02 21:06:09.796918 gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params.py
+-rw-r--r--   0        0        0     2349 2024-04-02 21:06:09.806264 gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py
+-rw-r--r--   0        0        0     2121 2024-04-02 21:06:09.813285 gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
+-rw-r--r--   0        0        0     2106 2024-04-02 21:06:09.821729 gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py
+-rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.828921 gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_model.py
+-rw-r--r--   0        0        0     1595 2024-04-02 21:06:09.836385 gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_error.py
+-rw-r--r--   0        0        0     1609 2024-04-02 21:06:09.845646 gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_success.py
+-rw-r--r--   0        0        0     2087 2024-04-02 23:02:40.027879 gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_body_params.py
+-rw-r--r--   0        0        0     1926 2024-04-02 23:02:40.027954 gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_body_params_files_inner.py
+-rw-r--r--   0        0        0     1693 2024-04-02 23:02:40.028029 gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_error.py
+-rw-r--r--   0        0        0     1707 2024-04-02 23:02:40.028100 gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_success.py
+-rw-r--r--   0        0        0     1595 2024-04-02 21:06:09.920600 gradientai-1.9.1/gradientai/openapi/client/test/test_delete_model_error.py
+-rw-r--r--   0        0        0     1087 2024-04-02 21:06:10.458193 gradientai-1.9.1/gradientai/openapi/client/test/test_embeddings_api.py
+-rw-r--r--   0        0        0     2242 2024-04-02 21:06:09.928651 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_body_params.py
+-rw-r--r--   0        0        0     1857 2024-04-02 21:06:09.940584 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py
+-rw-r--r--   0        0        0     1619 2024-04-02 21:06:09.949460 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_error.py
+-rw-r--r--   0        0        0     1747 2024-04-02 21:06:09.957081 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_success.py
+-rw-r--r--   0        0        0     1718 2024-04-02 21:06:09.966737 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py
+-rw-r--r--   0        0        0     1583 2024-04-02 21:06:09.973033 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_error.py
+-rw-r--r--   0        0        0     5829 2024-04-02 21:06:09.979063 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success.py
+-rw-r--r--   0        0        0     5055 2024-04-02 21:06:09.987342 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py
+-rw-r--r--   0        0        0     1938 2024-04-02 21:06:09.997669 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py
+-rw-r--r--   0        0        0     3256 2024-04-02 21:06:10.005551 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py
+-rw-r--r--   0        0        0     2800 2024-04-02 21:06:10.010890 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
+-rw-r--r--   0        0        0     2291 2024-04-02 21:06:10.021591 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
+-rw-r--r--   0        0        0     2066 2024-04-02 21:06:10.027698 gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py
+-rw-r--r--   0        0        0      876 2024-04-02 21:06:10.466006 gradientai-1.9.1/gradientai/openapi/client/test/test_files_api.py
+-rw-r--r--   0        0        0     2583 2024-04-02 21:06:10.034445 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params.py
+-rw-r--r--   0        0        0     2070 2024-04-02 21:06:10.040640 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py
+-rw-r--r--   0        0        0     2047 2024-04-02 21:06:10.047326 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
+-rw-r--r--   0        0        0     1844 2024-04-02 21:06:10.055514 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py
+-rw-r--r--   0        0        0     2108 2024-04-02 21:06:10.063530 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
+-rw-r--r--   0        0        0     2183 2024-04-02 21:06:10.071132 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_error.py
+-rw-r--r--   0        0        0     1792 2024-04-02 21:06:10.077033 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py
+-rw-r--r--   0        0        0     1766 2024-04-02 21:06:10.084327 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py
+-rw-r--r--   0        0        0     1748 2024-04-02 21:06:10.090376 gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_success.py
+-rw-r--r--   0        0        0     1758 2024-04-02 21:06:10.100215 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params.py
+-rw-r--r--   0        0        0     1899 2024-04-02 21:06:10.125636 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params_source.py
+-rw-r--r--   0        0        0     1904 2024-04-02 21:06:10.144238 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py
+-rw-r--r--   0        0        0     1910 2024-04-02 21:06:10.152562 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py
+-rw-r--r--   0        0        0     1631 2024-04-02 21:06:10.159600 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_error.py
+-rw-r--r--   0        0        0     2101 2024-04-02 21:06:10.167754 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_success.py
+-rw-r--r--   0        0        0     2299 2024-04-02 21:06:10.175433 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py
+-rw-r--r--   0        0        0     2018 2024-04-02 21:06:10.182073 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py
+-rw-r--r--   0        0        0     2123 2024-04-02 21:06:10.190615 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_body_params.py
+-rw-r--r--   0        0        0     1861 2024-04-02 21:06:10.197672 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py
+-rw-r--r--   0        0        0     1667 2024-04-02 21:06:10.207994 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_error.py
+-rw-r--r--   0        0        0     2299 2024-04-02 21:06:10.217113 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_success.py
+-rw-r--r--   0        0        0     2026 2024-04-02 21:06:10.223798 gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py
+-rw-r--r--   0        0        0     1717 2024-04-02 21:06:10.229190 gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_error.py
+-rw-r--r--   0        0        0     2126 2024-04-02 21:06:10.236708 gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success.py
+-rw-r--r--   0        0        0     1882 2024-04-02 21:06:10.241895 gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of.py
+-rw-r--r--   0        0        0     2202 2024-04-02 21:06:10.246805 gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1.py
+-rw-r--r--   0        0        0     1883 2024-04-02 21:06:10.253414 gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1_result.py
+-rw-r--r--   0        0        0     1559 2024-04-02 21:06:10.258844 gradientai-1.9.1/gradientai/openapi/client/test/test_get_model_error.py
+-rw-r--r--   0        0        0     2193 2024-04-02 21:06:10.264578 gradientai-1.9.1/gradientai/openapi/client/test/test_get_model_success.py
+-rw-r--r--   0        0        0     1631 2024-04-02 21:06:10.272082 gradientai-1.9.1/gradientai/openapi/client/test/test_list_embeddings_error.py
+-rw-r--r--   0        0        0     2101 2024-04-02 21:06:10.277361 gradientai-1.9.1/gradientai/openapi/client/test/test_list_embeddings_success.py
+-rw-r--r--   0        0        0     1923 2024-04-02 21:06:10.284407 gradientai-1.9.1/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py
+-rw-r--r--   0        0        0     1583 2024-04-02 21:06:10.290426 gradientai-1.9.1/gradientai/openapi/client/test/test_list_models_error.py
+-rw-r--r--   0        0        0     1695 2024-04-02 21:06:10.296286 gradientai-1.9.1/gradientai/openapi/client/test/test_list_models_success.py
+-rw-r--r--   0        0        0     2579 2024-04-02 21:06:10.302172 gradientai-1.9.1/gradientai/openapi/client/test/test_list_models_success_models_inner.py
+-rw-r--r--   0        0        0     2155 2024-04-02 21:06:10.307900 gradientai-1.9.1/gradientai/openapi/client/test/test_model_adapter.py
+-rw-r--r--   0        0        0     1568 2024-04-02 21:06:10.475138 gradientai-1.9.1/gradientai/openapi/client/test/test_models_api.py
+-rw-r--r--   0        0        0     1844 2024-04-02 21:06:10.312637 gradientai-1.9.1/gradientai/openapi/client/test/test_personalize_document_body_params.py
+-rw-r--r--   0        0        0     1691 2024-04-02 21:06:10.317720 gradientai-1.9.1/gradientai/openapi/client/test/test_personalize_document_error.py
+-rw-r--r--   0        0        0     1743 2024-04-02 21:06:10.323929 gradientai-1.9.1/gradientai/openapi/client/test/test_personalize_document_success.py
+-rw-r--r--   0        0        0     1066 2024-04-02 23:02:40.028172 gradientai-1.9.1/gradientai/openapi/client/test/test_rag_api.py
+-rw-r--r--   0        0        0     2044 2024-04-02 21:06:10.329773 gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_body_params.py
+-rw-r--r--   0        0        0     1954 2024-04-02 21:06:10.336161 gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py
+-rw-r--r--   0        0        0     1667 2024-04-02 21:06:10.341321 gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_error.py
+-rw-r--r--   0        0        0     1691 2024-04-02 21:06:10.347050 gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_success.py
+-rw-r--r--   0        0        0     1583 2024-04-02 21:06:10.355366 gradientai-1.9.1/gradientai/openapi/client/test/test_upload_file_error.py
+-rw-r--r--   0        0        0     1597 2024-04-02 21:06:10.362354 gradientai-1.9.1/gradientai/openapi/client/test/test_upload_file_success.py
+-rw-r--r--   0        0        0    22901 2024-04-02 23:02:40.028355 gradientai-1.9.1/gradientai/openapi/client_README.md
+-rw-r--r--   0        0        0        0 2023-08-31 18:54:00.559055 gradientai-1.9.1/gradientai/py.typed
+-rw-r--r--   0        0        0      210 2023-10-24 19:44:32.690293 gradientai-1.9.1/gradientai/pydantic_models/types.py
+-rw-r--r--   0        0        0     1865 2024-04-05 20:13:01.114329 gradientai-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 gradientai-1.9.1/PKG-INFO
```

### Comparing `gradientai-1.9.0/gradientai/__init__.py` & `gradientai-1.9.1/gradientai/__init__.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/__init__.pyi` & `gradientai-1.9.1/gradientai/__init__.pyi`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/_base_model.py` & `gradientai-1.9.1/gradientai/_base_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/_embeddings_model.py` & `gradientai-1.9.1/gradientai/_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/_gradient.py` & `gradientai-1.9.1/gradientai/_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,12 +478,21 @@
                     )
                     for (file_result, file_path) in zip(file_results, filepaths)
                 ],
             ),
         )
 
         return RAGCollection(
-            id=rag_result.id,
+            id_=rag_result.id,
+            files_api=self._files_api,
+            rag_api=self._rag_api,
+            workspace_id=self._workspace_id,
+        )
+
+    def get_rag_collection(self, *, id_: str) -> RAGCollection:
+        # TODO(matehal@gradient.ai, 04/05/2024): make request to backend once we have GET method for getting rag collection.
+        return RAGCollection(
+            id_=id_,
             files_api=self._files_api,
             rag_api=self._rag_api,
             workspace_id=self._workspace_id,
         )
```

### Comparing `gradientai-1.9.0/gradientai/_model.py` & `gradientai-1.9.1/gradientai/_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/_model_adapter.py` & `gradientai-1.9.1/gradientai/_model_adapter.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/_rag.py` & `gradientai-1.9.1/gradientai/_rag.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     _rag_api: RAGApi
     _files_api: FilesApi
     _workspace_id: str
 
     def __init__(
         self,
         *,
-        id: str,
+        id_: str,
         files_api: FilesApi,
         rag_api: RAGApi,
         workspace_id: str,
     ) -> None:
-        self._id = id
+        self._id = id_
         self._files_api = files_api
         self._rag_api = rag_api
         self._workspace_id = workspace_id
 
     @property
-    def id(self) -> str:
+    def id_(self) -> str:
         return self._id
 
     def add_files(self, *, filepaths: List[os.PathLike]) -> None:
         file_results = [
             self._files_api.upload_file(
                 file=file_,
                 type="ragUserFile",
```

### Comparing `gradientai-1.9.0/gradientai/_types.py` & `gradientai-1.9.1/gradientai/_types.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/helpers/asyncio_threads.py` & `gradientai-1.9.1/gradientai/helpers/asyncio_threads.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/helpers/env_manager.py` & `gradientai-1.9.1/gradientai/helpers/env_manager.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/__init__.py` & `gradientai-1.9.1/gradientai/openapi/client/__init__.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/api/blocks_api.py` & `gradientai-1.9.1/gradientai/openapi/client/api/blocks_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/api/embeddings_api.py` & `gradientai-1.9.1/gradientai/openapi/client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/api/files_api.py` & `gradientai-1.9.1/gradientai/openapi/client/api/files_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/api/models_api.py` & `gradientai-1.9.1/gradientai/openapi/client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/api/rag_api.py` & `gradientai-1.9.1/gradientai/openapi/client/api/rag_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/api_client.py` & `gradientai-1.9.1/gradientai/openapi/client/api_client.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/api_response.py` & `gradientai-1.9.1/gradientai/openapi/client/api_response.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/configuration.py` & `gradientai-1.9.1/gradientai/openapi/client/configuration.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/AddFilesToRagCollectionBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/AddFilesToRagCollectionBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/AddFilesToRagCollectionError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/AddFilesToRagCollectionError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/BaseModel.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/BaseModel.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/BlocksApi.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/BlocksApi.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CompleteModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateAudioTranscriptionBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateAudioTranscriptionError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateAudioTranscriptionSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionBodyParamsFilesInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionBodyParamsFilesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/CreateRagCollectionSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/DeleteModelError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/DeleteModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/EmbeddingsApi.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/EmbeddingsApi.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntityBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntityError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntitySuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FilesApi.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FilesApi.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/FineTuneModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1Result.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1Result.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GetModelError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GetModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/GetModelSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/GetModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ListEmbeddingsError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ListModelsError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ListModelsSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ModelAdapter.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ModelAdapter.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/ModelsApi.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/ModelsApi.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/PersonalizeDocumentError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/RAGApi.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/RAGApi.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/UploadFileError.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/UploadFileError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/docs/UploadFileSuccess.md` & `gradientai-1.9.1/gradientai/openapi/client/docs/UploadFileSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/exceptions.py` & `gradientai-1.9.1/gradientai/openapi/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/__init__.py` & `gradientai-1.9.1/gradientai/openapi/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/add_files_to_rag_collection_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/add_files_to_rag_collection_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/add_files_to_rag_collection_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/add_files_to_rag_collection_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/analyze_sentiment_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/base_model.py` & `gradientai-1.9.1/gradientai/openapi/client/models/base_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_guidance.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_body_params_guidance.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_rag.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_body_params_rag.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of10.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of10.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of2.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of2.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of3.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of3.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of4.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of4.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of5.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of5.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of6.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of6.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of7.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of7.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of8.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of8.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of9.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of9.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/complete_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_audio_transcription_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_audio_transcription_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_audio_transcription_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_model.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_model_body_params_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_body_params_files_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_body_params_files_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/create_rag_collection_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/delete_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/delete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success_entity_value.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_entity_success_entity_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/fine_tune_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params_source.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_success_rag_context.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of1_result.py` & `gradientai-1.9.1/gradientai/openapi/client/models/get_audio_transcription_success_one_of1_result.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/get_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/get_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/get_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/get_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/list_embeddings_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/list_embeddings_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/list_models_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/list_models_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/list_models_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/list_models_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/list_models_success_models_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/list_models_success_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/model_adapter.py` & `gradientai-1.9.1/gradientai/openapi/client/models/model_adapter.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/personalize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/personalize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/personalize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/summarize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/upload_file_error.py` & `gradientai-1.9.1/gradientai/openapi/client/models/upload_file_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/models/upload_file_success.py` & `gradientai-1.9.1/gradientai/openapi/client/models/upload_file_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/rest.py` & `gradientai-1.9.1/gradientai/openapi/client/rest.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_add_files_to_rag_collection_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_add_files_to_rag_collection_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_add_files_to_rag_collection_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_add_files_to_rag_collection_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_analyze_sentiment_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_base_model.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_base_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_blocks_api.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_blocks_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_rag.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_body_params_rag.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of10.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of10.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of2.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of2.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of3.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of3.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of4.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of4.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of5.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of5.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of6.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of6.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of7.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of7.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of8.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of8.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of9.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of9.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_complete_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_audio_transcription_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_audio_transcription_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_audio_transcription_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_model.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_body_params_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_body_params_files_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_body_params_files_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_create_rag_collection_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_delete_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_delete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_embeddings_api.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_embeddings_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_files_api.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_files_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_fine_tune_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params_source.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1_result.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1_result.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_get_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_get_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_list_embeddings_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_list_embeddings_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_list_models_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_list_models_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success_models_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_list_models_success_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_model_adapter.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_model_adapter.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_models_api.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_models_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_personalize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_personalize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_personalize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_rag_api.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_rag_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_summarize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_upload_file_error.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_upload_file_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client/test/test_upload_file_success.py` & `gradientai-1.9.1/gradientai/openapi/client/test/test_upload_file_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/gradientai/openapi/client_README.md` & `gradientai-1.9.1/gradientai/openapi/client_README.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.9.0/pyproject.toml` & `gradientai-1.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "gradient",
   "gradient ai",
 ]
 license = "MIT"
 name = "gradientai"
 readme = "README.md"
 repository = "https://github.com/Preemo-Inc/gradientai-python-sdk"
-version = "1.9.0"
+version = "1.9.1"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 pydantic = "^1.10.5, <2"
 python = "^3.8.1"
 python-dateutil = ">=2.8.2"
 urllib3 = ">= 1.25.3"
@@ -85,7 +85,8 @@
 show_error_codes = true
 warn_return_any = true
 warn_unused_ignores = true
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
+# TODO: Dummy todo so that Copybaras replace transform doesn't complain that it doesn't have any todos.
```

### Comparing `gradientai-1.9.0/PKG-INFO` & `gradientai-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradientai
-Version: 1.9.0
+Version: 1.9.1
 Summary: Gradient AI API
 Home-page: https://github.com/Preemo-Inc/gradientai-python-sdk
 License: MIT
 Keywords: Gradient AI API,ai,artificial intelligence,fine-tuning,large language model,llm,gradient,gradient ai
 Author: Gradient AI Support
 Author-email: support@gradient.ai
 Requires-Python: >=3.8.1,<4.0.0
```

