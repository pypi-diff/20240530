# Comparing `tmp/dataproc_jupyter_plugin-0.1.78.tar.gz` & `tmp/dataproc_jupyter_plugin-0.1.9.tar.gz`

## Comparing `dataproc_jupyter_plugin-0.1.78.tar` & `dataproc_jupyter_plugin-0.1.9.tar`

### file list

```diff
@@ -1,320 +1,180 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/.babelrc.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/CHANGELOG.md
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/RELEASE.md
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/babel.config.js
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/conftest.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/contributing.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/install.json
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/jest.config.js
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/package.json
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/setup.py
--rw-r--r--   0        0        0   283062 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/third-party-licenses.txt
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/tsconfig.test.json
--rw-r--r--   0        0        0   705839 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/yarn.lock
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/.storybook/main.ts
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/.storybook/preview.ts
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/__mocks__/utils.ts
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/_version.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/credentials.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/handlers.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/urls.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/commons/constants.py
--rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/controllers/airflow.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/controllers/bigquery.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/controllers/composer.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/controllers/dataproc.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/controllers/executor.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/dagTemplates/pysparkBatchTemplate-v1.txt
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/dagTemplates/pysparkJobTemplate-v1.txt
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/dagTemplates/wrapper_papermill.py
--rw-r--r--   0        0        0    22840 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/build_log.json
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/package.json
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/schemas/dataproc_jupyter_plugin/package.json.orig
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/schemas/dataproc_jupyter_plugin/plugin.json
--rw-r--r--   0        0        0  1545806 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/lib_index_js-webpack_sharing_consume_default_dayjs_dayjs.4a84c5d864548dcb01fa.js
--rw-r--r--   0        0        0  1377867 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/lib_index_js-webpack_sharing_consume_default_dayjs_dayjs.4a84c5d864548dcb01fa.js.map
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-384a07.42dfdff13beea989371e.js
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-384a07.42dfdff13beea989371e.js.map
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec560.cc9324c7e20080fbc031.js
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec560.cc9324c7e20080fbc031.js.map
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec561.081357944607bddbbe05.js
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec561.081357944607bddbbe05.js.map
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js-node_modules_mui_icons-material_u-cc508d.9aa8c20aa0888e2a92e3.js
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js-node_modules_mui_icons-material_u-cc508d.9aa8c20aa0888e2a92e3.js.map
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_dayjs_dayjs_min_js.cc7dddd8943ed70d880d.js
--rw-r--r--   0        0        0     9291 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/node_modules_dayjs_dayjs_min_js.cc7dddd8943ed70d880d.js.map
--rw-r--r--   0        0        0    51242 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/remoteEntry.ad737b405a4fd7314581.js
--rw-r--r--   0        0        0    50398 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/remoteEntry.ad737b405a4fd7314581.js.map
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/style.js
--rw-r--r--   0        0        0   290708 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/style_index_js.b02379ac12571d84953b.js
--rw-r--r--   0        0        0   245032 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/style_index_js.b02379ac12571d84953b.js.map
--rw-r--r--   0        0        0  6903165 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_antd_es_index_js.be0c3f83d9d0ff37f7e2.js
--rw-r--r--   0        0        0  5438633 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_antd_es_index_js.be0c3f83d9d0ff37f7e2.js.map
--rw-r--r--   0        0        0    72375 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_cache_dist_emotion-cache_browser_esm_js.f2f673918f81bfe03ef9.js
--rw-r--r--   0        0        0    65794 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_cache_dist_emotion-cache_browser_esm_js.f2f673918f81bfe03ef9.js.map
--rw-r--r--   0        0        0   887475 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_memoize_dist_emotion-memoize_esm_js-node_modules_mui_material_Ch-e54490.308912cac987044b02ba.js
--rw-r--r--   0        0        0   724520 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_memoize_dist_emotion-memoize_esm_js-node_modules_mui_material_Ch-e54490.308912cac987044b02ba.js.map
--rw-r--r--   0        0        0    44049 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.4cde8e9e15d4ab891563.js
--rw-r--r--   0        0        0    42638 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.4cde8e9e15d4ab891563.js.map
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_serialize_dist_emotion-serialize_browser_esm_js-node_modules_emo-cbc221.f7dec6bc93fa26e1763f.js
--rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_serialize_dist_emotion-serialize_browser_esm_js-node_modules_emo-cbc221.f7dec6bc93fa26e1763f.js.map
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.429866bf2e091089bf29.js
--rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.429866bf2e091089bf29.js.map
--rw-r--r--   0        0        0    22284 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui-chips-input_dist_mui-chips-input_es_js.e29a4165cdd2c9eb79ff.js
--rw-r--r--   0        0        0    20778 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui-chips-input_dist_mui-chips-input_es_js.e29a4165cdd2c9eb79ff.js.map
--rw-r--r--   0        0        0   480172 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui_icons-material_FirstPage_js-node_modules_mui_icons-material_LastPage-1a3770.aad9a12f81ede280c58f.js
--rw-r--r--   0        0        0   412381 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui_icons-material_FirstPage_js-node_modules_mui_icons-material_LastPage-1a3770.aad9a12f81ede280c58f.js.map
--rw-r--r--   0        0        0   328990 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui_material_Autocomplete_Autocomplete_js-node_modules_mui_material_Butt-b1a5ad.dafda14a8e260db58f63.js
--rw-r--r--   0        0        0   258127 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui_material_Autocomplete_Autocomplete_js-node_modules_mui_material_Butt-b1a5ad.dafda14a8e260db58f63.js.map
--rw-r--r--   0        0        0  1917808 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui_material_index_js.edd537f32d7e3b543759.js
--rw-r--r--   0        0        0  1315571 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_mui_material_index_js.edd537f32d7e3b543759.js.map
--rw-r--r--   0        0        0   468288 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-arborist_dist_module_js.292c1bc9709d6cb7aff1.js
--rw-r--r--   0        0        0   568183 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-arborist_dist_module_js.292c1bc9709d6cb7aff1.js.map
--rw-r--r--   0        0        0    30157 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-js-cron_dist_esm_index_js.2ea9c50bc11ab328e5d3.js
--rw-r--r--   0        0        0    29934 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-js-cron_dist_esm_index_js.2ea9c50bc11ab328e5d3.js.map
--rw-r--r--   0        0        0   155187 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-table_index_js.7812b8cc68ec0e1816ae.js
--rw-r--r--   0        0        0   283818 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-table_index_js.7812b8cc68ec0e1816ae.js.map
--rw-r--r--   0        0        0    21086 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_mjs.2df627aa59a51be0245a.js
--rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_mjs.2df627aa59a51be0245a.js.map
--rw-r--r--   0        0        0    42824 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react_jsx-runtime_js.eebbb94360a00664ea36.js
--rw-r--r--   0        0        0    50257 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_react_jsx-runtime_js.eebbb94360a00664ea36.js.map
--rw-r--r--   0        0        0   215673 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/static/vendors-node_modules_tzdata_timezone-data_json.f5046797c5ea1d5eee42.js
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/models/models.py
--rw-r--r--   0        0        0    14152 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/services/airflow.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/services/bigquery.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/services/composer.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/services/dataproc.py
--rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/services/executor.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/__init__.py
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_airflow.py
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_bigquery.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_composer.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_credentials.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_dataproc.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_executor.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_handlers.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/jupyter-config/nb-config/dataproc_jupyter_plugin.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/jupyter-config/server-config/dataproc_jupyter_plugin.json
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/kokoro/gcp_ubuntu_docker/continuous.cfg
--rwxr-xr-x   0        0        0     2108 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/kokoro/gcp_ubuntu_docker/kokoro_build.sh
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/kokoro/gcp_ubuntu_docker/presubmit.cfg
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/schema/plugin.json
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/custom.d.ts
--rw-r--r--   0        0        0    26394 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/index.ts
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/react-table-config.d.ts
--rw-r--r--   0        0        0    24234 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/batches/batchDetails.tsx
--rw-r--r--   0        0        0    32156 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/batches/batchService.tsx
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/batches/batches.tsx
--rw-r--r--   0        0        0    71279 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/batches/createBatch.tsx
--rw-r--r--   0        0        0    12653 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/batches/listBatches.tsx
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryDatasetInfo.tsx
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryDatasetInfoWrapper.tsx
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQuerySchema.tsx
--rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryService.tsx
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryTableInfo.tsx
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryTableInfoWrapper.tsx
--rw-r--r--   0        0        0    27696 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryWidget.tsx
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/bigQuery/previewDataInfo.tsx
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/cluster/cluster.tsx
--rw-r--r--   0        0        0    14710 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/cluster/clusterDetails.tsx
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/cluster/clusterServices.tsx
--rw-r--r--   0        0        0    14522 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/cluster/listCluster.tsx
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/BigQueryRegionDropdown.tsx
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/DataprocWidget.tsx
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/DynamicDropdown.tsx
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/MuiWrappedDropdown.tsx
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/MuiWrappedInput.tsx
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/MuiWrappedSelect.tsx
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/MuiWrappedTagsInput.tsx
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/NotebookButtonExtension.tsx
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/RegionDropdown.tsx
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/controls/SidePanelTitleWidget.tsx
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/dpms/databaseInfo.tsx
--rw-r--r--   0        0        0    13959 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/dpms/dpmsService.tsx
--rw-r--r--   0        0        0    19804 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/dpms/dpmsWidget.tsx
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/dpms/schemaInfo.tsx
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/dpms/tableInfo.tsx
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/gcs/gcsBrowserWidget.tsx
--rw-r--r--   0        0        0    12280 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/gcs/gcsDrive.ts
--rw-r--r--   0        0        0    10124 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/gcs/gcsService.ts
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/handler/handler.ts
--rw-r--r--   0        0        0    25684 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/jobs/jobDetails.tsx
--rw-r--r--   0        0        0    16026 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/jobs/jobServices.tsx
--rw-r--r--   0        0        0    15370 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/jobs/jobs.tsx
--rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/jobs/labelProperties.tsx
--rw-r--r--   0        0        0    42382 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/jobs/submitJob.tsx
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/login/authLogin.tsx
--rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/login/configSelection.tsx
--rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/notebookTemplates/listNotebookTemplates.tsx
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/notebookTemplates/notebookTemplates.tsx
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/notebookTemplates/notebookTemplatesService.tsx
--rw-r--r--   0        0        0    51869 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/runtime/createRunTime.tsx
--rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/runtime/listRuntimeTemplates.tsx
--rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/runtime/runtimeService.tsx
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/runtime/runtimeTemplate.tsx
--rw-r--r--   0        0        0    28331 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/createNotebookScheduler.tsx
--rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/executionHistory.tsx
--rw-r--r--   0        0        0    10157 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/listDagRuns.tsx
--rw-r--r--   0        0        0     8667 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/listDagTaskInstances.tsx
--rw-r--r--   0        0        0    18804 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/listNotebookScheduler.tsx
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/notebookJobs.tsx
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/notebookScheduler.tsx
--rw-r--r--   0        0        0    28734 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/scheduler/schedulerServices.tsx
--rw-r--r--   0        0        0    11314 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/sessions/listSessions.tsx
--rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/sessions/sessionDetails.tsx
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/sessions/sessionService.tsx
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/sessions/sessionTemplate.tsx
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/const.ts
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/deletePopup.tsx
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/errorPopup.tsx
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/globalFilter.tsx
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/importErrorPopup.tsx
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/jobDetailsInterface.ts
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/listRuntimeTemplateInterface.ts
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/loggingService.ts
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/metastoreService.ts
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/networkService.ts
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/paginationView.tsx
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/pollingImportErrorTimer.ts
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/pollingTimer.ts
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/previewPaginationView.tsx
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/projectService.ts
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/regionService.tsx
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/signalEmitter.ts
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/statusDisplay.tsx
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/tableData.tsx
--rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/utils.ts
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/src/utils/viewLogs.tsx
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/authLogin.css
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/base.css
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/batches.css
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/cluster.css
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/clusterDetails.css
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/createBatch.css
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/databaseInfo.css
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/dpms.css
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/gcsBucket.css
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/index.css
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/index.js
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/job.css
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/notebookScheduler.css
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/notebookTemplates.css
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/paginationView.css
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/popup.css
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/runtimeTemplate.css
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/sessionDetails.css
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/submitJob.css
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/Storage-icon-dark.svg
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/add_account_icon.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/add_runtime_template.svg
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/bigquery_logo.svg
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/bigquery_project_icon.svg
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/clone_icon.svg
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/clone_icon_disable.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/clone_job_icon.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/clone_job_icon_disable.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/cluster_error_icon.svg
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/cluster_icon.svg
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/cluster_running_icon.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/columns_icon.svg
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/create_cluster_icon.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dag_task_failed_icon.svg
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dag_task_success_icon.svg
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dark_search_clear_icon.svg
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/database_icon.svg
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/database_icon_dark.svg
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/database_widget_icon.svg
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dataproc_icon.svg
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dataset_explorer_dark_icon.svg
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dataset_explorer_icon.svg
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dataset_icon.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/datasets_icon.svg
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/delete_cluster_icon.svg
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/delete_icon.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/down_arrow_icon.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/download_icon.svg
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dpms_icon.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/dpms_icon_dark.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/edit_icon.svg
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/edit_icon_disable.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/edit_notebook_icon.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/error_icon.svg
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/expand_less.svg
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/expand_more.svg
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/filter_icon.svg
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_file_icon.svg
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_file_icon_dark.svg
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_folder_icon.svg
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_folder_icon_dark.svg
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_folder_new_icon.svg
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_refresh_icon.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_search_icon.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/gcs_upload_icon.svg
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/google-cloud.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/keyboard_arrow_down.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/left_arrow_icon.svg
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/logs_icon.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/next_page.svg
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/notebook_scheduler.svg
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/notebook_template_icon.svg
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/pause_icon.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/play_icon.svg
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/plus_icon.svg
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/plus_icon_disable.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/previous_page.svg
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/refresh_cluster_icon.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/refresh_icon.svg
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/restart_icon.svg
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/restart_icon_disable.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/right_arrow_icon.svg
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduled_notebooks_icon.svg
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_calendar_month.svg
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_delete.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_download.svg
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_edit_calendar.svg
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_edit_dag.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_pause.svg
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_play.svg
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/scheduler_trigger.svg
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/search_clear_icon.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/search_icon.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/search_icon_dark.svg
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/serverless_icon.svg
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/session_logs_icon.svg
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/settings_icon.svg
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/signin_google_icon.svg
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/start_cluster_icon.svg
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/start_cluster_icon_disable.svg
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/start_icon.svg
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/start_icon_disable.svg
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/stop_cluster_disable_icon.svg
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/stop_cluster_icon.svg
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/stop_disable_icon.svg
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/stop_icon.svg
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/stop_icon_disable.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/storage_icon.svg
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/submit_job_icon.svg
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/succeeded_icon.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/table_icon.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/table_icon_dark.svg
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/style/icons/view_logs_icon.svg
--rw-r--r--   0        0        0    10642 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/third_party/icons/pyspark_logo.svg
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/third_party/icons/python_logo.svg
--rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/third_party/icons/scala_logo.svg
--rw-r--r--   0        0        0    12024 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/third_party/icons/sparkr_logo.svg
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/ui-tests-3.6.6/README.md
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/ui-tests-3.6.6/jupyter_server_test_config.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/ui-tests-3.6.6/package.json
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/ui-tests-3.6.6/playwright.config.js
--rw-r--r--   0        0        0   131355 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/ui-tests-3.6.6/yarn.lock
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/ui-tests-3.6.6/tests/create_and_run_notebook.spec.ts
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/ui-tests-3.6.6/tests/settings_menu.spec.ts
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/LICENSE
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/README.md
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/pyproject.toml
--rw-r--r--   0        0        0    18684 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.78/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/RELEASE.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/babel.config.js
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/conftest.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/contributing.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/install.json
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/jest.config.js
+-rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/package.json
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/setup.py
+-rw-r--r--   0        0        0   161051 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/third-party-licenses.txt
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/tsconfig.test.json
+-rw-r--r--   0        0        0   438849 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/yarn.lock
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/_version.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/handlers.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/package.json
+-rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/schemas/dataproc_jupyter_plugin/package.json.orig
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/schemas/dataproc_jupyter_plugin/plugin.json
+-rw-r--r--   0        0        0   459810 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/103.ca53a71bbc39110a5446.js
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/103.ca53a71bbc39110a5446.js.LICENSE.txt
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/149.8f7854132903921d52a7.js
+-rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/224.e2fb2e283cf662fad21a.js
+-rw-r--r--   0        0        0   113855 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/259.df21118f4412cb9f48f8.js
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/259.df21118f4412cb9f48f8.js.LICENSE.txt
+-rw-r--r--   0        0        0   390837 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/282a64fb600cdac6ff79.svg
+-rw-r--r--   0        0        0    98404 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/42e369dc8c372973ba77.ttf
+-rw-r--r--   0        0        0    48880 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/431.0fe2364679fa00131586.js
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/431.0fe2364679fa00131586.js.LICENSE.txt
+-rw-r--r--   0        0        0    40148 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/434466b59545a8a1cac6.woff2
+-rw-r--r--   0        0        0    31156 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/4537fa06340ee62c264e.eot
+-rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/4bc359c27057b3ed0bac.woff
+-rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/4d2883443b24e424527f.woff2
+-rw-r--r--   0        0        0    57790 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/521.b4d3a2e8ae1079c1a368.js
+-rw-r--r--   0        0        0   264500 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/557.fa15c682905297847f16.js
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/557.fa15c682905297847f16.js.LICENSE.txt
+-rw-r--r--   0        0        0   558079 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/62.40e66fd78360da8433f1.js
+-rw-r--r--   0        0        0   507628 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/6519a15b08294be395ed.svg
+-rw-r--r--   0        0        0    30928 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/67172172eafce4563725.ttf
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/701.d51f75217c376d145919.js
+-rw-r--r--   0        0        0   106004 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/8b4e1b847e22233d4f46.eot
+-rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/937.40d418f92b7c5543ccf5.js
+-rw-r--r--   0        0        0    28123 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/94d5c7f1661301c4a6dc.png
+-rw-r--r--   0        0        0    50524 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/95b6a4840f8711ecab42.woff
+-rw-r--r--   0        0        0    42078 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/965.d85d4a0e1daf39f35245.js
+-rw-r--r--   0        0        0    63728 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/9fafd6c3e7bfc145db42.woff
+-rw-r--r--   0        0        0   107201 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/ae8fd02a7bb87479fe46.svg
+-rw-r--r--   0        0        0   105784 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/cb7f81f542f5c418a3bb.ttf
+-rw-r--r--   0        0        0    98640 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/d023c55fde220495f13a.eot
+-rw-r--r--   0        0        0    54488 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/e7d4d5340bbe57a01d8f.woff2
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/remoteEntry.0fa053e6df8a75cdf288.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/style.js
+-rw-r--r--   0        0        0    42566 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/tests/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/tests/test_handlers.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/jupyter-config/nb-config/dataproc_jupyter_plugin.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/jupyter-config/server-config/dataproc_jupyter_plugin.json
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/schema/plugin.json
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/custom.d.ts
+-rw-r--r--   0        0        0    11918 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/index.ts
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/react-table-config.d.ts
+-rw-r--r--   0        0        0    23145 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/batches/batchDetails.tsx
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/batches/batches.tsx
+-rw-r--r--   0        0        0    61122 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/batches/createBatch.tsx
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/batches/listBatches.tsx
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/cluster/cluster.tsx
+-rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/cluster/clusterDetails.tsx
+-rw-r--r--   0        0        0     8331 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/cluster/listCluster.tsx
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/dpms/databaseInfo.tsx
+-rw-r--r--   0        0        0    23420 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/dpms/dpmsWidget.tsx
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/dpms/tableInfo.tsx
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/handler/handler.ts
+-rw-r--r--   0        0        0    27277 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/jobs/jobDetails.tsx
+-rw-r--r--   0        0        0    17607 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/jobs/jobs.tsx
+-rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/jobs/labelProperties.tsx
+-rw-r--r--   0        0        0    37357 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/jobs/submitJob.tsx
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/login/authLogin.tsx
+-rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/login/configSelection.tsx
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/login/projectIdDropdown.tsx
+-rw-r--r--   0        0        0    40368 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/runtime/createRunTime.tsx
+-rw-r--r--   0        0        0    13798 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/runtime/listRuntimeTemplates.tsx
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/runtime/runtimeTemplate.tsx
+-rw-r--r--   0        0        0    14002 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/sessions/listSessions.tsx
+-rw-r--r--   0        0        0    14664 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/sessions/sessionDetails.tsx
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/batchService.tsx
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/clusterServices.tsx
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/const.ts
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/deletePopup.tsx
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/errorPopup.tsx
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/globalFilter.tsx
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/jobDetailsInterface.ts
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/jobServices.tsx
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/listRuntimeTemplateInterface.ts
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/paginationView.tsx
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/pollingTimer.ts
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/projectService.ts
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/runtimeService.tsx
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/sessionService.tsx
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/statusDisplay.tsx
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/tableData.tsx
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/utils.ts
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/src/utils/viewLogs.tsx
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/authLogin.css
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/base.css
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/batches.css
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/cluster.css
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/clusterDetails.css
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/createBatch.css
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/databaseInfo.css
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/dpms.css
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/index.css
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/index.js
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/job.css
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/paginationView.css
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/popup.css
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/runtimeTemplate.css
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/sessionDetails.css
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/submitJob.css
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/add_account_icon.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/add_runtime_template.svg
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/clone_icon.svg
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/clone_icon_disable.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/clone_job_icon.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/clone_job_icon_disable.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/cluster_error_icon.svg
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/cluster_icon.svg
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/cluster_running_icon.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/columns_icon.svg
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/create_cluster_icon.svg
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/database_icon.svg
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/database_widget_icon.svg
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/dataproc_icon.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/datasets_icon.svg
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/delete_cluster_icon.svg
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/delete_icon.svg
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/down_arrow_icon.svg
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/dpms_icon.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/edit_icon.svg
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/edit_icon_disable.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/error_icon.svg
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/expand_less.svg
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/expand_more.svg
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/filter_icon.svg
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/left_arrow_icon.svg
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/plus_icon.svg
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/plus_icon_disable.svg
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/refresh_cluster_icon.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/refresh_icon.svg
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/restart_icon.svg
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/restart_icon_disable.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/right_arrow_icon.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/search_clear_icon.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/search_icon.svg
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/serverless_icon.svg
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/settings_icon.svg
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/signin_google_icon.svg
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/start_cluster_icon.svg
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/start_cluster_icon_disable.svg
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/start_icon.svg
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/start_icon_disable.svg
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/stop_cluster_disable_icon.svg
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/stop_cluster_icon.svg
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/stop_disable_icon.svg
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/stop_icon.svg
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/stop_icon_disable.svg
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/submit_job_icon.svg
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/succeeded_icon.svg
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/table_icon.svg
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/style/icons/view_logs_icon.svg
+-rw-r--r--   0        0        0    10642 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/third_party/icons/pyspark_logo.svg
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/third_party/icons/python_logo.svg
+-rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/third_party/icons/scala_logo.svg
+-rw-r--r--   0        0        0    12024 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/third_party/icons/sparkr_logo.svg
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/README.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    18510 2020-02-02 00:00:00.000000 dataproc_jupyter_plugin-0.1.9/PKG-INFO
```

### Comparing `dataproc_jupyter_plugin-0.1.78/RELEASE.md` & `dataproc_jupyter_plugin-0.1.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/babel.config.js` & `dataproc_jupyter_plugin-0.1.9/babel.config.js`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/conftest.py` & `dataproc_jupyter_plugin-0.1.9/conftest.py`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/contributing.md` & `dataproc_jupyter_plugin-0.1.9/contributing.md`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/jest.config.js` & `dataproc_jupyter_plugin-0.1.9/jest.config.js`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/package.json` & `dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/package.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9542571428571428%*

 * *Differences: {"'dependencies'": "{'react-tagsinput': '^3.20.3', 'semantic-ui-css': '^2.5.0', "*

 * *                   "'semantic-ui-react': '^2.1.4', delete: ['@emotion/react', '@emotion/styled', "*

 * *                   "'@mui/icons-material', '@mui/material', '@mui/x-date-pickers', 'antd', "*

 * *                   "'dayjs', 'mui-chips-input', 'react-js-cron', 'tzdata', 'yup']}",*

 * * "'devDependencies'": "{delete: ['@babel/preset-env', '@babel/preset-react', "*

 * *                      "'@babel/preset-typescript', '@googleapis/storage',  […]*

```diff
@@ -3,97 +3,68 @@
         "email": "dataproc-plugins@google.com",
         "name": "google"
     },
     "bugs": {
         "url": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin/issues"
     },
     "dependencies": {
-        "@emotion/react": "^11.11.1",
-        "@emotion/styled": "^11.11.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
-        "@mui/icons-material": "^5.14.7",
-        "@mui/material": "^5.14.7",
-        "@mui/x-date-pickers": "^6.18.6",
         "@types/uuid": "^9.0.2",
-        "antd": "^5.12.8",
-        "dayjs": "^1.11.10",
-        "mui-chips-input": "^2.1.3",
         "react-arborist": "^3.1.0",
-        "react-js-cron": "^5.0.1",
         "react-spinners": "^0.13.8",
         "react-table": "^7.8.0",
+        "react-tagsinput": "^3.20.3",
         "react-toastify": "^9.1.3",
-        "tzdata": "^1.0.39",
-        "yup": "^1.2.0"
+        "semantic-ui-css": "^2.5.0",
+        "semantic-ui-react": "^2.1.4"
     },
     "description": "It is a plugin to work with dataproc services in Jupyterlab",
     "devDependencies": {
-        "@babel/preset-env": "^7.22.14",
-        "@babel/preset-react": "^7.22.5",
-        "@babel/preset-typescript": "^7.22.11",
-        "@googleapis/storage": "^6.0.0",
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
-        "@storybook/addon-essentials": "^7.4.0",
-        "@storybook/addon-interactions": "^7.4.0",
-        "@storybook/addon-links": "^7.4.0",
-        "@storybook/addon-onboarding": "^1.0.8",
-        "@storybook/blocks": "^7.4.0",
-        "@storybook/react": "^7.4.0",
-        "@storybook/react-webpack5": "^7.4.0",
-        "@storybook/testing-library": "^0.2.0",
         "@types/hoist-non-react-statics": "^3.3.1",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
-        "@types/react-dom": "^18.2.11",
         "@types/react-table": "^7.7.14",
         "@types/react-tagsinput": "^3.20.0",
         "@types/react-window": "^1.8.5",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
         "eslint-plugin-prettier": "^4.2.1",
-        "eslint-plugin-storybook": "^0.6.13",
         "generate-license-file": "^2.0.0",
         "jest": "^29.2.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.7",
-        "react": "^18.2.0",
-        "react-dom": "^18.2.0",
-        "react-tagsinput": "^3.20.3",
         "rimraf": "^4.4.1",
-        "semantic-ui-react": "^2.1.4",
         "source-map-loader": "^1.0.2",
-        "storybook": "^7.4.0",
         "style-loader": "^3.3.1",
         "stylelint": "^14.9.1",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^8.0.0",
         "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
         "typescript": "~5.0.2",
-        "webpack": "^5.88.2",
         "yjs": "^13.5.0"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
-            "plugin:prettier/recommended",
-            "plugin:storybook/recommended"
+            "plugin:prettier/recommended"
         ],
         "parser": "@typescript-eslint/parser",
         "parserOptions": {
             "project": "tsconfig.json",
             "sourceType": "module"
         },
         "plugins": [
@@ -150,14 +121,19 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.0fa053e6df8a75cdf288.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "dataproc_jupyter_plugin"
                 },
                 "managers": [
                     "pip"
@@ -187,35 +163,32 @@
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
-        "build-storybook": "storybook build",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf dataproc_jupyter_plugin/labextension dataproc_jupyter_plugin/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
-        "licenses": "jlpm generate-license-file --input package.json --output third-party-licenses.txt --overwrite",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "storybook": "storybook dev -p 6006",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
@@ -234,12 +207,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.78",
+    "version": "0.1.9",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/setup.py` & `dataproc_jupyter_plugin-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/tsconfig.json` & `dataproc_jupyter_plugin-0.1.9/tsconfig.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'compilerOptions'": "{'types': {delete: [1]}}"}*

```diff
@@ -16,16 +16,15 @@
         "resolveJsonModule": true,
         "rootDir": "src",
         "skipLibCheck": true,
         "strict": true,
         "strictNullChecks": true,
         "target": "ES2018",
         "types": [
-            "jest",
-            "node"
+            "jest"
         ]
     },
     "include": [
         "src/*",
         "src/**/*"
     ]
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/__mocks__/utils.ts` & `dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/tests/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-/**
- * @license
- * Copyright 2023 Google LLC
- *
- * Licensed under the Apache License, Version 2.0 (the "License");
- * you may not use this file except in compliance with the License.
- * You may obtain a copy of the License at
- *
- *   http://www.apache.org/licenses/LICENSE-2.0
- *
- * Unless required by applicable law or agreed to in writing, software
- * distributed under the License is distributed on an "AS IS" BASIS,
- * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
- * See the License for the specific language governing permissions and
- * limitations under the License.
- */
-export const authApi = async () => {
-  return {
-    access_token: 'storybook-access-token',
-    project_id: 'storybook-project',
-    region_id: 'storybook-region'
-  };
-};
+# Copyright 2023 Google LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Python unit tests for dataproc_jupyter_plugin."""
```

### Comparing `dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/package.json` & `dataproc_jupyter_plugin-0.1.9/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9542571428571428%*

 * *Differences: {"'dependencies'": "{'react-tagsinput': '^3.20.3', 'semantic-ui-css': '^2.5.0', "*

 * *                   "'semantic-ui-react': '^2.1.4', delete: ['@emotion/react', '@emotion/styled', "*

 * *                   "'@mui/icons-material', '@mui/material', '@mui/x-date-pickers', 'antd', "*

 * *                   "'dayjs', 'mui-chips-input', 'react-js-cron', 'tzdata', 'yup']}",*

 * * "'devDependencies'": "{delete: ['@babel/preset-env', '@babel/preset-react', "*

 * *                      "'@babel/preset-typescript', '@googleapis/storage',  […]*

```diff
@@ -3,97 +3,68 @@
         "email": "dataproc-plugins@google.com",
         "name": "google"
     },
     "bugs": {
         "url": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin/issues"
     },
     "dependencies": {
-        "@emotion/react": "^11.11.1",
-        "@emotion/styled": "^11.11.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
-        "@mui/icons-material": "^5.14.7",
-        "@mui/material": "^5.14.7",
-        "@mui/x-date-pickers": "^6.18.6",
         "@types/uuid": "^9.0.2",
-        "antd": "^5.12.8",
-        "dayjs": "^1.11.10",
-        "mui-chips-input": "^2.1.3",
         "react-arborist": "^3.1.0",
-        "react-js-cron": "^5.0.1",
         "react-spinners": "^0.13.8",
         "react-table": "^7.8.0",
+        "react-tagsinput": "^3.20.3",
         "react-toastify": "^9.1.3",
-        "tzdata": "^1.0.39",
-        "yup": "^1.2.0"
+        "semantic-ui-css": "^2.5.0",
+        "semantic-ui-react": "^2.1.4"
     },
     "description": "It is a plugin to work with dataproc services in Jupyterlab",
     "devDependencies": {
-        "@babel/preset-env": "^7.22.14",
-        "@babel/preset-react": "^7.22.5",
-        "@babel/preset-typescript": "^7.22.11",
-        "@googleapis/storage": "^6.0.0",
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
-        "@storybook/addon-essentials": "^7.4.0",
-        "@storybook/addon-interactions": "^7.4.0",
-        "@storybook/addon-links": "^7.4.0",
-        "@storybook/addon-onboarding": "^1.0.8",
-        "@storybook/blocks": "^7.4.0",
-        "@storybook/react": "^7.4.0",
-        "@storybook/react-webpack5": "^7.4.0",
-        "@storybook/testing-library": "^0.2.0",
         "@types/hoist-non-react-statics": "^3.3.1",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
-        "@types/react-dom": "^18.2.11",
         "@types/react-table": "^7.7.14",
         "@types/react-tagsinput": "^3.20.0",
         "@types/react-window": "^1.8.5",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
         "eslint-plugin-prettier": "^4.2.1",
-        "eslint-plugin-storybook": "^0.6.13",
         "generate-license-file": "^2.0.0",
         "jest": "^29.2.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.7",
-        "react": "^18.2.0",
-        "react-dom": "^18.2.0",
-        "react-tagsinput": "^3.20.3",
         "rimraf": "^4.4.1",
-        "semantic-ui-react": "^2.1.4",
         "source-map-loader": "^1.0.2",
-        "storybook": "^7.4.0",
         "style-loader": "^3.3.1",
         "stylelint": "^14.9.1",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^8.0.0",
         "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
         "typescript": "~5.0.2",
-        "webpack": "^5.88.2",
         "yjs": "^13.5.0"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
-            "plugin:prettier/recommended",
-            "plugin:storybook/recommended"
+            "plugin:prettier/recommended"
         ],
         "parser": "@typescript-eslint/parser",
         "parserOptions": {
             "project": "tsconfig.json",
             "sourceType": "module"
         },
         "plugins": [
@@ -150,19 +121,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.ad737b405a4fd7314581.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "dataproc_jupyter_plugin"
                 },
                 "managers": [
                     "pip"
@@ -192,35 +158,32 @@
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
-        "build-storybook": "storybook build",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf dataproc_jupyter_plugin/labextension dataproc_jupyter_plugin/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
-        "licenses": "jlpm generate-license-file --input package.json --output third-party-licenses.txt --overwrite",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "storybook": "storybook dev -p 6006",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
@@ -239,12 +202,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.78",
+    "version": "0.1.9",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/labextension/schemas/dataproc_jupyter_plugin/package.json.orig` & `dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/labextension/schemas/dataproc_jupyter_plugin/package.json.orig`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9582571428571428%*

 * *Differences: {"'dependencies'": "{'react-tagsinput': '^3.20.3', 'semantic-ui-css': '^2.5.0', "*

 * *                   "'semantic-ui-react': '^2.1.4', delete: ['@emotion/react', '@emotion/styled', "*

 * *                   "'@mui/icons-material', '@mui/material', '@mui/x-date-pickers', 'antd', "*

 * *                   "'dayjs', 'mui-chips-input', 'react-js-cron', 'tzdata', 'yup']}",*

 * * "'devDependencies'": "{delete: ['@babel/preset-env', '@babel/preset-react', "*

 * *                      "'@babel/preset-typescript', '@googleapis/storage',  […]*

```diff
@@ -3,97 +3,68 @@
         "email": "dataproc-plugins@google.com",
         "name": "google"
     },
     "bugs": {
         "url": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin/issues"
     },
     "dependencies": {
-        "@emotion/react": "^11.11.1",
-        "@emotion/styled": "^11.11.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
-        "@mui/icons-material": "^5.14.7",
-        "@mui/material": "^5.14.7",
-        "@mui/x-date-pickers": "^6.18.6",
         "@types/uuid": "^9.0.2",
-        "antd": "^5.12.8",
-        "dayjs": "^1.11.10",
-        "mui-chips-input": "^2.1.3",
         "react-arborist": "^3.1.0",
-        "react-js-cron": "^5.0.1",
         "react-spinners": "^0.13.8",
         "react-table": "^7.8.0",
+        "react-tagsinput": "^3.20.3",
         "react-toastify": "^9.1.3",
-        "tzdata": "^1.0.39",
-        "yup": "^1.2.0"
+        "semantic-ui-css": "^2.5.0",
+        "semantic-ui-react": "^2.1.4"
     },
     "description": "It is a plugin to work with dataproc services in Jupyterlab",
     "devDependencies": {
-        "@babel/preset-env": "^7.22.14",
-        "@babel/preset-react": "^7.22.5",
-        "@babel/preset-typescript": "^7.22.11",
-        "@googleapis/storage": "^6.0.0",
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
-        "@storybook/addon-essentials": "^7.4.0",
-        "@storybook/addon-interactions": "^7.4.0",
-        "@storybook/addon-links": "^7.4.0",
-        "@storybook/addon-onboarding": "^1.0.8",
-        "@storybook/blocks": "^7.4.0",
-        "@storybook/react": "^7.4.0",
-        "@storybook/react-webpack5": "^7.4.0",
-        "@storybook/testing-library": "^0.2.0",
         "@types/hoist-non-react-statics": "^3.3.1",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
-        "@types/react-dom": "^18.2.11",
         "@types/react-table": "^7.7.14",
         "@types/react-tagsinput": "^3.20.0",
         "@types/react-window": "^1.8.5",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
         "eslint-plugin-prettier": "^4.2.1",
-        "eslint-plugin-storybook": "^0.6.13",
         "generate-license-file": "^2.0.0",
         "jest": "^29.2.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.7",
-        "react": "^18.2.0",
-        "react-dom": "^18.2.0",
-        "react-tagsinput": "^3.20.3",
         "rimraf": "^4.4.1",
-        "semantic-ui-react": "^2.1.4",
         "source-map-loader": "^1.0.2",
-        "storybook": "^7.4.0",
         "style-loader": "^3.3.1",
         "stylelint": "^14.9.1",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^8.0.0",
         "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
         "typescript": "~5.0.2",
-        "webpack": "^5.88.2",
         "yjs": "^13.5.0"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
-            "plugin:prettier/recommended",
-            "plugin:storybook/recommended"
+            "plugin:prettier/recommended"
         ],
         "parser": "@typescript-eslint/parser",
         "parserOptions": {
             "project": "tsconfig.json",
             "sourceType": "module"
         },
         "plugins": [
@@ -187,35 +158,32 @@
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
-        "build-storybook": "storybook build",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf dataproc_jupyter_plugin/labextension dataproc_jupyter_plugin/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
-        "licenses": "jlpm generate-license-file --input package.json --output third-party-licenses.txt --overwrite",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "storybook": "storybook dev -p 6006",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
@@ -234,12 +202,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.78",
+    "version": "0.1.9",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/dataproc_jupyter_plugin/tests/test_handlers.py` & `dataproc_jupyter_plugin-0.1.9/dataproc_jupyter_plugin/tests/test_handlers.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,27 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 
 
-async def test_get_default_settings(jp_fetch):
-    response = await jp_fetch("dataproc-plugin", "settings")
+async def test_get_example(jp_fetch):
+    # When
+    response = await jp_fetch("dataproc-plugin", "get-example")
 
+    # Then
     assert response.code == 200
     payload = json.loads(response.body)
-    assert "enable_bigquery_integration" in payload
-    assert "log_path" in payload
-    assert payload["enable_bigquery_integration"] is False
-    assert payload["log_path"] is ""
-
-
-async def test_get_modified_settings(jp_fetch, jp_serverapp):
-    jp_serverapp.config.DataprocPluginConfig.enable_bigquery_integration = True
-    response = await jp_fetch("dataproc-plugin", "settings")
-    assert response.code == 200
-    payload = json.loads(response.body)
-    assert "enable_bigquery_integration" in payload
-    assert "log_path" in payload
-    assert payload["enable_bigquery_integration"] is True
-    assert payload["log_path"] is ""
+    assert payload == {
+        "data": "This is /dataproc-plugin/get-example endpoint!"
+    }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/custom.d.ts` & `dataproc_jupyter_plugin-0.1.9/src/custom.d.ts`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/src/react-table-config.d.ts` & `dataproc_jupyter_plugin-0.1.9/src/react-table-config.d.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,120 +1,120 @@
 import {
-  UseColumnOrderInstanceProps,
-  UseColumnOrderState,
-  UseExpandedHooks,
-  UseExpandedInstanceProps,
-  UseExpandedOptions,
-  UseExpandedRowProps,
-  UseExpandedState,
-  UseFiltersColumnOptions,
-  UseFiltersColumnProps,
-  UseFiltersInstanceProps,
-  UseFiltersOptions,
-  UseFiltersState,
-  UseGlobalFiltersColumnOptions,
-  UseGlobalFiltersInstanceProps,
-  UseGlobalFiltersOptions,
-  UseGlobalFiltersState,
-  UseGroupByCellProps,
-  UseGroupByColumnOptions,
-  UseGroupByColumnProps,
-  UseGroupByHooks,
-  UseGroupByInstanceProps,
-  UseGroupByOptions,
-  UseGroupByRowProps,
-  UseGroupByState,
-  UsePaginationInstanceProps,
-  UsePaginationOptions,
-  UsePaginationState,
-  UseResizeColumnsColumnOptions,
-  UseResizeColumnsColumnProps,
-  UseResizeColumnsOptions,
-  UseResizeColumnsState,
-  UseRowSelectHooks,
-  UseRowSelectInstanceProps,
-  UseRowSelectOptions,
-  UseRowSelectRowProps,
-  UseRowSelectState,
-  UseRowStateCellProps,
-  UseRowStateInstanceProps,
-  UseRowStateOptions,
-  UseRowStateRowProps,
-  UseRowStateState,
-  UseSortByColumnOptions,
-  UseSortByColumnProps,
-  UseSortByHooks,
-  UseSortByInstanceProps,
-  UseSortByOptions,
-  UseSortByState
-} from 'react-table'
-
-declare module 'react-table' {
-  // take this file as-is, or comment out the sections that don't apply to your plugin configuration
-
-  export interface TableOptions<D extends Record<string, unknown>>
-    extends UseExpandedOptions<D>,
-    UseFiltersOptions<D>,
-    UseGlobalFiltersOptions<D>,
-    UseGroupByOptions<D>,
-    UsePaginationOptions<D>,
-    UseResizeColumnsOptions<D>,
-    UseRowSelectOptions<D>,
-    UseRowStateOptions<D>,
-    UseSortByOptions<D>,
-    // note that having Record here allows you to add anything to the options, this matches the spirit of the
-    // underlying js library, but might be cleaner if it's replaced by a more specific type that matches your
-    // feature set, this is a safe default.
-    Record<string, unknown> { }
-
-  export interface Hooks<D extends Record<string, unknown> = Record<string, unknown>>
-    extends UseExpandedHooks<D>,
-    UseGroupByHooks<D>,
-    UseRowSelectHooks<D>,
-    UseSortByHooks<D> { }
-
-  export interface TableInstance<D extends Record<string, unknown> = Record<string, unknown>>
-    extends UseColumnOrderInstanceProps<D>,
-    UseExpandedInstanceProps<D>,
-    UseFiltersInstanceProps<D>,
-    UseGlobalFiltersInstanceProps<D>,
-    UseGroupByInstanceProps<D>,
-    UsePaginationInstanceProps<D>,
-    UseRowSelectInstanceProps<D>,
-    UseRowStateInstanceProps<D>,
-    UseSortByInstanceProps<D> { }
-
-  export interface TableState<D extends Record<string, unknown> = Record<string, unknown>>
-    extends UseColumnOrderState<D>,
-    UseExpandedState<D>,
-    UseFiltersState<D>,
-    UseGlobalFiltersState<D>,
-    UseGroupByState<D>,
-    UsePaginationState<D>,
-    UseResizeColumnsState<D>,
-    UseRowSelectState<D>,
-    UseRowStateState<D>,
-    UseSortByState<D> { }
-
-  export interface ColumnInterface<D extends Record<string, unknown> = Record<string, unknown>>
-    extends UseFiltersColumnOptions<D>,
-    UseGlobalFiltersColumnOptions<D>,
-    UseGroupByColumnOptions<D>,
-    UseResizeColumnsColumnOptions<D>,
-    UseSortByColumnOptions<D> { }
-
-  export interface ColumnInstance<D extends Record<string, unknown> = Record<string, unknown>>
-    extends UseFiltersColumnProps<D>,
-    UseGroupByColumnProps<D>,
-    UseResizeColumnsColumnProps<D>,
-    UseSortByColumnProps<D> { }
-
-  export interface Cell<D extends Record<string, unknown> = Record<string, unknown>, V = unknown>
-    extends UseGroupByCellProps<D>,
-    UseRowStateCellProps<D> { }
-
-  export interface Row<D extends Record<string, unknown> = Record<string, unknown>>
-    extends UseExpandedRowProps<D>,
-    UseGroupByRowProps<D>,
-    UseRowSelectRowProps<D>,
-    UseRowStateRowProps<D> { }
-}
+    UseColumnOrderInstanceProps,
+    UseColumnOrderState,
+    UseExpandedHooks,
+    UseExpandedInstanceProps,
+    UseExpandedOptions,
+    UseExpandedRowProps,
+    UseExpandedState,
+    UseFiltersColumnOptions,
+    UseFiltersColumnProps,
+    UseFiltersInstanceProps,
+    UseFiltersOptions,
+    UseFiltersState,
+    UseGlobalFiltersColumnOptions,
+    UseGlobalFiltersInstanceProps,
+    UseGlobalFiltersOptions,
+    UseGlobalFiltersState,
+    UseGroupByCellProps,
+    UseGroupByColumnOptions,
+    UseGroupByColumnProps,
+    UseGroupByHooks,
+    UseGroupByInstanceProps,
+    UseGroupByOptions,
+    UseGroupByRowProps,
+    UseGroupByState,
+    UsePaginationInstanceProps,
+    UsePaginationOptions,
+    UsePaginationState,
+    UseResizeColumnsColumnOptions,
+    UseResizeColumnsColumnProps,
+    UseResizeColumnsOptions,
+    UseResizeColumnsState,
+    UseRowSelectHooks,
+    UseRowSelectInstanceProps,
+    UseRowSelectOptions,
+    UseRowSelectRowProps,
+    UseRowSelectState,
+    UseRowStateCellProps,
+    UseRowStateInstanceProps,
+    UseRowStateOptions,
+    UseRowStateRowProps,
+    UseRowStateState,
+    UseSortByColumnOptions,
+    UseSortByColumnProps,
+    UseSortByHooks,
+    UseSortByInstanceProps,
+    UseSortByOptions,
+    UseSortByState
+  } from 'react-table'
+  
+  declare module 'react-table' {
+    // take this file as-is, or comment out the sections that don't apply to your plugin configuration
+  
+    export interface TableOptions<D extends Record<string, unknown>>
+      extends UseExpandedOptions<D>,
+        UseFiltersOptions<D>,
+        UseGlobalFiltersOptions<D>,
+        UseGroupByOptions<D>,
+        UsePaginationOptions<D>,
+        UseResizeColumnsOptions<D>,
+        UseRowSelectOptions<D>,
+        UseRowStateOptions<D>,
+        UseSortByOptions<D>,
+        // note that having Record here allows you to add anything to the options, this matches the spirit of the
+        // underlying js library, but might be cleaner if it's replaced by a more specific type that matches your
+        // feature set, this is a safe default.
+        Record<string, any> {}
+  
+    export interface Hooks<D extends Record<string, unknown> = Record<string, unknown>>
+      extends UseExpandedHooks<D>,
+        UseGroupByHooks<D>,
+        UseRowSelectHooks<D>,
+        UseSortByHooks<D> {}
+  
+    export interface TableInstance<D extends Record<string, unknown> = Record<string, unknown>>
+      extends UseColumnOrderInstanceProps<D>,
+        UseExpandedInstanceProps<D>,
+        UseFiltersInstanceProps<D>,
+        UseGlobalFiltersInstanceProps<D>,
+        UseGroupByInstanceProps<D>,
+        UsePaginationInstanceProps<D>,
+        UseRowSelectInstanceProps<D>,
+        UseRowStateInstanceProps<D>,
+        UseSortByInstanceProps<D> {}
+  
+    export interface TableState<D extends Record<string, unknown> = Record<string, unknown>>
+      extends UseColumnOrderState<D>,
+        UseExpandedState<D>,
+        UseFiltersState<D>,
+        UseGlobalFiltersState<D>,
+        UseGroupByState<D>,
+        UsePaginationState<D>,
+        UseResizeColumnsState<D>,
+        UseRowSelectState<D>,
+        UseRowStateState<D>,
+        UseSortByState<D> {}
+  
+    export interface ColumnInterface<D extends Record<string, unknown> = Record<string, unknown>>
+      extends UseFiltersColumnOptions<D>,
+        UseGlobalFiltersColumnOptions<D>,
+        UseGroupByColumnOptions<D>,
+        UseResizeColumnsColumnOptions<D>,
+        UseSortByColumnOptions<D> {}
+  
+    export interface ColumnInstance<D extends Record<string, unknown> = Record<string, unknown>>
+      extends UseFiltersColumnProps<D>,
+        UseGroupByColumnProps<D>,
+        UseResizeColumnsColumnProps<D>,
+        UseSortByColumnProps<D> {}
+  
+    export interface Cell<D extends Record<string, unknown> = Record<string, unknown>, V = any>
+      extends UseGroupByCellProps<D>,
+        UseRowStateCellProps<D> {}
+  
+    export interface Row<D extends Record<string, unknown> = Record<string, unknown>>
+      extends UseExpandedRowProps<D>,
+        UseGroupByRowProps<D>,
+        UseRowSelectRowProps<D>,
+        UseRowStateRowProps<D> {}
+  }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/batches/batchDetails.tsx` & `dataproc_jupyter_plugin-0.1.9/src/batches/batchDetails.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 
 import React, { useState, useEffect, useRef } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
 import LeftArrowIcon from '../../style/icons/left_arrow_icon.svg';
 import CloneJobIcon from '../../style/icons/clone_job_icon.svg';
 import ViewLogs from '../utils/viewLogs';
 import DeleteClusterIcon from '../../style/icons/delete_cluster_icon.svg';
+
+import { ClipLoader } from 'react-spinners';
 import {
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
   DATAPROC_CLUSTER_KEY,
   DATAPROC_CLUSTER_LABEL,
   BATCH_FIELDS_EXCLUDED,
   METASTORE_SERVICE_KEY,
   METASTORE_SERVICE_LABEL,
   NETWORK_KEY,
   NETWORK_LABEL,
@@ -36,71 +41,62 @@
   SPARK_HISTORY_SERVER,
   SPARK_HISTORY_SERVER_KEY,
   SUBNETWORK_KEY,
   SUBNETWORK_LABEL
 } from '../utils/const';
 import {
   BatchTypeValue,
-  IBatchInfoResponse,
+  authApi,
   batchDetailsOptionalDisplay,
   convertToDCUHours,
   convertToGBMonths,
   elapsedTime,
   jobTimeFormat,
   statusMessageBatch
 } from '../utils/utils';
 import DeletePopup from '../utils/deletePopup';
+import { toast, ToastContainer } from 'react-toastify';
 import 'react-toastify/dist/ReactToastify.css';
-import { BatchService } from './batchService';
+import { deleteBatchAPI } from '../utils/batchService';
 import { statusDisplay } from '../utils/statusDisplay';
 import PollingTimer from '../utils/pollingTimer';
-import CreateBatch from './createBatch';
-import errorIcon from '../../style/icons/error_icon.svg';
-import { CircularProgress } from '@mui/material';
 
 const iconLeftArrow = new LabIcon({
   name: 'launcher:left-arrow-icon',
   svgstr: LeftArrowIcon
 });
 const iconCloneJob = new LabIcon({
   name: 'launcher:clone-job-icon',
   svgstr: CloneJobIcon
 });
 const iconDeleteCluster = new LabIcon({
   name: 'launcher:delete-cluster-icon',
   svgstr: DeleteClusterIcon
 });
-const iconError = new LabIcon({
-  name: 'launcher:error-icon',
-  svgstr: errorIcon
-});
 
 type BatchDetailsProps = {
   batchSelected: string;
   setDetailedBatchView: (flag: boolean) => void;
-  setCreateBatchView: (flag: boolean) => void;
 };
 
 function BatchDetails({
   batchSelected,
-  setDetailedBatchView,
-  setCreateBatchView
+  setDetailedBatchView
 }: BatchDetailsProps) {
   const [batchInfoResponse, setBatchInfoResponse] = useState({
     uuid: '',
     state: '',
     createTime: '',
     runtimeInfo: {
       endpoints: {},
       approximateUsage: { milliDcuSeconds: '', shuffleStorageGbSeconds: '' }
     },
     creator: '',
     runtimeConfig: {
       version: '',
-      containerImage: '',
       properties: {
         'spark:spark.executor.instances': '',
         'spark:spark.driver.cores': '',
         'spark:spark.driver.memory': '',
         'spark:spark.executor.cores': '',
         'spark:spark.executor.memory': '',
         'spark:spark.dynamicAllocation.executorAllocationRatio': '',
@@ -135,22 +131,18 @@
         }
       }
     },
     stateHistory: [{ state: '', stateStartTime: '' }],
     stateTime: ''
   });
   const [regionName, setRegionName] = useState('');
-  const [errorView, setErrorView] = useState(false);
   const [labelDetail, setLabelDetail] = useState(['']);
   const [isLoading, setIsLoading] = useState(true);
   const [deletePopupOpen, setDeletePopupOpen] = useState(false);
   const [selectedBatch, setSelectedBatch] = useState('');
-  const [projectName, setProjectName] = useState('');
-  const [createBatch, setCreateBatch] = useState(false);
-
   const timer = useRef<NodeJS.Timeout | undefined>(undefined);
 
   const pollingBatchDetails = async (
     pollingFunction: () => void,
     pollingDisable: boolean
   ) => {
     timer.current = PollingTimer(
@@ -171,162 +163,146 @@
 
     return () => {
       pollingBatchDetails(getBatchDetails, true);
     };
   }, []);
 
   const getBatchDetails = async () => {
-    await BatchService.getBatchDetailsService(
-      setRegionName,
-      setProjectName,
-      batchSelected,
-      setBatchInfoResponse,
-      setLabelDetail,
-      setIsLoading,
-      setErrorView
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      setRegionName(credentials.region_id || '');
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/batches/${batchSelected}`,
+        {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              setBatchInfoResponse(responseResult);
+              if (responseResult.labels) {
+                const labelValue = Object.entries(responseResult.labels).map(
+                  ([key, value]) => `${key}:${value}`
+                );
+                setLabelDetail(labelValue);
+              }
+              setIsLoading(false);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error in getting Batch details', err);
+          toast.error(`Failed to fetch batch details ${batchSelected}`);
+        });
+    }
   };
 
-  const statusMsg = !errorView ? statusMessageBatch(batchInfoResponse) : '';
-  const startTime = !errorView
-    ? jobTimeFormat(batchInfoResponse.createTime)
-    : '';
-  const startTimeElapsed = !errorView
-    ? new Date(batchInfoResponse.createTime)
-    : new Date();
-
-  const endTime = !errorView
-    ? new Date(batchInfoResponse.stateTime)
-    : new Date();
+  const statusMsg = statusMessageBatch(batchInfoResponse);
+  const startTime = jobTimeFormat(batchInfoResponse.createTime);
+  const startTimeElapsed = new Date(batchInfoResponse.createTime);
+
+  const endTime = new Date(batchInfoResponse.stateTime);
 
   let jobStartTime: Date;
   let runTimeString = '';
 
   if (batchInfoResponse.stateHistory) {
     const lastStateHistory =
       batchInfoResponse.stateHistory[batchInfoResponse.stateHistory.length - 1];
     jobStartTime = new Date(lastStateHistory.stateStartTime);
     runTimeString = elapsedTime(endTime, jobStartTime);
   }
 
-  const batch = !errorView ? BatchTypeValue(batchInfoResponse) : '';
-  const batchConcat = !errorView
-    ? Object.keys(batchInfoResponse).filter(key => key.endsWith('Batch'))
-    : '';
+  const batch = BatchTypeValue(batchInfoResponse);
+  const batchConcat = Object.keys(batchInfoResponse).filter(key =>
+    key.endsWith('Batch')
+  );
   const elapsedTimeString = elapsedTime(
     new Date(batchInfoResponse.stateTime),
     startTimeElapsed
   );
 
   const handleDeleteBatch = (batchSelected: string) => {
     setSelectedBatch(batchSelected);
     setDeletePopupOpen(true);
   };
   const handleCancelDelete = () => {
     setDeletePopupOpen(false);
   };
 
   const handleDelete = async () => {
-    await BatchService.deleteBatchAPIService(selectedBatch);
+    await deleteBatchAPI(selectedBatch);
     handleDetailedBatchView();
     setDeletePopupOpen(false);
   };
-  const handleCloneBatch = async (batchInfoResponse: IBatchInfoResponse) => {
-    setCreateBatch(true);
-  };
 
   return (
     <div>
-      {batchInfoResponse.uuid === '' && isLoading && (
-        <div className="spin-loader-main">
-          <CircularProgress
-            className = "spin-loader-custom-style"
-            size={15}
-            aria-label="Loading Spinner"
-            data-testid="loader"
-          />
-          Loading Batch Details
+      <ToastContainer />
+      {batchInfoResponse.uuid === '' && (
+        <div className="loader-full-style">
+          {isLoading && (
+            <div>
+              <ClipLoader
+                color="#8A8A8A"
+                loading={true}
+                size={20}
+                aria-label="Loading Spinner"
+                data-testid="loader"
+              />
+              Loading Batch Details
+            </div>
+          )}
         </div>
       )}
-      {createBatch && (
-        <CreateBatch
-          setCreateBatch={setCreateBatch}
-          regionName={regionName}
-          projectName={projectName}
-          batchInfoResponse={batchInfoResponse}
-          createBatch={createBatch}
-        />
-      )}
       {deletePopupOpen && (
         <DeletePopup
           onCancel={() => handleCancelDelete()}
           onDelete={() => handleDelete()}
           deletePopupOpen={deletePopupOpen}
           DeleteMsg={
             'This will delete ' + selectedBatch + ' and cannot be undone.'
           }
         />
       )}
-      {errorView && (
-        <div className="error-view-parent">
-          <div
-            role="button"
-            aria-label="back-arrow-icon"
-            className="back-arrow-icon"
-            onClick={() => handleDetailedBatchView()}
-          >
-            <iconLeftArrow.react tag="div" className="logo-alignment-style" />
-          </div>
-          <div className="error-view-message-parent">
-            <iconError.react tag="div" className="logo-alignment-style" />
-            <div role="alert" className="error-view-message">
-              Unable to find the resource you requested
-            </div>
-          </div>
-        </div>
-      )}
-
-      {!errorView && !createBatch && batchInfoResponse.uuid !== '' && (
-        <div className="scroll">
-          <div className="scroll-fix-header cluster-details-header">
+      {batchInfoResponse.uuid !== '' && (
+        <div className="scroll-comp">
+          <div className="cluster-details-header">
             <div
               role="button"
               className="back-arrow-icon"
               onClick={() => handleDetailedBatchView()}
             >
-              <iconLeftArrow.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
+              <iconLeftArrow.react tag="div" />
             </div>
             <div className="cluster-details-title">{batchSelected}</div>
-            <div
-              role="button"
-              className="action-cluster-section"
-              onClick={() => handleCloneBatch(batchInfoResponse)}
-            >
+            <div className="action-disabled action-cluster-section">
               <div className="action-cluster-icon">
-                <iconCloneJob.react
-                  tag="div"
-                  className="logo-alignment-style"
-                />
+                <iconCloneJob.react tag="div" />
               </div>
               <div className="action-cluster-text">CLONE</div>
             </div>
 
             <div
               role="button"
               className="action-cluster-section"
               onClick={() => handleDeleteBatch(batchSelected)}
             >
               <div className="action-cluster-icon">
-                <iconDeleteCluster.react
-                  tag="div"
-                  className="logo-alignment-style"
-                />
+                <iconDeleteCluster.react tag="div" />
               </div>
               <div className="action-cluster-text">DELETE</div>
             </div>
             <ViewLogs batchInfoResponse={batchInfoResponse} />
           </div>
 
           <div className="batch-details-container-top">
@@ -459,22 +435,14 @@
                           ))}
                       </>
                     )
                   );
                 }
               )
             }
-            {batchInfoResponse.runtimeConfig.containerImage && (
-              <div className="row-details">
-                <div className="details-label">Image</div>
-                <div className="details-value">
-                  {batchInfoResponse.runtimeConfig.containerImage}
-                </div>
-              </div>
-            )}
 
             <div className="row-details">
               <div className="details-label">Properties</div>
               <div className="details-value"></div>
             </div>
             {Object.entries(batchInfoResponse.runtimeConfig.properties).map(
               ([key, value]) => (
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/batches/batches.tsx` & `dataproc_jupyter_plugin-0.1.9/src/login/authLogin.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -11,105 +11,112 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
+import { ReactWidget } from '@jupyterlab/apputils';
 import React, { useEffect, useState } from 'react';
-import ListBatches from './listBatches';
-import ListSessions from '../sessions/listSessions';
-import { DataprocWidget } from '../controls/DataprocWidget';
-import { LOGIN_ERROR_MESSAGE, LOGIN_STATE } from '../utils/const';
+import { LabIcon } from '@jupyterlab/ui-components';
+import signinGoogleIcon from '../../style/icons/signin_google_icon.svg';
+import { requestAPI } from '../handler/handler';
+import ConfigSelection from './configSelection';
+import { LOGIN_STATE, STATUS_SUCCESS } from '../utils/const';
 import { checkConfig } from '../utils/utils';
-import { CircularProgress } from '@mui/material';
+import { ClipLoader } from 'react-spinners';
 
-const BatchesComponent = (): React.JSX.Element => {
-  const [selectedMode, setSelectedMode] = useState('Batches');
-
-  const [loggedIn, setLoggedIn] = useState(false);
+// Create the LabIcon instance outside of the component
+const IconsigninGoogle = new LabIcon({
+  name: 'launcher:signin_google_icon',
+  svgstr: signinGoogleIcon
+});
+
+const AuthLoginComponent = (): React.JSX.Element => {
+  const [loginState, setLoginState] = useState(false);
+  const [isloginDisabled, setIsloginDisabled] = useState(false);
   const [configError, setConfigError] = useState(false);
   const [loginError, setLoginError] = useState(false);
   const [configLoading, setConfigLoading] = useState(true);
 
-  const selectedModeChange = (mode: 'Sessions' | 'Batches') => {
-    setSelectedMode(mode);
-  };
-
-  const toggleStyleSelection = (toggleItem: string) => {
-    if (selectedMode === toggleItem) {
-      return 'selected-header';
-    } else {
-      return 'unselected-header';
+  const login = async () => {
+    setIsloginDisabled(true);
+    const data = await requestAPI('login');
+    if (typeof data === 'object' && data !== null) {
+      const loginStatus = (data as { login: string }).login;
+      if (loginStatus === STATUS_SUCCESS) {
+        setLoginState(true);
+        setLoginError(false);
+        localStorage.setItem('loginState', LOGIN_STATE);
+      } else {
+        setLoginState(false);
+        localStorage.removeItem('loginState');
+      }
     }
   };
 
   useEffect(() => {
-    checkConfig(setLoggedIn, setConfigError, setLoginError);
+    checkConfig(setLoginState, setConfigError, setLoginError);
     const localstorageGetInformation = localStorage.getItem('loginState');
-    setLoggedIn(localstorageGetInformation === LOGIN_STATE);
-    if (loggedIn) {
+    setLoginState(localstorageGetInformation === LOGIN_STATE);
+    if (loginState) {
       setConfigLoading(false);
     }
   }, []);
 
   return (
-    <div className="component-level">
-      {configLoading && !loggedIn && !configError && !loginError && (
-        <div className="spin-loader-main">
-          <CircularProgress
-            className = "spin-loader-custom-style"
+    <div>
+      {configLoading && !loginState && !configError && !loginError && (
+        <div className="spin-loaderMain">
+          <ClipLoader
+            color="#8A8A8A"
+            loading={true}
             size={18}
             aria-label="Loading Spinner"
             data-testid="loader"
           />
-          Loading Batches
+          Loading Config Setup
         </div>
       )}
+      {!loginError && loginState && (
+        <ConfigSelection
+          loginState={loginState}
+          configError={configError}
+          setConfigError={setConfigError}
+        />
+      )}
       {loginError && (
-        <div role="alert" className="login-error">
-          {LOGIN_ERROR_MESSAGE}
-        </div>
+        <>
+          <div className="login-error">Please login to continue</div>
+          <div style={{ alignItems: 'center' }}>
+            <div
+              role="button"
+              className={
+                isloginDisabled
+                  ? 'signin-google-icon disabled'
+                  : 'signin-google-icon'
+              }
+              onClick={isloginDisabled ? undefined : login}
+            >
+              <IconsigninGoogle.react tag="div" />
+            </div>
+          </div>
+        </>
       )}
       {configError && (
-        <div role="alert" className="login-error">
+        <div className="login-error">
           Please configure gcloud with account, project-id and region
         </div>
       )}
-      {loggedIn && !configError && !loginError && (
-        <div className="clusters-list-component" role="tablist">
-          {
-            <div className="clusters-list-overlay" role="tab">
-              <div
-                role="tabpanel"
-                className={toggleStyleSelection('Batches')}
-                onClick={() => selectedModeChange('Batches')}
-              >
-                Batches
-              </div>
-              <div
-                role="tabpanel"
-                className={toggleStyleSelection('Sessions')}
-                onClick={() => selectedModeChange('Sessions')}
-              >
-                Sessions
-              </div>
-            </div>
-          }
-          <div>
-            {selectedMode === 'Sessions' ? (
-              <ListSessions />
-            ) : (
-              <ListBatches setLoggedIn={setLoggedIn} />
-            )}
-          </div>
-        </div>
-      )}
     </div>
   );
 };
 
-export class Batches extends DataprocWidget {
-  renderInternal(): React.JSX.Element {
-    return <BatchesComponent />;
+export class AuthLogin extends ReactWidget {
+  constructor() {
+    super();
+  }
+
+  render(): React.JSX.Element {
+    return <AuthLoginComponent />;
   }
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/batches/createBatch.tsx` & `dataproc_jupyter_plugin-0.1.9/src/batches/createBatch.tsx`

 * *Files 19% similar despite different names*

```diff
@@ -14,335 +14,221 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 import React, { ChangeEvent, useEffect, useState } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
 import LeftArrowIcon from '../../style/icons/left_arrow_icon.svg';
+import 'semantic-ui-css/semantic.min.css';
 import 'react-toastify/dist/ReactToastify.css';
+import { Input, Radio, Select, Dropdown } from 'semantic-ui-react';
 import {
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
   ARCHIVE_FILES_MESSAGE,
   ARGUMENTS_MESSAGE,
   ARTIFACT_REGISTERY,
+  BASE_URL,
+  BASE_URL_KEY,
+  BASE_URL_META,
+  BASE_URL_NETWORKS,
   CONTAINER_REGISTERY,
   CUSTOM_CONTAINERS,
   CUSTOM_CONTAINER_MESSAGE,
-  CUSTOM_CONTAINER_MESSAGE_PART,
   FILES_MESSAGE,
   JAR_FILE_MESSAGE,
   KEY_MESSAGE,
   METASTORE_MESSAGE,
-  NETWORK_TAG_MESSAGE,
+  PROJECT_LIST_URL,
   QUERY_FILE_MESSAGE,
+  REGION_URL,
   SECURITY_KEY,
   SELF_MANAGED_CLUSTER,
   SERVICE_ACCOUNT,
-  SHARED_VPC
+  STATUS_RUNNING
 } from '../utils/const';
+import TagsInput from 'react-tagsinput';
+import 'react-tagsinput/react-tagsinput.css';
 import LabelProperties from '../jobs/labelProperties';
 import { authApi } from '../utils/utils';
+import { ClipLoader } from 'react-spinners';
+import { toast } from 'react-toastify';
 import ErrorPopup from '../utils/errorPopup';
 import errorIcon from '../../style/icons/error_icon.svg';
-import { Input } from '../controls/MuiWrappedInput';
-import {
-  Autocomplete,
-  CircularProgress,
-  Radio,
-  TextField
-} from '@mui/material';
-import { DropdownProps } from 'semantic-ui-react';
-import { DynamicDropdown } from '../controls/DynamicDropdown';
-import { projectListAPI } from '../utils/projectService';
-import { BatchService } from './batchService';
-import { MuiChipsInput } from 'mui-chips-input';
+
+type Project = {
+  projectId: string;
+};
+
+type Cluster = {
+  clusterName: string;
+  status: {
+    state: string;
+  };
+};
+
+type Network = {
+  selfLink: any;
+  network: string;
+  subnetworks: string;
+};
+
+type Service = {
+  name: string;
+};
 
 const iconLeftArrow = new LabIcon({
   name: 'launcher:left-arrow-icon',
   svgstr: LeftArrowIcon
 });
 
 const iconError = new LabIcon({
   name: 'launcher:error-icon',
   svgstr: errorIcon
 });
 
 interface ICreateBatchProps {
-  setCreateBatchView?: (value: boolean) => void;
+  setCreateBatchView: (value: boolean) => void;
   regionName: string;
   projectName: string;
-  batchInfoResponse?: any;
-  createBatch?: boolean;
-  setCreateBatch?: (value: boolean) => void;
-}
-
-function batchTypeFunction(batchKey: string) {
-  let batchType = 'Spark';
-  switch (batchKey) {
-    case 'sparkRBatch':
-      batchType = 'SparkR';
-      return batchType;
-    case 'pysparkBatch':
-      batchType = 'PySpark';
-      return batchType;
-    case 'sparkSqlBatch':
-      batchType = 'SparkSql';
-      return batchType;
-    default:
-      return batchType;
-  }
 }
+let jarFileUris: string[] = [];
+let fileUris: string[] = [];
+let archiveFileUris: string[] = [];
+let argumentsUris: string[] = [];
+let networkUris: string[] = [];
+let key: string[] | (() => string[]) = [];
+let value: string[] | (() => string[]) = [];
+let pythonFileUris: string[] = [];
 
 function CreateBatch({
   setCreateBatchView,
   regionName,
-  projectName,
-  batchInfoResponse,
-  setCreateBatch,
-  createBatch
+  projectName
 }: ICreateBatchProps) {
-  let batchKeys: string[] = [];
-  let batchType = 'Spark';
-  let mainClass = '';
-  let mainJarFileUri = '';
-  let mainRFileUri = '';
-  let mainPythonFileUri = '';
-  let queryFileUri = '';
-  let serviceAccount = '';
-  let subNetwork = '';
-  let network = '';
-  let historyServer = '';
-  let historyServerValue = '';
-  let metastoreService = '';
-  let metaProject = '';
-  let containerImage = '';
-  let jarFileUris: string[] = [];
-  let fileUris: string[] = [];
-  let archiveFileUris: string[] = [];
-  let argumentsUris: string[] = [];
-  let networkUris: string[] | '' = [];
-  let key: string[] | (() => string[]) = [];
-  let value: string[] | (() => string[]) = [];
-  let pythonFileUris: string[] = [];
-  let keyType = '';
-  let keyRing = '';
-  let keys = '';
-  if (batchInfoResponse !== undefined) {
-    if (Object.keys(batchInfoResponse).length !== 0) {
-      for (const key in batchInfoResponse) {
-        if (batchInfoResponse.hasOwnProperty(key) && key.endsWith('Batch')) {
-          batchKeys.push(key);
-        }
-      }
-      batchType = batchTypeFunction(batchKeys[0]);
-      const batchTypeKey = batchKeys[0];
-      if (batchInfoResponse[batchKeys[0]].hasOwnProperty('queryFileUri')) {
-        queryFileUri = batchInfoResponse[batchKeys[0]].queryFileUri;
-      }
-      mainJarFileUri = batchInfoResponse[batchKeys[0]].mainJarFileUri;
-      mainClass = batchInfoResponse[batchKeys[0]].mainClass;
-      mainRFileUri = batchInfoResponse[batchKeys[0]].mainRFileUri;
-      mainPythonFileUri = batchInfoResponse[batchKeys[0]].mainPythonFileUri;
-      if (batchInfoResponse[batchTypeKey].hasOwnProperty('jarFileUris')) {
-        jarFileUris = batchInfoResponse[batchKeys[0]].jarFileUris;
-      }
-      if (batchInfoResponse[batchTypeKey].hasOwnProperty('fileUris')) {
-        fileUris = batchInfoResponse[batchKeys[0]].fileUris;
-      }
-      if (batchInfoResponse[batchTypeKey].hasOwnProperty('archiveUris')) {
-        archiveFileUris = batchInfoResponse[batchKeys[0]].archiveUris;
-      }
-      if (batchInfoResponse[batchTypeKey].hasOwnProperty('args')) {
-        argumentsUris = batchInfoResponse[batchKeys[0]].args;
-      }
-      if (batchInfoResponse[batchTypeKey].hasOwnProperty('pythonFileUris')) {
-        pythonFileUris = batchInfoResponse[batchKeys[0]].pythonFileUris;
-      }
-      serviceAccount =
-        batchInfoResponse?.environmentConfig?.executionConfig?.serviceAccount ||
-        '';
-      networkUris =
-        batchInfoResponse?.environmentConfig?.executionConfig?.networkTags ||
-        '';
-      subNetwork =
-        batchInfoResponse?.environmentConfig?.executionConfig?.subnetworkUri ||
-        '';
-
-      keyType =
-        batchInfoResponse?.environmentConfig?.executionConfig?.kmsKey || '';
-      const keyringValues = keyType.split('/'); // splitting keyrings and key form projects/projectName/locations/regionName/keyRings/keyRing/cryptoKeys/key
-      keyRing = keyringValues[5] ? keyringValues[5] : '';
-      keys = keyringValues[7] ? keyringValues[7] : '';
-      historyServerValue =
-        batchInfoResponse?.environmentConfig?.peripheralsConfig
-          ?.sparkHistoryServerConfig?.dataprocCluster || '';
-      if (historyServerValue !== '') {
-        const parts = historyServerValue.split('/'); //splitting to take cluster name from project/projectName/region/regionName/cluster/clusterName
-        historyServer = parts[parts.length - 1];
-      }
-      metastoreService =
-        batchInfoResponse?.environmentConfig?.peripheralsConfig
-          ?.metastoreService || 'None';
-      containerImage = batchInfoResponse?.runtimeConfig?.containerImage || '';
-      if (metastoreService != 'None') {
-        const metastoreDetails = metastoreService.split('/');
-        metaProject = metastoreDetails[1];
-      }
-    }
-  }
-
-  const selectedRadioInitialValue = mainJarFileUri ? 'mainJarURI' : 'mainClass';
-  const selectedKeyType = keyType ? 'customerManaged' : 'googleManaged';
   const [batchTypeList, setBatchTypeList] = useState([{}]);
   const [generationCompleted, setGenerationCompleted] = useState(false);
   const [hexNumber, setHexNumber] = useState('');
   const [batchIdSelected, setBatchIdSelected] = useState('');
-  const [batchTypeSelected, setBatchTypeSelected] = useState(batchType);
+  const [batchTypeSelected, setBatchTypeSelected] = useState('spark');
   const [versionSelected, setVersionSelected] = useState('2.1');
-  const [selectedRadio, setSelectedRadio] = useState(selectedRadioInitialValue);
-  const [mainClassSelected, setMainClassSelected] = useState(mainClass);
-  const [mainClassUpdated, setMainClassUpdated] = useState(false);
-  const [mainJarSelected, setMainJarSelected] = useState(mainJarFileUri);
-  const [mainJarUpdated, setMainJarUpdated] = useState(false);
-
-  const [mainRSelected, setMainRSelected] = useState(mainRFileUri);
+  const [selectedRadio, setSelectedRadio] = useState('mainClass');
   const [selectedRadioValue, setSelectedRadioValue] = useState('key');
-  const [containerImageSelected, setContainerImageSelected] =
-    useState(containerImage);
+  const [mainClassSelected, setMainClassSelected] = useState('');
+  const [mainJarSelected, setMainJarSelected] = useState('');
+  const [mainRSelected, setMainRSelected] = useState('');
+  const [containerImageSelected, setContainerImageSelected] = useState('');
   const [jarFilesSelected, setJarFilesSelected] = useState([...jarFileUris]);
   const [filesSelected, setFilesSelected] = useState([...fileUris]);
-  const [queryFileSelected, setQueryFileSelected] = useState(queryFileUri);
+  const [queryFileSelected, setQueryFileSelected] = useState('');
   const [ArchiveFilesSelected, setArchiveFileSelected] = useState([
     ...archiveFileUris
   ]);
   const [argumentsSelected, setArgumentsSelected] = useState([
     ...argumentsUris
   ]);
-  const [serviceAccountSelected, setServiceAccountSelected] =
-    useState(serviceAccount);
+  const [serviceAccountSelected, setServiceAccountSelected] = useState('');
   const [networkTagSelected, setNetworkTagSelected] = useState([
     ...networkUris
   ]);
   const [propertyDetail, setPropertyDetail] = useState(['']);
   const [selectedEncryptionRadio, setSelectedEncryptionRadio] =
-    useState(selectedKeyType);
+    useState('googleManaged');
   const [propertyDetailUpdated, setPropertyDetailUpdated] = useState(['']);
   const [keyValidation, setKeyValidation] = useState(-1);
   const [valueValidation, setValueValidation] = useState(-1);
   const [duplicateKeyError, setDuplicateKeyError] = useState(-1);
   const [labelDetail, setLabelDetail] = useState(key);
   const [labelDetailUpdated, setLabelDetailUpdated] = useState(value);
-  const [servicesList, setServicesList] = useState<string[]>([]);
-  const [servicesSelected, setServicesSelected] = useState(metastoreService);
-
-  const [clusterSelected, setClusterSelected] = useState(historyServer);
-  const [projectId, setProjectId] = useState(metaProject);
+  const [servicesList, setServicesList] = useState<
+    Array<{ key: string; value: string; text: string }>
+  >([]);
+  const [servicesSelected, setServicesSelected] = useState('None');
+
+  const [clusterSelected, setClusterSelected] = useState('');
+  const [projectId, setProjectId] = useState('');
+  const [region, setRegion] = useState('');
+  const [projectList, setProjectList] = useState([{}]);
+  const [regionList, setRegionList] = useState<
+    { value: string; key: string; text: string }[]
+  >([]);
   const [networkList, setNetworklist] = useState([{}]);
-  const [keyRinglist, setKeyRinglist] = useState<string[]>([]);
-  const [subNetworkList, setSubNetworklist] = useState<string[]>([]);
-  const [networkSelected, setNetworkSelected] = useState(network);
-  const [subNetworkSelected, setSubNetworkSelected] = useState(subNetwork);
+  const [keyRinglist, setKeyRinglist] = useState([{}]);
+  const [subNetworkList, setSubNetworklist] = useState<
+    { key: string; value: string; text: string }[]
+  >([]);
+  const [isLoadingRegion, setIsLoadingRegion] = useState(false);
+  const [networkSelected, setNetworkSelected] = useState('default');
+  const [subNetworkSelected, setSubNetworkSelected] = useState('default');
   const [isLoadingService, setIsLoadingService] = useState(false);
   const [error, setError] = useState({ isOpen: false, message: '' });
   const [parameterDetail, setParameterDetail] = useState(['']);
   const [parameterDetailUpdated, setParameterDetailUpdated] = useState(['']);
   const [additionalPythonFileSelected, setAdditionalPythonFileSelected] =
     useState([...pythonFileUris]);
-  const [mainPythonSelected, setMainPythonSelected] =
-    useState(mainPythonFileUri);
-  const [clustersList, setClustersList] = useState<string[]>([]);
+  const [mainPythonSelected, setMainPythonSelected] = useState('');
+  const [clustersList, setClustersList] = useState<
+    Array<{ key: string; value: string; text: string }>
+  >([]);
   const [additionalPythonFileValidation, setAdditionalPythonFileValidation] =
     useState(true);
   const [jarFileValidation, setJarFileValidation] = useState(true);
   const [fileValidation, setFileValidation] = useState(true);
   const [archieveFileValidation, setArchieveFileValidation] = useState(true);
   const [mainPythonValidation, setMainPythonValidation] = useState(true);
   const [queryFileValidation, setQueryFileValidation] = useState(true);
   const [mainRValidation, setMainRValidation] = useState(true);
   const [batchIdValidation, setBatchIdValidation] = useState(false);
   const [mainJarValidation, setMainJarValidation] = useState(true);
-  const [keyRingSelected, setKeyRingSelected] = useState(keyRing);
-  const [keySelected, setKeySelected] = useState(keys);
+  const [defaultValue, setDefaultValue] = useState('default');
+  const [keyRingSelected, setKeyRingSelected] = useState('');
+  const [keySelected, setKeySelected] = useState('');
   const [manualKeySelected, setManualKeySelected] = useState('');
   const [manualValidation, setManualValidation] = useState(true);
-  const [
-    additionalPythonFileDuplicateValidation,
-    setAdditionalPythonFileDuplicateValidation
-  ] = useState(false);
-  const [jarFileDuplicateValidation, setJarFileDuplicateValidation] =
-    useState(false);
-  const [fileDuplicateValidation, setFileDuplicateValidation] = useState(false);
-  const [archiveDuplicateValidation, setArchiveDuplicateValidation] =
-    useState(false);
-  const [argumentsDuplicateValidation, setArgumentsDuplicateValidation] =
-    useState(false);
-  const [networkTagsDuplicateValidation, setNetworkTagsDuplicateValidation] =
-    useState(false);
-  const [keylist, setKeylist] = useState<string[]>([]);
-  const [isloadingNetwork, setIsloadingNetwork] = useState(false);
-  const [selectedNetworkRadio, setSelectedNetworkRadio] = useState<
-    'sharedVpc' | 'projectNetwork'
-  >('projectNetwork');
-  const [sharedSubNetworkList, setSharedSubNetworkList] = useState<string[]>(
-    []
-  );
-  const [sharedvpcSelected, setSharedvpcSelected] = useState('');
-  const [projectInfo, setProjectInfo] = useState('');
+  const [keylist, setKeylist] = useState<
+    { key: string; value: string; text: string }[]
+  >([]);
+
   const handleCreateBatchBackView = () => {
-    if (setCreateBatchView) {
-      setCreateBatchView(false);
-    }
-    if (setCreateBatch) {
-      setCreateBatch(false);
-    }
+    setCreateBatchView(false);
+  };
+  const handleMainClassRadio = () => {
+    setSelectedRadio('mainClass');
+    setMainJarSelected('');
+    setMainClassSelected('');
   };
 
+  const handleMainJarRadio = () => {
+    setSelectedRadio('mainJarURI');
+    setMainClassSelected('');
+    setMainJarSelected('');
+  };
   const handlekeyRingRadio = () => {
     setSelectedRadioValue('key');
     setManualKeySelected('');
-    setManualValidation(true);
-  };
-
-  const handleGoogleManagedRadio = () => {
-    setSelectedEncryptionRadio('googleManaged');
-    setKeyRingSelected('');
-    setKeySelected('');
-    setManualKeySelected('');
   };
   const handlekeyManuallyRadio = () => {
     setSelectedRadioValue('manually');
     setKeyRingSelected('');
     setKeySelected('');
   };
   useEffect(() => {
-    if (keyRingSelected !== '') {
-      listKeysAPI(keyRingSelected);
-    }
-  }, [keyRingSelected]);
+    const batchTypeData = [
+      { key: 'spark', value: 'spark', text: 'Spark' },
+      { key: 'sparkR', value: 'sparkR', text: 'SparkR' },
+      { key: 'sparkSql', value: 'sparkSql', text: 'SparkSql' },
+      { key: 'pySpark', value: 'pySpark', text: 'PySpark' }
+    ];
 
-  useEffect(() => {
-    if (
-      batchInfoResponse === undefined ||
-      batchInfoResponse?.environmentConfig?.executionConfig?.subnetworkUri
-    ) {
-      if (networkSelected !== '') {
-        listSubNetworksAPI(networkSelected);
-      }
-    } else {
-      listSubNetworksAPI(networkSelected);
-    }
-  }, [networkSelected]);
-  useEffect(() => {
-    const batchTypeData = ['Spark', 'SparkR', 'SparkSql', 'PySpark'];
     setBatchTypeList(batchTypeData);
-
+    projectListAPI();
     listClustersAPI();
     listNetworksAPI();
     listKeyRingsAPI();
-    runtimeSharedProject();
-  }, [clusterSelected]);
+  }, [clusterSelected, defaultValue]);
 
   useEffect(() => {
     generateRandomHex();
   }, [
     batchIdSelected,
     mainClassSelected,
     mainRSelected,
@@ -355,220 +241,71 @@
     fileValidation,
     mainPythonValidation,
     queryFileValidation,
     keyValidation,
     valueValidation,
     batchIdValidation,
     duplicateKeyError,
-    manualValidation,
-    mainJarSelected,
-    jarFilesSelected,
-    keyRingSelected,
-    keySelected,
-    manualKeySelected
+    manualValidation
   ]);
-  useEffect(() => {
-    let batchKeys: string[] = [];
-
-    if (batchInfoResponse) {
-      const { environmentConfig } = batchInfoResponse;
-      if (environmentConfig) {
-        const executionConfig = environmentConfig.executionConfig;
-
-        if (executionConfig) {
-          const sharedVpcMatches =
-            /projects\/(?<project>[\w\-]+)\/regions\/(?<region>[\w\-]+)\/subnetworks\/(?<subnetwork>[\w\-]+)/.exec(
-              executionConfig.subnetworkUri
-            );
-          // Is this a shared VPC?
-          if (sharedVpcMatches?.groups?.['subnetwork']) {
-            setSharedvpcSelected(sharedVpcMatches?.groups?.['subnetwork']);
-            setSelectedNetworkRadio('sharedVpc');
-          } else {
-            setSubNetworkSelected(executionConfig.subnetworkUri);
-            setSelectedNetworkRadio('projectNetwork');
-          }
-        }
-      }
-
-      if (Object.keys(batchInfoResponse).length !== 0) {
-        if (batchInfoResponse.hasOwnProperty('labels')) {
-          const updatedLabelDetail = Object.entries(
-            batchInfoResponse.labels
-          ).map(([k, v]) => `${k}:${v}`);
-          setLabelDetail(prevLabelDetail => [
-            ...prevLabelDetail,
-            ...updatedLabelDetail
-          ]);
-          setLabelDetailUpdated(prevLabelDetailUpdated => [
-            ...prevLabelDetailUpdated,
-            ...updatedLabelDetail
-          ]);
-          for (const key in batchInfoResponse) {
-            if (key.endsWith('Batch')) {
-              batchKeys.push(key);
-            }
-          }
-          for (const key in batchInfoResponse) {
-            if (
-              batchInfoResponse.hasOwnProperty(key) &&
-              key.endsWith('Batch')
-            ) {
-              batchKeys.push(key);
-            }
-          }
-
-          if (batchInfoResponse.runtimeConfig.hasOwnProperty('properties')) {
-            const updatedPropertyDetail = Object.entries(
-              batchInfoResponse.runtimeConfig.properties
-            ).map(([k, v]) => `${k.substring(6)}:${v}`); // spark:spark.app.name , spark:spark.driver.cores - every property is appended with 'spark:' therefore getting the porperty key value after 'spark:'
-            setPropertyDetail(prevPropertyDetail => [
-              ...prevPropertyDetail,
-              ...updatedPropertyDetail
-            ]);
-            setPropertyDetailUpdated(prevPropertyDetailUpdated => [
-              ...prevPropertyDetailUpdated,
-              ...updatedPropertyDetail
-            ]);
-          }
-          if (
-            batchInfoResponse[batchKeys[0]].hasOwnProperty('queryVariables')
-          ) {
-            const updatedParamDetail = Object.entries(
-              batchInfoResponse[batchKeys[0]].queryVariables
-            ).map(([k, v]) => `${k}:${v}`);
-            setPropertyDetail(prevParameterDetail => [
-              ...prevParameterDetail,
-              ...updatedParamDetail
-            ]);
-            setPropertyDetailUpdated(prevParameterDetailUpdated => [
-              ...prevParameterDetailUpdated,
-              ...updatedParamDetail
-            ]);
-          }
-        }
-      }
-      listNetworksFromSubNetworkAPI(subNetwork);
-    }
-  }, []);
-
-  const runtimeSharedProject = async () => {
-    await BatchService.runtimeSharedProjectService(
-      setProjectInfo,
-      setSharedSubNetworkList
-    );
-  };
-
-  const handleMainClassRadio = () => {
-    setSelectedRadio('mainClass');
-    setMainJarSelected('');
-    setMainClassSelected('');
-    setMainJarValidation(true);
-  };
-
-  const handleMainJarRadio = () => {
-    setSelectedRadio('mainJarURI');
-    setMainClassSelected('');
-    setMainJarSelected('');
-    setMainJarValidation(true);
-  };
-
-  const listNetworksFromSubNetworkAPI = async (subNetwork: string) => {
-    await BatchService.listNetworksFromSubNetworkAPIService(
-      subNetwork,
-      setIsloadingNetwork,
-      setNetworkSelected
-    );
-  };
 
   function isSubmitDisabled() {
     const commonConditions =
       batchIdSelected === '' ||
       regionName === '' ||
-      batchIdValidation ||
-      (selectedNetworkRadio === 'sharedVpc' &&
-        sharedSubNetworkList.length === 0) ||
-      (selectedNetworkRadio === 'sharedVpc' && sharedvpcSelected === '') ||
-      (selectedEncryptionRadio === 'customerManaged' &&
-        selectedRadioValue === 'key' &&
-        keyRingSelected === '' &&
-        keySelected === '') ||
-      (selectedEncryptionRadio === 'customerManaged' &&
-        selectedRadioValue === 'manually' &&
-        manualKeySelected === '') ||
-      (selectedNetworkRadio === 'projectNetwork' &&
-        networkList.length !== 0 &&
-        subNetworkList.length === 0);
+      batchIdValidation
+      ;
+
     switch (batchTypeSelected) {
-      case 'Spark':
+      case 'spark':
         return (
           commonConditions ||
           (selectedRadio === 'mainClass' && mainClassSelected === '') ||
           (selectedRadio === 'mainJarURI' && mainJarSelected === '') ||
           !mainJarValidation ||
           !fileValidation ||
           !archieveFileValidation ||
-          !manualValidation ||
-          !jarFileValidation ||
-          fileDuplicateValidation ||
-          archiveDuplicateValidation ||
-          argumentsDuplicateValidation ||
-          networkTagsDuplicateValidation ||
-          jarFileDuplicateValidation
+          !manualValidation
         );
-      case 'SparkR':
+      case 'sparkR':
         return (
           commonConditions ||
           mainRSelected === '' ||
           !mainRValidation ||
           !fileValidation ||
           !archieveFileValidation ||
-          !manualValidation ||
-          fileDuplicateValidation ||
-          archiveDuplicateValidation ||
-          argumentsDuplicateValidation ||
-          networkTagsDuplicateValidation
+          !manualValidation
         );
-      case 'PySpark':
+      case 'pySpark':
         return (
           commonConditions ||
           mainPythonSelected === '' ||
           !mainPythonValidation ||
           !additionalPythonFileValidation ||
           !fileValidation ||
           !archieveFileValidation ||
-          !manualValidation ||
-          !jarFileValidation ||
-          additionalPythonFileDuplicateValidation ||
-          fileDuplicateValidation ||
-          archiveDuplicateValidation ||
-          argumentsDuplicateValidation ||
-          networkTagsDuplicateValidation ||
-          jarFileDuplicateValidation
+          !manualValidation
         );
-      case 'SparkSql':
+      case 'sparkSql':
         return (
           commonConditions ||
           queryFileSelected === '' ||
           !queryFileValidation ||
           !jarFileValidation ||
-          !manualValidation ||
-          networkTagsDuplicateValidation ||
-          jarFileDuplicateValidation
+          !manualValidation
         );
       default:
         return false;
     }
   }
 
   const handleValidationFiles = (
-    listOfFiles: string | string[],
+    listOfFiles: any,
     setValuesPart: any,
-    setValidationPart: (value: boolean) => void,
-    setDuplicateValidation?: (value: boolean) => void
+    setValidationPart: any
   ) => {
     if (typeof listOfFiles === 'string') {
       if (
         listOfFiles.startsWith('file://') ||
         listOfFiles.startsWith('gs://') ||
         listOfFiles.startsWith('hdfs://')
       ) {
@@ -577,118 +314,398 @@
         setValidationPart(false);
       }
       setValuesPart(listOfFiles);
     } else {
       if (listOfFiles.length === 0) {
         setValidationPart(true);
       } else {
-        listOfFiles.forEach((fileName: string) => {
+        listOfFiles.forEach((fileName: any) => {
           if (
             fileName.startsWith('file://') ||
             fileName.startsWith('gs://') ||
             fileName.startsWith('hdfs://')
           ) {
             setValidationPart(true);
           } else {
             setValidationPart(false);
           }
         });
       }
-      handleDuplicateValidation(setDuplicateValidation, listOfFiles);
       setValuesPart(listOfFiles);
     }
   };
-  const handleDuplicateValidation = (
-    setDuplicateValidation: ((value: boolean) => void) | undefined,
-    listOfFiles: string | string[]
-  ) => {
-    if (Array.isArray(listOfFiles)) {
-      const fileNames = listOfFiles.map((fileName: string) =>
-        fileName.toLowerCase()
-      );
-      const uniqueFileNames = new Set<string>();
-      const duplicateFileNames = fileNames.filter((fileName: string) => {
-        const isDuplicate = uniqueFileNames.has(fileName);
-        uniqueFileNames.add(fileName);
-        return isDuplicate;
-      });
-      if (duplicateFileNames.length > 0) {
-        setDuplicateValidation!(true);
-      } else {
-        setDuplicateValidation!(false);
-      }
-    }
-  };
-  const handleArguments = (
-    setDuplicateValidation: (value: boolean) => void,
-    listOfFiles: string[]
-  ) => {
-    setArgumentsSelected(listOfFiles);
-    handleDuplicateValidation(setDuplicateValidation, listOfFiles);
-  };
-  const handleNetworkTags = (
-    setDuplicateValidation: (value: boolean) => void,
-    listOfFiles: string[]
-  ) => {
-    setNetworkTagSelected(listOfFiles);
-    handleDuplicateValidation(setDuplicateValidation, listOfFiles);
-  };
 
   const listClustersAPI = async () => {
-    await BatchService.listClustersAPIService(setClustersList);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters?pageSize=100`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { clusters: Cluster[] }) => {
+              let transformClusterListData = [];
+
+              transformClusterListData = responseResult.clusters.filter(
+                (data: Cluster) => {
+                  if (data.status.state === STATUS_RUNNING) {
+                    return {
+                      clusterName: data.clusterName
+                    };
+                  }
+                }
+              );
+
+              const keyLabelStructure = transformClusterListData.map(obj => ({
+                key: obj.clusterName,
+                value: obj.clusterName,
+                text: obj.clusterName
+              }));
+              setClustersList(keyLabelStructure);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing clusters', err);
+        });
+    }
   };
   const listNetworksAPI = async () => {
-    await BatchService.listNetworksAPIService(
-      setNetworklist,
-      setNetworkSelected,
-      batchInfoResponse,
-      setIsloadingNetwork
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_NETWORKS}/projects/${credentials.project_id}/global/networks`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { items: Network[] }) => {
+              let transformedNetworkList = [];
+              /*
+         Extracting network from items
+         Example: "https://www.googleapis.com/compute/v1/projects/{projectName}/global/networks/",
+      */
+
+              transformedNetworkList = responseResult.items.map(
+                (data: Network) => {
+                  return {
+                    network: data.selfLink.split('/')[9]
+                  };
+                }
+              );
+              const keyLabelStructureNetwork = transformedNetworkList.map(
+                obj => ({
+                  key: obj.network,
+                  value: obj.network,
+                  text: obj.network
+                })
+              );
+              setNetworklist(keyLabelStructureNetwork);
+            })
+
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing Networks', err);
+        });
+    }
   };
-
   const listKeyRingsAPI = async () => {
-    await BatchService.listKeyRingsAPIService(setKeyRinglist);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_KEY}/projects/${credentials.project_id}/locations/${credentials.region_id}/keyRings`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              let transformedKeyList = [];
+              /*
+         Extracting network from items
+         Example: "https://www.googleapis.com/compute/v1/projects/{projectName}/global/networks/",
+      */
+
+              transformedKeyList = responseResult.keyRings.map((data: any) => {
+                return {
+                  name: data.name.split('/')[5]
+                };
+              });
+              const keyLabelStructureKeyRing = transformedKeyList.map(
+                (obj: { name: any }) => ({
+                  key: obj.name,
+                  value: obj.name,
+                  text: obj.name
+                })
+              );
+              setKeyRinglist(keyLabelStructureKeyRing);
+            })
+
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing Networks', err);
+        });
+    }
   };
-
-  const listKeysAPI = async (keyRing: string) => {
-    await BatchService.listKeysAPIService(keyRing, setKeylist, setKeySelected);
+  const listKeysAPI = async (keyRing: any) => {
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_KEY}/projects/${credentials.project_id}/locations/${credentials.region_id}/keyRings/${keyRing}/cryptoKeys`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              let transformedKeyList = [];
+              /*
+         Extracting network from items
+         Example: "https://www.googleapis.com/compute/v1/projects/{projectName}/global/networks/",
+      */
+
+              transformedKeyList = responseResult.cryptoKeys.map(
+                (data: any) => {
+                  return {
+                    name: data.name.split('/')[7]
+                  };
+                }
+              );
+              const keyLabelStructureKeyRing = transformedKeyList.map(
+                (obj: { name: any }) => ({
+                  key: obj.name,
+                  value: obj.name,
+                  text: obj.name
+                })
+              );
+              setKeylist(keyLabelStructureKeyRing);
+              setKeySelected(keyLabelStructureKeyRing[0].value);
+            })
+
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing Networks', err);
+        });
+    }
+  };
+  type SubnetworkData = {
+    subnetworks: string;
   };
-
   const listSubNetworksAPI = async (subnetwork: string) => {
-    await BatchService.listSubNetworksAPIService(
-      subnetwork,
-      setSubNetworklist,
-      setSubNetworkSelected,
-      batchInfoResponse,
-      setIsloadingNetwork
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_NETWORKS}/projects/${credentials.project_id}/global/networks/${subnetwork}`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { subnetworks: string[] }) => {
+              let transformedSubNetworkList = [];
+              /*
+         Extracting  subnetworks from Network
+         Example: "https://www.googleapis.com/compute/v1/projects/{projectName}/global/networks/subnetwork",
+      */
+
+              transformedSubNetworkList = responseResult.subnetworks.map(
+                (data: string) => {
+                  return {
+                    subnetworks: data.split(
+                      `${credentials.region_id}/subnetworks/`
+                    )[1]
+                  };
+                }
+              );
+              const keyLabelStructureSubNetwork = transformedSubNetworkList
+                .filter((obj: SubnetworkData) => obj.subnetworks !== undefined)
+                .map((obj: SubnetworkData) => ({
+                  key: obj.subnetworks,
+                  value: obj.subnetworks,
+                  text: obj.subnetworks
+                }));
+              setSubNetworklist(keyLabelStructureSubNetwork);
+              setDefaultValue(keyLabelStructureSubNetwork[0].value);
+              setSubNetworkSelected(keyLabelStructureSubNetwork[0].value);
+            })
+
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing Networks', err);
+        });
+    }
   };
+  const listMetaStoreAPI = async (data: undefined) => {
+    setIsLoadingService(true);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_META}/projects/${projectId}/locations/${data}/services`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { services: Service[] }) => {
+              let transformClusterListData = [];
+
+              transformClusterListData = responseResult.services.filter(
+                (data: Service) => {
+                  return {
+                    name: data.name
+                  };
+                }
+              );
 
-  const regionListAPI = async (
-    projectId: string,
-    network: string | undefined
-  ) => {
-    await BatchService.regionListAPIService(
-      projectId,
-      network,
-      setIsLoadingService,
-      regionName,
-      setServicesList
-    );
+              const keyLabelStructure = transformClusterListData.map(obj => ({
+                key: obj.name,
+                value: obj.name,
+                text: obj.name
+              }));
+              const noneOption = { key: 'None', value: 'None', text: 'None' };
+              setServicesList([noneOption, ...keyLabelStructure]);
+              setIsLoadingService(false);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoadingService(false);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing services', err);
+          setIsLoadingService(false);
+        });
+    }
+  };
+  const projectListAPI = async () => {
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(PROJECT_LIST_URL, {
+        method: 'GET',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { projects: Project[] }) => {
+              let transformedProjectList = [];
+              transformedProjectList = responseResult.projects.map(
+                (data: Project) => {
+                  return {
+                    value: data.projectId,
+                    key: data.projectId,
+                    text: data.projectId
+                  };
+                }
+              );
+              setProjectList(transformedProjectList);
+            })
+            .catch((e: Error) => console.log(e));
+        })
+        .catch((err: Error) => {
+          console.error('Error fetching project list', err);
+        });
+    }
+  };
+
+  type Region = {
+    name: string;
   };
 
-  const handleSharedSubNetwork = async (data: string | null) => {
-    if (data !== null) {
-      setSharedvpcSelected(data!.toString());
-      await handleProjectIdChange(projectId, data!.toString());
+  const regionListAPI = async (projectId: string) => {
+    setIsLoadingRegion(true);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(`${REGION_URL}${projectId}/regions`, {
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { items: Region[] }) => {
+              let transformedRegionList = [];
+              transformedRegionList = responseResult.items.map(
+                (data: Region) => {
+                  return {
+                    value: data.name,
+                    key: data.name,
+                    text: data.name
+                  };
+                }
+              );
+              setRegionList(transformedRegionList);
+              setIsLoadingRegion(false);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoadingRegion(false);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing regions', err);
+          setIsLoadingRegion(false);
+        });
     }
   };
 
   type Payload = {
-    [key: string]: unknown;
+    [key: string]: any;
   };
 
   type RuntimeConfig = {
     version: string;
     containerImage?: string;
     properties?: object;
   };
@@ -722,63 +739,39 @@
     mainRSelected: string,
     additionalPythonFileSelected: string[],
     mainPythonSelected: string,
     queryFileSelected: string
   ): Payload => {
     const payload: Payload = {};
 
-    if (batchTypeSelected === 'Spark') {
+    if (batchTypeSelected === 'spark') {
       payload.sparkBatch = {
         ...(mainJarSelected !== '' && { mainJarFileUri: mainJarSelected }),
-        ...(mainClassSelected !== '' && { mainClass: mainClassSelected }),
-        ...(ArchiveFilesSelected.length > 0 && {
-          archiveUris: ArchiveFilesSelected
-        }),
-        ...(filesSelected.length > 0 && {
-          fileUris: filesSelected
-        }),
-        ...(jarFilesSelected.length > 0 && { jarFileUris: jarFilesSelected }),
-        ...(argumentsSelected.length > 0 && { args: argumentsSelected })
+        ...(mainClassSelected !== '' && { mainClass: mainClassSelected })
       };
     }
-    if (batchTypeSelected === 'SparkR') {
+    if (batchTypeSelected === 'sparkR') {
       payload.sparkRBatch = {
-        ...(mainRSelected !== '' && { mainRFileUri: mainRSelected }),
-        ...(ArchiveFilesSelected.length > 0 && {
-          archiveUris: ArchiveFilesSelected
-        }),
-        ...(filesSelected.length > 0 && {
-          fileUris: filesSelected
-        }),
-        ...(argumentsSelected.length > 0 && { args: argumentsSelected })
+        ...(mainRSelected !== '' && { mainRFileUri: mainRSelected })
       };
     }
-    if (batchTypeSelected === 'PySpark') {
+    if (batchTypeSelected === 'pySpark') {
       payload.pysparkBatch = {
         ...(additionalPythonFileSelected.length > 0 && {
           pythonFileUris: additionalPythonFileSelected
         }),
         ...(mainPythonSelected !== '' && {
           mainPythonFileUri: mainPythonSelected
-        }),
-        ...(ArchiveFilesSelected.length > 0 && {
-          archiveUris: ArchiveFilesSelected
-        }),
-        ...(filesSelected.length > 0 && {
-          fileUris: filesSelected
-        }),
-        ...(jarFilesSelected.length > 0 && { jarFileUris: jarFilesSelected }),
-        ...(argumentsSelected.length > 0 && { args: argumentsSelected })
+        })
       };
     }
-    if (batchTypeSelected === 'SparkSql') {
+    if (batchTypeSelected === 'sparkSql') {
       payload.sparkSqlBatch = {
         ...(queryFileSelected !== '' && { queryFileUri: queryFileSelected }),
-        ...(parameterObject && { queryVariables: parameterObject }),
-        ...(jarFilesSelected.length > 0 && { jarFileUris: jarFilesSelected })
+        ...(parameterObject && { queryVariables: { query: parameterObject } })
       };
     }
 
     payload.labels = labelObject;
 
     payload.name = `projects/${projectName}/locations/${regionName}/batches/${batchIdSelected}`;
 
@@ -791,51 +784,49 @@
     } as RuntimeConfig;
 
     payload.environmentConfig = {
       executionConfig: {
         ...(serviceAccountSelected !== '' && {
           serviceAccount: serviceAccountSelected
         }),
-        ...(sharedvpcSelected &&
-          selectedNetworkRadio === 'sharedVpc' && {
-            subnetworkUri: `projects/${projectInfo}/regions/${regionName}/subnetworks/${sharedvpcSelected}`
-          }),
         ...(keySelected !== '' &&
-          selectedRadioValue === 'key' &&
-          keySelected !== undefined && {
+          selectedRadioValue === 'key' && {
             kmsKey: `projects/${projectName}/locations/${regionName}/keyRings/${keyRingSelected}/cryptoKeys/${keySelected}`
           }),
         ...(manualKeySelected !== '' &&
           selectedRadioValue === 'manually' && {
             kmsKey: manualKeySelected
           }),
-        ...(subNetworkSelected &&
-          selectedNetworkRadio === 'projectNetwork' && {
-            subnetworkUri: subNetworkSelected
-          }),
-        ...(sharedvpcSelected &&
-          selectedNetworkRadio === 'sharedVpc' && {
-            subnetworkUri: `projects/${projectInfo}/regions/${regionName}/subnetworks/${sharedvpcSelected}`
-          }),
+        subnetworkUri: subNetworkSelected,
         // networkUri:networkSelected,
         ...(networkTagSelected.length > 0 && {
           networkTags: networkTagSelected
         })
-      } as ExecutionConfig,
-      peripheralsConfig: {
+      } as ExecutionConfig
+    };
+
+    if (servicesSelected !== 'None' || clusterSelected !== '') {
+      payload.peripheralsConfig = {
         ...(servicesSelected !== 'None' && {
           metastoreService: servicesSelected
         }),
         ...(clusterSelected !== '' && {
           sparkHistoryServerConfig: {
-            dataprocCluster: `projects/${projectName}/regions/${regionName}/clusters/${clusterSelected}`
+            dataprocCluster: `projects/${projectName}/locations/${regionName}/clusters/${clusterSelected}`
           } as SparkHistoryServerConfig
         })
-      }
-    };
+      };
+    }
+
+    payload.archiveUris =
+      ArchiveFilesSelected.length > 0 ? ArchiveFilesSelected : undefined;
+    payload.fileUris = filesSelected.length > 0 ? filesSelected : undefined;
+    payload.jarFileUris =
+      jarFilesSelected.length > 0 ? jarFilesSelected : undefined;
+    payload.args = argumentsSelected.length > 0 ? argumentsSelected : undefined;
 
     return payload;
   };
 
   const handleSubmit = async () => {
     const credentials = await authApi();
     if (credentials) {
@@ -846,18 +837,15 @@
         const value = labelSplit[1];
         labelObject[key] = value;
       });
       const propertyObject: { [key: string]: string } = {};
       propertyDetailUpdated.forEach((label: string) => {
         const labelSplit = label.split(':');
         const key = labelSplit[0];
-        const value =
-          labelSplit.length > 2
-            ? labelSplit[1] + ':' + labelSplit[2]
-            : labelSplit[1];
+        const value = labelSplit[1];
         propertyObject[key] = value;
       });
       const parameterObject: { [key: string]: string } = {};
       parameterDetailUpdated.forEach((label: string) => {
         const labelSplit = label.split(':');
         const key = labelSplit[0];
         const value = labelSplit[1];
@@ -880,23 +868,40 @@
         batchIdSelected,
         parameterObject,
         mainRSelected,
         additionalPythonFileSelected,
         mainPythonSelected,
         queryFileSelected
       );
-      await BatchService.creatBatchSubmitService(
-        credentials,
-        payload,
-        batchIdSelected,
-        setCreateBatchView,
-        setCreateBatch,
-        setError,
-        error
-      );
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/batches?batchId=${batchIdSelected}`,
+        {
+          method: 'POST',
+          body: JSON.stringify(payload),
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then(async (response: Response) => {
+          if (response.ok) {
+            const responseResult = await response.json();
+            console.log(responseResult);
+            setCreateBatchView(false);
+          } else {
+            const errorResponse = await response.json();
+            console.log(errorResponse);
+            setError({ isOpen: true, message: errorResponse.error.message });
+          }
+        })
+        .catch((err: Error) => {
+          console.error('Error submitting Batch', err);
+          toast.error('Failed to submit the Batch');
+        });
     }
   };
   const generateRandomHex = () => {
     if (!generationCompleted) {
       const crypto = window.crypto || window.Crypto;
       const array = new Uint32Array(1);
       crypto.getRandomValues(array);
@@ -904,1059 +909,831 @@
       const paddedHex = hex.padStart(6, '0');
       setHexNumber('batch-' + paddedHex);
       setBatchIdSelected('batch-' + paddedHex);
       setGenerationCompleted(true);
     }
   };
 
-  const handleInputChange = (event: React.ChangeEvent<HTMLInputElement>) => {
+  const handleInputChange = (event: any) => {
     setHexNumber(event.target.value);
     event.target.value.length > 0
       ? setBatchIdValidation(false)
       : setBatchIdValidation(true);
     const newBatchId = event.target.value;
     setBatchIdSelected(newBatchId);
   };
-  const handleNetworkSharedVpcRadioChange = () => {
-    setSelectedNetworkRadio('sharedVpc');
-    setSubNetworkSelected(subNetworkList[0]!.toString());
-    setNetworkSelected(networkList[0]!.toString());
-  };
-  const handleSubNetworkRadioChange = () => {
-    setSelectedNetworkRadio('projectNetwork');
-    setSharedvpcSelected('');
-  };
-
-  const handleBatchTypeSelected = (data: DropdownProps | null) => {
-    if (data !== null) {
-      setBatchTypeSelected(data!.toString());
-    }
+  const handleBatchTypeSelected = (event: any, data: any) => {
+    setBatchTypeSelected(data.value);
     setFilesSelected([]);
     setJarFilesSelected([]);
     setAdditionalPythonFileSelected([]);
     setArchiveFileSelected([]);
     setArgumentsSelected([]);
     setMainPythonSelected('');
     setMainRSelected('');
     setQueryFileSelected('');
     setMainClassSelected('');
   };
 
-  const handleServiceSelected = (data: string | null) => {
-    if (data !== null) {
-      setServicesSelected(data!.toString());
-    }
+  const handleServiceSelected = (event: any, data: any) => {
+    setServicesSelected(data.value);
   };
-
-  const handleProjectIdChange = (data: any, network: string | undefined) => {
-    setProjectId(data ?? '');
-    setServicesList([]);
-    setServicesSelected('');
-    regionListAPI(data, network);
-  };
-  const handleNetworkChange = async (data: DropdownProps | null) => {
-    if (data !== null) {
-      setNetworkSelected(data!.toString());
-      await listSubNetworksAPI(data!.toString());
-      await handleProjectIdChange(projectId, data!.toString());
-    }
+  const handleProjectIdChange = (event: any, data: any) => {
+    regionListAPI(data.value);
+    setProjectId(data.value);
   };
-  const handleSubNetworkChange = (data: string | null) => {
-    if (data !== null) {
-      setSubNetworkSelected(data!.toString());
-    }
+  const handleRegionChange = (event: any, data: any) => {
+    setRegion(data.value);
+    listMetaStoreAPI(data.value);
   };
-  const handleKeyRingChange = (data: string | null) => {
-    if (data !== null) {
-      setKeyRingSelected(data!.toString());
-      listKeysAPI(data!.toString());
-    }
+  const handleNetworkChange = (event: any, data: any) => {
+    setNetworkSelected(data.value);
+    listSubNetworksAPI(data.value);
   };
-  const handlekeyChange = (data: string | null) => {
-    if (data !== null) {
-      setKeySelected(data!.toString());
-    }
+  const handleSubNetworkChange = (event: any, data: any) => {
+    setSubNetworkSelected(data.value);
   };
-  const handleMainClassSelected = (value: string) => {
-    setMainClassUpdated(true);
-    setMainClassSelected(value);
+  const handleKeyRingChange = (event: any, data: any) => {
+    setKeyRingSelected(data.value);
+    listKeysAPI(data.value);
   };
-  const handleMainJarSelected = (value: string) => {
-    setMainJarUpdated(true);
-    handleValidationFiles(value, setMainJarSelected, setMainJarValidation);
+  const handlekeyChange = (event: any, data: any) => {
+    setKeySelected(data.value);
   };
 
-  const handleClusterSelected = (data: string | null) => {
-    setClusterSelected(data ?? '');
+  const handleClusterSelected = (event: any, data: any) => {
+    setClusterSelected(data.value);
   };
   const handleManualKeySelected = (event: ChangeEvent<HTMLInputElement>) => {
     const inputValue = event.target.value;
     const numericRegex =
       /^projects\/[^/]+\/locations\/[^/]+\/keyRings\/[^/]+\/cryptoKeys\/[^/]+$/;
 
     if (numericRegex.test(inputValue) || inputValue === '') {
       setManualValidation(true);
     } else {
       setManualValidation(false);
     }
 
     setManualKeySelected(inputValue);
   };
+
   return (
     <div>
-      <div className="cluster-details-header">
-        <div
-          className="back-arrow-icon"
-          onClick={() => handleCreateBatchBackView()}
-        >
-          <iconLeftArrow.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+      <div className="scroll-comp">
+        <div className="cluster-details-header">
+          <div
+            className="back-arrow-icon"
+            onClick={() => handleCreateBatchBackView()}
+          >
+            <iconLeftArrow.react tag="div" />
+          </div>
+          <div className="cluster-details-title">Create batch</div>
         </div>
-        <div className="cluster-details-title">Create batch</div>
-      </div>
-      <div className="submit-job-container">
-        <form onSubmit={handleSubmit}>
-          <div className="submit-job-label-header">Batch info</div>
-          <div className="select-text-overlay">
+        <div className="submit-job-container">
+          <form onSubmit={handleSubmit}>
+            <div className="submit-job-label-header">Batch info</div>
+            <div className="create-batches-message">Batch ID*</div>
             <Input
-              className="create-batch-style"
+              className="create-batch-style "
               value={hexNumber}
               onChange={e => handleInputChange(e)}
               type="text"
-              Label="Batch ID*"
             />
-          </div>
-          {batchIdValidation && (
-            <div className="error-key-parent">
-              <iconError.react tag="div" className="logo-alignment-style" />
-              <div className="error-key-missing">ID is required</div>
-            </div>
-          )}
-          <div className="select-text-overlay">
-            <Input
-              className="create-batch-style region-disable"
+            {batchIdValidation && (
+              <div className="error-key-parent">
+                <iconError.react tag="div" />
+                <div className="error-key-missing">ID is required</div>
+              </div>
+            )}
+            <div className="create-batches-message">Region*</div>
+            <Select
+              search
+              className="select-job-style"
               value={regionName}
               type="text"
               disabled={true}
-              Label="Region*"
+              options={[]}
+              placeholder={regionName}
             />
-          </div>
-          <div className="submit-job-label-header">Container</div>
-          <div className="select-text-overlay">
-            <Autocomplete
-              className="project-region-select"
+            <div className="submit-job-label-header">Container</div>
+            <div className="create-batches-message">Batch type*</div>
+            <Select
+              search
+              className="select-job-style"
               value={batchTypeSelected}
+              type="text"
               options={batchTypeList}
-              onChange={(_event, val) => handleBatchTypeSelected(val)}
-              renderInput={params => (
-                <TextField {...params} label=" Batch type*" />
-              )}
+              onChange={handleBatchTypeSelected}
             />
-          </div>
-          <div className="select-text-overlay">
+            <div className="create-batches-message">Runtime version*</div>
+
             <Input
               className="create-batch-style "
               value={versionSelected}
               onChange={e => setVersionSelected(e.target.value)}
               type="text"
-              Label="Runtime version*"
             />
-          </div>
-          {batchTypeSelected === 'Spark' && (
-            <div>
+            {batchTypeSelected === 'spark' && (
               <div>
-                <div className="create-batch-radio">
-                  <Radio
-                    size="small"
-                    className="select-batch-radio-style"
-                    value="mainClass"
-                    checked={selectedRadio === 'mainClass'}
-                    onChange={handleMainClassRadio}
-                  />
-                  <div className="create-batch-message">Main class</div>
-                </div>
-                <div className="create-batch-sub-message">
-                  The fully qualified name of a class in a provided or standard
-                  jar file, for example, com.example.wordcount.
+                <div>
+                  <div className="create-batch-radio">
+                    <Radio
+                      className="select-batch-radio-style"
+                      value="mainClass"
+                      checked={selectedRadio === 'mainClass'}
+                      onChange={handleMainClassRadio}
+                    />
+                    <div className="create-batch-message">Main class</div>
+                  </div>
+                  <div className="create-batch-sub-message">
+                    The fully qualified name of a class in a provided or
+                    standard jar file, for example, com.example.wordcount.
+                  </div>
                 </div>
-              </div>
-              {selectedRadio === 'mainClass' && (
-                <div className="create-batch-input">
-                  <div className="select-text-overlay">
+                {selectedRadio === 'mainClass' && (
+                  <div className="create-batch-input">
+                    <div className="create-batch-message">Main class*</div>
                     <Input
-                      className="create-batch-style-mini"
+                      className="create-batch-style "
                       value={mainClassSelected}
-                      onChange={e => handleMainClassSelected(e.target.value)}
+                      onChange={e => setMainClassSelected(e.target.value)}
                       type="text"
-                      Label="Main class*"
                     />
-                  </div>
-
-                  {selectedRadio === 'mainClass' &&
-                    mainClassSelected === '' &&
-                    mainClassUpdated && (
-                      <div className="error-key-parent">
-                        <iconError.react
-                          tag="div"
-                          className="logo-alignment-style"
-                        />
-                        <div className="error-key-missing">
-                          Main class is required
+                    {selectedRadio === 'mainClass' &&
+                      mainClassSelected === '' && (
+                        <div className="error-key-parent">
+                          <iconError.react tag="div" />
+                          <div className="error-key-missing">
+                            Main class is required
+                          </div>
                         </div>
-                      </div>
-                    )}
-                </div>
-              )}
-            </div>
-          )}
-          {batchTypeSelected === 'Spark' && (
-            <div>
+                      )}
+                  </div>
+                )}
+              </div>
+            )}
+            {batchTypeSelected === 'spark' && (
               <div>
-                <div className="create-batch-radio">
-                  <Radio
-                    size="small"
-                    className="select-batch-radio-style"
-                    value="mainJarURI"
-                    checked={selectedRadio === 'mainJarURI'}
-                    onChange={handleMainJarRadio}
-                  />
-                  <div className="create-batch-message">Main jar URI</div>
-                </div>
-                <div className="create-batch-sub-message">
-                  A provided jar file to use the main class of that jar file.
+                <div>
+                  <div className="create-batch-radio">
+                    <Radio
+                      className="select-batch-radio-style"
+                      value="mainJarURI"
+                      checked={selectedRadio === 'mainJarURI'}
+                      onChange={handleMainJarRadio}
+                    />
+                    <div className="create-batch-message">Main jar URI</div>
+                  </div>
+                  <div className="create-batch-sub-message">
+                    A provided jar file to use the main class of that jar file.
+                  </div>
                 </div>
-              </div>
-              {selectedRadio === 'mainJarURI' && (
-                <div className="create-batch-input">
-                  <div className="select-text-overlay">
+                {selectedRadio === 'mainJarURI' && (
+                  <div className="create-batch-input">
+                    <div className="create-batch-message">Main jar*</div>
                     <Input
-                      className="create-batch-style-mini"
+                      className="create-batch-style "
                       value={mainJarSelected}
-                      onChange={e => handleMainJarSelected(e.target.value)}
+                      onChange={e =>
+                        handleValidationFiles(
+                          e.target.value,
+                          setMainJarSelected,
+                          setMainJarValidation
+                        )
+                      }
                       type="text"
-                      Label="Main jar*"
                     />
-                  </div>
-
-                  {selectedRadio === 'mainJarURI' &&
-                    mainJarSelected === '' &&
-                    mainJarUpdated &&
-                    mainJarValidation && (
+                    {selectedRadio === 'mainJarURI' &&
+                      mainJarSelected === '' && (
+                        <div className="error-key-parent">
+                          <iconError.react tag="div" />
+                          <div className="error-key-missing">
+                            Main jar is required
+                          </div>
+                        </div>
+                      )}
+                    {!mainJarValidation && (
                       <div className="error-key-parent">
-                        <iconError.react
-                          tag="div"
-                          className="logo-alignment-style"
-                        />
+                        <iconError.react tag="div" />
                         <div className="error-key-missing">
-                          Main jar is required
+                          File must include a valid scheme prefix: 'file://',
+                          'gs://', or 'hdfs://'
                         </div>
                       </div>
                     )}
-                  {!mainJarValidation && mainJarSelected !== '' && (
-                    <div className="error-key-parent">
-                      <iconError.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
-                      <div className="error-key-missing">
-                        File must include a valid scheme prefix: 'file://',
-                        'gs://', or 'hdfs://'
-                      </div>
-                    </div>
-                  )}
-                </div>
-              )}
-            </div>
-          )}
-          {batchTypeSelected === 'SparkR' && (
-            <>
-              <div className="select-text-overlay">
+                  </div>
+                )}
+              </div>
+            )}
+
+            {batchTypeSelected === 'sparkR' && (
+              <>
+                <div className="create-batch-message">Main R file*</div>
                 <Input
                   className="create-batch-style"
                   onChange={e =>
                     handleValidationFiles(
                       e.target.value,
                       setMainRSelected,
                       setMainRValidation
                     )
                   }
                   addOnBlur={true}
                   value={mainRSelected}
-                  Label="Main R file*"
                 />
-              </div>
-
-              {!mainRValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    File must include a valid scheme prefix: 'file://', 'gs://',
-                    or 'hdfs://'
+                {!mainRValidation && (
+                  <div className="error-key-parent">
+                    <iconError.react tag="div" />
+                    <div className="error-key-missing">
+                      File must include a valid scheme prefix: 'file://',
+                      'gs://', or 'hdfs://'
+                    </div>
                   </div>
-                </div>
-              )}
-              {mainRValidation && (
-                <div className="submit-job-message-input">
-                  {QUERY_FILE_MESSAGE}
-                </div>
-              )}
-            </>
-          )}
-          {batchTypeSelected === 'PySpark' && (
-            <>
-              <div className="select-text-overlay">
+                )}
+                {mainRValidation && (
+                  <div className="submit-job-message">{QUERY_FILE_MESSAGE}</div>
+                )}
+              </>
+            )}
+            {batchTypeSelected === 'pySpark' && (
+              <>
+                <div className="create-batch-message">Main python file*</div>
                 <Input
                   //placeholder="Main R file*"
                   className="create-batch-style"
                   onChange={e =>
                     handleValidationFiles(
                       e.target.value,
                       setMainPythonSelected,
                       setMainPythonValidation
                     )
                   }
                   addOnBlur={true}
                   value={mainPythonSelected}
-                  Label=" Main python file*"
                 />
-              </div>
-              {!mainPythonValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    File must include a valid scheme prefix: 'file://', 'gs://',
-                    or 'hdfs://'
+                {!mainPythonValidation && (
+                  <div className="error-key-parent">
+                    <iconError.react tag="div" />
+                    <div className="error-key-missing">
+                      File must include a valid scheme prefix: 'file://',
+                      'gs://', or 'hdfs://'
+                    </div>
                   </div>
+                )}
+                {mainPythonValidation && (
+                  <div className="submit-job-message">{QUERY_FILE_MESSAGE}</div>
+                )}
+              </>
+            )}
+            {batchTypeSelected === 'pySpark' && (
+              <>
+                <div className="create-batches-message">
+                  Additional python files
                 </div>
-              )}
-              {mainPythonValidation && (
-                <div className="submit-job-message-input">
-                  {QUERY_FILE_MESSAGE}
-                </div>
-              )}
-            </>
-          )}
-          {batchTypeSelected === 'PySpark' && (
-            <>
-              <div className="select-text-overlay">
-                <MuiChipsInput
+                <TagsInput
                   className="select-job-style"
                   onChange={e =>
                     handleValidationFiles(
                       e,
                       setAdditionalPythonFileSelected,
-                      setAdditionalPythonFileValidation,
-                      setAdditionalPythonFileDuplicateValidation
+                      setAdditionalPythonFileValidation
                     )
                   }
                   addOnBlur={true}
                   value={additionalPythonFileSelected}
                   inputProps={{ placeholder: '' }}
-                  label="Additional python files"
                 />
-              </div>
-              {!additionalPythonFileValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    All files must include a valid scheme prefix: 'file://',
-                    'gs://', or 'hdfs://'
-                  </div>
-                </div>
-              )}
-              {additionalPythonFileDuplicateValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Duplicate paths are not allowed
+                {!additionalPythonFileValidation && (
+                  <div className="error-key-parent">
+                    <iconError.react tag="div" />
+                    <div className="error-key-missing">
+                      All files must include a valid scheme prefix: 'file://',
+                      'gs://', or 'hdfs://'
+                    </div>
                   </div>
-                </div>
-              )}
-            </>
-          )}
-          {batchTypeSelected === 'SparkSql' && (
-            <>
-              <div className="select-text-overlay">
+                )}
+              </>
+            )}
+            {batchTypeSelected === 'sparkSql' && (
+              <>
+                <div className="create-batch-message">Query file*</div>
                 <Input
                   //placeholder="Main R file*"
                   className="create-batch-style"
                   onChange={e =>
                     handleValidationFiles(
                       e.target.value,
                       setQueryFileSelected,
                       setQueryFileValidation
                     )
                   }
                   addOnBlur={true}
                   value={queryFileSelected}
-                  Label="Query file*"
                 />
-              </div>
-
-              {!queryFileValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    File must include a valid scheme prefix: 'file://', 'gs://',
-                    or 'hdfs://'
+                {!queryFileValidation && (
+                  <div className="error-key-parent">
+                    <iconError.react tag="div" />
+                    <div className="error-key-missing">
+                      File must include a valid scheme prefix: 'file://',
+                      'gs://', or 'hdfs://'
+                    </div>
                   </div>
-                </div>
-              )}
-              {queryFileValidation && (
-                <div className="create-messagelist">{QUERY_FILE_MESSAGE}</div>
-              )}
-            </>
-          )}
-          <div className="select-text-overlay">
+                )}
+                {queryFileValidation && (
+                  <div className="create-messagelist">{QUERY_FILE_MESSAGE}</div>
+                )}
+              </>
+            )}
+            <div className="create-batches-message">Custom container image</div>
             <Input
               className="create-batch-style "
               value={containerImageSelected}
               onChange={e => setContainerImageSelected(e.target.value)}
               type="text"
-              placeholder="Enter URI, for example, gcr.io/my-project-id/my-image:1.0.1"
-              Label="Custom container image"
+              placeholder=""
             />
-          </div>
-          <div className="create-custom-messagelist">
-            {CUSTOM_CONTAINER_MESSAGE}{' '}
-          </div>{' '}
-          <div className="create-container-message">
-            <div className="create-container-image-message">
-              {CUSTOM_CONTAINER_MESSAGE_PART}
-            </div>
-            <div
-              className="learn-more-url"
-              onClick={() => {
-                window.open(`${CONTAINER_REGISTERY}`, '_blank');
-              }}
-            >
-              Container Registry
-            </div>
-            &nbsp; <div className="create-container-image-message">or</div>
-            &nbsp;
-            <div
-              className="learn-more-url"
-              onClick={() => {
-                window.open(`${ARTIFACT_REGISTERY}`, '_blank');
-              }}
-            >
-              Artifact Registry
-            </div>
-            {' . '}
-            <div
-              className="learn-more-url"
-              onClick={() => {
-                window.open(`${CUSTOM_CONTAINERS}`, '_blank');
-              }}
-            >
-              Learn more
+            <div className="create-custom-messagelist">
+              {CUSTOM_CONTAINER_MESSAGE}
+              <div className="create-container-message">
+                <div
+                  className="create-batch-learn-more"
+                  onClick={() => {
+                    window.open(`${CONTAINER_REGISTERY}`, '_blank');
+                  }}
+                >
+                  Container Registry
+                </div>
+                {' or '}
+                <div
+                  className="create-batch-learn-more"
+                  onClick={() => {
+                    window.open(`${ARTIFACT_REGISTERY}`, '_blank');
+                  }}
+                >
+                  Artifact Registry
+                </div>
+                {' . '}
+                <div
+                  className="submit-job-learn-more"
+                  onClick={() => {
+                    window.open(`${CUSTOM_CONTAINERS}`, '_blank');
+                  }}
+                >
+                  Learn more
+                </div>
+              </div>
             </div>
-          </div>
-          {
-            batchTypeSelected !== 'SparkR' && (
-              <>
-                <div className="select-text-overlay">
-                  <MuiChipsInput
+            {batchTypeSelected === 'spark' ||
+              (batchTypeSelected === 'sparkSql' && (
+                <>
+                  <div className="create-batches-message">Jar files</div>
+                  <TagsInput
                     className="select-job-style"
                     onChange={e =>
                       handleValidationFiles(
                         e,
                         setJarFilesSelected,
-                        setJarFileValidation,
-                        setJarFileDuplicateValidation
+                        setJarFileValidation
                       )
                     }
                     addOnBlur={true}
                     value={jarFilesSelected}
                     inputProps={{ placeholder: '' }}
-                    label="Jar files"
                   />
-                </div>
-
-                {!jarFileValidation && (
-                  <div className="error-key-parent">
-                    <iconError.react
-                      tag="div"
-                      className="logo-alignment-style"
-                    />
-                    <div className="error-key-missing">
-                      All files must include a valid scheme prefix: 'file://',
-                      'gs://', or 'hdfs://'
-                    </div>
-                  </div>
-                )}
-                {jarFileDuplicateValidation && (
-                  <div className="error-key-parent">
-                    <iconError.react
-                      tag="div"
-                      className="logo-alignment-style"
-                    />
-                    <div className="error-key-missing">
-                      Duplicate paths are not allowed
+                  {!jarFileValidation && (
+                    <div className="error-key-parent">
+                      <iconError.react tag="div" />
+                      <div className="error-key-missing">
+                        All files must include a valid scheme prefix: 'file://',
+                        'gs://', or 'hdfs://'
+                      </div>
                     </div>
-                  </div>
-                )}
-                {jarFileValidation && !jarFileDuplicateValidation && (
-                  <div className="create-messagelist">{JAR_FILE_MESSAGE}</div>
-                )}
-              </>
-            )
-            //) )
-          }
-          {batchTypeSelected !== 'SparkSql' && (
-            <>
-              <div className="select-text-overlay">
-                <MuiChipsInput
+                  )}
+                  {jarFileValidation && (
+                    <div className="create-messagelist">{JAR_FILE_MESSAGE}</div>
+                  )}
+                </>
+              ))}
+            {batchTypeSelected !== 'sparkSql' && (
+              <>
+                <div className="create-batches-message">Files</div>
+                <TagsInput
                   className="select-job-style"
                   onChange={e =>
                     handleValidationFiles(
                       e,
                       setFilesSelected,
-                      setFileValidation,
-                      setFileDuplicateValidation
+                      setFileValidation
                     )
                   }
                   addOnBlur={true}
                   value={filesSelected}
                   inputProps={{ placeholder: '' }}
-                  label="Files"
                 />
-              </div>
-              {!fileValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    All files must include a valid scheme prefix: 'file://',
-                    'gs://', or 'hdfs://'
-                  </div>
-                </div>
-              )}
-              {fileDuplicateValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Duplicate paths are not allowed
+                {!fileValidation && (
+                  <div className="error-key-parent">
+                    <iconError.react tag="div" />
+                    <div className="error-key-missing">
+                      All files must include a valid scheme prefix: 'file://',
+                      'gs://', or 'hdfs://'
+                    </div>
                   </div>
-                </div>
-              )}
-              {fileValidation && !fileDuplicateValidation && (
-                <div className="create-messagelist">{FILES_MESSAGE}</div>
-              )}
-            </>
-          )}
-          {batchTypeSelected !== 'SparkSql' && (
-            <>
-              <div className="select-text-overlay">
-                <MuiChipsInput
+                )}
+                {fileValidation && (
+                  <div className="create-messagelist">{FILES_MESSAGE}</div>
+                )}
+              </>
+            )}
+            {batchTypeSelected !== 'sparkSql' && (
+              <>
+                <div className="create-batches-message">Archive files</div>
+                <TagsInput
                   className="select-job-style"
                   onChange={e =>
                     handleValidationFiles(
                       e,
                       setArchiveFileSelected,
-                      setArchieveFileValidation,
-                      setArchiveDuplicateValidation
+                      setArchieveFileValidation
                     )
                   }
                   addOnBlur={true}
                   value={ArchiveFilesSelected}
                   inputProps={{ placeholder: '' }}
-                  label="Archive files"
                 />
-              </div>
-              {!archieveFileValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    All files must include a valid scheme prefix: 'file://',
-                    'gs://', or 'hdfs://'
+                {!archieveFileValidation && (
+                  <div className="error-key-parent">
+                    <iconError.react tag="div" />
+                    <div className="error-key-missing">
+                      All files must include a valid scheme prefix: 'file://',
+                      'gs://', or 'hdfs://'
+                    </div>
                   </div>
-                </div>
-              )}
-              {archiveDuplicateValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Duplicate paths are not allowed
+                )}
+                {archieveFileValidation && (
+                  <div className="create-messagelist">
+                    {ARCHIVE_FILES_MESSAGE}
                   </div>
-                </div>
-              )}
-              {archieveFileValidation && !archiveDuplicateValidation && (
-                <div className="create-messagelist">
-                  {ARCHIVE_FILES_MESSAGE}
-                </div>
-              )}
-            </>
-          )}
-          {batchTypeSelected !== 'SparkSql' && (
-            <>
-              <div className="select-text-overlay">
-                <MuiChipsInput
+                )}
+              </>
+            )}
+            {batchTypeSelected !== 'sparkSql' && (
+              <>
+                <div className="create-batches-message">Arguments</div>
+                <TagsInput
                   className="select-job-style"
-                  onChange={e =>
-                    handleArguments(setArgumentsDuplicateValidation, e)
-                  }
+                  onChange={e => setArgumentsSelected(e)}
                   addOnBlur={true}
                   value={argumentsSelected}
                   inputProps={{ placeholder: '' }}
-                  label="Arguments"
                 />
-              </div>
-              {argumentsDuplicateValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Duplicate paths are not allowed
-                  </div>
-                </div>
-              )}
-              {!argumentsDuplicateValidation && (
                 <div className="create-messagelist">{ARGUMENTS_MESSAGE}</div>
-              )}
-            </>
-          )}
-          {batchTypeSelected === 'SparkSql' && (
-            <>
-              <div className="submit-job-label-header">Query parameters</div>
-              <LabelProperties
-                labelDetail={parameterDetail}
-                setLabelDetail={setParameterDetail}
-                labelDetailUpdated={parameterDetailUpdated}
-                setLabelDetailUpdated={setParameterDetailUpdated}
-                buttonText="ADD PARAMETER"
-                keyValidation={keyValidation}
-                setKeyValidation={setKeyValidation}
-                valueValidation={valueValidation}
-                setValueValidation={setValueValidation}
-                duplicateKeyError={duplicateKeyError}
-                setDuplicateKeyError={setDuplicateKeyError}
-              />
-            </>
-          )}
-          <div className="submit-job-label-header">Execution Configuration</div>
-          <div className="select-text-overlay">
+              </>
+            )}
+            {batchTypeSelected === 'sparkSql' && (
+              <>
+                <div className="submit-job-label-header">Query parameters</div>
+                <LabelProperties
+                  labelDetail={parameterDetail}
+                  setLabelDetail={setParameterDetail}
+                  labelDetailUpdated={parameterDetailUpdated}
+                  setLabelDetailUpdated={setParameterDetailUpdated}
+                  buttonText="ADD PARAMETER"
+                  keyValidation={keyValidation}
+                  setKeyValidation={setKeyValidation}
+                  valueValidation={valueValidation}
+                  setValueValidation={setValueValidation}
+                  duplicateKeyError={duplicateKeyError}
+                  setDuplicateKeyError={setDuplicateKeyError}
+                />
+              </>
+            )}
+            <div className="submit-job-label-header">
+              Execution Configuration
+            </div>
+            <div className="create-batches-message">Service account</div>
             <Input
               className="create-batch-style "
               value={serviceAccountSelected}
               onChange={e => setServiceAccountSelected(e.target.value)}
               type="text"
               placeholder=""
-              Label="Service account"
             />
-          </div>
-          <div className="create-custom-messagelist">
-            If not provided, the default GCE service account will be used.
-            <div
-              className="submit-job-learn-more"
-              onClick={() => {
-                window.open(`${SERVICE_ACCOUNT}`, '_blank');
-              }}
-            >
-              Learn more
-            </div>
-          </div>
-          <div className="submit-job-label-header">Network Configuration</div>
-          <div className="runtime-message">
-            Establishes connectivity for the VM instances in this cluster.
-          </div>
-          <div>
-            <div className="create-runtime-radio">
-              <Radio
-                size="small"
-                className="select-runtime-radio-style"
-                value="projectNetwork"
-                checked={selectedNetworkRadio === 'projectNetwork'}
-                onChange={() => handleSubNetworkRadioChange()}
-              />
-              <div className="create-batch-message">
-                Networks in this project
-              </div>
-            </div>
-          </div>
-          <div>
-            <div className="create-runtime-radio">
-              <Radio
-                size="small"
-                className="select-runtime-radio-style"
-                value="sharedVpc"
-                checked={selectedNetworkRadio === 'sharedVpc'}
-                onChange={() => handleNetworkSharedVpcRadioChange()}
-              />
-              <div className="create-batch-message">
-                Networks shared from host project: "{projectInfo}"
-              </div>
-            </div>
-            <div className="create-runtime-sub-message-network">
-              Choose a shared VPC network from project that is different from
-              this cluster's project.{' '}
+            <div className="create-messagelist">
+              If not provided, the default GCE service account will be used.
               <div
-                className="submit-job-learn-more"
+                className="create-batch-learn-more"
                 onClick={() => {
-                  window.open(`${SHARED_VPC}`, '_blank');
+                  window.open(`${SERVICE_ACCOUNT}`, '_blank');
                 }}
               >
                 Learn more
               </div>
             </div>
-          </div>
-          <div>
-            {selectedNetworkRadio === 'projectNetwork' && (
-              <div className="create-batch-network">
-                {isloadingNetwork ? (
-                  <div className="metastore-loader">
-                    <CircularProgress
-                      size={25}
-                      aria-label="Loading Spinner"
-                      data-testid="loader"
-                    />
-                  </div>
-                ) : (
-                  <>
-                    <div className="select-text-overlay">
-                      <Autocomplete
-                        options={networkList}
-                        value={networkSelected}
-                        onChange={(_event, val) => handleNetworkChange(val)}
-                        renderInput={params => (
-                          <TextField {...params} label="Primary network*" />
-                        )}
-                      />
-                    </div>
-                    <div className="select-text-overlay subnetwork-style">
-                      <Autocomplete
-                        options={subNetworkList}
-                        value={subNetworkSelected}
-                        onChange={(_event, val) => handleSubNetworkChange(val)}
-                        renderInput={params => (
-                          <TextField {...params} label="subnetwork" />
-                        )}
-                      />
-                    </div>
-                  </>
-                )}
+            <div className="submit-job-label-header">Network Configuration</div>
+            <div className="create-batches-message">
+              Establishes connectivity for the VM instances in this cluster.
+            </div>
+            <div className="create-batches-message">
+              Networks in this project
+            </div>
+            <div className="create-batch-network">
+              <div className="create-batch-network-message">
+                Primary network*
               </div>
-            )}
-            {selectedNetworkRadio === 'projectNetwork' &&
-              networkList.length === 0 && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    No local networks are available.
-                  </div>
-                </div>
-              )}
-            {!isloadingNetwork &&
-              selectedNetworkRadio === 'projectNetwork' &&
-              networkList.length !== 0 &&
-              subNetworkList.length === 0 && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Please select a valid network and subnetwork.
-                  </div>
-                </div>
-              )}
+              <div className="create-batch-network-message">Subnetwork</div>
+            </div>
+            <div>
+              <div className="create-batch-network">
+                <Select
+                  search
+                  className="select-primary-network-style"
+                  value={networkSelected}
+                  onChange={handleNetworkChange}
+                  type="text"
+                  options={networkList}
+                />
 
-            {selectedNetworkRadio === 'sharedVpc' && (
-              <div className="select-text-overlay">
-                <Autocomplete
-                  options={sharedSubNetworkList}
-                  value={sharedvpcSelected}
-                  onChange={(_event, val) => handleSharedSubNetwork(val)}
-                  renderInput={params => (
-                    <TextField {...params} label="Shared subnetwork" />
-                  )}
+                <Select
+                  search
+                  className="select-sub-network-style"
+                  value={subNetworkSelected}
+                  onChange={handleSubNetworkChange}
+                  type="text"
+                  options={subNetworkList}
+                  placeholder={defaultValue}
                 />
               </div>
-            )}
-            {selectedNetworkRadio === 'sharedVpc' &&
-              sharedSubNetworkList.length === 0 && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    No shared subnetworks are available in this region.
-                  </div>
-                </div>
-              )}
-          </div>
-          <div className="select-text-overlay">
-            <MuiChipsInput
+            </div>
+            <div className="create-batches-message">Network tags*</div>
+            <TagsInput
               className="select-job-style"
-              onChange={e =>
-                handleNetworkTags(setNetworkTagsDuplicateValidation, e)
-              }
+              onChange={e => setNetworkTagSelected(e)}
               addOnBlur={true}
               value={networkTagSelected}
               inputProps={{ placeholder: '' }}
-              label="Network tags"
             />
-          </div>
-          {networkTagsDuplicateValidation && (
-            <div className="error-key-parent">
-              <iconError.react tag="div" className="logo-alignment-style" />
-              <div className="error-key-missing">
-                Duplicate paths are not allowed
-              </div>
-            </div>
-          )}
-          {!networkTagsDuplicateValidation && (
-            <div className="create-messagelist">{NETWORK_TAG_MESSAGE}</div>
-          )}
-          <div>
-            <div className="submit-job-label-header">Encryption</div>
             <div>
-              <div className="create-batch-radio">
-                <Radio
-                  size="small"
-                  className="select-batch-radio-style"
-                  value="googleManaged"
-                  checked={selectedEncryptionRadio === 'googleManaged'}
-                  onChange={handleGoogleManagedRadio}
-                />
-                <div className="create-batch-message">
-                  Google-managed encryption key
+              <div className="submit-job-label-header">Encryption</div>
+              <div>
+                <div className="create-batch-radio">
+                  <Radio
+                    className="select-batch-radio-style"
+                    value="googleManaged"
+                    checked={selectedEncryptionRadio === 'googleManaged'}
+                    onChange={() => setSelectedEncryptionRadio('googleManaged')}
+                  />
+                  <div className="create-batch-message">
+                    Google-managed encryption key
+                  </div>
                 </div>
-              </div>
-              <div className="create-batch-sub-message">
-                No configuration required
-              </div>
-            </div>
-            <div>
-              <div className="create-batch-radio">
-                <Radio
-                  size="small"
-                  className="select-batch-radio-style"
-                  value="googleManaged"
-                  checked={selectedEncryptionRadio === 'customerManaged'}
-                  onChange={() => setSelectedEncryptionRadio('customerManaged')}
-                />
-                <div className="create-batch-message">
-                  Customer-managed encryption key (CMEK)
+                <div className="create-batch-sub-message">
+                  No configuration required
                 </div>
               </div>
-              <div className="create-batch-sub-message">
-                Manage via{' '}
-                <div
-                  className="submit-job-learn-more"
-                  onClick={() => {
-                    window.open(
-                      `${SECURITY_KEY}?project=${projectName}`,
-                      '_blank'
-                    );
-                  }}
-                >
-                  Google Cloud Key Management Service
+              <div>
+                <div className="create-batch-radio">
+                  <Radio
+                    className="select-batch-radio-style"
+                    value="googleManaged"
+                    checked={selectedEncryptionRadio === 'customerManaged'}
+                    onChange={() =>
+                      setSelectedEncryptionRadio('customerManaged')
+                    }
+                  />
+                  <div className="create-batch-message">
+                    Customer-managed encryption key (CMEK)
+                  </div>
                 </div>
-              </div>
-              {selectedEncryptionRadio === 'customerManaged' && (
-                <>
-                  <div>
+                <div className="create-batch-sub-message">
+                  Manage via{' '}
+                  <div
+                    className="create-batch-learn-more"
+                    onClick={() => {
+                      window.open(`${SECURITY_KEY}`, '_blank');
+                    }}
+                  >
+                    Google Cloud Key Management Service
+                  </div>
+                </div>
+                {selectedEncryptionRadio === 'customerManaged' && (
+                  <>
                     <div className="create-batch-encrypt">
-                      <Radio
-                        size="small"
-                        className="select-batch-encrypt-radio-style"
-                        value="mainClass"
-                        checked={selectedRadioValue === 'key'}
-                        onChange={handlekeyRingRadio}
-                      />
-                      <div className="select-text-overlay">
-                        <Autocomplete
-                          disabled={
-                            selectedRadioValue === 'manually' ? true : false
-                          }
-                          options={keyRinglist}
+                      <div className="create-batch-encrypt-message">
+                        keyRings
+                      </div>
+                      <div className="create-batch-encrypt-message">keys</div>
+                    </div>
+                    <div>
+                      <div className="create-batch-encrypt">
+                        <Radio
+                          className="select-batch-encrypt-radio-style"
+                          value="mainClass"
+                          checked={selectedRadioValue === 'key'}
+                          onChange={handlekeyRingRadio}
+                        />
+
+                        <Select
+                          search
+                          className="select-primary-network-style"
                           value={keyRingSelected}
-                          onChange={(_event, val) => handleKeyRingChange(val)}
-                          renderInput={params => (
-                            <TextField {...params} label="Key rings" />
-                          )}
+                          type="text"
+                          disabled={selectedRadioValue === 'manually'}
+                          onChange={handleKeyRingChange}
+                          options={keyRinglist}
                         />
-                      </div>
-                      <div className="select-text-overlay subnetwork-style">
-                        <Autocomplete
-                          disabled={
-                            selectedRadioValue === 'manually' ? true : false
-                          }
-                          options={keylist}
+
+                        <Select
+                          search
+                          className="select-sub-network-style"
                           value={keySelected}
-                          onChange={(_event, val) => handlekeyChange(val)}
-                          renderInput={params => (
-                            <TextField {...params} label="Keys" />
-                          )}
+                          disabled={selectedRadioValue === 'manually'}
+                          onChange={handlekeyChange}
+                          type="text"
+                          options={keylist}
                         />
                       </div>
                     </div>
-                  </div>
-                  <div className="manual-input">
-                    <div className="encrypt">
-                      <Radio
-                        size="small"
-                        className="select-batch-encrypt-radio-style "
-                        value="mainClass"
-                        checked={selectedRadioValue === 'manually'}
-                        onChange={handlekeyManuallyRadio}
-                      />
-                      <div className="select-text-overlay">
+                    <div className="manual-input">
+                      <div className="create-batch-encrypt-message">
+                        Enter key Manually
+                      </div>
+                      <div className="encrypt">
+                        <Radio
+                          className="select-batch-encrypt-radio-style "
+                          value="mainClass"
+                          checked={selectedRadioValue === 'manually'}
+                          onChange={handlekeyManuallyRadio}
+                        />
                         <Input
-                          className={
-                            selectedRadioValue === 'key'
-                              ? 'disable-text create-batch-key manual-key'
-                              : 'create-batch-style manual-key'
-                          }
+                          className="create-batch-style "
                           value={manualKeySelected}
                           type="text"
                           disabled={selectedRadioValue === 'key'}
                           onChange={handleManualKeySelected}
-                          Label="Enter key manually"
                         />
+                       
                       </div>
+                      {!manualValidation && (
+                          <div className="error-key-parent">
+                            <iconError.react tag="div" />
+                            <div className="error-key-missing">
+                              {KEY_MESSAGE}
+                            </div>
+                          </div>
+                        )}
                     </div>
-                    {!manualValidation && (
-                      <div className="error-key-parent-manual">
-                        <iconError.react
-                          tag="div"
-                          className="logo-alignment-style"
-                        />
-                        <div className="error-key-missing">{KEY_MESSAGE}</div>
-                      </div>
-                    )}
-                  </div>
-                </>
-              )}
+                  </>
+                )}
+              </div>
             </div>
-          </div>
-          <div className="submit-job-label-header">
-            Peripheral Configuration
-          </div>
-          <div className="create-batches-message">
-            Configure Dataproc to use Dataproc Metastore as its Hive metastore.
-            <div
-              className="submit-job-learn-more"
-              onClick={() => {
-                window.open(`${SELF_MANAGED_CLUSTER}`, '_blank');
-              }}
-            >
-              Learn more
+
+            <div className="submit-job-label-header">
+              Peripheral Configuration
             </div>
-          </div>
-          <div className="create-messagelist">{METASTORE_MESSAGE}</div>
-          <div className="select-text-overlay">
-            <DynamicDropdown
+            <div className="create-batches-message">
+              Configure Dataproc to use Dataproc Metastore as its Hive
+              metastore.
+              <div
+                className="create-batch-learn-more"
+                onClick={() => {
+                  window.open(`${SELF_MANAGED_CLUSTER}`, '_blank');
+                }}
+              >
+                Learn more
+              </div>
+            </div>
+            <div className="create-messagelist">{METASTORE_MESSAGE}</div>
+            <div className="create-batches-message">Metastore project</div>
+            <Select
+              search
+              placeholder={projectId}
+              className="select-job-style"
               value={projectId}
-              onChange={(_, projectId) =>
-                handleProjectIdChange(projectId, networkSelected)
-              }
-              fetchFunc={projectListAPI}
-              label="Project ID"
-              // Always show the clear indicator and hide the dropdown arrow
-              // make it very clear that this is an autocomplete.
-              sx={{
-                '& .MuiAutocomplete-clearIndicator': {
-                  visibility: 'hidden'
-                }
-              }}
-              popupIcon={null}
+              onChange={handleProjectIdChange}
+              options={projectList}
             />
-          </div>
-          <div className="select-text-overlay">
+            <div className="create-batches-message">Metastore region</div>
+            {isLoadingRegion ? (
+              <ClipLoader
+                loading={true}
+                size={25}
+                aria-label="Loading Spinner"
+                data-testid="loader"
+              />
+            ) : (
+              <Select
+                search
+                placeholder={region}
+                className="select-job-style"
+                value={region}
+                onChange={handleRegionChange}
+                options={regionList}
+              />
+            )}
+
+            <div className="create-batches-message">Metastore service</div>
             {isLoadingService ? (
-              <div className="metastore-loader">
-                <CircularProgress
-                  size={25}
-                  aria-label="Loading Spinner"
-                  data-testid="loader"
-                />
-              </div>
+              <ClipLoader
+                loading={true}
+                size={25}
+                aria-label="Loading Spinner"
+                data-testid="loader"
+              />
             ) : (
-              <Autocomplete
-                options={servicesList}
+              <Select
+                search
+                className="select-job-style"
                 value={servicesSelected}
-                onChange={(_event, val) => handleServiceSelected(val)}
-                renderInput={params => (
-                  <TextField {...params} label="Metastore services" />
-                )}
+                type="text"
+                options={servicesList}
+                onChange={handleServiceSelected}
+                placeholder="None"
               />
             )}
-          </div>
-          <div className="submit-job-label-header">History server cluster</div>
-          <div className="create-batches-message">
-            Choose a history server cluster to store logs in.{' '}
-          </div>
-          <div className="select-text-overlay">
-            <Autocomplete
-              options={clustersList}
+
+            <div className="submit-job-label-header">
+              History server cluster
+            </div>
+            <div className="create-batches-message">
+              Choose a history server cluster to store logs in.{' '}
+            </div>
+            <div className="create-batches-message">History server cluster</div>
+
+            <Dropdown
+              className="select-job-style"
+              search
+              selection
               value={clusterSelected}
-              onChange={(_event, val) => handleClusterSelected(val)}
-              noOptionsText="No history server clusters available"
-              renderInput={params => (
-                <TextField {...params} label="History server cluster" />
-              )}
+              onChange={handleClusterSelected}
+              options={clustersList}
+              placeholder="Search..."
             />
-          </div>
-          <div className="submit-job-label-header">Properties</div>
-          <LabelProperties
-            labelDetail={propertyDetail}
-            setLabelDetail={setPropertyDetail}
-            labelDetailUpdated={propertyDetailUpdated}
-            setLabelDetailUpdated={setPropertyDetailUpdated}
-            buttonText="ADD PROPERTY"
-            keyValidation={keyValidation}
-            setKeyValidation={setKeyValidation}
-            valueValidation={valueValidation}
-            setValueValidation={setValueValidation}
-            duplicateKeyError={duplicateKeyError}
-            setDuplicateKeyError={setDuplicateKeyError}
-          />
-          <div className="submit-job-label-header">Labels</div>
-          <LabelProperties
-            labelDetail={labelDetail}
-            setLabelDetail={setLabelDetail}
-            labelDetailUpdated={labelDetailUpdated}
-            setLabelDetailUpdated={setLabelDetailUpdated}
-            buttonText="ADD LABEL"
-            keyValidation={keyValidation}
-            setKeyValidation={setKeyValidation}
-            valueValidation={valueValidation}
-            setValueValidation={setValueValidation}
-            duplicateKeyError={duplicateKeyError}
-            setDuplicateKeyError={setDuplicateKeyError}
-            batchInfoResponse={batchInfoResponse}
-            createBatch={createBatch}
-          />
-          <div className="job-button-style-parent">
-            <div
-              className={
-                isSubmitDisabled()
-                  ? 'submit-button-disable-style'
-                  : 'submit-button-style'
-              }
-              aria-label="submit Batch"
-            >
+            <div className="submit-job-label-header">Properties</div>
+            <LabelProperties
+              labelDetail={propertyDetail}
+              setLabelDetail={setPropertyDetail}
+              labelDetailUpdated={propertyDetailUpdated}
+              setLabelDetailUpdated={setPropertyDetailUpdated}
+              buttonText="ADD PROPERTY"
+              keyValidation={keyValidation}
+              setKeyValidation={setKeyValidation}
+              valueValidation={valueValidation}
+              setValueValidation={setValueValidation}
+              duplicateKeyError={duplicateKeyError}
+              setDuplicateKeyError={setDuplicateKeyError}
+            />
+            <div className="submit-job-label-header">Labels</div>
+            <LabelProperties
+              labelDetail={labelDetail}
+              setLabelDetail={setLabelDetail}
+              labelDetailUpdated={labelDetailUpdated}
+              setLabelDetailUpdated={setLabelDetailUpdated}
+              buttonText="ADD LABEL"
+              keyValidation={keyValidation}
+              setKeyValidation={setKeyValidation}
+              valueValidation={valueValidation}
+              setValueValidation={setValueValidation}
+              duplicateKeyError={duplicateKeyError}
+              setDuplicateKeyError={setDuplicateKeyError}
+            />
+            <div className="job-button-style-parent">
               <div
-                onClick={() => {
-                  if (!isSubmitDisabled()) {
-                    handleSubmit();
-                  }
-                }}
+                className={
+                  isSubmitDisabled()
+                    ? 'submit-button-disable-style'
+                    : 'submit-button-style'
+                }
+                aria-label="submit Batch"
               >
-                SUBMIT
+                <div
+                  onClick={() => {
+                    if (!isSubmitDisabled()) {
+                      handleSubmit();
+                    }
+                  }}
+                >
+                  SUBMIT
+                </div>
               </div>
+              <div
+                className="job-cancel-button-style"
+                aria-label="cancel Batch"
+              >
+                <div onClick={() => handleCreateBatchBackView()}>CANCEL</div>
+              </div>
+              {error.isOpen && (
+                <ErrorPopup
+                  onCancel={() => setError({ isOpen: false, message: '' })}
+                  errorPopupOpen={error.isOpen}
+                  DeleteMsg={error.message}
+                />
+              )}
             </div>
-            <div className="job-cancel-button-style" aria-label="cancel Batch">
-              <div onClick={() => handleCreateBatchBackView()}>CANCEL</div>
-            </div>
-            {error.isOpen && (
-              <ErrorPopup
-                onCancel={() => setError({ isOpen: false, message: '' })}
-                errorPopupOpen={error.isOpen}
-                errorMsg={error.message}
-              />
-            )}
-          </div>
-        </form>
+          </form>
+        </div>
       </div>
     </div>
   );
 }
 
 export default CreateBatch;
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/batches/listBatches.tsx` & `dataproc_jupyter_plugin-0.1.9/src/login/configSelection.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -11,424 +11,403 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-import React, { useEffect, useRef, useState } from 'react';
-import { useTable, useGlobalFilter, usePagination } from 'react-table';
+import React, { useState, useEffect } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
-import SubmitJobIcon from '../../style/icons/submit_job_icon.svg';
-import filterIcon from '../../style/icons/filter_icon.svg';
-import SucceededIcon from '../../style/icons/succeeded_icon.svg';
-import clusterRunningIcon from '../../style/icons/cluster_running_icon.svg';
-import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
-import GlobalFilter from '../utils/globalFilter';
+import settingsIcon from '../../style/icons/settings_icon.svg';
 import {
-  BatchStatus,
-  STATUS_CREATING,
-  STATUS_DELETING,
-  STATUS_FAIL,
-  STATUS_PENDING,
-  STATUS_PROVISIONING,
-  STATUS_RUNNING,
-  STATUS_SUCCESS
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
+  REGION_URL,
+  USER_INFO_URL
 } from '../utils/const';
-import TableData from '../utils/tableData';
-import { PaginationView } from '../utils/paginationView';
-import { ICellProps } from '../utils/utils';
-import { BatchService } from './batchService';
-import PollingTimer from '../utils/pollingTimer';
-import DeletePopup from '../utils/deletePopup';
-import BatchDetails from './batchDetails';
-import CreateBatch from './createBatch';
-
-import deleteIcon from '../../style/icons/delete_icon.svg';
-import { CircularProgress } from '@mui/material';
-
-const iconSubmitJob = new LabIcon({
-  name: 'launcher:submit-job-icon',
-  svgstr: SubmitJobIcon
+import { authApi } from '../utils/utils';
+import { Select } from 'semantic-ui-react';
+import 'semantic-ui-css/semantic.min.css';
+import { requestAPI } from '../handler/handler';
+import ClipLoader from 'react-spinners/ClipLoader';
+import { ToastContainer, ToastOptions, toast } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
+import THIRD_PARTY_LICENSES from '../../third-party-licenses.txt';
+import ListRuntimeTemplates from '../runtime/listRuntimeTemplates';
+import expandLessIcon from '../../style/icons/expand_less.svg';
+import expandMoreIcon from '../../style/icons/expand_more.svg';
+import CreateRuntime from '../runtime/createRunTime';
+import { SessionTemplate } from '../utils/listRuntimeTemplateInterface';
+import { ProjectIDDropdown } from './projectIdDropdown';
+
+const iconExpandLess = new LabIcon({
+  name: 'launcher:expand-less-icon',
+  svgstr: expandLessIcon
 });
-const iconFilter = new LabIcon({
-  name: 'launcher:filter-icon',
-  svgstr: filterIcon
-});
-const iconSucceeded = new LabIcon({
-  name: 'launcher:succeeded-icon',
-  svgstr: SucceededIcon
-});
-
-const iconClusterRunning = new LabIcon({
-  name: 'launcher:cluster-running-icon',
-  svgstr: clusterRunningIcon
-});
-const iconClusterError = new LabIcon({
-  name: 'launcher:cluster-error-icon',
-  svgstr: clusterErrorIcon
-});
-const iconDelete = new LabIcon({
-  name: 'launcher:delete-icon',
-  svgstr: deleteIcon
+const iconExpandMore = new LabIcon({
+  name: 'launcher:expand-more-icon',
+  svgstr: expandMoreIcon
 });
 
-interface IBatchesList {
-  batchID: string;
-  status: string;
-  location: string;
-  creationTime: string;
-  type: string | undefined;
-  elapsedTime: string;
-  actions: React.JSX.Element;
-}
-
-function ListBatches({ setLoggedIn }: any) {
-  const [detailedBatchView, setDetailedBatchView] = useState(false);
-
-  const [createBatchView, setCreateBatchView] = useState(false);
-
-  const [batchesList, setBatchesList] = useState<IBatchesList[]>([]);
-  const [isLoading, setIsLoading] = useState(true);
-  const [batchSelected, setBatchSelected] = useState('');
-  const [pollingDisable, setPollingDisable] = useState(false);
-  const [deletePopupOpen, setDeletePopupOpen] = useState(false);
-  const [selectedBatch, setSelectedBatch] = useState('');
-  const [regionName, setRegionName] = useState('');
-  const [projectName, setProjectName] = useState('');
-  const timer = useRef<NodeJS.Timeout | undefined>(undefined);
-  const pollingBatches = async (
-    pollingFunction: () => void,
-    pollingDisable: boolean
-  ) => {
-    timer.current = PollingTimer(
-      pollingFunction,
-      pollingDisable,
-      timer.current
-    );
+function ConfigSelection({ loginState, configError, setConfigError }: any) {
+  const Iconsettings = new LabIcon({
+    name: 'launcher:settings_icon',
+    svgstr: settingsIcon
+  });
+
+  const [projectId, setProjectId] = useState('');
+  const [region, setRegion] = useState('');
+  const [regionList, setRegionList] = useState([{}]);
+  const [isLoading, setIsLoading] = useState(false);
+  const [isLoadingUser, setIsLoadingUser] = useState(true);
+  const [isLoadingRegion, setIsLoadingRegion] = useState(true);
+  const [isDropdownOpen, setIsDropdownOpen] = useState(false);
+  const [regionEmpty, SetRegionEmpty] = useState(true);
+  const [isSaveDisabled, setIsSaveDisabled] = useState(true);
+  const [userInfo, setUserInfo] = useState({
+    email: '',
+    picture: ''
+  });
+  const [expandRuntimeTemplate, setExpandRuntimeTemplate] = useState(true);
+  const [openCreateTemplate, setOpenCreateTemplate] = useState(false);
+
+  const [selectedRuntimeClone, setSelectedRuntimeClone] =
+    useState<SessionTemplate>();
+
+  const handleProjectIdChange = (projectId: string) => {
+    setRegionList([]);
+    SetRegionEmpty(true);
+    if (projectId.length !== 0) {
+      regionListAPI(projectId);
+      setProjectId(projectId);
+      setIsSaveDisabled(false);
+    }
   };
-  const data = batchesList;
-  const columns = React.useMemo(
-    () => [
-      {
-        Header: 'Batch ID',
-        accessor: 'batchID'
-      },
-      {
-        Header: 'Status',
-        accessor: 'status'
-      },
-      {
-        Header: 'Location',
-        accessor: 'location'
-      },
-      {
-        Header: 'Creation time',
-        accessor: 'creationTime'
-      },
-      {
-        Header: 'Elapsed time',
-        accessor: 'elapsedTime'
-      },
-      {
-        Header: 'Type',
-        accessor: 'type'
-      },
-      {
-        Header: 'Actions',
-        accessor: 'actions'
-      }
-    ],
-    []
-  );
 
-  const {
-    getTableProps,
-    getTableBodyProps,
-    headerGroups,
-    rows,
-    prepareRow,
-    state,
-    preGlobalFilteredRows,
-    setGlobalFilter,
-    page,
-    canPreviousPage,
-    canNextPage,
-    nextPage,
-    previousPage,
-    setPageSize,
-    state: { pageIndex, pageSize }
-  } = useTable(
-    //@ts-ignore react-table 'columns' which is declared here on type 'TableOptions<ICluster>'
-    { columns, data, autoResetPage: false, initialState: { pageSize: 50 } },
-    useGlobalFilter,
-    usePagination
-  );
-
-  const handleCreateBatchOpen = () => {
-    setCreateBatchView(true);
+  const handleRegionChange = (event: any, data: any) => {
+    setRegion(data.value);
+    if (projectId) {
+      setIsSaveDisabled(false);
+    }
+    setIsDropdownOpen(false);
   };
 
-  const tableDataCondition = (cell: ICellProps) => {
-    if (cell.column.Header === 'Batch ID') {
-      return (
-        <td
-          role="button"
-          {...cell.getCellProps()}
-          className="cluster-name"
-          onClick={() => handleBatchDetails(cell.value)}
-        >
-          {cell.value}
-        </td>
-      );
-    } else if (cell.column.Header === 'Status') {
-      return (
-        <td {...cell.getCellProps()} className="clusters-table-data">
-          <div key="Status" className="cluster-status-parent">
-            {cell.value === STATUS_RUNNING && (
-              <iconClusterRunning.react
-                tag="div"
-                className="logo-alignment-style"
-              />
-            )}
-            {cell.value === STATUS_FAIL && (
-              <iconClusterError.react
-                tag="div"
-                className="logo-alignment-style"
-              />
-            )}
-            {cell.value === STATUS_SUCCESS && (
-              <iconSucceeded.react tag="div" className="logo-alignment-style" />
-            )}
-            {(cell.value === STATUS_PROVISIONING ||
-              cell.value === STATUS_CREATING ||
-              cell.value === STATUS_PENDING ||
-              cell.value === STATUS_DELETING) && (
-              <CircularProgress
-                size={15}
-                aria-label="Loading Spinner"
-                data-testid="loader"
-              />
-            )}
-            <div className="cluster-status">
-              {cell.value && cell.value.toLowerCase()}
-            </div>
-          </div>
-        </td>
-      );
-    } else {
-      return (
-        <td {...cell.getCellProps()} className="clusters-table-data">
-          {cell.render('Cell')}
-        </td>
-      );
+  const handleSave = async () => {
+    setIsLoading(true);
+    setIsSaveDisabled(true);
+    const dataToSend = { projectId: projectId, region: region };
+    try {
+      const data = await requestAPI<any>('configuration', {
+        body: JSON.stringify(dataToSend),
+        method: 'POST'
+      });
+      if (typeof data === 'object' && data !== null) {
+        const configStatus = (data as { config: string }).config;
+        setIsLoading(false);
+        if (configStatus && !toast.isActive('custom-toast')) {
+          const toastifyCustomStyle: ToastOptions<{}> = {
+            hideProgressBar: true,
+            autoClose: false,
+            theme: 'dark',
+            position: toast.POSITION.BOTTOM_CENTER,
+            toastId: 'custom-toast'
+          };
+          if (configStatus.includes('Failed')) {
+            toast.error(configStatus, toastifyCustomStyle);
+          } else {
+            toast.success(
+              `${configStatus} - You will need to restart Jupyter in order for the new project and region to fully take effect.`,
+              toastifyCustomStyle
+            );
+          }
+        }
+      }
+    } catch (reason) {
+      console.error(`Error on POST {dataToSend}.\n${reason}`);
     }
   };
 
-  interface IBatchData {
-    name: string;
-    state: BatchStatus;
-    createTime: string;
-    stateTime: Date;
-  }
-
-  const listBatchAPI = async () => {
-    await BatchService.listBatchAPIService(
-      setRegionName,
-      setProjectName,
-      renderActions,
-      setBatchesList,
-      setIsLoading,
-      setLoggedIn
-    );
+  const displayUserInfo = async () => {
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(USER_INFO_URL, {
+        method: 'GET',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      })
+        .then((response: any) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              setUserInfo(responseResult);
+              setIsLoadingUser(false);
+            })
+            .catch((e: any) => console.log(e));
+        })
+        .catch((err: any) => {
+          setIsLoadingUser(false);
+          console.error('Error displaying user info', err);
+          toast.error('Failed to fetch user information');
+        });
+    }
   };
 
-  const handleBatchDetails = (selectedName: string) => {
-    pollingBatches(listBatchAPI, true);
-    setBatchSelected(selectedName);
-    setDetailedBatchView(true);
-  };
-  const handleDeleteBatch = (data: IBatchData) => {
-    if (data.state !== BatchStatus.STATUS_PENDING) {
-      /*
-      Extracting project id
-      Example: "projects/{project}/locations/{location}/batches/{batch_id}"
-      */
-      setSelectedBatch(data.name.split('/')[5]);
-      setDeletePopupOpen(true);
+  const regionListAPI = async (projectId: any) => {
+    try {
+      const credentials = await authApi();
+      if (credentials) {
+        fetch(`${REGION_URL}${projectId}/regions`, {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        })
+          .then((response: any) => {
+            if (response.ok) {
+              SetRegionEmpty(true);
+              return response.json();
+            } else {
+              setIsDropdownOpen(false);
+              setIsSaveDisabled(true);
+              SetRegionEmpty(false);
+              if (!toast.isActive('custom-toast-error')) {
+                toast.error(response.status + ' Permission Denied', {
+                  position: toast.POSITION.BOTTOM_CENTER,
+                  toastId: 'custom-toast-error'
+                });
+              }
+              throw new Error(`Request failed with status ${response.status}`);
+            }
+          })
+          .then((responseResult: any) => {
+            let transformedRegionList = [];
+            transformedRegionList = responseResult.items.map((data: any) => {
+              return {
+                value: data.name,
+                key: data.name,
+                text: data.name
+              };
+            });
+            setRegionList(transformedRegionList);
+            setIsDropdownOpen(false);
+            SetRegionEmpty(false);
+            setIsLoadingRegion(false);
+          })
+          .catch((error: any) => {
+            setIsLoadingRegion(false);
+            console.error('Error fetching region list:', error.message);
+          });
+      }
+    } catch (error) {
+      setIsLoadingRegion(false);
+      console.error('Error fetching region list:');
+      toast.error('Failed to fetch the regions');
     }
   };
-  const handleCancelDelete = () => {
-    setDeletePopupOpen(false);
+  const handleDropdownOpen = () => {
+    if (regionEmpty) {
+      setIsDropdownOpen(true);
+    }
   };
 
-  const handleDelete = async () => {
-    await BatchService.deleteBatchAPIService(selectedBatch);
-    listBatchAPI();
-    setDetailedBatchView(false);
-    setDeletePopupOpen(false);
+  /**
+   * onClick handler for when user's click on the "license" link in
+   * the user info box.
+   */
+  const handleLicenseClick = async () => {
+    const licenseWindow = window.open('about:blank');
+    if (licenseWindow) {
+      const preEle = licenseWindow.document.createElement('pre');
+      preEle.textContent = THIRD_PARTY_LICENSES;
+      licenseWindow.document.body.appendChild(preEle);
+    }
   };
 
-  const renderActions = (data: IBatchData) => {
-    return (
-      <div
-        className="actions-icon"
-        role="button"
-        aria-label="Delete Job"
-        aria-disabled={data.state === BatchStatus.STATUS_PENDING}
-      >
-        <div
-          className={
-            data.state === BatchStatus.STATUS_PENDING
-              ? 'icon-buttons-style-delete-batch-disable'
-              : 'icon-buttons-style-delete-batch'
-          }
-          title="Delete Batch"
-          onClick={() => handleDeleteBatch(data)}
-        >
-          {data.state === BatchStatus.STATUS_PENDING ? (
-            <iconDelete.react
-              tag="div"
-              className="icon-white logo-alignment-style icon-delete"
-            />
-          ) : (
-            <iconDelete.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
-          )}
-        </div>
-      </div>
-    );
+  const fetchProjectRegion = async () => {
+    const credentials = await authApi();
+    if (credentials && credentials.project_id && credentials.region_id) {
+      handleProjectIdChange(credentials.project_id);
+      setProjectId(credentials.project_id);
+      setRegion(credentials.region_id);
+      setConfigError(false);
+    } else if (credentials && credentials.config_error === 1) {
+      setConfigError(true);
+    }
   };
 
-  useEffect(() => {
-    if (!pollingDisable) {
-      listBatchAPI();
-    }
+  const handleRuntimeExpand = () => {
+    let runTimeMode = !expandRuntimeTemplate;
+    setExpandRuntimeTemplate(runTimeMode);
+  };
 
-    return () => {
-      pollingBatches(listBatchAPI, true);
-    };
-  }, [pollingDisable, detailedBatchView]);
   useEffect(() => {
-    if (!detailedBatchView && !isLoading) {
-      pollingBatches(listBatchAPI, pollingDisable);
+    if (loginState) {
+      fetchProjectRegion();
+      displayUserInfo();
+    } else {
+      displayUserInfo();
     }
-  }, [isLoading]);
-
+    setSelectedRuntimeClone(undefined);
+  }, []);
   return (
     <div>
-      {deletePopupOpen && (
-        <DeletePopup
-          onCancel={() => handleCancelDelete()}
-          onDelete={() => handleDelete()}
-          deletePopupOpen={deletePopupOpen}
-          DeleteMsg={
-            'This will delete ' + selectedBatch + ' and cannot be undone.'
-          }
-        />
-      )}
-      {detailedBatchView && (
-        <BatchDetails
-          batchSelected={batchSelected}
-          setDetailedBatchView={setDetailedBatchView}
-          setCreateBatchView={setCreateBatchView}
-        />
-      )}
-      {createBatchView && (
-        <CreateBatch
-          setCreateBatchView={setCreateBatchView}
-          regionName={regionName}
-          projectName={projectName}
+      <ToastContainer />
+      {isLoadingUser && isLoadingRegion && !configError ? (
+        <div className="spin-loaderMain">
+          <ClipLoader
+            color="#8A8A8A"
+            loading={true}
+            size={20}
+            aria-label="Loading Spinner"
+            data-testid="loader"
+          />
+          Loading Config Setup
+        </div>
+      ) : !configError && openCreateTemplate ? (
+        <CreateRuntime
+          setOpenCreateTemplate={setOpenCreateTemplate}
+          selectedRuntimeClone={selectedRuntimeClone}
         />
-      )}
+      ) : (
+        <div className="settings-component">
+          <div className="settings-overlay">
+            <div>
+              <Iconsettings.react tag="div" />
+            </div>
+            <div className="settings-text">Settings</div>
+          </div>
+          <div className="settings-seperator"></div>
+          <div className="config-overlay">
+            <div className="config-form">
+              <div className="project-overlay">
+                <label className="project-text" htmlFor="project-id">
+                  Project ID
+                </label>
+                <ProjectIDDropdown
+                  projectId={projectId}
+                  onProjectIdChange={handleProjectIdChange}
+                />
+              </div>
 
-      {!detailedBatchView && !createBatchView && (
-        <>
-          <div className="create-batch-wrapper ">
-            <div
-              className="create-batch-overlay"
-              onClick={() => {
-                handleCreateBatchOpen();
-              }}
-            >
-              <div className="create-icon">
-                <iconSubmitJob.react
-                  tag="div"
-                  className="logo-alignment-style"
+              <div className="region-overlay">
+                <label className="region-text" htmlFor="region-id">
+                  Region
+                </label>
+
+                <Select
+                  search
+                  onClick={handleDropdownOpen}
+                  placeholder={region}
+                  className="region-select"
+                  value={region}
+                  onChange={handleRegionChange}
+                  options={regionList}
+                  isDisabled={isDropdownOpen}
                 />
               </div>
-              <div className="create-text">Create Batch</div>
+              <div className="save-overlay">
+                <button
+                  className={
+                    isSaveDisabled ? 'save-button disabled' : 'save-button'
+                  }
+                  disabled={isSaveDisabled}
+                  onClick={handleSave}
+                >
+                  Save
+                </button>
+                {isLoading && (
+                  <div className="save-loader">
+                    <ClipLoader
+                      loading={true}
+                      size={25}
+                      aria-label="Loading Spinner"
+                      data-testid="loader"
+                    />
+                  </div>
+                )}
+              </div>
             </div>
-          </div>
-
-          {batchesList.length > 0 && !createBatchView ? (
-            <div>
-              <div className="filter-cluster-overlay">
-                <div className="filter-cluster-icon">
-                  <iconFilter.react
-                    tag="div"
-                    className="icon-white logo-alignment-style"
+            {isDropdownOpen && (
+              <div className="region-loader">
+                <ClipLoader
+                  loading={true}
+                  size={15}
+                  aria-label="Loading Spinner"
+                  data-testid="loader"
+                />
+              </div>
+            )}
+            <div className="user-info-card">
+              <div className="google-header">
+                This account is managed by google.com
+              </div>
+              <div className="seperator"></div>
+              <div className="user-overlay">
+                <div className="user-image-overlay">
+                  <img
+                    src={userInfo.picture}
+                    alt="User Image"
+                    className="user-image"
                   />
                 </div>
-                <div className="filter-cluster-text"></div>
-                <div className="filter-cluster-section">
-                  <GlobalFilter
-                    preGlobalFilteredRows={preGlobalFilteredRows}
-                    globalFilter={state.globalFilter}
-                    setGlobalFilter={setGlobalFilter}
-                    setPollingDisable={setPollingDisable}
-                  />
+                <div className="user-details">
+                  <div className="user-email">{userInfo.email}</div>
                 </div>
               </div>
-              <div className="clusters-list-table-parent">
-                <TableData
-                  getTableProps={getTableProps}
-                  headerGroups={headerGroups}
-                  getTableBodyProps={getTableBodyProps}
-                  isLoading={isLoading}
-                  rows={rows}
-                  page={page}
-                  prepareRow={prepareRow}
-                  tableDataCondition={tableDataCondition}
-                  fromPage="Batches"
-                />
-                {batchesList.length > 50 && (
-                  <PaginationView
-                    pageSize={pageSize}
-                    setPageSize={setPageSize}
-                    pageIndex={pageIndex}
-                    allData={batchesList}
-                    previousPage={previousPage}
-                    nextPage={nextPage}
-                    canPreviousPage={canPreviousPage}
-                    canNextPage={canNextPage}
-                  />
-                )}
+              <div className="seperator"></div>
+              <div className="google-header">
+                <a
+                  href="https://policies.google.com/privacy?hl=en"
+                  target="_blank"
+                  rel="noopener noreferrer"
+                >
+                  Privacy Policy
+                </a>
+                <span className="privacy-terms"> • </span>
+                <a
+                  href="https://policies.google.com/terms?hl=en"
+                  target="_blank"
+                  rel="noopener noreferrer"
+                >
+                  Terms of Service
+                </a>
+                <span className="footer-divider"> • </span>
+                <a onClick={handleLicenseClick} href="#">
+                  Licenses
+                </a>
               </div>
             </div>
-          ) : (
-            <div>
-              {isLoading && (
-                <div className="spin-loader-main">
-                  <CircularProgress
-                    className = "spin-loader-custom-style"
-                    size={18}
-                    aria-label="Loading Spinner"
-                    data-testid="loader"
-                  />
-                  Loading Batches
-                </div>
-              )}
-              {!isLoading && (
-                <div className="no-data-style">No rows to display</div>
-              )}
+          </div>
+          <div>
+            <div className="runtime-title-section">
+              <div className="runtime-title-part">
+                Serverless Runtime Templates
+              </div>
+              <div
+                className="expand-icon"
+                onClick={() => handleRuntimeExpand()}
+              >
+                {expandRuntimeTemplate ? (
+                  <iconExpandLess.react tag="div" />
+                ) : (
+                  <iconExpandMore.react tag="div" />
+                )}
+              </div>
             </div>
-          )}
-        </>
+            {expandRuntimeTemplate && (
+              <ListRuntimeTemplates
+                openCreateTemplate={openCreateTemplate}
+                setOpenCreateTemplate={setOpenCreateTemplate}
+                setSelectedRuntimeClone={setSelectedRuntimeClone}
+              />
+            )}
+          </div>
+        </div>
       )}
     </div>
   );
 }
 
-export default ListBatches;
+export default ConfigSelection;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryTableInfo.tsx` & `dataproc_jupyter_plugin-0.1.9/src/utils/tableData.tsx`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,81 @@
 /**
  * @license
- * Copyright 2024 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *   http://www.apache.org/licenses/LICENSE-2.0
  *
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-import React, { useEffect, useState } from 'react';
-import { BigQueryService } from './bigQueryService';
-import { CircularProgress } from '@mui/material';
-
-const BigQueryTableInfo = ({
-  title,
-  dataset,
-  projectId
-}: {
-  title: string;
-  dataset: string;
-  projectId: string;
-}) => {
-  const [datasetInfo, setDatasetInfo] = useState<any>({});
-  const [tableInfo, setTableInfo] = useState<any>({});
-  const [isLoading, setIsLoading] = useState(true);
-
-  useEffect(() => {
-    BigQueryService.getBigQueryDatasetInfoAPIService(
-      dataset,
-      projectId,
-      setDatasetInfo
-    );
-  }, []);
-
-  useEffect(() => {
-    BigQueryService.getBigQueryTableInfoAPIService(
-      title,
-      dataset,
-      setTableInfo,
-      datasetInfo,
-      projectId,
-      setIsLoading
-    );
-  }, [datasetInfo]);
+import React from 'react';
+import { ClipLoader } from 'react-spinners';
 
+function TableData({
+  getTableProps,
+  headerGroups,
+  getTableBodyProps,
+  isLoading,
+  rows,
+  page,
+  prepareRow,
+  tableDataCondition,
+  fromPage
+}: any) {
+  const displayData = page ? page: rows
   return (
-    <>
-      {isLoading ? (
-        <div className="database-loader">
-          <div>
-            <CircularProgress
-              className = "spin-loader-custom-style"
-              size={20}
+    <table {...getTableProps()} className="clusters-list-table">
+      <thead>
+        {headerGroups.map((headerGroup: any) => (
+          <tr
+            {...headerGroup.getHeaderGroupProps()}
+            className="cluster-list-table-header"
+          >
+            {headerGroup.headers.map((column: any) => (
+              <th
+                {...column.getHeaderProps()}
+                className="clusters-table-header"
+              >
+                {column.render('Header')}
+              </th>
+            ))}
+          </tr>
+        ))}
+      </thead>
+      <tbody {...getTableBodyProps()} className="clusters-table-body">
+        {isLoading ? (
+          <div className="spin-loader">
+            <ClipLoader
+              color="#8A8A8A"
+              loading={true}
+              size={18}
               aria-label="Loading Spinner"
               data-testid="loader"
             />
+            Loading {fromPage}
           </div>
-          Loading table details
-        </div>
-      ) : (
-        <>
-          <div className="db-title">Table info</div>
-          <div className="table-container">
-            <table className="db-table">
-              <tbody>
-                {Object.keys(tableInfo).map((tableData, index) => (
-                  <tr key={index} className="tr-row">
-                    <td className="bold-column">{tableData}</td>
-                    <td>{tableInfo[tableData]}</td>
-                  </tr>
-                ))}
-              </tbody>
-            </table>
-          </div>
-        </>
-      )}
-    </>
+        ) : (
+          displayData.map((row: any) => {
+            prepareRow(row);
+            return (
+              <tr {...row.getRowProps()} className="cluster-list-data-parent">
+                {row.cells.map((cell: any) => {
+                  return tableDataCondition(cell);
+                })}
+              </tr>
+            );
+          })
+        )}
+      </tbody>
+    </table>
   );
-};
+}
 
-export default BigQueryTableInfo;
+export default TableData;
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/bigQuery/bigQueryWidget.tsx` & `dataproc_jupyter_plugin-0.1.9/src/dpms/dpmsWidget.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,896 +1,722 @@
 /**
  * @license
- * Copyright 2024 Google LLC
+ * Copyright 2023 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *   http://www.apache.org/licenses/LICENSE-2.0
  *
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
+import { ReactWidget } from '@jupyterlab/apputils';
 import { JupyterLab } from '@jupyterlab/application';
 import React, { useEffect, useState } from 'react';
-import { Tree, NodeRendererProps, NodeApi } from 'react-arborist';
+import { Tree, NodeRendererProps } from 'react-arborist';
 import { LabIcon } from '@jupyterlab/ui-components';
-import bigQueryProjectIcon from '../../style/icons/bigquery_project_icon.svg';
-import datasetIcon from '../../style/icons/dataset_icon.svg';
+import databaseIcon from '../../style/icons/database_icon.svg';
 import tableIcon from '../../style/icons/table_icon.svg';
 import columnsIcon from '../../style/icons/columns_icon.svg';
+import refreshIcon from '../../style/icons/refresh_icon.svg';
 import databaseWidgetIcon from '../../style/icons/database_widget_icon.svg';
 import datasetsIcon from '../../style/icons/datasets_icon.svg';
 import searchIcon from '../../style/icons/search_icon.svg';
 import rightArrowIcon from '../../style/icons/right_arrow_icon.svg';
 import downArrowIcon from '../../style/icons/down_arrow_icon.svg';
 import searchClearIcon from '../../style/icons/search_clear_icon.svg';
+import { Database } from './databaseInfo';
 import { MainAreaWidget } from '@jupyterlab/apputils';
 import { v4 as uuidv4 } from 'uuid';
+import 'semantic-ui-css/semantic.min.css';
 import { auto } from '@popperjs/core';
-import { IThemeManager } from '@jupyterlab/apputils';
 import {
-  CircularProgress,
-  IconButton,
-  InputAdornment,
-  TextField
-} from '@mui/material';
-import { TitleComponent } from '../controls/SidePanelTitleWidget';
-import { BigQueryService } from './bigQueryService';
-import { ISettingRegistry } from '@jupyterlab/settingregistry';
-import { BigQueryDatasetWrapper } from './bigQueryDatasetInfoWrapper';
-import { BigQueryTableWrapper } from './bigQueryTableInfoWrapper';
-import { DataprocWidget } from '../controls/DataprocWidget';
-import { handleDebounce } from '../utils/utils';
-
+  BASE_URL,
+  API_HEADER_CONTENT_TYPE,
+  API_HEADER_BEARER,
+  CATALOG_SEARCH,
+  COLUMN_API,
+  QUERY_DATABASE,
+  QUERY_TABLE
+} from '../utils/const';
+import { authApi } from '../utils/utils';
+import { Table } from './tableInfo';
+import { ClipLoader } from 'react-spinners';
+import { ToastContainer, toast } from 'react-toastify';
+
+const iconDatabase = new LabIcon({
+  name: 'launcher:database-icon',
+  svgstr: databaseIcon
+});
+const iconTable = new LabIcon({
+  name: 'launcher:table-icon',
+  svgstr: tableIcon
+});
+const iconColumns = new LabIcon({
+  name: 'launcher:columns-icon',
+  svgstr: columnsIcon
+});
 const iconDatasets = new LabIcon({
   name: 'launcher:datasets-icon',
   svgstr: datasetsIcon
 });
 const iconDatabaseWidget = new LabIcon({
   name: 'launcher:databse-widget-icon',
   svgstr: databaseWidgetIcon
 });
+const iconRefresh = new LabIcon({
+  name: 'launcher:refresh-icon',
+  svgstr: refreshIcon
+});
+const iconSearch = new LabIcon({
+  name: 'launcher:search-icon',
+  svgstr: searchIcon
+});
 const iconRightArrow = new LabIcon({
   name: 'launcher:right-arrow-icon',
   svgstr: rightArrowIcon
 });
 const iconDownArrow = new LabIcon({
   name: 'launcher:down-arrow-icon',
   svgstr: downArrowIcon
 });
-const calculateDepth = (node: NodeApi): number => {
+const iconSearchClear = new LabIcon({
+  name: 'launcher:search-clear-icon',
+  svgstr: searchClearIcon
+});
+
+const calculateDepth = (node: any): number => {
   let depth = 0;
   let currentNode = node;
   while (currentNode.parent) {
     depth++;
     currentNode = currentNode.parent;
   }
   return depth;
 };
 
-let timeoutId: NodeJS.Timeout | null = null; // Define timeoutId
-
-const debounce = (func: Function, delay: number) => {
-  return (...args: any) => {
-    clearTimeout(timeoutId as NodeJS.Timeout); // Clear the timeout
-    timeoutId = setTimeout(() => {
-      func(...args);
-    }, delay);
-  };
-};
-
-const BigQueryComponent = ({
-  app,
-  settingRegistry,
-  themeManager
-}: {
-  app: JupyterLab;
-  settingRegistry: ISettingRegistry;
-  themeManager: IThemeManager;
-}): JSX.Element => {
-  const iconSearchClear = new LabIcon({
-    name: 'launcher:search-clear-icon',
-    svgstr: searchClearIcon
-  });
-  const iconBigQueryProject = new LabIcon({
-    name: 'launcher:bigquery-project-icon',
-    svgstr: bigQueryProjectIcon
-  });
-  const iconDataset = new LabIcon({
-    name: 'launcher:dataset-icon',
-    svgstr: datasetIcon
-  });
-  const iconTable = new LabIcon({
-    name: 'launcher:table-icon',
-    svgstr: tableIcon
-  });
-
-  const iconColumns = new LabIcon({
-    name: 'launcher:columns-icon',
-    svgstr: columnsIcon
-  });
-  const iconSearch = new LabIcon({
-    name: 'launcher:search-icon',
-    svgstr: searchIcon
-  });
-
-  const [projectNameInfo, setProjectNameInfo] = useState<string[]>([]);
+const DpmsComponent = ({ app }: { app: JupyterLab }): JSX.Element => {
   const [searchTerm, setSearchTerm] = useState('');
   const [notebookValue, setNotebookValue] = useState<string>('');
   const [dataprocMetastoreServices, setDataprocMetastoreServices] =
     useState('');
   const [isLoading, setIsLoading] = useState(true);
-  const [databaseNames, setDatabaseNames] = useState<string[]>([]);
-
-  const [dataSetResponse, setDataSetResponse] = useState<any>();
-  const [tableResponse, setTableResponse] = useState<any>();
-  const [schemaResponse, setSchemaResponse] = useState<any>();
-
-  const [treeStructureData, setTreeStructureData] = useState<any>([]);
-
-  const [currentNode, setCurrentNode] = useState<any>();
-  const [isIconLoading, setIsIconLoading] = useState(false);
-
-  const [searchResponse, setSearchResponse] = useState<any>([]);
-  const [searchLoading, setSearchLoading] = useState(false);
-
-  const [height, setHeight] = useState(window.innerHeight - 125);
-
-  function handleUpdateHeight() {
-    let updateHeight = window.innerHeight - 125;
-    setHeight(updateHeight);
-  }
-
-  // Debounce the handleUpdateHeight function
-  const debouncedHandleUpdateHeight = handleDebounce(handleUpdateHeight, 500);
-
-  // Add event listener for window resize using useEffect
-  useEffect(() => {
-    window.addEventListener('resize', debouncedHandleUpdateHeight);
-
-    // Cleanup function to remove event listener on component unmount
-    return () => {
-      window.removeEventListener('resize', debouncedHandleUpdateHeight);
-    };
-  }, []);
-
-  const getBigQueryColumnDetails = async (
-    tableId: string,
-    datasetId: string,
-    projectId: string | undefined
-  ) => {
-    if (tableId && datasetId && projectId) {
-      await BigQueryService.getBigQueryColumnDetailsAPIService(
-        datasetId,
-        tableId,
-        projectId,
-        setIsIconLoading,
-        setSchemaResponse
-      );
-    }
-  };
-
-  interface IDataEntry {
-    id: string;
-    name: string;
-    type: string;
-    description: string;
-    children: any;
-  }
-
-  const treeStructureforProjects = () => {
-    const data = projectNameInfo.map(projectName => ({
-      id: uuidv4(),
-      name: projectName,
-      children: []
-    }));
-
-    data.sort((a, b) => a.name.localeCompare(b.name));
-
-    setTreeStructureData(data);
-  };
-
-  const treeStructureforDatasets = () => {
-    let tempData = [...treeStructureData];
-
-    tempData.forEach((projectData: any) => {
-      if (projectData.name === currentNode.data.name) {
-        projectData['children'] = databaseNames.map(datasetName => ({
-          id: uuidv4(),
-          name: datasetName,
-          children: []
-        }));
-      }
-    });
-
-    tempData.sort((a, b) => a.name.localeCompare(b.name));
-
-    tempData.forEach(db => {
-      db.children.sort((a: any, b: any) => a.name.localeCompare(b.name));
-    });
-
-    setTreeStructureData(tempData);
-  };
-
-  const treeStructureforTables = () => {
-    let tempData = [...treeStructureData];
-
-    tempData.forEach((projectData: any) => {
-      if (projectData.name === currentNode.parent.data.name) {
-        projectData.children.forEach((dataset: any) => {
-          if (tableResponse.length > 0 && tableResponse[0].tableReference) {
-            if (dataset.name === tableResponse[0].tableReference.datasetId) {
-              dataset['children'] = tableResponse.map((tableDetails: any) => ({
-                id: uuidv4(),
-                name: tableDetails.tableReference.tableId,
-                children: []
-              }));
-            }
-          } else {
-            if (dataset.name === tableResponse) {
-              dataset['children'] = false;
-            }
-          }
-        });
-      }
-    });
-
-    setTreeStructureData(tempData);
-  };
-
-  const treeStructureforSchema = () => {
-    let tempData = [...treeStructureData];
-
-    tempData.forEach((projectData: any) => {
-      if (projectData.name === currentNode.parent.parent.data.name) {
-        projectData.children.forEach((dataset: any) => {
-          if (dataset.name === schemaResponse.tableReference.datasetId) {
-            dataset.children.forEach((table: any) => {
-              if (table.name === schemaResponse.tableReference.tableId) {
-                if (schemaResponse.schema?.fields) {
-                  table['children'] = schemaResponse.schema?.fields.map(
-                    (column: any) => ({
-                      id: uuidv4(),
-                      name: column.name,
-                      type: column.type,
-                      mode: column.mode,
-                      key: column.key,
-                      collation: column.collation,
-                      defaultValue: column.defaultValue,
-                      policyTags: column.policyTags,
-                      dataPolicies: column.dataPolicies,
-                      tableDescription: column.tableDescription,
-                      description: column.description
-                    })
-                  );
-                } else {
-                  table['children'] = false;
-                }
+  const [noDpmsInstance, setNoDpmsInstance] = useState(false);
+  const [session, setSession] = useState(false);
+  const [cluster, setCluster] = useState(false);
+  const [entries, setEntries] = useState<string[]>([]);
+  const [columnResponse, setColumnResponse] = useState<string[]>([]);
+  const [databaseDetails, setDatabaseDetails] = useState({});
+  const [tableDescription, setTableDescription] = useState({});
+  const getColumnDetails = async (name: string) => {
+    const credentials = await authApi();
+    if (credentials && notebookValue) {
+      fetch(`${COLUMN_API}${name}`, {
+        method: 'GET',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token,
+          'X-Goog-User-Project': credentials.project_id || ''
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then(async (responseResult: unknown) => {
+              setColumnResponse((prevResponse: any) => [
+                ...prevResponse,
+                responseResult
+              ]);
+              if (data) {
+                setIsLoading(false);
               }
+            })
+            .catch((e: Error) => {
+              console.log(e);
             });
-          }
+        })
+        .catch((err: Error) => {
+          console.error('Error getting column details', err);
+          toast.error('Error getting column details');
         });
-      }
-    });
-    setTreeStructureData(tempData);
+    }
   };
-
-  const handleSearchTreeStructure = () => {
-    if (
-      searchResponse &&
-      searchResponse.results &&
-      searchResponse.results.length > 0
-    ) {
-      let data: any = [];
-      searchResponse.results.forEach((searchData: any) => {
-        let tempData = [...data];
-        //first time data is empty
-        if (tempData.length === 0) {
-          tempData.push({
-            id: uuidv4(),
-            name: searchData.linkedResource.split('/')[4],
-            children: [
-              {
-                id: uuidv4(),
-                name: searchData.linkedResource.split('/')[6],
-                children: searchData.linkedResource.split('/')[8]
-                  ? [
-                      {
-                        id: uuidv4(),
-                        name: searchData.linkedResource.split('/')[8],
-                        children: []
-                      }
-                    ]
-                  : []
-              }
-            ]
-          });
-        } else {
-          //To check if project is already exist or not
-          let projectDataAlreadyExist = tempData.filter(projectData => {
-            return projectData.name === searchData.linkedResource.split('/')[4];
-          });
-          //if project is already exist
-          if (projectDataAlreadyExist.length !== 0) {
-            tempData.forEach((projectData: any) => {
-              if (
-                projectData.name === searchData.linkedResource.split('/')[4]
-              ) {
-                //To check if dataset is already exist or not
-                let datasetDataAlreadyExist = projectData['children'].filter(
-                  (datasetData: any) => {
-                    return (
-                      datasetData.name ===
-                      searchData.linkedResource.split('/')[6]
-                    );
-                  }
-                );
-                //if dataset is already exist
-                if (datasetDataAlreadyExist.length !== 0) {
-                  projectData['children'].forEach((datasetData: any) => {
-                    if (
-                      datasetData.name ===
-                        searchData.linkedResource.split('/')[6] &&
-                      projectData.name ===
-                        searchData.linkedResource.split('/')[4]
-                    ) {
-                      if (searchData.linkedResource.split('/')[8]) {
-                        datasetData['children'].push({
-                          id: uuidv4(),
-                          name: searchData.linkedResource.split('/')[8],
-                          children: []
-                        });
-                      }
-                    }
-                  });
-                } else {
-                  //if dataset is not exist
-                  projectData['children'].push({
-                    id: uuidv4(),
-                    name: searchData.linkedResource.split('/')[6],
-                    children: searchData.linkedResource.split('/')[8]
-                      ? [
-                          {
-                            id: uuidv4(),
-                            name: searchData.linkedResource.split('/')[8],
-                            children: []
-                          }
-                        ]
-                      : []
-                  });
-                }
-              }
-            });
-          }
-          //if project is not exist
-          else {
-            tempData.push({
-              id: uuidv4(),
-              name: searchData.linkedResource.split('/')[4],
-              children: [
-                {
-                  id: uuidv4(),
-                  name: searchData.linkedResource.split('/')[6],
-                  children: searchData.linkedResource.split('/')[8]
-                    ? [
-                        {
-                          id: uuidv4(),
-                          name: searchData.linkedResource.split('/')[8],
-                          children: []
-                        }
-                      ]
-                    : []
+  const getTableDetails = async (database: string) => {
+    const credentials = await authApi();
+    if (credentials && notebookValue) {
+      const requestBody = {
+        query: `${QUERY_TABLE}${credentials.project_id}.${credentials.region_id}.${dataprocMetastoreServices}.${database}`,
+        scope: {
+          includeProjectIds: [credentials.project_id]
+        }
+      };
+      fetch(`${CATALOG_SEARCH}`, {
+        method: 'POST',
+        body: JSON.stringify(requestBody),
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token,
+          'X-Goog-User-Project': credentials.project_id || ''
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              const filteredEntries = responseResult.results.filter(
+                (entry: { displayName: string }) => entry.displayName
+              );
+              const tableNames: string[] = [];
+              const entryNames: string[] = [];
+              const updatedTableDetails: { [key: string]: string } = {};
+              filteredEntries.forEach(
+                (entry: {
+                  displayName: string;
+                  relativeResourceName: string;
+                  description: string;
+                }) => {
+                  tableNames.push(entry.displayName);
+                  entryNames.push(entry.relativeResourceName);
+                  const description = entry.description || 'None';
+                  updatedTableDetails[entry.displayName] = description;
                 }
-              ]
+              );
+              setEntries(entryNames);
+              setTableDescription(updatedTableDetails);
+            })
+            .catch((e: Error) => {
+              console.log(e);
             });
-          }
-        }
-        data = tempData;
-      });
-      setTreeStructureData(data);
+        })
+        .catch((err: Error) => {
+          console.error('Error getting table details', err);
+          toast.error('Error getting table details');
+        });
     }
   };
+  const database: { [dbName: string]: { [tableName: string]: string[] } } = {};
+  columnResponse.forEach((res: any) => {
+    /* fullyQualifiedName : dataproc_metastore:projectId.location.metastore_instance.database_name.table_name
+fetching database name from fully qualified name structure */
+    const dbName = res.fullyQualifiedName.split('.').slice(-2, -1)[0];
+    const tableName = res.displayName;
+    const columns = res.schema.columns.map(
+      (column: {
+        column: string;
+        type: string;
+        mode: string;
+        description: string;
+      }) => ({
+        name: column.column,
+        type: column.type.toUpperCase(),
+        mode: column.mode,
+        description: column?.description || 'None'
+      })
+    );
 
-  const handleSearch = (value: string) => {
-    if (value !== '') {
-      BigQueryService.getBigQuerySearchAPIService(
-        value,
-        setSearchLoading,
-        setSearchResponse
-      );
-    } else {
-      getBigQueryProjects();
+    if (!database[dbName]) {
+      database[dbName] = {};
     }
-  };
 
-  const debouncedHandleSearch = debounce(handleSearch, 500);
+    if (!database[dbName][tableName]) {
+      database[dbName][tableName] = [];
+    }
 
-  const handleSearchTerm = (event: React.ChangeEvent<HTMLInputElement>) => {
+    database[dbName][tableName].push(...columns);
+  });
+  const data = Object.entries(database).map(([dbName, tables]) => ({
+    id: uuidv4(),
+    name: dbName,
+    children: Object.entries(tables).map(([tableName, columns]) => ({
+      id: uuidv4(),
+      name: tableName,
+      desciption: '',
+      children: columns.map((column: any) => ({
+        id: uuidv4(),
+        name: column.name,
+        type: column.type,
+        mode: column.mode,
+        description: column.description
+      }))
+    }))
+  }));
+  data.sort((a, b) => a.name.localeCompare(b.name));
+
+  data.forEach(db => {
+    db.children.sort((a, b) => a.name.localeCompare(b.name));
+    db.children.forEach(table => {
+      table.children.sort((a, b) => a.name.localeCompare(b.name));
+    });
+  });
+
+  const handleSearch = (event: React.ChangeEvent<HTMLInputElement>) => {
     setSearchTerm(event.target.value);
-    debouncedHandleSearch(event.target.value);
   };
-
-  const openedWidgets: Record<string, boolean> = {};
-  const handleNodeClick = (node: NodeApi) => {
+  const searchMatch = (node: { data: { name: string } }, term: string) => {
+    return node.data.name.toLowerCase().includes(term.toLowerCase());
+  };
+  const openedWidgets: string[] = [];
+  const handleNodeClick = (node: any) => {
     const depth = calculateDepth(node);
     const widgetTitle = node.data.name;
     if (!openedWidgets[widgetTitle]) {
-      if (depth === 2) {
-        const content = new BigQueryDatasetWrapper(
+      if (depth === 1) {
+        const content = new Database(
           node.data.name,
-          node?.parent?.data?.name,
-          themeManager
+          dataprocMetastoreServices,
+          databaseDetails
         );
-        const widget = new MainAreaWidget<BigQueryDatasetWrapper>({ content });
+        const widget = new MainAreaWidget<Database>({ content });
         const widgetId = 'node-widget-db';
         widget.id = widgetId;
         widget.title.label = node.data.name;
         widget.title.closable = true;
         widget.title.icon = iconDatabaseWidget;
         app.shell.add(widget, 'main');
-        widget.disposed.connect(() => {
-          const widgetTitle = widget.title.label;
-          delete openedWidgets[widgetTitle];
-        });
-      } else if (depth === 3 && node.parent && node.parent.parent) {
+      } else if (depth === 2) {
         const database = node.parent.data.name;
-        const projectId = node.parent.parent.data.name;
-
-        const content = new BigQueryTableWrapper(
+        const column = node.data.children;
+        const content = new Table(
           node.data.name,
+          dataprocMetastoreServices,
           database,
-          projectId,
-          themeManager
+          column,
+          tableDescription
         );
-        const widget = new MainAreaWidget<BigQueryTableWrapper>({ content });
+        const widget = new MainAreaWidget<Table>({ content });
         const widgetId = `node-widget-${uuidv4()}`;
         widget.id = widgetId;
         widget.title.label = node.data.name;
         widget.title.closable = true;
         widget.title.icon = iconDatasets;
         app.shell.add(widget, 'main');
-        widget.disposed.connect(() => {
-          const widgetTitle = widget.title.label;
-          delete openedWidgets[widgetTitle];
-        });
       }
       openedWidgets[widgetTitle] = node.data.name;
     }
   };
+  const clearState = () => {
+    setSearchTerm('');
+    setNotebookValue('');
+    setDataprocMetastoreServices('');
+    setIsLoading(true);
+    setEntries([]);
+    setColumnResponse([]);
+    setDatabaseDetails({});
+  };
+  const handleRefreshClick = () => {
+    clearState();
+    setIsLoading(true);
+    getActiveNotebook();
+  };
   const handleSearchClear = () => {
     setSearchTerm('');
-    getBigQueryProjects();
   };
-  type NodeProps = NodeRendererProps<IDataEntry> & {
-    onClick: (node: NodeRendererProps<IDataEntry>['node']) => void;
+  type NodeProps = NodeRendererProps<any> & {
+    onClick: (node: any) => void;
   };
   const Node = ({ node, style, onClick }: NodeProps) => {
     const handleToggle = () => {
-      if (calculateDepth(node) === 1 && !node.isOpen) {
-        setCurrentNode(node);
-        setIsIconLoading(true);
-        getBigQueryDatasets(node.data.name);
-      } else if (calculateDepth(node) === 2 && !node.isOpen) {
-        setCurrentNode(node);
-        setIsIconLoading(true);
-        getBigQueryTables(node.data.name, node.parent?.data?.name);
-      } else if (calculateDepth(node) === 3 && node.parent && !node.isOpen) {
-        setCurrentNode(node);
-        setIsIconLoading(true);
-        getBigQueryColumnDetails(
-          node.data.name,
-          node.parent?.data?.name,
-          node?.parent?.parent?.data?.name
-        );
-      } else {
-        node.toggle();
-      }
+      node.toggle();
     };
     const handleIconClick = (event: React.MouseEvent) => {
       if (event.currentTarget.classList.contains('caret-icon')) {
         handleToggle();
       }
     };
     const handleTextClick = (event: React.MouseEvent) => {
       event.stopPropagation();
       onClick(node);
     };
     const renderNodeIcon = () => {
       const depth = calculateDepth(node);
-      const hasChildren =
-        (node.children && node.children.length > 0) ||
-        (depth !== 4 && node.children);
+      const hasChildren = node.children && node.children.length > 0;
       const arrowIcon = hasChildren ? (
-        isIconLoading && currentNode.data.name === node.data.name ? (
-          <div className="big-query-loader-style">
-            <CircularProgress
-              size={16}
-              aria-label="Loading Spinner"
-              data-testid="loader"
-            />
-          </div>
-        ) : node.isOpen ? (
+        node.isOpen ? (
           <>
             <div
               role="treeitem"
               className="caret-icon right"
               onClick={handleIconClick}
             >
-              <iconDownArrow.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
+              <iconDownArrow.react tag="div" />
             </div>
           </>
         ) : (
           <div
             role="treeitem"
             className="caret-icon down"
             onClick={handleIconClick}
           >
-            <iconRightArrow.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
+            <iconRightArrow.react tag="div" />
           </div>
         )
-      ) : (
-        <div style={{ width: '29px' }}></div>
-      );
+      ) : null;
       if (searchTerm) {
-        const arrowIcon = hasChildren ? (
-          isIconLoading && currentNode.data.name === node.data.name ? (
-            <div className="big-query-loader-style">
-              <CircularProgress
-                size={16}
-                aria-label="Loading Spinner"
-                data-testid="loader"
-              />
-            </div>
-          ) : node.isOpen ? (
+        const arrowIcon =
+          hasChildren && node.isOpen ? (
             <>
               <div
                 role="treeitem"
                 className="caret-icon right"
                 onClick={handleIconClick}
               >
-                <iconDownArrow.react
-                  tag="div"
-                  className="icon-white logo-alignment-style"
-                />
+                <iconDownArrow.react tag="div" />
               </div>
             </>
           ) : (
             <div
               role="treeitem"
               className="caret-icon down"
               onClick={handleIconClick}
             >
-              <iconRightArrow.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
+              <iconRightArrow.react tag="div" />
             </div>
-          )
-        ) : (
-          <div style={{ width: '29px' }}></div>
-        );
+          );
         if (depth === 1) {
           return (
             <>
               {arrowIcon}
               <div role="img" className="db-icon" onClick={handleIconClick}>
-                <iconBigQueryProject.react
-                  tag="div"
-                  className="icon-white logo-alignment-style"
-                />
+                <iconDatabase.react tag="div" />
               </div>
             </>
           );
         } else if (depth === 2) {
           return (
             <>
               {arrowIcon}
-              <div role="img" className="db-icon" onClick={handleIconClick}>
-                <iconDataset.react
-                  tag="div"
-                  className="icon-white logo-alignment-style"
-                />
-              </div>
-            </>
-          );
-        } else if (depth === 3) {
-          return (
-            <>
-              {arrowIcon}
               <div role="img" className="table-icon" onClick={handleIconClick}>
-                <iconTable.react
-                  tag="div"
-                  className="icon-white logo-alignment-style"
-                />
+                <iconTable.react tag="div" />
               </div>
             </>
           );
         }
 
         return (
           <>
-            <iconColumns.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
+            <iconColumns.react tag="div" />
           </>
         );
       }
       if (depth === 1) {
         return (
           <>
             {arrowIcon}
             <div role="img" className="db-icon" onClick={handleIconClick}>
-              <iconBigQueryProject.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
+              <iconDatabase.react tag="div" />
             </div>
           </>
         );
       } else if (depth === 2) {
         return (
           <>
             {arrowIcon}
-            <div role="img" className="db-icon" onClick={handleIconClick}>
-              <iconDataset.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
-            </div>
-          </>
-        );
-      } else if (depth === 3) {
-        return (
-          <>
-            {arrowIcon}
             <div role="img" className="table-icon" onClick={handleIconClick}>
-              <iconTable.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
+              <iconTable.react tag="div" />
             </div>
           </>
         );
       }
 
       return (
         <>
-          <iconColumns.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconColumns.react tag="div" />
         </>
       );
     };
 
     return (
       <div style={style}>
         {renderNodeIcon()}
-        <div role="treeitem" title={node.data.name} onClick={handleTextClick}>
+        <div role="treeitem" onClick={handleTextClick}>
           {node.data.name}
         </div>
-        <div title={node?.data?.type} className="dpms-column-type-text">
-          {node.data.type}
-        </div>
       </div>
     );
   };
-
-  const getBigQueryProjects = async () => {
-    await BigQueryService.getBigQueryProjectsListAPIService(setProjectNameInfo);
+  const getDatabaseDetails = async () => {
+    const credentials = await authApi();
+    if (credentials && notebookValue) {
+      const requestBody = {
+        query: `${QUERY_DATABASE}${credentials.project_id}.${credentials.region_id}.${dataprocMetastoreServices}`,
+        scope: {
+          includeProjectIds: [credentials.project_id]
+        }
+      };
+      fetch(`${CATALOG_SEARCH}`, {
+        method: 'POST',
+        body: JSON.stringify(requestBody),
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token,
+          'X-Goog-User-Project': credentials.project_id || ''
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then(async (responseResult: any) => {
+              const filteredEntries = responseResult.results.filter(
+                (entry: { displayName: string }) => entry.displayName
+              );
+              const databaseNames: string[] = [];
+              const updatedDatabaseDetails: { [key: string]: string } = {};
+              filteredEntries.forEach(
+                (entry: { description: string; displayName: string }) => {
+                  databaseNames.push(entry.displayName);
+                  const description = entry.description || 'None';
+                  updatedDatabaseDetails[entry.displayName] = description;
+                }
+              );
+              setDatabaseDetails(updatedDatabaseDetails);
+              databaseNames.map(async (db: string) => {
+                await getTableDetails(db);
+              });
+            })
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error getting database details', err);
+          toast.error('Error getting database details');
+        });
+    }
   };
-
-  const getBigQueryDatasets = async (projectId: string) => {
-    await BigQueryService.getBigQueryDatasetsAPIService(
-      notebookValue,
-      settingRegistry,
-      setDatabaseNames,
-      setDataSetResponse,
-      projectId,
-      setIsIconLoading,
-      setIsLoading
-    );
+  const getClusterDetails = async () => {
+    const credentials = await authApi();
+    if (credentials && notebookValue) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters/${notebookValue}`,
+        {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then(async (responseResult: any) => {
+              const metastoreServices =
+                responseResult.config?.metastoreConfig
+                  ?.dataprocMetastoreService;
+              if (metastoreServices) {
+                const lastIndex = metastoreServices.lastIndexOf('/');
+                const instanceName =
+                  lastIndex !== -1
+                    ? metastoreServices.substring(lastIndex + 1)
+                    : '';
+                setDataprocMetastoreServices(instanceName);
+                setNoDpmsInstance(false);
+                setCluster(false);
+              } else {
+                setNoDpmsInstance(true);
+                setCluster(true);
+              }
+            })
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error listing session details', err);
+          toast.error('Failed to fetch session details');
+        });
+    }
   };
-
-  const getBigQueryTables = async (
-    datasetId: string,
-    projectId: string | undefined
-  ) => {
-    if (datasetId && projectId) {
-      await BigQueryService.getBigQueryTableAPIService(
-        notebookValue,
-        datasetId,
-        setDatabaseNames,
-        setTableResponse,
-        projectId,
-        setIsIconLoading
-      );
+  const getSessionDetails = async () => {
+    const credentials = await authApi();
+    if (credentials && notebookValue) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessionTemplates/${notebookValue}`,
+        {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then(async (responseResult: any) => {
+              const metastoreServices =
+                responseResult.environmentConfig?.peripheralsConfig
+                  ?.metastoreService;
+              if (metastoreServices) {
+                const lastIndex = metastoreServices.lastIndexOf('/');
+                const instanceName =
+                  lastIndex !== -1
+                    ? metastoreServices.substring(lastIndex + 1)
+                    : '';
+                setDataprocMetastoreServices(instanceName);
+                setNoDpmsInstance(false);
+               setSession(false);
+              } else {
+                setNoDpmsInstance(true);
+                setSession(true);
+              }
+            })
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error listing clusters details', err);
+          toast.error('Failed to fetch cluster details');
+        });
     }
   };
-
   const getActiveNotebook = () => {
-    setNotebookValue('bigframes');
-    setDataprocMetastoreServices('bigframes');
+    const notebookVal = localStorage.getItem('notebookValue');
+    // notebookVal: clustername/cluster or sessionname/session getting only the cluster or session name
+    if (notebookVal?.includes('/clusters')) {
+      const clusterName = notebookVal.split('/')
+      const clusterVal = clusterName.slice(0, -1).join('/')
+      setNotebookValue(clusterVal);
+      getClusterDetails();
+    } else if(notebookVal?.includes('/sessions')){
+      const sessionName = notebookVal.split('/')
+      const sessionVal = sessionName.slice(0, -1).join('/')
+      setNotebookValue(sessionVal);
+      getSessionDetails();
+    }
+    else {
+      setNoDpmsInstance(true);
+    }
   };
   useEffect(() => {
     getActiveNotebook();
     return () => {
       setNotebookValue('');
     };
   }, [notebookValue]);
-
   useEffect(() => {
-    getBigQueryProjects();
+    getDatabaseDetails();
   }, [dataprocMetastoreServices]);
-
-  useEffect(() => {
-    if (projectNameInfo.length > 0) {
-      treeStructureforProjects();
-    }
-  }, [projectNameInfo]);
-
-  useEffect(() => {
-    if (dataSetResponse) {
-      treeStructureforDatasets();
-    }
-  }, [dataSetResponse]);
-
-  useEffect(() => {
-    if (tableResponse) {
-      treeStructureforTables();
-    }
-  }, [tableResponse]);
-
-  useEffect(() => {
-    if (schemaResponse) {
-      treeStructureforSchema();
-    }
-  }, [schemaResponse]);
-
-  useEffect(() => {
-    if (treeStructureData.length > 0 && treeStructureData[0].name !== '') {
-      setIsLoading(false);
-    }
-    if (currentNode) {
-      currentNode?.toggle();
-    }
-  }, [treeStructureData]);
-
   useEffect(() => {
-    handleSearchTreeStructure();
-    setSearchLoading(false);
-  }, [searchResponse]);
-
+    entries.forEach(async (entry: string) => {
+      await getColumnDetails(entry);
+    });
+  }, [entries]);
   return (
-    <div className="dpms-Wrapper">
-      <TitleComponent
-        titleStr="Dataset Explorer"
-        isPreview
-        getBigQueryProjects={getBigQueryProjects}
-      />
-      <>
-        <div>
-          {isLoading ? (
-            <div className="database-loader">
-              <div>
-                <CircularProgress
-                  className="spin-loader-custom-style"
-                  size={20}
-                  aria-label="Loading Spinner"
-                  data-testid="loader"
-                />
-              </div>
-              Loading datasets
-            </div>
-          ) : (
-            <>
-              <div className="search-field">
-                <TextField
-                  placeholder="Enter your keyword to search"
-                  type="text"
-                  variant="outlined"
-                  fullWidth
-                  size="small"
-                  onChange={handleSearchTerm}
-                  value={searchTerm}
-                  InputProps={{
-                    startAdornment: (
-                      <InputAdornment position="start">
-                        {!searchLoading ? (
-                          <iconSearch.react
-                            tag="div"
-                            className="icon-white logo-alignment-style"
-                          />
-                        ) : (
-                          <CircularProgress
-                            size={16}
-                            aria-label="Loading Spinner"
-                            data-testid="loader"
-                          />
-                        )}
-                      </InputAdornment>
-                    ),
-                    endAdornment: searchTerm && (
-                      <IconButton
-                        aria-label="toggle password visibility"
-                        onClick={handleSearchClear}
-                      >
-                        <iconSearchClear.react
-                          tag="div"
-                          className="icon-white logo-alignment-style search-clear-icon"
-                        />
-                      </IconButton>
-                    )
-                  }}
-                />
+    <>
+      <div>
+        <div className="dpms-title">Metadata Explorer</div>
+        <div
+          role="button"
+          aria-label="refresh"
+          className="refresh-icon"
+          data-tip="Refresh"
+          onClick={handleRefreshClick}
+        >
+          <iconRefresh.react tag="div" />
+        </div>
+      </div>
+      {!noDpmsInstance ? (
+        <>
+          <div>
+            {isLoading ? (
+              <div className="database-loader">
+                <div>
+                  <ClipLoader
+                    color="#8A8A8A"
+                    loading={true}
+                    size={20}
+                    aria-label="Loading Spinner"
+                    data-testid="loader"
+                  />
+                </div>
+                Loading databases
               </div>
-              <div className="tree-container">
-                {treeStructureData.length > 0 &&
-                  treeStructureData[0].name !== '' && (
-                    <Tree
-                      className="dataset-tree"
-                      data={treeStructureData}
-                      openByDefault={searchTerm === '' ? false : true}
-                      indent={24}
-                      width={auto}
-                      height={height}
-                      rowHeight={36}
-                      overscanCount={1}
-                      paddingTop={30}
-                      paddingBottom={10}
-                      padding={25}
-                      idAccessor={(node: any) => node.id}
+            ) : (
+              <>
+                <div className="ui category search">
+                  <div className="ui icon input">
+                    <input
+                      className="search-field"
+                      type="text"
+                      value={searchTerm}
+                      onChange={handleSearch}
+                      placeholder="Search your DBs and tables"
+                    />
+                    <div className="search-icon">
+                      <iconSearch.react tag="div" />
+                    </div>
+                    {searchTerm &&
+                    <div
+                      role="button"
+                      className="search-clear-icon"
+                      onClick={handleSearchClear}
                     >
-                      {(props: NodeRendererProps<any>) => (
-                        <Node {...props} onClick={handleNodeClick} />
-                      )}
-                    </Tree>
-                  )}
-              </div>
-            </>
-          )}
-        </div>
-      </>
-    </div>
+                      <iconSearchClear.react tag="div" />
+                    </div>
+                    }
+                  </div>
+                </div>
+                <div className="tree-container">
+                  <Tree
+                    className="Tree"
+                    data={data}
+                    openByDefault={false}
+                    indent={24}
+                    width={auto}
+                    height={500}
+                    rowHeight={36}
+                    overscanCount={1}
+                    paddingTop={30}
+                    paddingBottom={10}
+                    padding={25}
+                    searchTerm={searchTerm}
+                    searchMatch={searchMatch}
+                    idAccessor={node => node.id}
+                  >
+                    {(props: NodeRendererProps<any>) => (
+                      <Node {...props} onClick={handleNodeClick} />
+                    )}
+                  </Tree>
+                  <ToastContainer />
+                </div>
+              </>
+            )}
+          </div>
+        </>
+      ) : (
+        session ? (
+        <div className="dpms-error">
+          DPMS is not configured for this runtime template. Please attach DPMS or
+          activate DPMS sync with data catalog
+        </div>) : (cluster ? (<div className="dpms-error">
+          DPMS is not configured for this cluster. Please attach DPMS or
+          activate DPMS sync with data catalog
+        </div>):(<div className="dpms-error">
+        DPMS schema explorer not set up
+        </div>))
+      )}
+    </>
   );
 };
 
-export class BigQueryWidget extends DataprocWidget {
+export class dpmsWidget extends ReactWidget {
   app: JupyterLab;
-  settingRegistry: ISettingRegistry;
-  enableBigqueryIntegration: boolean;
 
-  constructor(
-    app: JupyterLab,
-    settingRegistry: ISettingRegistry,
-    enableBigqueryIntegration: boolean,
-    themeManager: IThemeManager
-  ) {
-    super(themeManager);
+  constructor(app: JupyterLab) {
+    super();
     this.app = app;
-    this.settingRegistry = settingRegistry;
-    this.enableBigqueryIntegration = enableBigqueryIntegration;
   }
 
-  renderInternal(): JSX.Element {
-    return (
-      <BigQueryComponent
-        app={this.app}
-        settingRegistry={this.settingRegistry}
-        themeManager={this.themeManager}
-      />
-    );
+  render(): JSX.Element {
+    return <DpmsComponent app={this.app} />;
   }
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/cluster/clusterDetails.tsx` & `dataproc_jupyter_plugin-0.1.9/src/cluster/clusterDetails.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -24,31 +24,40 @@
 import StopClusterIcon from '../../style/icons/stop_cluster_icon.svg';
 import StopClusterDisableIcon from '../../style/icons/stop_cluster_disable_icon.svg';
 import DeleteClusterIcon from '../../style/icons/delete_cluster_icon.svg';
 import errorIcon from '../../style/icons/error_icon.svg';
 import clusterRunningIcon from '../../style/icons/cluster_running_icon.svg';
 import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
 import stopIcon from '../../style/icons/stop_icon.svg';
-import { ClusterService } from './clusterServices';
 import {
+  deleteClusterApi,
+  startClusterApi,
+  stopClusterApi
+} from '../utils/clusterServices';
+import {
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
   STATUS_CREATING,
   STATUS_DELETING,
   STATUS_ERROR,
   STATUS_PROVISIONING,
   STATUS_RUNNING,
   STATUS_STARTING,
   STATUS_STOPPED,
   STATUS_STOPPING
 } from '../utils/const';
+import { authApi } from '../utils/utils';
+import ClipLoader from 'react-spinners/ClipLoader';
 import ViewLogs from '../utils/viewLogs';
 import DeletePopup from '../utils/deletePopup';
+import { toast, ToastContainer } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
 import SubmitJob from '../jobs/submitJob';
 import PollingTimer from '../utils/pollingTimer';
-import { JobService } from '../jobs/jobServices';
-import { CircularProgress } from '@mui/material';
 
 const iconLeftArrow = new LabIcon({
   name: 'launcher:left-arrow-icon',
   svgstr: LeftArrowIcon
 });
 const iconStartCluster = new LabIcon({
   name: 'launcher:start-cluster-icon',
@@ -90,58 +99,53 @@
   clusterSelected: string;
   setDetailedView: (value: boolean) => void;
   setDetailedClusterView?: (value: boolean) => void;
   detailedJobView?: boolean;
   setDetailedJobView?: (value: boolean) => void;
   setSubmitJobView?: (value: boolean) => void;
   submitJobView: boolean;
+  clusterResponse: any;
   selectedJobClone: any;
   setSelectedJobClone?: (value: boolean) => void;
 }
 function ClusterDetails({
   clusterSelected,
   setDetailedView,
   setDetailedClusterView,
   detailedJobView,
   setSubmitJobView,
   setDetailedJobView,
   submitJobView,
+  clusterResponse,
   selectedJobClone,
   setSelectedJobClone
 }: IClusterDetailsProps) {
   const [clusterInfo, setClusterInfo] = useState({
     status: { state: '' },
     clusterName: '',
     clusterUuid: ''
   });
   const [isLoading, setIsLoading] = useState(true);
   const [errorView, setErrorView] = useState(false);
   const [projectName, setProjectName] = useState('');
   const [deletePopupOpen, setDeletePopupOpen] = useState(false);
   const [selectedCluster, setSelectedCluster] = useState('');
-
-  const [clusterResponse, setClusterResponse] = useState([]);
-
   const timer = useRef<NodeJS.Timeout | undefined>(undefined);
 
   const pollingClusterDetails = async (
     pollingFunction: () => void,
     pollingDisable: boolean
   ) => {
     timer.current = PollingTimer(
       pollingFunction,
       pollingDisable,
       timer.current
     );
   };
 
-  const listClustersAPI = async () => {
-    await JobService.listClustersAPIService(setClusterResponse);
-  };
-
   const handleDetailedView = () => {
     pollingClusterDetails(getClusterDetails, true);
     setDetailedView(false);
     setDetailedClusterView?.(false);
     setDetailedJobView?.(false);
   };
 
@@ -150,28 +154,55 @@
     setDeletePopupOpen(true);
   };
   const handleCancelDelete = () => {
     setDeletePopupOpen(false);
   };
 
   const handleDelete = async () => {
-    await ClusterService.deleteClusterApi(selectedCluster);
+    await deleteClusterApi(selectedCluster);
 
     setDeletePopupOpen(false);
     handleDetailedView();
   };
 
   const getClusterDetails = async () => {
-    await ClusterService.getClusterDetailsService(
-      setProjectName,
-      clusterSelected,
-      setErrorView,
-      setIsLoading,
-      setClusterInfo
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      setProjectName(credentials.project_id || '');
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters/${clusterSelected}`,
+        {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              if (responseResult.error && responseResult.error.code === 404) {
+                setErrorView(true);
+              }
+              setClusterInfo(responseResult);
+              setIsLoading(false);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error listing clusters Details', err);
+          toast.error(`Failed to fetch cluster details ${clusterSelected}`);
+        });
+    }
   };
 
   const clusterDetailsAction = () => {
     return (
       <div className="cluster-details-action-parent">
         <div
           role="button"
@@ -179,84 +210,68 @@
           className={
             clusterInfo.status.state === STATUS_STOPPED
               ? 'action-cluster-section'
               : 'action-cluster-section disabled'
           }
           onClick={() =>
             clusterInfo.status.state === STATUS_STOPPED &&
-            ClusterService.startClusterApi(clusterInfo.clusterName)
+            startClusterApi(clusterInfo.clusterName)
           }
         >
           <div
             className="action-cluster-icon"
             role="button"
             aria-disabled={clusterInfo.status.state !== STATUS_STOPPED}
           >
             {clusterInfo.status.state === STATUS_STOPPED ? (
-              <iconStartCluster.react
-                tag="div"
-                className="logo-alignment-style"
-              />
+              <iconStartCluster.react tag="div" />
             ) : (
-              <iconStartClusterDisable.react
-                tag="div"
-                className="logo-alignment-style"
-              />
+              <iconStartClusterDisable.react tag="div" />
             )}
           </div>
           <div className="action-cluster-text">START</div>
         </div>
         <div
           role="button"
           aria-disabled={clusterInfo.status.state !== STATUS_RUNNING}
           className={
             clusterInfo.status.state === STATUS_RUNNING
               ? 'action-cluster-section'
               : 'action-cluster-section disabled'
           }
           onClick={() =>
             clusterInfo.status.state === STATUS_RUNNING &&
-            ClusterService.stopClusterApi(clusterInfo.clusterName)
+            stopClusterApi(clusterInfo.clusterName)
           }
         >
           <div className="action-cluster-icon">
             {clusterInfo.status.state === STATUS_RUNNING ? (
-              <iconStopCluster.react
-                tag="div"
-                className="logo-alignment-style"
-              />
+              <iconStopCluster.react tag="div" />
             ) : (
-              <iconStopClusterDisable.react
-                tag="div"
-                className="logo-alignment-style"
-              />
+              <iconStopClusterDisable.react tag="div" />
             )}
           </div>
           <div className="action-cluster-text">STOP</div>
         </div>
         <div
           role="button"
           className="action-cluster-section"
           onClick={() => handleDeleteCluster(clusterInfo.clusterName)}
         >
           <div className="action-cluster-icon">
-            <iconDeleteCluster.react
-              tag="div"
-              className="logo-alignment-style"
-            />
+            <iconDeleteCluster.react tag="div" />
           </div>
           <div className="action-cluster-text">DELETE</div>
         </div>
       </div>
     );
   };
 
   useEffect(() => {
     getClusterDetails();
-    listClustersAPI();
     pollingClusterDetails(getClusterDetails, false);
 
     return () => {
       pollingClusterDetails(getClusterDetails, true);
     };
   }, []);
 
@@ -266,18 +281,18 @@
         <div className="error-view-parent">
           <div
             role="button"
             aria-label="back-arrow-icon"
             className="back-arrow-icon"
             onClick={() => handleDetailedView()}
           >
-            <iconLeftArrow.react tag="div" className="logo-alignment-style" />
+            <iconLeftArrow.react tag="div" />
           </div>
           <div className="error-view-message-parent">
-            <iconError.react tag="div" className="logo-alignment-style" />
+            <iconError.react tag="div" />
             <div role="alert" className="error-view-message">
               Unable to find the resource you requested
             </div>
           </div>
         </div>
       )}
       {submitJobView && !detailedJobView && (
@@ -294,30 +309,28 @@
           deletePopupOpen={deletePopupOpen}
           DeleteMsg={
             'This will delete ' + selectedCluster + ' and cannot be undone.'
           }
         />
       )}
       {!submitJobView && (
-        <div className="scroll">
+        <div className="scroll-comp">
+          <ToastContainer />
           {!errorView && clusterInfo.clusterName !== '' ? (
             <div>
               {!detailedJobView && (
                 <div>
                   <div className="cluster-details-header">
                     <div
                       role="button"
                       aria-label="back-arrow-icon"
                       className="back-arrow-icon"
                       onClick={() => handleDetailedView()}
                     >
-                      <iconLeftArrow.react
-                        tag="div"
-                        className="icon-white logo-alignment-style"
-                      />
+                      <iconLeftArrow.react tag="div" />
                     </div>
                     <div className="cluster-details-title">Cluster details</div>
                     {clusterDetailsAction()}
                     <ViewLogs
                       clusterInfo={clusterInfo}
                       projectName={projectName}
                     />
@@ -346,38 +359,31 @@
                       <div className="cluster-details-label">Status</div>
                       <div
                         className="cluster-detail-status-parent"
                         aria-status={clusterInfo.status.state}
                         aria-label={clusterInfo.status.state}
                       >
                         {clusterInfo.status.state === STATUS_RUNNING && (
-                          <iconClusterRunning.react
-                            tag="div"
-                            className="logo-alignment-style"
-                          />
+                          <iconClusterRunning.react tag="div" />
                         )}
                         {clusterInfo.status.state === STATUS_STOPPED && (
-                          <iconStop.react
-                            tag="div"
-                            className="logo-alignment-style"
-                          />
+                          <iconStop.react tag="div" />
                         )}
                         {clusterInfo.status.state === STATUS_ERROR && (
-                          <iconClusterError.react
-                            tag="div"
-                            className="logo-alignment-style"
-                          />
+                          <iconClusterError.react tag="div" />
                         )}
                         {(clusterInfo.status.state === STATUS_PROVISIONING ||
                           clusterInfo.status.state === STATUS_CREATING ||
                           clusterInfo.status.state === STATUS_STARTING ||
                           clusterInfo.status.state === STATUS_STOPPING ||
                           clusterInfo.status.state === STATUS_DELETING) && (
                           <div>
-                            <CircularProgress
+                            <ClipLoader
+                              color="#8A8A8A"
+                              loading={true}
                               size={15}
                               aria-label="Loading Spinner"
                               data-testid="loader"
                             />
                           </div>
                         )}
                         <div className="cluster-status">
@@ -396,30 +402,32 @@
               <JobComponent
                 clusterSelected={clusterSelected}
                 setDetailedView={setDetailedView}
                 detailedJobView={detailedJobView}
                 setDetailedJobView={setDetailedJobView}
                 setSubmitJobView={setSubmitJobView}
                 setSelectedJobClone={setSelectedJobClone}
+                clusterResponse={clusterResponse}
               />
             </div>
           ) : (
-            <>
+            <div className="loader-full-style">
               {isLoading && (
-                <div className="spin-loader-main">
-                  <CircularProgress
-                    className = "spin-loader-custom-style"
-                    size={18}
+                <div>
+                  <ClipLoader
+                    color="#8A8A8A"
+                    loading={true}
+                    size={20}
                     aria-label="Loading Spinner"
                     data-testid="loader"
                   />
                   Loading Cluster Details
                 </div>
               )}
-            </>
+            </div>
           )}
         </div>
       )}
     </div>
   );
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/cluster/listCluster.tsx` & `dataproc_jupyter_plugin-0.1.9/src/cluster/cluster.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -11,74 +11,49 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-import React, { useEffect, useRef, useState } from 'react';
-import { useTable, useGlobalFilter, usePagination } from 'react-table';
+import { ReactWidget } from '@jupyterlab/apputils';
+import React, { useState, useEffect, useRef } from 'react';
+import JobComponent from '../jobs/jobs';
+import ClusterDetails from './clusterDetails';
+import { authApi, checkConfig, statusValue } from '../utils/utils';
 import { LabIcon } from '@jupyterlab/ui-components';
-import createClusterIcon from '../../style/icons/create_cluster_icon.svg';
-import filterIcon from '../../style/icons/filter_icon.svg';
+import startIcon from '../../style/icons/start_icon.svg';
 import stopIcon from '../../style/icons/stop_icon.svg';
-import clusterRunningIcon from '../../style/icons/cluster_running_icon.svg';
-import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
-import {
-  CREATE_CLUSTER_URL,
-  ClusterStatus,
-  STATUS_CREATING,
-  STATUS_DELETING,
-  STATUS_ERROR,
-  STATUS_PROVISIONING,
-  STATUS_RUNNING,
-  STATUS_STARTING,
-  STATUS_STOPPED,
-  STATUS_STOPPING
-} from '../utils/const';
-import GlobalFilter from '../utils/globalFilter';
-import TableData from '../utils/tableData';
-import { PaginationView } from '../utils/paginationView';
-import { ICellProps } from '../utils/utils';
-
 import restartIcon from '../../style/icons/restart_icon.svg';
-import restartDisableIcon from '../../style/icons/restart_icon_disable.svg';
-import startIcon from '../../style/icons/start_icon.svg';
 import startDisableIcon from '../../style/icons/start_icon_disable.svg';
 import stopDisableIcon from '../../style/icons/stop_icon_disable.svg';
+import restartDisableIcon from '../../style/icons/restart_icon_disable.svg';
+import {
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
+  POLLING_TIME_LIMIT,
+  API_HEADER_BEARER,
+  LOGIN_STATE,
+  ClusterStatus
+} from '../utils/const';
+import ListCluster from './listCluster';
+import { ClipLoader } from 'react-spinners';
+import { toast, ToastContainer } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
+import { startClusterApi, stopClusterApi } from '../utils/clusterServices';
 import PollingTimer from '../utils/pollingTimer';
-import { ClusterService } from './clusterServices';
-import { CircularProgress } from '@mui/material';
 
-const iconCreateCluster = new LabIcon({
-  name: 'launcher:create-cluster-icon',
-  svgstr: createClusterIcon
-});
-const iconFilter = new LabIcon({
-  name: 'launcher:filter-icon',
-  svgstr: filterIcon
+const iconStart = new LabIcon({
+  name: 'launcher:start-icon',
+  svgstr: startIcon
 });
-
 const iconStop = new LabIcon({
   name: 'launcher:stop-icon',
   svgstr: stopIcon
 });
-
-const iconClusterRunning = new LabIcon({
-  name: 'launcher:cluster-running-icon',
-  svgstr: clusterRunningIcon
-});
-const iconClusterError = new LabIcon({
-  name: 'launcher:cluster-error-icon',
-  svgstr: clusterErrorIcon
-});
-const iconStart = new LabIcon({
-  name: 'launcher:start-icon',
-  svgstr: startIcon
-});
 const iconRestart = new LabIcon({
   name: 'launcher:restart-icon',
   svgstr: restartIcon
 });
 
 const iconStartDisable = new LabIcon({
   name: 'launcher:start-disable-icon',
@@ -89,125 +64,208 @@
   svgstr: stopDisableIcon
 });
 const iconRestartDisable = new LabIcon({
   name: 'launcher:restart-disable-icon',
   svgstr: restartDisableIcon
 });
 
-interface ICluster {
-  clusterName: string;
-  status: string;
-  clusterImage: string;
-  region: string;
-  zone: string;
-  totalWorkersNode: string;
-  schedulesDeletion: string;
-  actions: React.ReactNode;
-}
-
-interface IListClusterProps {
-  setClusterSelected: (value: string) => void;
-  detailedView: boolean;
-  setDetailedView: (value: boolean) => void;
-  setLoggedIn: (value: boolean) => void;
-}
-function ListCluster({
-  setClusterSelected,
-  detailedView,
-  setDetailedView,
-  setLoggedIn
-}: IListClusterProps) {
-  const [clustersList, setClustersList] = useState<ICluster[]>([]);
+const ClusterComponent = (): React.JSX.Element => {
+  type Mode = 'Clusters' | 'Serverless' | 'Jobs';
+  const [clustersList, setclustersList] = useState([]);
+  const [clusterResponse, setClusterResponse] = useState([]);
+  const [detailedJobView, setDetailedJobView] = useState(false);
+  const [submitJobView, setSubmitJobView] = useState(false);
   const [restartEnabled, setRestartEnabled] = useState(false);
+  const [selectedMode, setSelectedMode] = useState<Mode>('Clusters');
   const [isLoading, setIsLoading] = useState(true);
+  const [clusterSelected, setClusterSelected] = useState<string>('');
   const [pollingDisable, setPollingDisable] = useState(false);
+  const [detailedView, setDetailedView] = useState(false);
+  const [loggedIn, setLoggedIn] = useState(false);
+  const [configError, setConfigError] = useState(false);
+  const [loginError, setLoginError] = useState(false);
+  const [configLoading, setConfigLoading] = useState(true);
   const [projectId, setProjectId] = useState('');
   const timer = useRef<NodeJS.Timeout | undefined>(undefined);
+  const [selectedJobClone, setSelectedJobClone] = useState({});
 
   const pollingClusters = async (
     pollingFunction: () => void,
     pollingDisable: boolean
   ) => {
     timer.current = PollingTimer(
       pollingFunction,
       pollingDisable,
       timer.current
     );
   };
-  const data = clustersList;
-  const columns = React.useMemo(
-    () => [
-      {
-        Header: 'Name',
-        accessor: 'clusterName'
-      },
-      {
-        Header: 'Status',
-        accessor: 'status'
-      },
-      {
-        Header: 'Cluster image name',
-        accessor: 'clusterImage'
-      },
-      {
-        Header: 'Region',
-        accessor: 'region'
-      },
-      {
-        Header: 'Zone',
-        accessor: 'zone'
-      },
-      {
-        Header: 'Total worker nodes',
-        accessor: 'totalWorkersNode'
-      },
-      {
-        Header: 'Scheduled deletion',
-        accessor: 'schedulesDeletion'
-      },
-      {
-        Header: 'Actions',
-        accessor: 'actions'
-      }
-    ],
-    []
-  );
 
-  const listClustersAPI = async () => {
-    await ClusterService.listClustersAPIService(
-      setProjectId,
-      renderActions,
-      setClustersList,
-      setIsLoading,
-      setLoggedIn
-    );
+  const selectedModeChange = (mode: Mode) => {
+    setSelectedMode(mode);
   };
 
+  const listClustersAPI = async (
+    nextPageToken?: string,
+    previousClustersList?: object
+  ) => {
+    const credentials = await authApi();
+    const pageToken = nextPageToken ?? '';
+    if (credentials) {
+      setProjectId(credentials.project_id || '');
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters?pageSize=50&pageToken=${pageToken}`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              let transformClusterListData = [];
+              if (responseResult && responseResult.clusters) {
+                setClusterResponse(responseResult);
+                transformClusterListData = responseResult.clusters.map(
+                  (data: any) => {
+                    const statusVal = statusValue(data);
+                    /*
+                     Extracting zone from zoneUri
+                      Example: "projects/{project}/zones/{zone}"
+                  */
+                    const zoneUri =
+                      data.config.gceClusterConfig.zoneUri.split('/');
+
+                    return {
+                      clusterUuid: data.clusterUuid,
+                      status: statusVal,
+                      clusterName: data.clusterName,
+                      clusterImage: data.config.softwareConfig.imageVersion,
+                      region: data.labels['goog-dataproc-location'],
+                      zone: zoneUri[zoneUri.length - 1],
+                      totalWorkersNode: data.config.workerConfig
+                        ? data.config.workerConfig.numInstances
+                        : 0,
+                      schedulesDeletion: data.config.lifecycleConfig
+                        ? 'On'
+                        : 'Off',
+                      actions: renderActions(data)
+                    };
+                  }
+                );
+              }
+              const existingClusterData = previousClustersList ?? [];
+              //setStateAction never type issue
+              const allClustersData: any = [
+                ...(existingClusterData as []),
+                ...transformClusterListData
+              ];
+
+              if (responseResult.nextPageToken) {
+                listClustersAPI(responseResult.nextPageToken, allClustersData);
+              } else {
+                setclustersList(allClustersData);
+                setIsLoading(false);
+                setLoggedIn(true);
+              }
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error listing clusters', err);
+          toast.error('Failed to fetch clusters');
+        });
+    }
+  };
   const handleClusterDetails = (selectedName: string) => {
     pollingClusters(listClustersAPI, true);
     setClusterSelected(selectedName);
     setDetailedView(true);
   };
 
-  const statusApi = async (selectedCluster: string) => {
-    await ClusterService.statusApiService(
-      selectedCluster,
-      listClustersAPI,
-      timer
-    );
+  const statusApi = async (selectedcluster: string) => {
+    const credentials = await authApi();
+    if (credentials) {
+      await fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters/${selectedcluster}`,
+        {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then(
+              (responseResult: {
+                status: { state: ClusterStatus };
+                clusterName: string;
+              }) => {
+                if (
+                  responseResult.status.state === ClusterStatus.STATUS_STOPPED
+                ) {
+                  startClusterApi(selectedcluster);
+                  clearInterval(timer.current);
+                }
+              }
+            )
+            .catch((e: Error) => console.log(e));
+        })
+        .catch((err: Error) => {
+          console.error('Error fetching status', err);
+          toast.error(`Failed to fetch the status ${selectedcluster}`);
+        });
+
+      listClustersAPI();
+    }
   };
 
-  const restartClusterApi = async (selectedCluster: string) => {
-    await ClusterService.restartClusterApiService(
-      selectedCluster,
-      setRestartEnabled,
-      listClustersAPI,
-      timer,
-      statusApi
-    );
+  const restartClusterApi = async (selectedcluster: string) => {
+    setRestartEnabled(true);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters/${selectedcluster}:stop`,
+        {
+          method: 'POST',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: Response) => {
+              console.log(responseResult);
+              listClustersAPI();
+              timer.current = setInterval(() => {
+                statusApi(selectedcluster);
+              }, POLLING_TIME_LIMIT);
+            })
+            .catch((e: Error) => console.log(e));
+        })
+        .catch((err: Error) => {
+          console.error('Error restarting cluster', err);
+          toast.error(`Failed to restart the cluster ${selectedcluster}`);
+        });
+
+      listClustersAPI();
+      setRestartEnabled(false);
+    }
   };
 
   const startButton = (data: {
     status: { state: ClusterStatus };
     clusterName: string;
   }) => {
     return (
@@ -221,30 +279,23 @@
           data.status.state === ClusterStatus.STATUS_STOPPED &&
           restartEnabled !== true
             ? 'icon-buttons-style'
             : 'icon-buttons-style-disable'
         }
         title="Start Cluster"
         onClick={
-          data.status.state === ClusterStatus.STATUS_STOPPED && !restartEnabled
-            ? () => ClusterService.startClusterApi(data.clusterName)
+          data.status.state === ClusterStatus.STATUS_STOPPED
+            ? () => startClusterApi(data.clusterName)
             : undefined
         }
       >
-        {data.status.state === ClusterStatus.STATUS_STOPPED &&
-        !restartEnabled ? (
-          <iconStart.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+        {data.status.state === ClusterStatus.STATUS_STOPPED ? (
+          <iconStart.react tag="div" />
         ) : (
-          <iconStartDisable.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconStartDisable.react tag="div" />
         )}
       </div>
     );
   };
 
   const stopButton = (data: {
     status: { state: ClusterStatus };
@@ -258,28 +309,22 @@
           data.status.state === ClusterStatus.STATUS_RUNNING
             ? 'icon-buttons-style'
             : 'icon-buttons-style-disable'
         }
         title="Stop Cluster"
         onClick={
           data.status.state === ClusterStatus.STATUS_RUNNING
-            ? () => ClusterService.stopClusterApi(data.clusterName)
+            ? () => stopClusterApi(data.clusterName)
             : undefined
         }
       >
         {data.status.state === ClusterStatus.STATUS_RUNNING ? (
-          <iconStop.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconStop.react tag="div" />
         ) : (
-          <iconStopDisable.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconStopDisable.react tag="div" />
         )}
       </div>
     );
   };
 
   const restartButton = (data: {
     status: { state: ClusterStatus };
@@ -298,23 +343,17 @@
         onClick={
           data.status.state === ClusterStatus.STATUS_RUNNING
             ? () => restartClusterApi(data.clusterName)
             : undefined
         }
       >
         {data.status.state === ClusterStatus.STATUS_RUNNING ? (
-          <iconRestart.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconRestart.react tag="div" />
         ) : (
-          <iconRestartDisable.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconRestartDisable.react tag="div" />
         )}
       </div>
     );
   };
   const renderActions = (data: {
     status: { state: ClusterStatus };
     clusterName: string;
@@ -324,198 +363,132 @@
         {startButton(data)}
         {stopButton(data)}
         {restartButton(data)}
       </div>
     );
   };
 
-  useEffect(() => {
-    if (!pollingDisable) {
-      listClustersAPI();
+  const toggleStyleSelection = (toggleItem: string) => {
+    if (selectedMode === toggleItem) {
+      return 'selected-header';
+    } else {
+      return 'unselected-header';
     }
+  };
 
-    return () => {
-      pollingClusters(listClustersAPI, true);
-    };
-  }, [pollingDisable, detailedView]);
   useEffect(() => {
-    if (!detailedView && !isLoading) {
+    checkConfig(setLoggedIn, setConfigError, setLoginError);
+    const localstorageGetInformation = localStorage.getItem('loginState');
+    setLoggedIn(localstorageGetInformation === LOGIN_STATE);
+    if (loggedIn) {
+      setConfigLoading(false);
+    }
+    listClustersAPI();
+    if (!detailedView && selectedMode === 'Clusters') {
       pollingClusters(listClustersAPI, pollingDisable);
     }
-  }, [isLoading]);
 
-  const tableDataCondition = (cell: ICellProps) => {
-    if (cell.column.Header === 'Name') {
-      return (
-        <td
-          {...cell.getCellProps()}
-          role="button"
-          className="cluster-name"
-          onClick={() =>
-            cell.row.original.status !== STATUS_DELETING &&
-            handleClusterDetails(cell.value)
-          }
-        >
-          {cell.value}
-        </td>
-      );
-    } else if (cell.column.Header === 'Status') {
-      return (
-        <td {...cell.getCellProps()} className="clusters-table-data">
-          <div
-            key="Status"
-            className="cluster-status-parent"
-            role="status"
-            aria-labels={cell.value}
-          >
-            {cell.value === STATUS_RUNNING && (
-              <iconClusterRunning.react
-                tag="div"
-                className="logo-alignment-style"
-              />
-            )}
-            {cell.value === STATUS_STOPPED && (
-              <iconStop.react tag="div" className="logo-alignment-style" />
-            )}
-            {cell.value === STATUS_ERROR && (
-              <iconClusterError.react
-                tag="div"
-                className="logo-alignment-style"
-              />
-            )}
-            {(cell.value === STATUS_PROVISIONING ||
-              cell.value === STATUS_CREATING ||
-              cell.value === STATUS_STARTING ||
-              cell.value === STATUS_STOPPING ||
-              cell.value === STATUS_DELETING) && (
-              <CircularProgress
-                size={15}
-                aria-label="Loading Spinner"
-                data-testid="loader"
-              />
-            )}
-            <div className="cluster-status">
-              {cell.value && cell.value.toLowerCase()}
-            </div>
-          </div>
-        </td>
-      );
-    } else {
-      return (
-        <td {...cell.getCellProps()} className="clusters-table-data">
-          {cell.render('Cell')}
-        </td>
-      );
-    }
-  };
-
-  const {
-    getTableProps,
-    getTableBodyProps,
-    headerGroups,
-    rows,
-    prepareRow,
-    state,
-    preGlobalFilteredRows,
-    setGlobalFilter,
-    page,
-    canPreviousPage,
-    canNextPage,
-    nextPage,
-    previousPage,
-    setPageSize,
-    state: { pageIndex, pageSize }
-  } = useTable(
-    //@ts-ignore react-table 'columns' which is declared here on type 'TableOptions<ICluster>'
-    { columns, data, autoResetPage: false, initialState: { pageSize: 50 } },
-    useGlobalFilter,
-    usePagination
-  );
+    return () => {
+      pollingClusters(listClustersAPI, true);
+    };
+  }, [pollingDisable, detailedView, selectedMode]);
 
   return (
-    <div>
-      <div className="create-cluster-overlay">
-        <div
-          role="button"
-          className="create-cluster-sub-overlay"
-          onClick={() => {
-            window.open(`${CREATE_CLUSTER_URL}?project=${projectId}`, '_blank');
-          }}
-        >
-          <div className="create-icon">
-            <iconCreateCluster.react
-              tag="div"
-              className="logo-alignment-style"
-            />
-          </div>
-          <div className="create-text">Create cluster</div>
+    <div className="component-level">
+      {configLoading && !loggedIn && !configError && !loginError && (
+        <div className="spin-loaderMain">
+          <ClipLoader
+            color="#8A8A8A"
+            loading={true}
+            size={18}
+            aria-label="Loading Spinner"
+            data-testid="loader"
+          />
+          Loading Clusters
         </div>
-      </div>
-
-      {clustersList.length > 0 ? (
-        <div>
-          <div className="filter-cluster-overlay">
-            <div className="filter-cluster-icon">
-              <iconFilter.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
-            </div>
-            <div className="filter-cluster-text"></div>
-            <div className="filter-cluster-section">
-              <GlobalFilter
-                preGlobalFilteredRows={preGlobalFilteredRows}
-                globalFilter={state.globalFilter}
-                setGlobalFilter={setGlobalFilter}
-                setPollingDisable={setPollingDisable}
-              />
-            </div>
-          </div>
-          <div className="clusters-list-table-parent">
-            <TableData
-              getTableProps={getTableProps}
-              headerGroups={headerGroups}
-              getTableBodyProps={getTableBodyProps}
-              isLoading={isLoading}
-              rows={rows}
-              page={page}
-              prepareRow={prepareRow}
-              tableDataCondition={tableDataCondition}
-              fromPage="Clusters"
+      )}
+      {loggedIn && !configError ? (
+        <>
+          {detailedView && (
+            <ClusterDetails
+              clusterSelected={clusterSelected}
+              setDetailedView={setDetailedView}
+              detailedJobView={detailedJobView}
+              setDetailedJobView={setDetailedJobView}
+              submitJobView={submitJobView}
+              clusterResponse={clusterResponse}
+              selectedJobClone={selectedJobClone}
+              setSelectedJobClone={setSelectedJobClone}
+              setSubmitJobView={setSubmitJobView}
             />
-            {clustersList.length > 50 && (
-              <PaginationView
-                pageSize={pageSize}
-                setPageSize={setPageSize}
-                pageIndex={pageIndex}
-                allData={clustersList}
-                previousPage={previousPage}
-                nextPage={nextPage}
-                canPreviousPage={canPreviousPage}
-                canNextPage={canNextPage}
-              />
-            )}
-          </div>
-        </div>
-      ) : (
-        <div>
-          {isLoading && (
-            <div className="spin-loader-main">
-              <CircularProgress
-                className = "spin-loader-custom-style"
-                size={18}
-                aria-label="Loading Spinner"
-                data-testid="loader"
-              />
-              Loading Clusters
-            </div>
           )}
-          {!isLoading && (
-            <div className="no-data-style">No rows to display</div>
+          {!detailedView && (
+            <div className="clusters-list-component" role="tablist">
+              {!detailedJobView && !submitJobView && (
+                <div className="clusters-list-overlay" role="tab">
+                  <div
+                    role="tabpanel"
+                    className={toggleStyleSelection('Clusters')}
+                    onClick={() => selectedModeChange('Clusters')}
+                  >
+                    Clusters
+                  </div>
+                  <div
+                    role="tabpanel"
+                    className={toggleStyleSelection('Jobs')}
+                    onClick={() => selectedModeChange('Jobs')}
+                  >
+                    Jobs
+                  </div>
+                </div>
+              )}
+              <div>
+                {selectedMode === 'Jobs' ? (
+                  <JobComponent
+                    clustersList={clustersList}
+                    detailedJobView={detailedJobView}
+                    setDetailedJobView={setDetailedJobView}
+                    submitJobView={submitJobView}
+                    setSubmitJobView={setSubmitJobView}
+                    setDetailedView={setDetailedView}
+                    clusterResponse={clusterResponse}
+                    selectedJobClone={selectedJobClone}
+                    setSelectedJobClone={setSelectedJobClone}
+                  />
+                ) : (
+                  <ListCluster
+                    clustersList={clustersList}
+                    isLoading={isLoading}
+                    setPollingDisable={setPollingDisable}
+                    listClustersAPI={listClustersAPI}
+                    handleClusterDetails={handleClusterDetails}
+                    project_id={projectId}
+                  />
+                )}
+              </div>
+              <ToastContainer />
+            </div>
           )}
+        </>
+      ) : (
+        loginError && (
+          <div className="login-error">Please login to continue</div>
+        )
+      )}
+      {configError && (
+        <div className="login-error">
+          Please configure gcloud with account, project-id and region
         </div>
       )}
     </div>
   );
-}
+};
 
-export default ListCluster;
+export class Cluster extends ReactWidget {
+  constructor() {
+    super();
+  }
+
+  render(): React.JSX.Element {
+    return <ClusterComponent />;
+  }
+}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/controls/MuiWrappedDropdown.tsx` & `dataproc_jupyter_plugin-0.1.9/src/utils/runtimeService.tsx`

 * *Files 27% similar despite different names*

```diff
@@ -10,41 +10,40 @@
  *
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
-import {
-  Autocomplete,
-  AutocompleteProps,
-  TextField,
-  styled
-} from '@mui/material';
-import React from 'react';
-
-type Props = Omit<
-  AutocompleteProps<string, undefined, undefined, undefined>,
-  'renderInput'
->;
 
-function DropdownInternal(props: Props) {
-  const { className, value, onChange, options } = props;
-  return (
-    <Autocomplete
-      className={className}
-      value={value}
-      onChange={onChange}
-      options={options}
-      renderInput={params => <TextField {...params} placeholder="Search..." />}
-    />
-  );
-}
+import {
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
+  API_HEADER_BEARER
+} from '../utils/const';
+import { authApi } from '../utils/utils';
+import { toast } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
 
-export const Dropdown = styled(DropdownInternal)<Props>({
-  '& .MuiInputBase-root': {
-    padding: 0
-  },
-  '& .MuiOutlinedInput-notchedOutline': {
-    borderStyle: 'none'
+export const deleteRuntimeTemplateAPI = async (selectedRuntimeTemplate: string,selectedRuntimeTemplateDisplayName:string) => {
+  const credentials = await authApi();
+  if (credentials) {
+    fetch(
+      `${BASE_URL}/${selectedRuntimeTemplate}`,
+      {
+        method: 'DELETE',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      }
+    )
+      .then((response: Response) => {
+        toast.success(`${selectedRuntimeTemplateDisplayName} is deleted successfully`);
+        console.log(response);
+      })
+      .catch((err: Error) => {
+        console.error('Error deleting session', err);
+        toast.error(`Failed to delete the session ${selectedRuntimeTemplateDisplayName}`);
+      });
   }
-});
+};
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/handler/handler.ts` & `dataproc_jupyter_plugin-0.1.9/src/handler/handler.ts`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,16 @@
   // Make request to Jupyter API
   const settings = ServerConnection.makeSettings();
   const requestUrl = URLExt.join(settings.baseUrl, 'dataproc-plugin', endPoint);
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
-  } catch (error) {
-    throw new ServerConnection.NetworkError(error as Error);
+  } catch (error: any) {
+    throw new ServerConnection.NetworkError(error);
   }
 
   let data: any = await response.text();
 
   if (data.length > 0) {
     try {
       data = JSON.parse(data);
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/jobs/jobDetails.tsx` & `dataproc_jupyter_plugin-0.1.9/src/jobs/jobDetails.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -14,45 +14,53 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 import React, { useEffect, useRef, useState } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
 import LeftArrowIcon from '../../style/icons/left_arrow_icon.svg';
+import 'semantic-ui-css/semantic.min.css';
 import CloneJobIcon from '../../style/icons/clone_job_icon.svg';
 import StopClusterIcon from '../../style/icons/stop_cluster_icon.svg';
 import StopClusterDisableIcon from '../../style/icons/stop_cluster_disable_icon.svg';
 import DeleteClusterIcon from '../../style/icons/delete_cluster_icon.svg';
 import EditIcon from '../../style/icons/edit_icon.svg';
 import EditIconDisable from '../../style/icons/edit_icon_disable.svg';
 import DeletePopup from '../utils/deletePopup';
-import { JOB_FIELDS_EXCLUDED, STATUS_RUNNING } from '../utils/const';
 import {
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
+  JOB_FIELDS_EXCLUDED,
+  LABEL_TEXT,
+  STATUS_RUNNING
+} from '../utils/const';
+import {
+  authApi,
   elapsedTime,
   jobDetailsOptionalDisplay,
   jobTimeFormat,
   jobTypeDisplay,
   jobTypeValue,
   jobTypeValueArguments,
-  statusMessage,
-  toastifyCustomStyle
+  statusMessage
 } from '../utils/utils';
 
 import ClusterDetails from '../cluster/clusterDetails';
+import { ClipLoader } from 'react-spinners';
 import LabelProperties from './labelProperties';
 import SubmitJob from './submitJob';
 import ViewLogs from '../utils/viewLogs';
-import { toast } from 'react-toastify';
+import { toast, ToastContainer } from 'react-toastify';
 import 'react-toastify/dist/ReactToastify.css';
 import { statusDisplay } from '../utils/statusDisplay';
-import { JobService } from './jobServices';
+import { stopJobApi, deleteJobApi } from '../utils/jobServices';
 import errorIcon from '../../style/icons/error_icon.svg';
 import PollingTimer from '../utils/pollingTimer';
 import { IJobDetails } from '../utils/jobDetailsInterface';
-import { CircularProgress } from '@mui/material';
 
 const iconLeftArrow = new LabIcon({
   name: 'launcher:left-arrow-icon',
   svgstr: LeftArrowIcon
 });
 const iconCloneJob = new LabIcon({
   name: 'launcher:clone-job-icon',
@@ -79,28 +87,30 @@
   svgstr: EditIconDisable
 });
 const iconError = new LabIcon({
   name: 'launcher:error-icon',
   svgstr: errorIcon
 });
 interface IJobDetailsProps {
-  jobSelected: string;
+  jobSelected: any;
   setDetailedJobView: (value: boolean) => void;
+  stopJobApi: (jobId: string) => Promise<void>;
+  deleteJobApi: (jobId: string) => Promise<void>;
   region: any;
   setDetailedView: (value: boolean) => void;
-  clusterResponse: object;
-  fromPage: string;
+  clusterResponse: any;
+  clustersList: object;
 }
 function JobDetails({
   jobSelected,
   setDetailedJobView,
   region,
   setDetailedView,
   clusterResponse,
-  fromPage
+  clustersList
 }: IJobDetailsProps) {
   const initialJobDetails: IJobDetails = {
     status: { state: '', stateStartTime: '' },
     statusHistory: [{ stateStartTime: '' }],
     labels: {},
     reference: { jobId: '' },
     jobUuid: '',
@@ -142,16 +152,16 @@
     },
     placement: { clusterName: '' }
   };
   const [jobInfo, setjobInfo] = useState<IJobDetails>({ ...initialJobDetails });
   const [jobInfoResponse, setjobInfoResponse] = useState<IJobDetails>({
     ...initialJobDetails
   });
-  const key: string[] | (() => string[]) = [];
-  const value: string[] | (() => string[]) = [];
+  const key: any[] | (() => any[]) = [];
+  const value: any[] | (() => any[]) = [];
   const [labelEditMode, setLabelEditMode] = useState(false);
   const [labelDetail, setLabelDetail] = useState(key); //Final label value is stored
   const [labelDetailUpdated, setLabelDetailUpdated] = useState(value); //temporary storage to validate the label data being typed
   const [detailedClusterView, setDetailedClusterView] = useState(false);
   const [isLoading, setIsLoading] = useState(true);
   const [selectedJobClone, setSelectedJobClone] = useState({});
   const [submitJobView, setSubmitJobView] = useState(false);
@@ -178,15 +188,15 @@
   const handleDetailedJobView = () => {
     pollingJobDetails(getJobDetails, true);
     setDetailedJobView(false);
   };
 
   const handleDetailedClusterView = () => {
     pollingJobDetails(getJobDetails, true);
-    if (fromPage !== 'clusters') {
+    if (!clustersList) {
       setDetailedJobView(false);
     }
     setDetailedClusterView(true);
   };
 
   useEffect(() => {
     if (labelEditMode) {
@@ -196,38 +206,65 @@
       pollingJobDetails(getJobDetails, false);
     }
 
     return () => {
       pollingJobDetails(getJobDetails, true);
     };
   }, [labelEditMode]);
+
   const handleJobLabelEdit = () => {
     setLabelEditMode(true);
     setLabelDetailUpdated(labelDetail);
   };
   const handleDeleteJob = (jobId: string) => {
     setSelectedJobId(jobId);
     setDeletePopupOpen(true);
   };
   const handleStopJob = async (jobId: string) => {
     setSelectedJobId(jobId);
-    await JobService.stopJobApi(selectedJobId);
+    await stopJobApi(selectedJobId);
   };
   const handleCancelDelete = () => {
     setDeletePopupOpen(false);
   };
 
   const handleDelete = async () => {
-    await JobService.deleteJobApi(selectedJobId);
+    await deleteJobApi(selectedJobId);
     setDeletePopupOpen(false);
     handleDetailedJobView();
   };
 
   const updateJobDetails = async (payloadJob: object) => {
-    await JobService.updateJobDetailsService(payloadJob, jobSelected);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/jobs/${jobSelected}?updateMask=${LABEL_TEXT}`,
+        {
+          method: 'PATCH',
+          body: JSON.stringify(payloadJob),
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResultJob: Response) => {
+              toast.success(`Request to update job ${jobSelected} submitted`);
+              console.log(responseResultJob);
+            })
+            .catch((e: Error) => console.error(e));
+        })
+        .catch((err: Error) => {
+          console.error('Error in updating job', err);
+          toast.error(`Failed to update the job ${jobSelected}`);
+        });
+    }
   };
 
   const handleSaveEdit = () => {
     const payload = jobInfoResponse;
     const labelObject: { [key: string]: string } = {};
     labelDetailUpdated.forEach((label: string) => {
       /*
@@ -238,57 +275,81 @@
 
       const key = labelParts[0];
       const value = labelParts[1];
       labelObject[key] = value;
     });
     payload.labels = labelObject;
     updateJobDetails(payload);
-    toast.success(
-      `Request to update job ${jobSelected} submitted`,
-      toastifyCustomStyle
-    );
     setLabelEditMode(false);
     getJobDetails();
   };
 
   const handleCancelEdit = () => {
     setLabelEditMode(false);
   };
 
   const getJobDetails = async () => {
-    await JobService.getJobDetailsService(
-      jobSelected,
-      setErrorView,
-      setIsLoading,
-      setjobInfoResponse,
-      setjobInfo,
-      setLabelDetail,
-      setSelectedJobClone
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/jobs/${jobSelected}`,
+        {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              setjobInfoResponse(responseResult);
+              const labelValue: string[] = [];
+              if (responseResult.labels) {
+                for (const [key, value] of Object.entries(
+                  responseResult.labels
+                )) {
+                  labelValue.push(`${key}:${value}`);
+                }
+              }
+              setjobInfo(responseResult);
+              setLabelDetail(labelValue);
+              setIsLoading(false);
+              setSelectedJobClone(responseResult);
+            })
+            .catch((e: Error) => {
+              console.error(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error in getting job details', err);
+          toast.error(`Failed to fetch job details ${jobSelected}`);
+        });
+    }
   };
 
-  const startTime = !errorView
-    ? jobTimeFormat(jobInfo.statusHistory[0].stateStartTime)
-    : '';
-  const job = !errorView ? jobTypeValue(jobInfo) : '';
-  const jobType = !errorView ? jobTypeDisplay(job) : '';
-  const jobArgument = !errorView ? jobTypeValueArguments(jobInfo) : '';
-  const jobTypeConcat = !errorView ? jobArgument + 'Job' : '';
+  const startTime = jobTimeFormat(jobInfo.statusHistory[0].stateStartTime);
+  const job = jobTypeValue(jobInfo);
+  const jobType = jobTypeDisplay(job);
+  const jobArgument = jobTypeValueArguments(jobInfo);
+  const jobTypeConcat = jobArgument + 'Job';
   //@ts-ignore string used as index
-  const argumentsList = !errorView ? jobInfo[jobTypeConcat].args : '';
-  const statusMsg = !errorView ? statusMessage(jobInfo) : '';
-  const endTime = !errorView
-    ? new Date(jobInfo.status.stateStartTime)
-    : new Date();
-  const jobStartTime = !errorView
-    ? new Date(jobInfo.statusHistory[0].stateStartTime)
-    : new Date();
+  const argumentsList = jobInfo[jobTypeConcat].args;
+  const statusMsg = statusMessage(jobInfo);
+  const endTime = new Date(jobInfo.status.stateStartTime);
+  const jobStartTime = new Date(
+    jobInfo.statusHistory[jobInfo.statusHistory.length - 1].stateStartTime
+  );
+  const elapsedTimeString = elapsedTime(endTime, jobStartTime);
 
-  let elapsedTimeString = !errorView ? elapsedTime(endTime, jobStartTime) : '';
-  const statusStyleSelection = (jobInfo: IJobDetails) => {
+  const statusStyleSelection = (jobInfo: any) => {
     if (jobInfo.status.state === STATUS_RUNNING) {
       return 'action-cluster-section'; //CSS class
     } else {
       return 'action-cluster-section disabled';
     }
   };
 
@@ -315,23 +376,20 @@
   return (
     <div>
       {errorView && (
         <div className="error-view-parent">
           <div
             role="button"
             className="back-arrow-icon"
-            onClick={() => handleDetailedJobView()}
+            onClick={() => setErrorView(false)}
           >
-            <iconLeftArrow.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
+            <iconLeftArrow.react tag="div" />
           </div>
           <div className="error-view-message-parent">
-            <iconError.react tag="div" className="logo-alignment-style" />
+            <iconError.react tag="div" />
             <div className="error-view-message">
               Unable to find the resource you requested
             </div>
           </div>
         </div>
       )}
       {submitJobView && !detailedClusterView && (
@@ -354,83 +412,69 @@
       {detailedClusterView && (
         <ClusterDetails
           clusterSelected={jobInfo.placement.clusterName}
           setDetailedView={setDetailedView}
           setDetailedClusterView={setDetailedClusterView}
           submitJobView={submitJobView}
           selectedJobClone={selectedJobClone}
+          clusterResponse={clusterResponse}
           setSubmitJobView={setSubmitJobView}
           setDetailedJobView={setDetailedJobView}
           setSelectedJobClone={setSelectedJobClone}
         />
       )}
       {!submitJobView && !detailedClusterView && !errorView && (
-        <div className="scroll">
+        <div className="scroll-comp">
           {jobInfo.jobUuid !== '' && (
             <div>
-              <div className="scroll-fix-header cluster-details-header">
+              <div className="cluster-details-header">
                 <div
                   className="back-arrow-icon"
                   role="button"
                   aria-label="Delete Job"
                   onClick={() => handleDetailedJobView()}
                 >
-                  <iconLeftArrow.react
-                    tag="div"
-                    className="icon-white logo-alignment-style"
-                  />
+                  <iconLeftArrow.react tag="div" />
                 </div>
                 <div className="cluster-details-title">Job details</div>
                 <div
                   role="button"
                   className="action-cluster-section"
                   onClick={() => handleCloneJob()}
                 >
                   <div className="action-cluster-icon">
-                    <iconCloneJob.react
-                      tag="div"
-                      className="logo-alignment-style"
-                    />
+                    <iconCloneJob.react tag="div" />
                   </div>
                   <div className="action-cluster-text">CLONE</div>
                 </div>
 
                 <div
                   role="button"
                   className={statusStyleSelection(jobInfo)}
                   onClick={() =>
                     jobInfo.status.state === STATUS_RUNNING &&
                     handleStopJob(jobInfo.reference.jobId)
                   }
                 >
                   <div className="action-cluster-icon">
                     {jobInfo.status.state === STATUS_RUNNING ? (
-                      <iconStopCluster.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                      <iconStopCluster.react tag="div" />
                     ) : (
-                      <iconStopClusterDisable.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                      <iconStopClusterDisable.react tag="div" />
                     )}
                   </div>
                   <div className="action-cluster-text">STOP</div>
                 </div>
                 <div
                   role="button"
                   className="action-cluster-section"
                   onClick={() => handleDeleteJob(jobInfo.reference.jobId)}
                 >
                   <div className="action-cluster-icon">
-                    <iconDeleteCluster.react
-                      tag="div"
-                      className="logo-alignment-style"
-                    />
+                    <iconDeleteCluster.react tag="div" />
                   </div>
                   <div className="action-cluster-text">DELETE</div>
                 </div>
                 <ViewLogs
                   clusterName={jobInfo.placement.clusterName}
                   setErrorView={setErrorView}
                 />
@@ -452,14 +496,15 @@
                   <div className="cluster-details-label">Type</div>
                   <div className="cluster-details-value">Dataproc Job</div>
                 </div>
                 <div className="row-details">
                   <div className="cluster-details-label">Status</div>
                   {statusDisplay(statusMsg)}
                 </div>
+                <ToastContainer />
               </div>
               <div className="cluster-details-header">
                 <div className="cluster-details-title">Configuration</div>
               </div>
               <div className="job-edit-header">
                 <div
                   role="button"
@@ -537,43 +582,45 @@
                   <div className="row-details">
                     <div className="cluster-details-label">Query script</div>
                     <div className="cluster-details-value">
                       {jobInfo.sparkSqlJob.queryList.queries}
                     </div>
                   </div>
                 )}
-                {Object.keys(jobInfo[jobTypeConcat as keyof IJobDetails]).map(
-                  (titleData: string) => {
-                    //@ts-ignore string used as index
-                    const valueData = jobInfo[jobTypeConcat][titleData];
-                    return (
-                      !JOB_FIELDS_EXCLUDED.includes(titleData) && (
-                        <div className="row-details">
-                          <div className="cluster-details-label">
-                            {jobDetailsOptionalDisplay(titleData)}
-                          </div>
-                          {typeof valueData === 'string' ? (
-                            <div className="cluster-details-value">
-                              {valueData}
+                {
+                  Object.keys(jobInfo[jobTypeConcat as keyof IJobDetails]).map(
+                    (titleData: string) => {
+                      //@ts-ignore string used as index
+                      const valueData = jobInfo[jobTypeConcat][titleData];
+                      return (
+                        !JOB_FIELDS_EXCLUDED.includes(titleData) && (
+                          <div className="row-details">
+                            <div className="cluster-details-label">
+                              {jobDetailsOptionalDisplay(titleData)}
                             </div>
-                          ) : (
-                            valueData.length > 0 &&
-                            !JOB_FIELDS_EXCLUDED.includes(titleData) && (
+                            {typeof valueData === 'string' ? (
                               <div className="cluster-details-value">
-                                {valueData.map((item: string) => {
-                                  return <div>{item}</div>;
-                                })}
+                                {valueData}
                               </div>
-                            )
-                          )}
-                        </div>
-                      )
-                    );
-                  }
-                )}
+                            ) : (
+                              valueData.length > 0 &&
+                              !JOB_FIELDS_EXCLUDED.includes(titleData) && (
+                                <div className="cluster-details-value">
+                                  {valueData.map((item: string) => {
+                                    return <div>{item}</div>;
+                                  })}
+                                </div>
+                              )
+                            )}
+                          </div>
+                        )
+                      );
+                    }
+                  )
+                }
 
                 {jobInfo?.scheduling &&
                   jobInfo.scheduling.maxFailuresPerHour && (
                     <div className="row-details">
                       <div className="cluster-details-label">
                         Max restarts per hour
                       </div>
@@ -633,17 +680,17 @@
                 <div className="job-details-label-row">
                   <div className="cluster-details-label">Labels</div>
                   {!labelEditMode ? (
                     <div className="job-label-style-parent">
                       {labelDetail.length > 0
                         ? labelDetail.map(label => {
                             /*
-                          Extracting key, value from label
-                             Example: "{client:dataproc_jupyter_plugin}"
-                       */
+                            Extracting key, value from label
+                               Example: "{client:dataproc_jupyter_plugin}"
+                         */
                             const labelParts = label.split(':');
 
                             return (
                               <div key={label} className="job-label-style">
                                 {labelParts[0]} : {labelParts[1]}
                               </div>
                             );
@@ -689,31 +736,33 @@
                       >
                         CANCEL
                       </div>
                     </div>
                   </div>
                 )}
               </div>
+              <ToastContainer />
             </div>
           )}
 
           {jobInfo.jobUuid === '' && (
-            <>
+            <div className="loader-full-style">
               {isLoading && (
-                <div className="spin-loader-main">
-                  <CircularProgress
-                    className = "spin-loader-custom-style"
-                    size={18}
+                <div>
+                  <ClipLoader
+                    color="#8A8A8A"
+                    loading={true}
+                    size={20}
                     aria-label="Loading Spinner"
                     data-testid="loader"
                   />
                   Loading Job Details
                 </div>
               )}
-            </>
+            </div>
           )}
         </div>
       )}
     </div>
   );
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/jobs/jobs.tsx` & `dataproc_jupyter_plugin-0.1.9/src/jobs/jobs.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -13,45 +13,58 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 import React, { useState, useEffect, useRef } from 'react';
 import { useTable, useGlobalFilter, usePagination } from 'react-table';
-import { ICellProps } from '../utils/utils';
+import {
+  authApi,
+  jobTimeFormat,
+  jobTypeValue,
+  elapsedTime,
+  statusMessage,
+  jobTypeDisplay,
+  ICellProps
+} from '../utils/utils';
 import { LabIcon } from '@jupyterlab/ui-components';
 import filterIcon from '../../style/icons/filter_icon.svg';
 import cloneIcon from '../../style/icons/clone_icon.svg';
 import stopIcon from '../../style/icons/stop_icon.svg';
 import JobDetails from './jobDetails';
 import stopDisableIcon from '../../style/icons/stop_disable_icon.svg';
 import deleteIcon from '../../style/icons/delete_icon.svg';
 import clusterRunningIcon from '../../style/icons/cluster_running_icon.svg';
 import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
 import SucceededIcon from '../../style/icons/succeeded_icon.svg';
 import SubmitJobIcon from '../../style/icons/submit_job_icon.svg';
 import {
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
   ClusterStatus,
   STATUS_CANCELLED,
   STATUS_CREATING,
   STATUS_DELETING,
   STATUS_FAIL,
   STATUS_PROVISIONING,
   STATUS_STARTING,
   STATUS_STOPPING,
   STATUS_SUCCESS
 } from '../utils/const';
+import ClipLoader from 'react-spinners/ClipLoader';
 import SubmitJob from './submitJob';
 import GlobalFilter from '../utils/globalFilter';
 import TableData from '../utils/tableData';
 import DeletePopup from '../utils/deletePopup';
-import { JobService } from './jobServices';
+import { toast, ToastContainer } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
+import { stopJobApi, deleteJobApi } from '../utils/jobServices';
 import { PaginationView } from '../utils/paginationView';
 import PollingTimer from '../utils/pollingTimer';
-import { CircularProgress } from '@mui/material';
 
 const iconFilter = new LabIcon({
   name: 'launcher:filter-icon',
   svgstr: filterIcon
 });
 const iconClone = new LabIcon({
   name: 'launcher:clone-icon',
@@ -89,29 +102,26 @@
 function JobComponent({
   clusterSelected,
   detailedJobView,
   setDetailedJobView,
   submitJobView,
   setSubmitJobView,
   setDetailedView,
+  clusterResponse,
   selectedJobClone,
   setSelectedJobClone,
-  fromPage
+  clustersList
 }: any) {
-  const controller = useRef(new AbortController());
   const [jobsList, setjobsList] = useState([]);
-  const [jobSelected, setjobSelected] = useState<string>('');
+  const [jobSelected, setjobSelected] = useState({});
   const [isLoading, setIsLoading] = useState(true);
   const [pollingDisable, setPollingDisable] = useState(false);
   const [region, setRegion] = useState('');
   const [deletePopupOpen, setDeletePopupOpen] = useState(false);
   const [selectedJobId, setSelectedJobId] = useState('');
-
-  const [clusterResponse, setClusterResponse] = useState([]);
-
   const timer = useRef<NodeJS.Timeout | undefined>(undefined);
 
   const pollingJobs = async (
     pollingFunction: () => void,
     pollingDisable: boolean
   ) => {
     timer.current = PollingTimer(
@@ -179,39 +189,108 @@
   };
   const handleDeleteJob = (jobId: string) => {
     setSelectedJobId(jobId);
     setDeletePopupOpen(true);
   };
   const handleStopJob = async (jobId: string) => {
     setSelectedJobId(jobId);
-    await JobService.stopJobApi(jobId);
+    await stopJobApi(jobId);
   };
   const handleCancelDelete = () => {
     setDeletePopupOpen(false);
   };
 
   const handleDelete = async () => {
-    await JobService.deleteJobApi(selectedJobId);
+    await deleteJobApi(selectedJobId);
     setDeletePopupOpen(false);
   };
 
-  const listJobsAPI = async () => {
-    controller.current.abort(); 
-    controller.current = new AbortController(); 
-    await JobService.listJobsAPIService(
-      clusterSelected,
-      setIsLoading,
-      setjobsList,
-      renderActions,
-      controller.current.signal 
-    );
-  };
-
-  const listClustersAPI = async () => {
-    await JobService.listClustersAPIService(setClusterResponse);
+  const listJobsAPI = async (
+    nextPageToken?: string,
+    previousJobsList?: object
+  ) => {
+    const credentials = await authApi();
+    const clusterName = clusterSelected ?? '';
+    const pageToken = nextPageToken ?? '';
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/jobs?pageSize=50&pageToken=${pageToken}&&clusterName=${clusterName}`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              let transformJobListData = [];
+              if (responseResult && responseResult.jobs) {
+                transformJobListData = responseResult.jobs.map((data: any) => {
+                  const startTime = jobTimeFormat(
+                    data.statusHistory[0].stateStartTime
+                  );
+                  const job = jobTypeValue(data);
+                  const jobType = jobTypeDisplay(job);
+                  const endTime = data.status.stateStartTime;
+                  const jobStartTime = new Date(
+                    data.statusHistory[0].stateStartTime
+                  );
+
+                  const elapsedTimeString = elapsedTime(endTime, jobStartTime);
+
+                  const statusMsg = statusMessage(data);
+
+                  const labelvalue = [];
+                  if (data.labels) {
+                    for (const [key, value] of Object.entries(data.labels)) {
+                      labelvalue.push(`${key} : ${value}`);
+                    }
+                  } else {
+                    labelvalue.push('None');
+                  }
+                  return {
+                    jobid: data.reference.jobId,
+                    status: statusMsg,
+                    region: credentials.region_id,
+                    type: jobType,
+                    starttime: startTime,
+                    elapsedtime: elapsedTimeString,
+                    labels: labelvalue,
+                    actions: renderActions(data)
+                  };
+                });
+              }
+              const existingJobsData = previousJobsList ?? [];
+              //setStateAction never type issue
+              let allJobsData: any = [
+                ...(existingJobsData as []),
+                ...transformJobListData
+              ];
+
+              if (responseResult.nextPageToken) {
+                listJobsAPI(responseResult.nextPageToken, allJobsData);
+              } else {
+                setjobsList(allJobsData);
+                setIsLoading(false);
+              }
+            })
+            .catch((e: Error) => {
+              console.error(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error listing jobs', err);
+          toast.error('Failed to fetch jobs');
+        });
+    }
   };
 
   const handleCloneJob = (data: object) => {
     setSubmitJobView(true);
     setSelectedJobClone(data);
   };
   const renderActions = (data: {
@@ -224,18 +303,15 @@
       <div className="actions-icon">
         <div
           role="button"
           className="icon-buttons-style"
           title="Clone Job"
           onClick={() => handleCloneJob(data)}
         >
-          <iconClone.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconClone.react tag="div" />
         </div>
         <div
           role="button"
           aria-disabled={data.status.state !== ClusterStatus.STATUS_RUNNING}
           className={
             data.status.state === ClusterStatus.STATUS_RUNNING
               ? 'icon-buttons-style'
@@ -245,23 +321,17 @@
           onClick={
             data.status.state === ClusterStatus.STATUS_RUNNING
               ? () => handleStopJob(jobId)
               : undefined
           }
         >
           {data.status.state === ClusterStatus.STATUS_RUNNING ? (
-            <iconStop.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
+            <iconStop.react tag="div" />
           ) : (
-            <iconStopDisable.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
+            <iconStopDisable.react tag="div" />
           )}
         </div>
         <div
           role="button"
           aria-disabled={data.status.state !== ClusterStatus.STATUS_RUNNING}
           className={
             data.status.state === ClusterStatus.STATUS_RUNNING
@@ -271,41 +341,35 @@
           title="Delete Job"
           onClick={
             data.status.state !== ClusterStatus.STATUS_RUNNING
               ? () => handleDeleteJob(jobId)
               : undefined
           }
         >
-          <iconDelete.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          {data.status.state === ClusterStatus.STATUS_RUNNING ? (
+            <iconDelete.react tag="div" />
+          ) : (
+            <iconDelete.react tag="div" />
+          )}
         </div>
       </div>
     );
   };
 
   useEffect(() => {
-    if (!pollingDisable) {
-      listJobsAPI();
-      listClustersAPI();
+    listJobsAPI();
+    if (!detailedJobView) {
+      pollingJobs(listJobsAPI, pollingDisable);
     }
+
     return () => {
-      controller.current.abort();
-      if (timer.current) {
-        clearTimeout(timer.current);
-      }
+      pollingJobs(listJobsAPI, true);
     };
   }, [pollingDisable, detailedJobView]);
-  
-  useEffect(() => {
-    if (!detailedJobView && !isLoading) {
-      pollingJobs(listJobsAPI, pollingDisable);
-    }
-  }, [isLoading]);
+
   const tableDataCondition = (cell: ICellProps) => {
     if (cell.column.Header === 'Job ID') {
       return (
         <td
           role="button"
           {...cell.getCellProps()}
           className="cluster-name"
@@ -316,37 +380,27 @@
       );
     }
     if (cell.column.Header === 'Status' && cell.value) {
       return (
         <td {...cell.getCellProps()} className="clusters-table-data">
           <div key="Status" className="cluster-status-parent">
             {cell.value === ClusterStatus.STATUS_RUNNING && (
-              <iconClusterRunning.react
-                tag="div"
-                className="logo-alignment-style"
-              />
-            )}
-            {cell.value === STATUS_CANCELLED && (
-              <iconStop.react tag="div" className="logo-alignment-style" />
-            )}
-            {cell.value === STATUS_FAIL && (
-              <iconClusterError.react
-                tag="div"
-                className="logo-alignment-style"
-              />
-            )}
-            {cell.value === STATUS_SUCCESS && (
-              <iconSucceeded.react tag="div" className="logo-alignment-style" />
+              <iconClusterRunning.react tag="div" />
             )}
+            {cell.value === STATUS_CANCELLED && <iconStop.react tag="div" />}
+            {cell.value === STATUS_FAIL && <iconClusterError.react tag="div" />}
+            {cell.value === STATUS_SUCCESS && <iconSucceeded.react tag="div" />}
             {(cell.value === STATUS_PROVISIONING ||
               cell.value === STATUS_CREATING ||
               cell.value === STATUS_STARTING ||
               cell.value === STATUS_STOPPING ||
               cell.value === STATUS_DELETING) && (
-              <CircularProgress
+              <ClipLoader
+                color="#8A8A8A"
+                loading={true}
                 size={15}
                 aria-label="Loading Spinner"
                 data-testid="loader"
               />
             )}
             <div className="cluster-status">{cell.value.toLowerCase()}</div>
           </div>
@@ -397,14 +451,15 @@
     { columns, data, autoResetPage: false, initialState: { pageSize: 50 } },
     useGlobalFilter,
     usePagination
   );
 
   return (
     <div>
+      <ToastContainer />
       {submitJobView && !detailedJobView && (
         <SubmitJob
           setSubmitJobView={setSubmitJobView}
           selectedJobClone={selectedJobClone}
           clusterResponse={clusterResponse}
         />
       )}
@@ -418,65 +473,63 @@
           }
         />
       )}
       {!submitJobView && detailedJobView && (
         <JobDetails
           jobSelected={jobSelected}
           setDetailedJobView={setDetailedJobView}
+          stopJobApi={stopJobApi}
+          deleteJobApi={deleteJobApi}
           region={region}
           setDetailedView={setDetailedView}
           clusterResponse={clusterResponse}
-          fromPage={fromPage}
+          clustersList={clustersList}
         />
       )}
       {!submitJobView && !detailedJobView && (
         <div>
-          {clusterResponse && clusterResponse.length > 0 && (
-            <div className="create-cluster-overlay">
-              <div
-                role="button"
-                className="create-cluster-sub-overlay"
-                onClick={() => {
-                  handleSubmitJobOpen();
-                }}
-              >
-                <div className="create-icon">
-                  <iconSubmitJob.react
-                    tag="div"
-                    className="logo-alignment-style"
-                  />
+          {clusterResponse &&
+            clusterResponse.clusters &&
+            clusterResponse.clusters.length > 0 && (
+              <div className="create-cluster-overlay">
+                <div
+                  role="button"
+                  className="create-cluster-sub-overlay"
+                  onClick={() => {
+                    handleSubmitJobOpen();
+                  }}
+                >
+                  <div className="create-cluster-icon">
+                    <iconSubmitJob.react tag="div" />
+                  </div>
+                  <div className="create-cluster-text">SUBMIT JOB</div>
                 </div>
-                <div className="create-text">SUBMIT JOB</div>
               </div>
-            </div>
-          )}
+            )}
           {jobsList.length > 0 ? (
             <div>
               <div className="filter-cluster-overlay">
                 <div className="filter-cluster-icon">
-                  <iconFilter.react
-                    tag="div"
-                    className="icon-white logo-alignment-style"
-                  />
+                  <iconFilter.react tag="div" />
                 </div>
                 <div className="filter-cluster-text"></div>
                 <div className="filter-cluster-section">
                   <GlobalFilter
                     preGlobalFilteredRows={preGlobalFilteredRows}
                     globalFilter={state.globalFilter}
                     setGlobalFilter={setGlobalFilter}
                     setPollingDisable={setPollingDisable}
                   />
                 </div>
               </div>
               <div
                 className={
-                  clusterSelected
-                    ? 'jobs-list-table-parent-small'
-                    : 'jobs-list-table-parent'
+                  clusterResponse
+                    ? 'jobs-list-table-parent'
+                    : 'jobs-list-table-parent-small'
                 }
               >
                 <TableData
                   getTableProps={getTableProps}
                   headerGroups={headerGroups}
                   getTableBodyProps={getTableBodyProps}
                   isLoading={isLoading}
@@ -499,17 +552,18 @@
                   />
                 )}
               </div>
             </div>
           ) : (
             <div>
               {isLoading && (
-                <div className="spin-loader-main">
-                  <CircularProgress
-                    className = "spin-loader-custom-style"
+                <div className="spin-loaderMain">
+                  <ClipLoader
+                    color="#8A8A8A"
+                    loading={true}
                     size={20}
                     aria-label="Loading Spinner"
                     data-testid="loader"
                   />
                   Loading Jobs
                 </div>
               )}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/jobs/labelProperties.tsx` & `dataproc_jupyter_plugin-0.1.9/src/jobs/labelProperties.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 import React, { useEffect } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
 import plusIcon from '../../style/icons/plus_icon.svg';
 import plusIconDisable from '../../style/icons/plus_icon_disable.svg';
 import deleteIcon from '../../style/icons/delete_icon.svg';
 import errorIcon from '../../style/icons/error_icon.svg';
+import { Input } from 'semantic-ui-react';
 import { DEFAULT_LABEL_DETAIL } from '../utils/const';
-import { Input } from '../controls/MuiWrappedInput';
 
 const iconPlus = new LabIcon({
   name: 'launcher:plus-icon',
   svgstr: plusIcon
 });
 const iconPlusDisable = new LabIcon({
   name: 'launcher:plus-disable-icon',
@@ -51,42 +51,32 @@
   keyValidation,
   setKeyValidation,
   valueValidation,
   setValueValidation,
   duplicateKeyError,
   setDuplicateKeyError,
   labelEditMode,
-  selectedRuntimeClone,
-  batchInfoResponse,
-  createBatch,
-  fromPage
+  selectedRuntimeClone
 }: any) {
-  /*
-  labelDetail used to store the permanent label details when onblur
-  labelDetailUpdated used to store the temporay label details when onchange
+  /* 
+  labelDetail used to store the permanent label details when onblur 
+  labelDetailUpdated used to store the temporay label details when onchange 
   */
   useEffect(() => {
-    if (!labelEditMode && fromPage !== 'scheduler') {
-      if (
-        buttonText === 'ADD LABEL' &&
-        !selectedJobClone &&
-        selectedRuntimeClone === undefined &&
-        !createBatch
-      ) {
+    if (!labelEditMode) {
+      if (buttonText === 'ADD LABEL' && !selectedJobClone && selectedRuntimeClone===undefined) {
         setLabelDetail([DEFAULT_LABEL_DETAIL]);
         setLabelDetailUpdated([DEFAULT_LABEL_DETAIL]);
       } else {
-        setLabelDetailUpdated([]);
         setLabelDetail([]);
       }
     }
   }, []);
 
-  const handleAddLabel = (event: React.MouseEvent<HTMLElement>) => {
-    event.preventDefault();
+  const handleAddLabel = () => {
     const labelAdd = [...labelDetail];
     labelAdd.push(':');
     setLabelDetailUpdated(labelAdd);
     setLabelDetail(labelAdd);
   };
 
   const handleDeleteLabel = (index: number, value: string) => {
@@ -103,80 +93,80 @@
     if (duplicateKeyError === -1) {
       setLabelDetail(labelDetailUpdated);
     }
   };
   const handleEditLabel = (value: string, index: number, keyValue: string) => {
     const labelEdit = [...labelDetail];
 
-    labelEdit.forEach((data, dataNumber: number) => {
+    labelEdit.forEach((data, dataNumber: any) => {
       if (index === dataNumber) {
         /*
           allowed aplhanumeric and spaces and underscores
         */
         const regexp = /^[a-z0-9-_]+$/;
         if (keyValue === 'key') {
           if (
-            (value.search(regexp) === -1 ||
-              value.charAt(0) !== value.charAt(0).toLowerCase()) &&
-            buttonText === 'ADD LABEL'
+            value.search(regexp) === -1 ||
+            value.charAt(0) !== value.charAt(0).toLowerCase()
           ) {
             setKeyValidation(index);
           } else {
             setKeyValidation(-1);
           }
 
           // Check for duplicate key when editing
           const newKey = value;
           const duplicateIndex = labelEdit.findIndex(
             (label, i) => i !== index && label.split(':')[0] === newKey
           );
-          if (duplicateIndex !== -1 && buttonText === 'ADD LABEL') {
+          if (duplicateIndex !== -1) {
             setDuplicateKeyError(index);
           } else {
             setDuplicateKeyError(-1);
           }
 
           data = data.replace(data.split(':')[0], value);
         } else {
-          if (value.search(regexp) === -1 && buttonText === 'ADD LABEL') {
+          if (value.search(regexp) === -1) {
             setValueValidation(index);
           } else {
             setValueValidation(-1);
           }
           /*
-          value is split from labels
+          value is split from labels 
           Example:"client:dataproc_jupyter_plugin"
           */
           if (data.split(':')[1] === '') {
             data = data + value;
           } else {
             data = data.replace(data.split(':')[1], value);
           }
         }
       }
       labelEdit[dataNumber] = data;
     });
+
     setLabelDetailUpdated(labelEdit);
   };
 
-  const styleAddLabelButton = (buttonText: string, labelDetail: string) => {
+  const styleAddLabelButton = (buttonText: string, labelDetail: any) => {
     if (
       buttonText === 'ADD LABEL' &&
       (labelDetail.length === 0 ||
         labelDetail[labelDetail.length - 1].split(':')[0].length > 0) &&
       duplicateKeyError === -1
     ) {
       return 'job-add-label-button';
     } else if (
       buttonText === 'ADD LABEL' &&
       (labelDetail.length === 0 ||
         labelDetail[labelDetail.length - 1].split(':')[0].length === 0) &&
       duplicateKeyError !== -1
     ) {
-      return 'job-add-property-button-disabled';
+      return 'job-add-label-button-disabled';
     } else if (
       buttonText !== 'ADD LABEL' &&
       (labelDetail.length === 0 ||
         labelDetail[labelDetail.length - 1].split(':')[0].length > 0)
     ) {
       return 'job-add-property-button';
     } else {
@@ -184,130 +174,96 @@
     }
   };
 
   return (
     <div>
       <div className="job-label-edit-parent">
         {labelDetail.length > 0 &&
-          labelDetail.map((label: string, index: number) => {
+          labelDetail.map((label: any, index: number) => {
             /*
                      Extracting key, value from label
                       Example: "{client:dataProc_plugin}"
                   */
             const labelSplit = label.split(':');
 
             return (
               <div key={label}>
                 <div className="job-label-edit-row">
                   <div className="key-message-wrapper">
-                    <div className="select-text-overlay-label">
-                      <Input
-                        sx={{ margin: 0 }}
-                        className={`edit-input-style ${
-                          labelSplit[0] === '' ||
-                          buttonText !== 'ADD LABEL' ||
-                          duplicateKeyError !== -1
-                            ? ''
-                            : ' disable-text'
-                        }`}
-                        disabled={
-                          labelSplit[0] === '' ||
-                          buttonText !== 'ADD LABEL' ||
-                          duplicateKeyError !== -1
-                            ? false
-                            : true
-                        }
-                        onBlur={() => handleEditLabelSwitch()}
-                        onChange={e =>
-                          handleEditLabel(e.target.value, index, 'key')
-                        }
-                        defaultValue={labelSplit[0]}
-                        Label={`Key ${index + 1}*`}
-                      />
-                    </div>
-
-                    {labelDetailUpdated[index].split(':')[0] === '' &&
-                    labelDetailUpdated[index] !== '' &&
-                    duplicateKeyError !== index ? (
+                    <Input
+                      placeholder={`Key ${index + 1}*`}
+                      className="edit-input-style"
+                      disabled={
+                        labelSplit[0] === '' ||
+                        buttonText !== 'ADD LABEL' ||
+                        duplicateKeyError !== -1
+                          ? false
+                          : true
+                      }
+                      onBlur={() => handleEditLabelSwitch()}
+                      onChange={e =>
+                        handleEditLabel(e.target.value, index, 'key')
+                      }
+                      defaultValue={labelSplit[0]}
+                    />
+
+                    {labelDetailUpdated[index].split(':')[0] === '' ? (
                       <div role="alert" className="error-key-parent">
-                        <iconError.react
-                          tag="div"
-                          className="logo-alignment-style"
-                        />
+                        <iconError.react tag="div" />
                         <div className="error-key-missing">key is required</div>
                       </div>
                     ) : (
                       keyValidation === index &&
                       buttonText === 'ADD LABEL' && (
                         <div className="error-key-parent">
-                          <iconError.react
-                            tag="div"
-                            className="logo-alignment-style"
-                          />
+                          <iconError.react tag="div" />
                           <div className="error-key-missing">
                             Only hyphens (-), underscores (_), lowercase
                             characters, and numbers are allowed. Keys must start
                             with a lowercase character. International characters
                             are allowed.
                           </div>
                         </div>
                       )
                     )}
                     {duplicateKeyError === index &&
                       buttonText === 'ADD LABEL' && (
                         <div className="error-key-parent">
-                          <iconError.react
-                            tag="div"
-                            className="logo-alignment-style"
-                          />
+                          <iconError.react tag="div" />
                           <div className="error-key-missing">
                             The key is already present
                           </div>
                         </div>
                       )}
                   </div>
                   <div className="key-message-wrapper">
-                    <div className="select-text-overlay-label">
-                      <Input
-                        sx={{ margin: 0 }}
-                        className={`edit-input-style ${
-                          label === DEFAULT_LABEL_DETAIL &&
-                          buttonText === 'ADD LABEL'
-                            ? ' disable-text'
-                            : ''
-                        }`}
-                        onBlur={() => handleEditLabelSwitch()}
-                        onChange={e =>
-                          handleEditLabel(e.target.value, index, 'value')
-                        }
-                        disabled={
-                          label === DEFAULT_LABEL_DETAIL &&
-                          buttonText === 'ADD LABEL'
-                        }
-                        defaultValue={
-                          labelSplit.length > 2
-                            ? labelSplit[1] + ':' + labelSplit[2]
-                            : labelSplit[1]
-                        }
-                        Label={`Value ${index + 1}`}
-                      />
-                    </div>
-                    {valueValidation === index && (
-                      <div className="error-key-parent">
-                        <iconError.react
-                          tag="div"
-                          className="logo-alignment-style"
-                        />
-                        <div className="error-key-missing">
-                          Only hyphens (-), underscores (_), lowercase
-                          characters, and numbers are allowed. International
-                          characters are allowed.
+                    <Input
+                      placeholder={`Value ${index + 1}`}
+                      className="edit-input-style"
+                      onBlur={() => handleEditLabelSwitch()}
+                      onChange={e =>
+                        handleEditLabel(e.target.value, index, 'value')
+                      }
+                      disabled={
+                        label === DEFAULT_LABEL_DETAIL &&
+                        buttonText === 'ADD LABEL'
+                      }
+                      defaultValue={labelSplit[1]}
+                    />
+                    {valueValidation === index &&
+                      buttonText === 'ADD LABEL' && (
+                        <div className="error-key-parent">
+                          <iconError.react tag="div" />
+                          <div className="error-key-missing">
+                            Only hyphens (-), underscores (_), lowercase
+                            characters, and numbers are allowed. International
+                            characters are allowed.
+                          </div>
                         </div>
-                      </div>
-                    )}
+                      )}
                   </div>
 
                   <div
                     role="button"
                     className={
                       label === DEFAULT_LABEL_DETAIL &&
                       buttonText === 'ADD LABEL'
@@ -321,66 +277,46 @@
                           buttonText === 'ADD LABEL'
                         )
                       ) {
                         handleDeleteLabel(index, labelSplit[0]);
                       }
                     }}
                   >
-                    <iconDelete.react
-                      tag="div"
-                      className="logo-alignment-style"
-                    />
+                    <iconDelete.react tag="div" />
                   </div>
                   <></>
                 </div>
               </div>
             );
           })}
-        <button
+        <div
+          role="button"
           className={styleAddLabelButton(buttonText, labelDetail)}
-          onClick={e => {
-            const buttonClasses = e.currentTarget.className;
-            const isDisabled =
-              buttonClasses.includes('job-add-label-button-disabled') ||
-              buttonClasses.includes('job-add-property-button-disabled');
-
-            if (!isDisabled) {
-              if (
-                labelDetail.length === 0 ||
-                labelDetail[labelDetail.length - 1].split(':')[0].length > 0
-              ) {
-                handleAddLabel(e);
-              }
-            } else {
-              e.preventDefault();
-            }
+          onClick={() => {
+            (labelDetail.length === 0 ||
+              labelDetail[labelDetail.length - 1].split(':')[0].length > 0) &&
+              handleAddLabel();
           }}
         >
           {labelDetail.length === 0 ||
           labelDetail[labelDetail.length - 1].split(':')[0].length > 0 ? (
-            <iconPlus.react
-              tag="div"
-              className="icon-black logo-alignment-style"
-            />
+            <iconPlus.react tag="div" />
           ) : (
-            <iconPlusDisable.react
-              tag="div"
-              className="icon-black-disable logo-alignment-style"
-            />
+            <iconPlusDisable.react tag="div" />
           )}
-          <span
+          <div
             className={
               labelDetail.length === 0 ||
               labelDetail[labelDetail.length - 1].split(':')[0].length > 0
                 ? 'job-edit-text'
                 : 'job-edit-text-disabled'
             }
           >
             {buttonText}
-          </span>
-        </button>
+          </div>
+        </div>
       </div>
     </div>
   );
 }
 
 export default LabelProperties;
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/jobs/submitJob.tsx` & `dataproc_jupyter_plugin-0.1.9/src/jobs/submitJob.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -11,37 +11,40 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-import React, { SyntheticEvent, useEffect, useState } from 'react';
+import React, { useEffect, useState } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
 import LeftArrowIcon from '../../style/icons/left_arrow_icon.svg';
+import { Input, Select } from 'semantic-ui-react';
+import 'semantic-ui-css/semantic.min.css';
 import LabelProperties from './labelProperties';
 import { authApi } from '../utils/utils';
-
+import TagsInput from 'react-tagsinput';
+import 'react-tagsinput/react-tagsinput.css';
 import {
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
   ARCHIVE_FILES_MESSAGE,
   ARGUMENTS_MESSAGE,
+  BASE_URL,
   FILES_MESSAGE,
   JAR_FILE_MESSAGE,
   MAIN_CLASS_MESSAGE,
   MAX_RESTART_MESSAGE,
   QUERY_FILE_MESSAGE,
   RESTART_JOB_URL,
   STATUS_RUNNING
 } from '../utils/const';
 import errorIcon from '../../style/icons/error_icon.svg';
-import { Input } from '../controls/MuiWrappedInput';
-import { DropdownProps } from 'semantic-ui-react';
-import { Autocomplete, TextField } from '@mui/material';
-import { MuiChipsInput } from 'mui-chips-input';
-import { JobService } from './jobServices';
+import { toast, ToastContainer } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
 
 const iconLeftArrow = new LabIcon({
   name: 'launcher:left-arrow-icon',
   svgstr: LeftArrowIcon
 });
 const iconError = new LabIcon({
   name: 'launcher:error-icon',
@@ -55,77 +58,76 @@
     if (key.endsWith('Job')) {
       jobKeys.push(key);
     }
   }
   return jobKeys;
 }
 function jobTypeFunction(jobKey: string) {
-  let jobType = 'Spark';
+  let jobType = 'spark';
   switch (jobKey) {
     case 'sparkRJob':
-      jobType = 'SparkR';
+      jobType = 'sparkR';
       return jobType;
     case 'pysparkJob':
-      jobType = 'PySpark';
+      jobType = 'pySpark';
       return jobType;
     case 'sparkSqlJob':
-      jobType = 'SparkSql';
+      jobType = 'sparkSql';
       return jobType;
     default:
       return jobType;
   }
 }
-const handleOptionalFields = (selectedJobClone: any, jobTypeKey: string) => {
+const handleOptionalFields = (selectedJobClone: any, jobTypeKey: any) => {
   let args: string[] = [];
   let jarFileUris: string[] = [];
   let archiveUris: string[] = [];
   let fileUris: string[] = [];
   let maxFailuresPerHour = '';
   let pythonFileUris: string[] = [];
   if (selectedJobClone[jobTypeKey].hasOwnProperty('fileUris')) {
-    fileUris = selectedJobClone[jobTypeKey].fileUris;
+    fileUris = [selectedJobClone[jobTypeKey].fileUris];
   }
 
   if (selectedJobClone[jobTypeKey].hasOwnProperty('jarFileUris')) {
-    jarFileUris = selectedJobClone[jobTypeKey].jarFileUris;
+    jarFileUris = [selectedJobClone[jobTypeKey].jarFileUris];
   }
 
   if (selectedJobClone[jobTypeKey].hasOwnProperty('args')) {
-    args = selectedJobClone[jobTypeKey].args;
+    args = [selectedJobClone[jobTypeKey].args];
   }
 
   if (selectedJobClone[jobTypeKey].hasOwnProperty('archiveUris')) {
-    archiveUris = selectedJobClone[jobTypeKey].archiveUris;
+    archiveUris = [selectedJobClone[jobTypeKey].archiveUris];
   }
 
   if (selectedJobClone[jobTypeKey].hasOwnProperty('pythonFileUris')) {
-    pythonFileUris = selectedJobClone[jobTypeKey].pythonFileUris;
+    pythonFileUris = [selectedJobClone[jobTypeKey].pythonFileUris];
   }
 
   if (selectedJobClone.hasOwnProperty('scheduling')) {
     maxFailuresPerHour = selectedJobClone.scheduling.maxFailuresPerHour;
   }
   return {
     fileUris,
     jarFileUris,
     args,
     archiveUris,
     pythonFileUris,
     maxFailuresPerHour
   };
 };
-function SubmitJob({
-  setSubmitJobView,
-  selectedJobClone,
-  clusterResponse
-}: any) {
+function SubmitJob(
+  this: any,
+  { setSubmitJobView, selectedJobClone, clusterResponse }: any
+) {
   const [clusterList, setClusterList] = useState([{}]);
   const [jobTypeList, setJobTypeList] = useState([{}]);
   const [querySourceTypeList, setQuerySourceTypeList] = useState([{}]);
-
+  const [clusterSelected, setClusterSelected] = useState('');
   const [jobIdSelected, setJobIdSelected] = useState('');
   const [propertyDetail, setPropertyDetail] = useState(['']);
   const [propertyDetailUpdated, setPropertyDetailUpdated] = useState(['']);
   const [parameterDetail, setParameterDetail] = useState(['']);
   const [parameterDetailUpdated, setParameterDetailUpdated] = useState(['']);
   const [hexNumber, setHexNumber] = useState('');
   const [submitDisabled, setSubmitDisabled] = useState(true);
@@ -133,42 +135,39 @@
   let args: string[] = [];
   let jarFileUris: string[] = [];
   let archiveUris: string[] = [];
   let fileUris: string[] = [];
   let pythonFileUris: string[] = [];
   let maxFailuresPerHour = '';
   let mainRFileUri = '';
-  let jobType = 'Spark';
+  let jobType = 'spark';
   let mainPythonFileUri = '';
   let queryFileUri = '';
   let queryType = '';
   let queryList = '';
   let mainClass = '';
-  let clusterSelectedValue = '';
   let key: string[] | (() => string[]) = [];
   let value: string[] | (() => string[]) = [];
   let jobKeys: string[] = [];
   if (Object.keys(selectedJobClone).length !== 0) {
     jobKeys = jobKey(selectedJobClone);
     const jobTypeKey = jobKeys[0];
     jobType = jobTypeFunction(jobKeys[0]);
 
     if (selectedJobClone[jobTypeKey].hasOwnProperty('queryFileUri')) {
       queryFileUri = selectedJobClone[jobTypeKey].queryFileUri;
-      queryType = 'Query file';
+      queryType = 'queryFile';
     }
     if (selectedJobClone[jobTypeKey].hasOwnProperty('queryList')) {
       queryList = selectedJobClone[jobTypeKey].queryList.queries[0];
-      queryType = 'Query text';
+      queryType = 'queryText';
     }
     mainJarFileUri = selectedJobClone[jobKeys[0]].mainJarFileUri;
     mainClass = selectedJobClone[jobKeys[0]].mainClass;
     mainRFileUri = selectedJobClone[jobKeys[0]].mainRFileUri;
-    clusterSelectedValue = selectedJobClone.placement.clusterName;
-
     mainPythonFileUri = selectedJobClone[jobKeys[0]].mainPythonFileUri;
     ({
       fileUris,
       jarFileUris,
       args,
       archiveUris,
       pythonFileUris,
@@ -176,15 +175,14 @@
     } = handleOptionalFields(selectedJobClone, jobTypeKey));
   }
   const initialMainClassSelected =
     mainJarFileUri && mainJarFileUri !== '' ? mainJarFileUri : mainClass;
   const [mainClassSelected, setMainClassSelected] = useState(
     initialMainClassSelected
   );
-  const [clusterSelected, setClusterSelected] = useState(clusterSelectedValue);
   const [mainRSelected, setMainRSelected] = useState(mainRFileUri);
   const [mainPythonSelected, setMainPythonSelected] =
     useState(mainPythonFileUri);
   const [jarFileSelected, setJarFileSelected] = useState([...jarFileUris]);
   const [fileSelected, setFileSelected] = useState([...fileUris]);
   const [archieveFileSelected, setArchieveFileSelected] = useState([
     ...archiveUris
@@ -210,93 +208,80 @@
   const [queryFileValidation, setQueryFileValidation] = useState(true);
   const [mainRValidation, setMainRValidation] = useState(true);
   const [mainClassValidation, setMainClassValidation] = useState(true);
   const [generationCompleted, setGenerationCompleted] = useState(false);
   const [keyValidation, setKeyValidation] = useState(-1);
   const [valueValidation, setValueValidation] = useState(-1);
   const [jobIdValidation, setjobIdValidation] = useState(true);
-  const [jobIdSpecialValidation, setjobIdSpecialValidation] = useState(false);
   const [duplicateKeyError, setDuplicateKeyError] = useState(-1);
   const [mainClassActive, setMainClassActive] = useState(false);
-  const [
-    additionalPythonFileDuplicateValidation,
-    setAdditionalPythonFileDuplicateValidation
-  ] = useState(false);
-  const [jarFileDuplicateValidation, setJarFileDuplicateValidation] =
-    useState(false);
-  const [fileDuplicateValidation, setFileDuplicateValidation] = useState(false);
-  const [archiveDuplicateValidation, setArchiveDuplicateValidation] =
-    useState(false);
-  const [argumentsDuplicateValidation, setArgumentsDuplicateValidation] =
-    useState(false);
+
   const handleCancelJobButton = () => {
     setSubmitJobView(false);
   };
   const handleSubmitJobView = () => {
     if (!submitDisabled) {
       submitJob();
       setSubmitJobView(false);
     }
   };
 
   const handleSubmitJobBackView = () => {
     setSubmitJobView(false);
   };
 
-  const handleClusterSelected = (data: DropdownProps | null) => {
-    if (data !== null) {
-      setClusterSelected(data!.toString());
-    }
+  const handleClusterSelected = (event: any, data: any) => {
+    setClusterSelected(data.value);
   };
 
-  const handleJobTypeSelected = (data: DropdownProps | null) => {
-    if (data !== null) {
-      setJobTypeSelected(data!.toString());
-    }
+  const handleJobTypeSelected = (event: any, data: any) => {
+    setJobTypeSelected(data.value);
     setFileSelected([]);
     setJarFileSelected([]);
     setAdditionalPythonFileSelected([]);
     setArchieveFileSelected([]);
     setArgumentSelected([]);
     setMainPythonSelected('');
     setMainRSelected('');
     setQueryTextSelected('');
     setQueryFileSelected('');
     setMainClassSelected('');
   };
-
-  const handleQuerySourceTypeSelected = (
-    event: SyntheticEvent<Element, Event>,
-    data: DropdownProps | null
-  ) => {
-    if (data !== null) {
-      setQuerySourceSelected(data!.toString());
-    }
+  const handleQuerySourceTypeSelected = (event: any, data: any) => {
+    setQuerySourceSelected(data.value);
   };
-  interface IClusterData {
-    clusterName: string;
-    status: string;
-  }
 
   useEffect(() => {
     let transformClusterListData = [];
-    transformClusterListData = clusterResponse.filter((data: IClusterData) => {
-      if (data.status === STATUS_RUNNING) {
-        return data.clusterName;
+    transformClusterListData = clusterResponse.clusters.filter((data: any) => {
+      if (data.status.state === STATUS_RUNNING) {
+        return {
+          clusterName: data.clusterName
+        };
       }
     });
 
-    const keyLabelStructure = transformClusterListData.map(
-      (obj: { clusterName: string }) => obj.clusterName
-    );
-    setClusterList(keyLabelStructure);
-    const jobTypeData = ['Spark', 'SparkR', 'SparkSql', 'PySpark'];
+    const keyLabelStructure = transformClusterListData.map((obj: any) => ({
+      key: obj.clusterName,
+      value: obj.clusterName,
+      text: obj.clusterName
+    }));
 
+    setClusterList(keyLabelStructure);
+    const jobTypeData = [
+      { key: 'spark', value: 'spark', text: 'Spark' },
+      { key: 'sparkR', value: 'sparkR', text: 'SparkR' },
+      { key: 'sparkSql', value: 'sparkSql', text: 'SparkSql' },
+      { key: 'pySpark', value: 'pySpark', text: 'PySpark' }
+    ];
+    const querySourceData = [
+      { key: 'queryFile', value: 'queryFile', text: 'Query file' },
+      { key: 'queryText', value: 'queryText', text: 'Query text' }
+    ];
     setJobTypeList(jobTypeData);
-    const querySourceData = ['Query file', 'Query text'];
     setQuerySourceTypeList(querySourceData);
   }, []);
   useEffect(() => {
     disableSubmitButtonIfInvalid();
     generateRandomHex();
   }, [
     clusterSelected,
@@ -312,93 +297,69 @@
     mainRValidation,
     fileValidation,
     mainPythonValidation,
     queryFileValidation,
     keyValidation,
     valueValidation,
     jobIdValidation,
-    jobIdSpecialValidation,
-    duplicateKeyError,
-    jarFileDuplicateValidation,
-    additionalPythonFileDuplicateValidation,
-    fileDuplicateValidation,
-    argumentsDuplicateValidation,
-    archiveDuplicateValidation
+    duplicateKeyError
   ]);
   const disableSubmitButtonIfInvalid = () => {
-    const isSparkJob = jobTypeSelected === 'Spark';
-    const isSparkRJob = jobTypeSelected === 'SparkR';
-    const isPySparkJob = jobTypeSelected === 'PySpark';
-    const isSparkSqlJob = jobTypeSelected === 'SparkSql';
+    const isSparkJob = jobTypeSelected === 'spark';
+    const isSparkRJob = jobTypeSelected === 'sparkR';
+    const isPySparkJob = jobTypeSelected === 'pySpark';
+    const isSparkSqlJob = jobTypeSelected === 'sparkSql';
     if (
       clusterSelected !== '' &&
       jobIdSelected !== '' &&
       ((isSparkJob &&
         mainClassSelected.length !== 0 &&
         jarFileValidation &&
         fileValidation &&
         archieveFileValidation &&
         keyValidation === -1 &&
         valueValidation === -1 &&
         jobIdValidation &&
-        !jobIdSpecialValidation &&
-        duplicateKeyError === -1 &&
-        !fileDuplicateValidation &&
-        !archiveDuplicateValidation &&
-        !argumentsDuplicateValidation &&
-        !jarFileDuplicateValidation) ||
+        duplicateKeyError === -1) ||
         (isSparkRJob &&
           mainRSelected !== '' &&
           mainRValidation &&
           fileValidation &&
           keyValidation === -1 &&
           valueValidation === -1 &&
           jobIdValidation &&
-          !jobIdSpecialValidation &&
-          duplicateKeyError === -1! &&
-          !fileDuplicateValidation &&
-          !argumentsDuplicateValidation) ||
+          duplicateKeyError === -1) ||
         (isPySparkJob &&
           mainPythonSelected !== '' &&
           mainPythonValidation &&
           additionalPythonFileValidation &&
           jarFileValidation &&
           fileValidation &&
           archieveFileValidation &&
           keyValidation === -1 &&
           valueValidation === -1 &&
           jobIdValidation &&
-          !jobIdSpecialValidation &&
-          duplicateKeyError === -1 &&
-          !additionalPythonFileDuplicateValidation &&
-          !fileDuplicateValidation &&
-          !archiveDuplicateValidation &&
-          !argumentsDuplicateValidation &&
-          !jarFileDuplicateValidation) ||
+          duplicateKeyError === -1) ||
         (isSparkSqlJob &&
           queryFileSelected !== '' &&
-          querySourceSelected === 'Query file' &&
+          querySourceSelected === 'queryFile' &&
           queryFileValidation &&
           jarFileValidation &&
           keyValidation === -1 &&
           valueValidation === -1 &&
           jobIdValidation &&
-          !jobIdSpecialValidation &&
-          duplicateKeyError === -1 &&
-          !jarFileDuplicateValidation) ||
+          duplicateKeyError === -1) ||
         (isSparkSqlJob &&
           queryTextSelected !== '' &&
-          querySourceSelected === 'Query text' &&
+          querySourceSelected === 'queryText' &&
           jarFileValidation &&
           keyValidation === -1 &&
           valueValidation === -1 &&
           jobIdValidation &&
-          !jobIdSpecialValidation &&
-          duplicateKeyError === -1 &&
-          !jarFileDuplicateValidation))
+          duplicateKeyError === -1))
     ) {
       setSubmitDisabled(false);
     } else {
       setSubmitDisabled(true);
     }
   };
 
@@ -450,21 +411,21 @@
       setHexNumber('job-' + paddedHex);
       setJobIdSelected('job-' + paddedHex);
       setGenerationCompleted(true);
     }
   };
 
   const createPySparkPayload = (
-    mainPythonSelected: string,
-    propertyObject: { [key: string]: string },
-    jarFileSelected: string[] | string,
-    fileSelected: string[] | string,
-    archieveFileSelected: string[] | string,
-    argumentSelected: string[] | string,
-    additionalPythonFileSelected: string[] | string
+    mainPythonSelected: any,
+    propertyObject: any,
+    jarFileSelected: any,
+    fileSelected: any,
+    archieveFileSelected: any,
+    argumentSelected: any,
+    additionalPythonFileSelected: any
   ) => {
     return {
       pysparkJob: {
         mainPythonFileUri: mainPythonSelected,
         ...(propertyObject && {
           properties: propertyObject
         }),
@@ -474,30 +435,30 @@
         ...(fileSelected !== '' && {
           fileUris: fileSelected
         }),
         ...(archieveFileSelected !== '' && {
           archiveUris: archieveFileSelected
         }),
         ...(argumentSelected !== '' && {
-          args: argumentSelected
+          args: [argumentSelected]
         }),
         ...(additionalPythonFileSelected !== '' && {
           pythonFileUris: [additionalPythonFileSelected]
         })
       }
     };
   };
 
   const createSparkPayload = (
-    mainClassSelected: string,
-    propertyObject: { [key: string]: string },
-    archieveFileSelected: string[] | string,
-    fileSelected: string[] | string,
-    jarFileSelected: string[] | string,
-    argumentSelected: string[] | string
+    mainClassSelected: any,
+    propertyObject: any,
+    archieveFileSelected: any,
+    fileSelected: any,
+    jarFileSelected: any,
+    argumentSelected: any
   ) => {
     return {
       sparkJob: {
         mainJarFileUri: mainClassSelected,
         ...(propertyObject && {
           properties: propertyObject
         }),
@@ -507,62 +468,62 @@
         ...(fileSelected !== '' && {
           fileUris: [fileSelected]
         }),
         ...(jarFileSelected !== '' && {
           jarFileUris: jarFileSelected
         }),
         ...(argumentSelected !== '' && {
-          args: argumentSelected
+          args: [argumentSelected]
         })
       }
     };
   };
 
   const createSparkRPayload = (
-    mainRSelected: string,
-    propertyObject: { [key: string]: string },
-    fileSelected: string[] | string,
-    argumentSelected: string[] | string
+    mainRSelected: any,
+    propertyObject: any,
+    fileSelected: any,
+    argumentSelected: any
   ) => {
     return {
       sparkRJob: {
         mainRFileUri: mainRSelected,
         ...(propertyObject && {
           properties: propertyObject
         }),
         ...(fileSelected !== '' && {
           fileUris: [fileSelected]
         }),
         ...(argumentSelected !== '' && {
-          args: argumentSelected
+          args: [argumentSelected]
         })
       }
     };
   };
 
   const createSparkSqlPayload = (
-    propertyObject: { [key: string]: string },
-    jarFileSelected: string[] | string,
+    propertyObject: any,
+    jarFileSelected: any,
     querySourceSelected: string,
-    queryFileSelected: string,
-    queryTextSelected: string
+    queryFileSelected: any,
+    queryTextSelected: any
   ) => {
     return {
       sparkSqlJob: {
         ...(propertyObject && {
           properties: propertyObject
         }),
         ...(jarFileSelected !== '' && {
           jarFileUris: [jarFileSelected]
         }),
         scriptVariables: {},
-        ...(querySourceSelected === 'Query file' && {
+        ...(querySourceSelected === 'queryFile' && {
           queryFileUri: queryFileSelected
         }),
-        ...(querySourceSelected === 'Query text' && {
+        ...(querySourceSelected === 'queryText' && {
           queryList: { queries: [queryTextSelected] }
         })
       }
     };
   };
 
   const submitJob = async () => {
@@ -595,72 +556,95 @@
           reference: { jobId: jobIdSelected, projectId: '' },
           ...(maxRestartSelected !== '' && {
             scheduling: { maxFailuresPerHour: maxRestartSelected }
           }),
           ...(labelObject && {
             labels: labelObject
           }),
-          ...(jobTypeSelected === 'PySpark' &&
+          ...(jobTypeSelected === 'pySpark' &&
             createPySparkPayload(
               mainPythonSelected,
               propertyObject,
               jarFileSelected,
               fileSelected,
               archieveFileSelected,
               argumentSelected,
               additionalPythonFileSelected
             )),
-          ...(jobTypeSelected === 'Spark' &&
+          ...(jobTypeSelected === 'spark' &&
             createSparkPayload(
               mainClassSelected,
               propertyObject,
               archieveFileSelected,
               fileSelected,
               jarFileSelected,
               argumentSelected
             )),
-          ...(jobTypeSelected === 'SparkR' &&
+          ...(jobTypeSelected === 'sparkR' &&
             createSparkRPayload(
               mainRSelected,
               propertyObject,
               fileSelected,
               argumentSelected
             )),
-          ...(jobTypeSelected === 'SparkSql' &&
+          ...(jobTypeSelected === 'sparkSql' &&
             createSparkSqlPayload(
               propertyObject,
               jarFileSelected,
               querySourceSelected,
               queryFileSelected,
               queryTextSelected
             ))
         }
       };
-      await JobService.submitJobService(payload, jobIdSelected, credentials);
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/jobs:submit`,
+        {
+          method: 'POST',
+          body: JSON.stringify(payload),
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: any) => {
+          if (response.status === 200) {
+            response
+              .json()
+              .then((responseResult: any) => {
+                console.log(responseResult);
+                toast.success(`Job ${jobIdSelected} successfully submitted`);
+              })
+              .catch((e: any) => {
+                console.log(e);
+              });
+          } else {
+            throw new Error(`API failed with status: ${response.status}`);
+          }
+        })
+        .catch((err: any) => {
+          console.error('Error submitting job', err);
+          toast.error('Failed to submit the job');
+        });
     }
   };
-  const handleJobIdChange = (event: React.ChangeEvent<HTMLInputElement>) => {
+  const handleInputChange = (event: any) => {
     event.target.value.length > 0
       ? setjobIdValidation(true)
       : setjobIdValidation(false);
-
-    const regexp = /^[a-zA-Z0-9-_]+$/;
-    event.target.value.search(regexp)
-      ? setjobIdSpecialValidation(true)
-      : setjobIdSpecialValidation(false);
     setHexNumber(event.target.value);
     const newJobId = event.target.value;
     setJobIdSelected(newJobId);
   };
 
   const handleValidationFiles = (
-    listOfFiles: string | string[],
+    listOfFiles: any,
     setValuesPart: any,
-    setValidationPart: (value: boolean) => void,
-    setDuplicateValidation?: (value: boolean) => void
+    setValidationPart: any
   ) => {
     if (typeof listOfFiles === 'string') {
       if (
         listOfFiles.startsWith('file://') ||
         listOfFiles.startsWith('gs://') ||
         listOfFiles.startsWith('hdfs://')
       ) {
@@ -669,582 +653,463 @@
         setValidationPart(false);
       }
       setValuesPart(listOfFiles);
     } else {
       if (listOfFiles.length === 0) {
         setValidationPart(true);
       } else {
-        listOfFiles.forEach((fileName: string) => {
+        listOfFiles.forEach((fileName: any) => {
           if (
             fileName.startsWith('file://') ||
             fileName.startsWith('gs://') ||
             fileName.startsWith('hdfs://')
           ) {
             setValidationPart(true);
           } else {
             setValidationPart(false);
           }
         });
       }
-      handleDuplicateValidation(setDuplicateValidation, listOfFiles);
       setValuesPart(listOfFiles);
     }
   };
-  const handleDuplicateValidation = (
-    setDuplicateValidation: ((value: boolean) => void) | undefined,
-    listOfFiles: string | string[]
-  ) => {
-    if (Array.isArray(listOfFiles)) {
-      const fileNames = listOfFiles.map((fileName: string) =>
-        fileName.toLowerCase()
-      );
-      const uniqueFileNames = new Set<string>();
-      const duplicateFileNames = fileNames.filter((fileName: string) => {
-        const isDuplicate = uniqueFileNames.has(fileName);
-        uniqueFileNames.add(fileName);
-        return isDuplicate;
-      });
-      if (duplicateFileNames.length > 0) {
-        setDuplicateValidation!(true);
-      } else {
-        setDuplicateValidation!(false);
-      }
-    }
-  };
-  const handleArgumentsSelection = (
-    setDuplicateValidation: (value: boolean) => void,
-    listOfFiles: string[]
-  ) => {
-    setArgumentSelected(listOfFiles);
-    handleDuplicateValidation(setDuplicateValidation, listOfFiles);
-  };
+
   return (
     <div>
-      <div className="cluster-details-header">
-        <div
-          role="button"
-          className="back-arrow-icon"
-          onClick={() => handleSubmitJobBackView()}
-        >
-          <iconLeftArrow.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+      <div className="scroll-comp">
+        <div className="cluster-details-header">
+          <div
+            role="button"
+            className="back-arrow-icon"
+            onClick={() => handleSubmitJobBackView()}
+          >
+            <iconLeftArrow.react tag="div" />
+          </div>
+          <div className="cluster-details-title">Submit a job</div>
         </div>
-        <div className="cluster-details-title">Submit a job</div>
-      </div>
-      <div className="submit-job-container">
-        <div className="submit-job-label-header">Cluster</div>
-        <div>Choose a cluster to run your job in.</div>
-
-        {clusterList.length === 0 ? (
-          <Input className="input-style" value="No clusters running" readOnly />
-        ) : (
-          <div className="select-text-overlay">
-            <Autocomplete
+        <div className="submit-job-container">
+          <div className="submit-job-label-header">Cluster</div>
+          <div className="submit-job-cluster-message">
+            Choose a cluster to run your job in.
+          </div>
+          {clusterList.length === 0 ? (
+            <Input
+              className="input-style"
+              value="No clusters running"
+              readOnly
+            />
+          ) : (
+            <Select
+              search
+              placeholder="Cluster*"
+              onChange={handleClusterSelected}
+              className="select-job-style"
               options={clusterList}
               value={clusterSelected}
-              onChange={(_event, val) => handleClusterSelected(val)}
-              renderInput={params => <TextField {...params} label="Cluster*" />}
             />
-          </div>
-        )}
-        <div className="submit-job-label-header">Job</div>
-        <div className="select-text-overlay">
+          )}
+          <div className="submit-job-label-header">Job</div>
+          <div className="submit-job-cluster-message">Job ID*</div>
           <Input
-            className="submit-job-input-style"
-            onChange={e => handleJobIdChange(e)}
+            className="input-style"
+            onChange={e => handleInputChange(e)}
             type="text"
             value={hexNumber}
-            Label="Job ID*"
           />
-        </div>
-
-        {!jobIdValidation && (
-          <div className="error-key-parent">
-            <iconError.react tag="div" className="logo-alignment-style" />
-            <div className="error-key-missing">ID is required</div>
-          </div>
-        )}
-        {jobIdSpecialValidation && jobIdValidation && (
-          <div className="error-key-parent">
-            <iconError.react tag="div" className="logo-alignment-style" />
-            <div className="error-key-missing">
-              ID must contain only letters, numbers, hyphens, and underscores
+          {!jobIdValidation && (
+            <div className="error-key-parent">
+              <iconError.react tag="div" />
+              <div className="error-key-missing">ID is required</div>
             </div>
-          </div>
-        )}
+          )}
+          <div className="submit-job-cluster-message">Job type*</div>
 
-        <div className="select-text-overlay">
-          <Autocomplete
-            className="project-region-select"
-            onChange={(_event, val) => handleJobTypeSelected(val)}
+          <Select
+            search
+            onChange={handleJobTypeSelected}
+            className="select-job-style"
             options={jobTypeList}
             value={jobTypeSelected}
-            renderInput={params => <TextField {...params} label=" Job type*" />}
           />
-        </div>
 
-        {jobTypeSelected === 'SparkSql' && (
-          <>
-            <div className="select-text-overlay">
-              <Autocomplete
-                className="project-region-select"
-                onChange={(_event, val) =>
-                  handleQuerySourceTypeSelected(_event, val)
-                }
+          {jobTypeSelected === 'sparkSql' && (
+            <>
+              <div className="submit-job-cluster-message">
+                Query source type*
+              </div>
+              <Select
+                search
+                onChange={handleQuerySourceTypeSelected}
+                className="select-job-style"
                 options={querySourceTypeList}
                 value={querySourceSelected}
-                renderInput={params => (
-                  <TextField {...params} label="Query source type*" />
-                )}
               />
-            </div>
-          </>
-        )}
-        {querySourceSelected === 'Query file' &&
-          jobTypeSelected === 'SparkSql' && (
-            <>
-              <div className="select-text-overlay">
+            </>
+          )}
+          {querySourceSelected === 'queryFile' &&
+            jobTypeSelected === 'sparkSql' && (
+              <>
+                <div className="submit-job-cluster-message">Query file*</div>
                 <Input
-                  className="submit-job-input-style"
+                  className="input-style"
                   onChange={e =>
                     handleValidationFiles(
                       e.target.value,
                       setQueryFileSelected,
                       setQueryFileValidation
                     )
                   }
                   addOnBlur={true}
                   value={queryFileSelected}
-                  Label="Query file*"
                 />
-              </div>
-
-              {!queryFileValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    File must include a valid scheme prefix: 'file://', 'gs://',
-                    or 'hdfs://'
+                {!queryFileValidation && (
+                  <div className="error-key-parent">
+                    <iconError.react tag="div" />
+                    <div className="error-key-missing">
+                      File must include a valid scheme prefix: 'file://',
+                      'gs://', or 'hdfs://'
+                    </div>
                   </div>
-                </div>
-              )}
-              {queryFileValidation && (
-                <div className="submit-job-message-input">
-                  {QUERY_FILE_MESSAGE}
-                </div>
-              )}
-            </>
-          )}
-        {querySourceSelected === 'Query text' &&
-          jobTypeSelected === 'SparkSql' && (
-            <>
-              <div className="select-text-overlay">
+                )}
+                {queryFileValidation && (
+                  <div className="submit-job-message">{QUERY_FILE_MESSAGE}</div>
+                )}
+              </>
+            )}
+          {querySourceSelected === 'queryText' &&
+            jobTypeSelected === 'sparkSql' && (
+              <>
+                <div className="submit-job-cluster-message">Query text*</div>
                 <Input
-                  className="submit-job-input-style"
+                  className="input-style"
                   onChange={e => setQueryTextSelected(e.target.value)}
                   value={queryTextSelected}
-                  Label=" Query text*"
                 />
+                <div className="submit-job-message">The query to execute</div>
+              </>
+            )}
+          {jobTypeSelected === 'spark' && (
+            <>
+              <div className="submit-job-cluster-message">
+                Main class or jar*
               </div>
-
-              <div className="submit-job-message-input">
-                The query to execute
-              </div>
-            </>
-          )}
-        {jobTypeSelected === 'Spark' && (
-          <>
-            <div className="select-text-overlay">
               <Input
-                className="submit-job-input-style"
+                className="input-style"
                 onChange={e =>
                   handleValidationFiles(
                     e.target.value,
                     setMainClassSelected,
                     setMainClassValidation
                   )
                 }
                 onBlur={() => setMainClassActive(true)}
                 addOnBlur={true}
                 value={mainClassSelected}
-                Label="Main class or jar*"
               />
-            </div>
-
-            {mainClassSelected === '' && mainClassActive && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  Main class or jar is required
+              {mainClassSelected === '' && mainClassActive && (
+                <div className="error-key-parent">
+                  <iconError.react tag="div" />
+                  <div className="error-key-missing">
+                    Main class or jar is required
+                  </div>
                 </div>
-              </div>
-            )}
-            {(mainClassSelected !== '' || !mainClassActive) && (
-              <div className="submit-job-message-input">
-                {MAIN_CLASS_MESSAGE}
-              </div>
-            )}
-          </>
-        )}
-        {jobTypeSelected === 'SparkR' && (
-          <>
-            <div className="select-text-overlay">
+              )}
+              {(mainClassSelected !== '' || !mainClassActive) && (
+                <div className="submit-job-message">{MAIN_CLASS_MESSAGE}</div>
+              )}
+            </>
+          )}
+          {jobTypeSelected === 'sparkR' && (
+            <>
+              <div className="submit-job-cluster-message">Main R file*</div>
               <Input
-                className="submit-job-input-style"
+                className="input-style"
                 onChange={e =>
                   handleValidationFiles(
                     e.target.value,
                     setMainRSelected,
                     setMainRValidation
                   )
                 }
                 addOnBlur={true}
                 value={mainRSelected}
-                Label="Main R file*"
               />
-            </div>
-
-            {!mainRValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  File must include a valid scheme prefix: 'file://', 'gs://',
-                  or 'hdfs://'
+              {!mainRValidation && (
+                <div className="error-key-parent">
+                  <iconError.react tag="div" />
+                  <div className="error-key-missing">
+                    File must include a valid scheme prefix: 'file://', 'gs://',
+                    or 'hdfs://'
+                  </div>
                 </div>
+              )}
+              {mainRValidation && (
+                <div className="submit-job-message">{QUERY_FILE_MESSAGE}</div>
+              )}
+            </>
+          )}
+          {jobTypeSelected === 'pySpark' && (
+            <>
+              <div className="submit-job-cluster-message">
+                Main Python file*
               </div>
-            )}
-            {mainRValidation && (
-              <div className="submit-job-message-input">
-                {QUERY_FILE_MESSAGE}
-              </div>
-            )}
-          </>
-        )}
-        {jobTypeSelected === 'PySpark' && (
-          <>
-            <div className="select-text-overlay">
               <Input
-                className="submit-job-input-style"
+                className="input-style"
                 onChange={e =>
                   handleValidationFiles(
                     e.target.value,
                     setMainPythonSelected,
                     setMainPythonValidation
                   )
                 }
                 addOnBlur={true}
                 value={mainPythonSelected}
-                Label="Main Python file*"
               />
-            </div>
-
-            {!mainPythonValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  File must include a valid scheme prefix: 'file://', 'gs://',
-                  or 'hdfs://'
+              {!mainPythonValidation && (
+                <div className="error-key-parent">
+                  <iconError.react tag="div" />
+                  <div className="error-key-missing">
+                    File must include a valid scheme prefix: 'file://', 'gs://',
+                    or 'hdfs://'
+                  </div>
                 </div>
+              )}
+              {mainPythonValidation && (
+                <div className="submit-job-message">{QUERY_FILE_MESSAGE}</div>
+              )}
+            </>
+          )}
+          {jobTypeSelected === 'pySpark' && (
+            <>
+              <div className="submit-job-cluster-message">
+                Additional python files
               </div>
-            )}
-            {mainPythonValidation && (
-              <div className="submit-job-message-input">
-                {QUERY_FILE_MESSAGE}
-              </div>
-            )}
-          </>
-        )}
-        {jobTypeSelected === 'PySpark' && (
-          <>
-            <div className="select-text-overlay">
-              <MuiChipsInput
+              <TagsInput
                 className="select-job-style"
                 onChange={e =>
                   handleValidationFiles(
                     e,
                     setAdditionalPythonFileSelected,
-                    setAdditionalPythonFileValidation,
-                    setAdditionalPythonFileDuplicateValidation
+                    setAdditionalPythonFileValidation
                   )
                 }
                 addOnBlur={true}
                 value={additionalPythonFileSelected}
                 inputProps={{ placeholder: '' }}
-                label="Additional python files"
               />
-            </div>
-            {!additionalPythonFileValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  All files must include a valid scheme prefix: 'file://',
-                  'gs://', or 'hdfs://'
-                </div>
-              </div>
-            )}
-            {additionalPythonFileDuplicateValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  Duplicate paths are not allowed
+              {!additionalPythonFileValidation && (
+                <div className="error-key-parent">
+                  <iconError.react tag="div" />
+                  <div className="error-key-missing">
+                    All files must include a valid scheme prefix: 'file://',
+                    'gs://', or 'hdfs://'
+                  </div>
                 </div>
-              </div>
-            )}
-          </>
-        )}
-        {jobTypeSelected !== 'SparkR' && (
-          <>
-            <div className="select-text-overlay">
-              <MuiChipsInput
+              )}
+            </>
+          )}
+          {jobTypeSelected !== 'sparkR' && (
+            <>
+              <div className="submit-job-cluster-message">Jar files</div>
+              <TagsInput
                 className="select-job-style"
                 onChange={e =>
                   handleValidationFiles(
                     e,
                     setJarFileSelected,
-                    setJarFileValidation,
-                    setJarFileDuplicateValidation
+                    setJarFileValidation
                   )
                 }
                 addOnBlur={true}
                 value={jarFileSelected}
                 inputProps={{ placeholder: '' }}
-                label="Jar files"
               />
-            </div>
-            {jarFileDuplicateValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  Duplicate paths are not allowed
-                </div>
-              </div>
-            )}
-            {!jarFileValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  All files must include a valid scheme prefix: 'file://',
-                  'gs://', or 'hdfs://'
+              {!jarFileValidation && (
+                <div className="error-key-parent">
+                  <iconError.react tag="div" />
+                  <div className="error-key-missing">
+                    All files must include a valid scheme prefix: 'file://',
+                    'gs://', or 'hdfs://'
+                  </div>
                 </div>
-              </div>
-            )}
-            {jarFileValidation && !jarFileDuplicateValidation && (
-              <div className="submit-job-message">{JAR_FILE_MESSAGE}</div>
-            )}
-          </>
-        )}
-        {jobTypeSelected !== 'SparkSql' && (
-          <>
-            <div className="select-text-overlay">
-              <MuiChipsInput
+              )}
+              {jarFileValidation && (
+                <div className="submit-job-message">{JAR_FILE_MESSAGE}</div>
+              )}
+            </>
+          )}
+          {jobTypeSelected !== 'sparkSql' && (
+            <>
+              <div className="submit-job-cluster-message">Files</div>
+              <TagsInput
                 className="select-job-style"
                 onChange={e =>
-                  handleValidationFiles(
-                    e,
-                    setFileSelected,
-                    setFileValidation,
-                    setFileDuplicateValidation
-                  )
+                  handleValidationFiles(e, setFileSelected, setFileValidation)
                 }
                 addOnBlur={true}
                 value={fileSelected}
                 inputProps={{ placeholder: '' }}
-                label="Files"
               />
-            </div>
-            {fileDuplicateValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  Duplicate paths are not allowed
-                </div>
-              </div>
-            )}
-            {!fileValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  All files must include a valid scheme prefix: 'file://',
-                  'gs://', or 'hdfs://'
+              {!fileValidation && (
+                <div className="error-key-parent">
+                  <iconError.react tag="div" />
+                  <div className="error-key-missing">
+                    All files must include a valid scheme prefix: 'file://',
+                    'gs://', or 'hdfs://'
+                  </div>
                 </div>
-              </div>
-            )}
-            {fileValidation && !fileDuplicateValidation && (
-              <div className="submit-job-message">{FILES_MESSAGE}</div>
-            )}
-          </>
-        )}
-        {(jobTypeSelected === 'Spark' || jobTypeSelected === 'PySpark') && (
-          <>
-            <div className="select-text-overlay">
-              <MuiChipsInput
+              )}
+              {fileValidation && (
+                <div className="submit-job-message">{FILES_MESSAGE}</div>
+              )}
+            </>
+          )}
+          {(jobTypeSelected === 'spark' || jobTypeSelected === 'pySpark') && (
+            <>
+              <div className="submit-job-cluster-message">Archive files</div>
+              <TagsInput
                 className="select-job-style"
                 onChange={e =>
                   handleValidationFiles(
                     e,
                     setArchieveFileSelected,
-                    setArchieveFileValidation,
-                    setArchiveDuplicateValidation
+                    setArchieveFileValidation
                   )
                 }
                 addOnBlur={true}
                 value={archieveFileSelected}
                 inputProps={{ placeholder: '' }}
-                label="Archive files"
               />
-            </div>
-            {archiveDuplicateValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  Duplicate paths are not allowed
+              {!archieveFileValidation && (
+                <div className="error-key-parent">
+                  <iconError.react tag="div" />
+                  <div className="error-key-missing">
+                    All files must include a valid scheme prefix: 'file://',
+                    'gs://', or 'hdfs://'
+                  </div>
                 </div>
-              </div>
-            )}
-            {!archieveFileValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  All files must include a valid scheme prefix: 'file://',
-                  'gs://', or 'hdfs://'
+              )}
+              {archieveFileValidation && (
+                <div className="submit-job-message">
+                  {ARCHIVE_FILES_MESSAGE}
                 </div>
-              </div>
-            )}
-            {archieveFileValidation && !archiveDuplicateValidation && (
-              <div className="submit-job-message">{ARCHIVE_FILES_MESSAGE}</div>
-            )}
-          </>
-        )}
-        {jobTypeSelected !== 'SparkSql' && (
-          <>
-            <div className="select-text-overlay">
-              <MuiChipsInput
+              )}
+            </>
+          )}
+          {jobTypeSelected !== 'sparkSql' && (
+            <>
+              <div className="submit-job-cluster-message">Arguments</div>
+              <TagsInput
                 className="select-job-style"
-                onChange={e =>
-                  handleArgumentsSelection(setArgumentsDuplicateValidation, e)
-                }
+                onChange={e => setArgumentSelected(e)}
                 value={argumentSelected}
-                addOnBlur={true}
                 inputProps={{ placeholder: '' }}
-                label="Arguments"
               />
-            </div>
-            {argumentsDuplicateValidation && (
-              <div className="error-key-parent">
-                <iconError.react tag="div" className="logo-alignment-style" />
-                <div className="error-key-missing">
-                  Duplicate paths are not allowed
-                </div>
-              </div>
-            )}
-            {!argumentsDuplicateValidation && (
               <div className="submit-job-message">{ARGUMENTS_MESSAGE}</div>
-            )}
-          </>
-        )}
-        {querySourceSelected === 'Query file' &&
-          jobTypeSelected === 'SparkSql' && (
-            <>
-              <div className="submit-job-label-header">Query parameters</div>
-              <LabelProperties
-                labelDetail={parameterDetail}
-                setLabelDetail={setParameterDetail}
-                labelDetailUpdated={parameterDetailUpdated}
-                setLabelDetailUpdated={setParameterDetailUpdated}
-                selectedJobClone={selectedJobClone ? true : false}
-                buttonText="ADD PARAMETER"
-                keyValidation={keyValidation}
-                setKeyValidation={setKeyValidation}
-                valueValidation={valueValidation}
-                setValueValidation={setValueValidation}
-                duplicateKeyError={duplicateKeyError}
-                setDuplicateKeyError={setDuplicateKeyError}
-              />
             </>
           )}
-        <div className="select-text-overlay">
+          {querySourceSelected === 'queryFile' &&
+            jobTypeSelected === 'sparkSql' && (
+              <>
+                <div className="submit-job-label-header">Query parameters</div>
+                <LabelProperties
+                  labelDetail={parameterDetail}
+                  setLabelDetail={setParameterDetail}
+                  labelDetailUpdated={parameterDetailUpdated}
+                  setLabelDetailUpdated={setParameterDetailUpdated}
+                  selectedJobClone={selectedJobClone ? true : false}
+                  buttonText="ADD PARAMETER"
+                  keyValidation={keyValidation}
+                  setKeyValidation={setKeyValidation}
+                  valueValidation={valueValidation}
+                  setValueValidation={setValueValidation}
+                  duplicateKeyError={duplicateKeyError}
+                  setDuplicateKeyError={setDuplicateKeyError}
+                />
+              </>
+            )}
+          <div className="submit-job-cluster-message">
+            Max restarts per hour
+          </div>
           <Input
-            className="submit-job-input-style"
+            className="input-style"
             onChange={e => setMaxRestartSelected(e.target.value)}
             value={maxRestartSelected}
-            Label="Max restarts per hour"
           />
-        </div>
-
-        <div className="submit-job-message-with-link">
-          {MAX_RESTART_MESSAGE}
-          <div
-            className="submit-job-learn-more"
-            onClick={() => {
-              window.open(`${RESTART_JOB_URL}`, '_blank');
-            }}
-          >
-            Learn more
-          </div>
-        </div>
-
-        <div className="submit-job-label-header">Properties</div>
-        <LabelProperties
-          labelDetail={propertyDetail}
-          setLabelDetail={setPropertyDetail}
-          labelDetailUpdated={propertyDetailUpdated}
-          setLabelDetailUpdated={setPropertyDetailUpdated}
-          selectedJobClone={selectedJobClone ? true : false}
-          buttonText="ADD PROPERTY"
-          keyValidation={keyValidation}
-          setKeyValidation={setKeyValidation}
-          valueValidation={valueValidation}
-          setValueValidation={setValueValidation}
-          duplicateKeyError={duplicateKeyError}
-          setDuplicateKeyError={setDuplicateKeyError}
-        />
-        <div className="submit-job-label-header">Labels</div>
-        <LabelProperties
-          labelDetail={labelDetail}
-          setLabelDetail={setLabelDetail}
-          labelDetailUpdated={labelDetailUpdated}
-          setLabelDetailUpdated={setLabelDetailUpdated}
-          selectedJobClone={selectedJobClone ? true : false}
-          buttonText="ADD LABEL"
-          keyValidation={keyValidation}
-          setKeyValidation={setKeyValidation}
-          valueValidation={valueValidation}
-          setValueValidation={setValueValidation}
-          duplicateKeyError={duplicateKeyError}
-          setDuplicateKeyError={setDuplicateKeyError}
-        />
-        <div className="job-button-style-parent">
-          <div
-            className={
-              submitDisabled
-                ? 'submit-button-disable-style'
-                : 'submit-button-style'
-            }
-          >
+          <div className="submit-job-message-with-link">
+            {MAX_RESTART_MESSAGE}
             <div
-              role="button"
+              className="submit-job-learn-more"
               onClick={() => {
-                handleSubmitJobView();
+                window.open(`${RESTART_JOB_URL}`, '_blank');
               }}
             >
-              SUBMIT
+              Learn more
             </div>
           </div>
-          <div className="job-cancel-button-style">
+
+          <div className="submit-job-label-header">Properties</div>
+          <LabelProperties
+            labelDetail={propertyDetail}
+            setLabelDetail={setPropertyDetail}
+            labelDetailUpdated={propertyDetailUpdated}
+            setLabelDetailUpdated={setPropertyDetailUpdated}
+            selectedJobClone={selectedJobClone ? true : false}
+            buttonText="ADD PROPERTY"
+            keyValidation={keyValidation}
+            setKeyValidation={setKeyValidation}
+            valueValidation={valueValidation}
+            setValueValidation={setValueValidation}
+            duplicateKeyError={duplicateKeyError}
+            setDuplicateKeyError={setDuplicateKeyError}
+          />
+          <div className="submit-job-label-header">Labels</div>
+          <LabelProperties
+            labelDetail={labelDetail}
+            setLabelDetail={setLabelDetail}
+            labelDetailUpdated={labelDetailUpdated}
+            setLabelDetailUpdated={setLabelDetailUpdated}
+            selectedJobClone={selectedJobClone ? true : false}
+            buttonText="ADD LABEL"
+            keyValidation={keyValidation}
+            setKeyValidation={setKeyValidation}
+            valueValidation={valueValidation}
+            setValueValidation={setValueValidation}
+            duplicateKeyError={duplicateKeyError}
+            setDuplicateKeyError={setDuplicateKeyError}
+          />
+          <div className="job-button-style-parent">
             <div
-              role="button"
-              onClick={() => {
-                handleCancelJobButton();
-              }}
+              className={
+                submitDisabled
+                  ? 'submit-button-disable-style'
+                  : 'submit-button-style'
+              }
             >
-              CANCEL
+              <div
+                role="button"
+                onClick={() => {
+                  handleSubmitJobView();
+                }}
+              >
+                SUBMIT
+              </div>
+            </div>
+            <div className="job-cancel-button-style">
+              <div
+                role="button"
+                onClick={() => {
+                  handleCancelJobButton();
+                }}
+              >
+                CANCEL
+              </div>
             </div>
           </div>
+          <ToastContainer />
         </div>
       </div>
     </div>
   );
 }
 
 export default SubmitJob;
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/runtime/createRunTime.tsx` & `dataproc_jupyter_plugin-0.1.9/src/runtime/createRunTime.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -13,86 +13,73 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 import React, { ChangeEvent, useEffect, useState } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
+import 'semantic-ui-css/semantic.min.css';
 import 'react-toastify/dist/ReactToastify.css';
+import { Input, Select } from 'semantic-ui-react';
 import {
   API_HEADER_BEARER,
   API_HEADER_CONTENT_TYPE,
-  ARTIFACT_REGISTERY,
-  gcpServiceUrls,
-  CONTAINER_REGISTERY,
-  CUSTOM_CONTAINERS,
-  CUSTOM_CONTAINER_MESSAGE,
-  CUSTOM_CONTAINER_MESSAGE_PART,
-  LOGIN_ERROR_MESSAGE,
-  LOGIN_STATE,
-  SHARED_VPC,
-  SERVICE_ACCOUNT
+  BASE_URL,
+  BASE_URL_META,
+  BASE_URL_NETWORKS,
+  PROJECT_LIST_URL,
+  REGION_URL,
+  STATUS_RUNNING,
+  USER_INFO_URL
 } from '../utils/const';
+import TagsInput from 'react-tagsinput';
+import 'react-tagsinput/react-tagsinput.css';
 import LabelProperties from '../jobs/labelProperties';
-import {
-  authApi,
-  toastifyCustomStyle,
-  iconDisplay,
-  loggedFetch,
-  checkConfig
-} from '../utils/utils';
+import { authApi } from '../utils/utils';
+import { ClipLoader } from 'react-spinners';
 import ErrorPopup from '../utils/errorPopup';
 import errorIcon from '../../style/icons/error_icon.svg';
 import { toast } from 'react-toastify';
-import LeftArrowIcon from '../../style/icons/left_arrow_icon.svg';
-import { Input } from '../controls/MuiWrappedInput';
-import { Select } from '../controls/MuiWrappedSelect';
-import { JupyterLab } from '@jupyterlab/application';
-import { KernelSpecAPI } from '@jupyterlab/services';
-import { ILauncher } from '@jupyterlab/launcher';
-import { DropdownProps } from 'semantic-ui-react';
 
-import { DynamicDropdown } from '../controls/DynamicDropdown';
-import { projectListAPI } from '../utils/projectService';
-import {
-  Autocomplete,
-  CircularProgress,
-  Radio,
-  TextField
-} from '@mui/material';
-import { DataprocLoggingService, LOG_LEVEL } from '../utils/loggingService';
-import { MuiChipsInput } from 'mui-chips-input';
-import { RunTimeSerive } from './runtimeService';
-
-const iconLeftArrow = new LabIcon({
-  name: 'launcher:left-arrow-icon',
-  svgstr: LeftArrowIcon
-});
+type Project = {
+  projectId: string;
+};
+
+type Cluster = {
+  clusterName: string;
+  status: {
+    state: string;
+  };
+};
+
+type Network = {
+  selfLink: string;
+  network: string;
+  subnetworks: string;
+};
+
+type Service = {
+  name: string;
+};
 
 const iconError = new LabIcon({
   name: 'launcher:error-icon',
   svgstr: errorIcon
 });
 
 let networkUris: string[] = [];
 let key: string[] | (() => string[]) = [];
 let value: string[] | (() => string[]) = [];
 
 function CreateRunTime({
   setOpenCreateTemplate,
-  selectedRuntimeClone,
-  launcher,
-  app,
-  fromPage
+  selectedRuntimeClone
 }: {
   setOpenCreateTemplate: (value: boolean) => void;
   selectedRuntimeClone: any;
-  launcher: ILauncher;
-  app: JupyterLab;
-  fromPage: string;
 }) {
   const [generationCompleted, setGenerationCompleted] = useState(false);
   const [displayNameSelected, setDisplayNameSelected] = useState('');
   const [desciptionSelected, setDescriptionSelected] = useState('');
   const [runTimeSelected, setRunTimeSelected] = useState('');
   const [versionSelected, setVersionSelected] = useState('2.1');
   const [pythonRepositorySelected, setPythonRepositorySelected] = useState('');
@@ -102,76 +89,65 @@
   const [propertyDetail, setPropertyDetail] = useState(['']);
   const [propertyDetailUpdated, setPropertyDetailUpdated] = useState(['']);
   const [keyValidation, setKeyValidation] = useState(-1);
   const [valueValidation, setValueValidation] = useState(-1);
   const [duplicateKeyError, setDuplicateKeyError] = useState(-1);
   const [labelDetail, setLabelDetail] = useState(key);
   const [labelDetailUpdated, setLabelDetailUpdated] = useState(value);
-  const [servicesList, setServicesList] = useState<string[]>([]);
+  const [servicesList, setServicesList] = useState<
+    Array<{ key: string; value: string; text: string }>
+  >([]);
   const [servicesSelected, setServicesSelected] = useState('');
   const [clusterSelected, setClusterSelected] = useState('');
-  const [projectId, setProjectId] = useState<string | null>('');
+  const [projectId, setProjectId] = useState('None');
   const [region, setRegion] = useState('');
-  const [containerImageSelected, setContainerImageSelected] = useState('');
-  const [serviceAccountSelected, setServiceAccountSelected] = useState('');
+  const [projectList, setProjectList] = useState([{}]);
+  const [regionList, setRegionList] = useState<
+    { value: string; key: string; text: string }[]
+  >([]);
   const [networkList, setNetworklist] = useState([{}]);
-  const [subNetworkList, setSubNetworklist] = useState<string[]>([]);
-  const [networkSelected, setNetworkSelected] = useState('');
-  const [subNetworkSelected, setSubNetworkSelected] = useState('');
+  const [subNetworkList, setSubNetworklist] = useState<
+    { key: string; value: string; text: string }[]
+  >([]);
+  const [isLoadingRegion, setIsLoadingRegion] = useState(false);
+  const [networkSelected, setNetworkSelected] = useState('default');
+  const [subNetworkSelected, setSubNetworkSelected] = useState('default');
   const [isLoadingService, setIsLoadingService] = useState(false);
   const [error, setError] = useState({ isOpen: false, message: '' });
-  const [clustersList, setClustersList] = useState<string[]>([]);
+  const [clustersList, setClustersList] = useState<
+    Array<{ key: string; value: string; text: string }>
+  >([]);
   const [runTimeValidation, setRuntimeValidation] = useState(false);
   const [descriptionValidation, setDescriptionValidation] = useState(false);
   const [displayNameValidation, setDisplayNameValidation] = useState(false);
   const [versionValidation, setVersionValidation] = useState(false);
   const [idleValidation, setIdleValidation] = useState(false);
   const [autoValidation, setAutoValidation] = useState(false);
-  const [defaultValue, setDefaultValue] = useState('');
+  const [defaultValue, setDefaultValue] = useState('default');
   const [idleTimeSelected, setIdleTimeSelected] = useState('');
   const [timeSelected, setTimeSelected] = useState('');
   const [autoTimeSelected, setAutoTimeSelected] = useState('');
   const [autoSelected, setAutoSelected] = useState('');
   const [timeList, setTimeList] = useState([{}]);
   const [createTime, setCreateTime] = useState('');
   const [userInfo, setUserInfo] = useState('');
-  const [duplicateValidation, setDuplicateValidation] = useState(false);
-  const [isloadingNetwork, setIsloadingNetwork] = useState(false);
-  const [selectedNetworkRadio, setSelectedNetworkRadio] = useState<
-    'sharedVpc' | 'projectNetwork'
-  >('projectNetwork');
-  const [projectInfo, setProjectInfo] = useState('');
-  const [configError, setConfigError] = useState(false);
-  const [loggedIn, setLoggedIn] = useState(false);
-  const [loginError, setLoginError] = useState(false);
-  const [configLoading, setConfigLoading] = useState(true);
 
-  const [sharedSubNetworkList, setSharedSubNetworkList] = useState<string[]>(
-    []
-  );
-  const [sharedvpcSelected, setSharedvpcSelected] = useState('');
   useEffect(() => {
-    checkConfig(setLoggedIn, setConfigError, setLoginError);
-    const localstorageGetInformation = localStorage.getItem('loginState');
-    setLoggedIn(localstorageGetInformation === LOGIN_STATE);
-    if (loggedIn) {
-      setConfigLoading(false);
-    }
     const timeData = [
       { key: 'h', value: 'h', text: 'hour' },
       { key: 'm', value: 'm', text: 'min' },
       { key: 's', value: 's', text: 'sec' }
     ];
-
+   
     setTimeList(timeData);
     updateLogic();
+    projectListAPI();
     listClustersAPI();
     listNetworksAPI();
-    runtimeSharedProject();
-  }, []);
+  }, [selectedRuntimeClone, clusterSelected, defaultValue]);
 
   useEffect(() => {
     if (selectedRuntimeClone === undefined) {
       generateRandomHex();
     }
   }, [
     runTimeSelected,
@@ -184,74 +160,58 @@
     autoValidation,
     descriptionValidation,
     runTimeValidation,
     projectId,
     region,
     servicesSelected
   ]);
-
-  useEffect(() => {
-    if (networkSelected !== '') {
-      listSubNetworksAPI(networkSelected);
-    }
-  }, [networkSelected]);
-
   const displayUserInfo = async () => {
-    await RunTimeSerive.displayUserInfoService(setUserInfo);
-  };
-
-  const runtimeSharedProject = async () => {
-    await RunTimeSerive.runtimeSharedProjectService(
-      setProjectInfo,
-      setSharedSubNetworkList
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(USER_INFO_URL, {
+        method: 'GET',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              setUserInfo(responseResult.email);
+            })
+            .catch((e: Error) => console.log(e));
+        })
+        .catch((err: Error) => {
+          console.error('Error displaying user info', err);
+          toast.error('Failed to fetch user information');
+        });
+    }
   };
-
   const updateLogic = () => {
     if (selectedRuntimeClone !== undefined) {
       const {
         jupyterSession,
         name,
         description,
         runtimeConfig,
         creator,
         createTime,
         environmentConfig
       } = selectedRuntimeClone;
-      const displayName = jupyterSession?.displayName
-        ? jupyterSession.displayName
-        : '';
-      const runTimeID = name.split('/')[5] ? name.split('/')[5] : '';
-      const descriptionDetail = description ? description : '';
-      const versionDetail = runtimeConfig?.version
-        ? runtimeConfig.version
-        : '2.1';
-      const containerImage = runtimeConfig?.containerImage
-        ? runtimeConfig.containerImage
-        : '';
-
-      let pythonRepositorySelected = '';
-
-      if (
-        runtimeConfig?.repositoryConfig?.pypiRepositoryConfig?.pypiRepository
-      ) {
-        pythonRepositorySelected =
-          runtimeConfig.repositoryConfig.pypiRepositoryConfig.pypiRepository;
-        setPythonRepositorySelected(pythonRepositorySelected);
-      }
 
-      setDisplayNameSelected(displayName);
-      /*
+      setDisplayNameSelected(jupyterSession.displayName);
+       /*
          Extracting runtimeId from name
          Example: "projects/{projectName}/locations/{region}/sessionTemplates/{runtimeid}",
       */
-      setRunTimeSelected(runTimeID);
-      setDescriptionSelected(descriptionDetail);
-      setVersionSelected(versionDetail);
-      setContainerImageSelected(containerImage);
+      setRunTimeSelected(name.split('/')[5]);
+      setDescriptionSelected(description);
+      setVersionSelected(runtimeConfig.version);
       setUserInfo(creator);
       setCreateTime(createTime);
 
       let runtimeKeys: string[] = [];
       if (Object.keys(selectedRuntimeClone).length !== 0) {
         if (selectedRuntimeClone.hasOwnProperty('labels')) {
           const updatedLabelDetail = Object.entries(
@@ -286,41 +246,25 @@
       }
 
       if (environmentConfig) {
         const executionConfig = environmentConfig.executionConfig;
         const peripheralsConfig = environmentConfig.peripheralsConfig;
 
         if (executionConfig) {
-          if (executionConfig.serviceAccount) {
-            setServiceAccountSelected(executionConfig.serviceAccount);
-          }
-          const sharedVpcMatches =
-            /projects\/(?<project>[\w\-]+)\/regions\/(?<region>[\w\-]+)\/subnetworks\/(?<subnetwork>[\w\-]+)/.exec(
-              executionConfig.subnetworkUri
-            );
-          // Is this a shared VPC?
-          if (sharedVpcMatches?.groups?.['subnetwork']) {
-            setSharedvpcSelected(sharedVpcMatches?.groups?.['subnetwork']);
-            setSelectedNetworkRadio('sharedVpc');
-          } else {
-            setSubNetworkSelected(executionConfig.subnetworkUri);
-            setSelectedNetworkRadio('projectNetwork');
-          }
-
+          setSubNetworkSelected(executionConfig.subnetworkUri);
           if (executionConfig.hasOwnProperty('idleTtl')) {
-            const idleTtlUnit = executionConfig.idleTtl.slice(-1);
+            const idleTtlUnit = executionConfig.idleTtl.slice(-1); // Extracting the last character 's'
 
             setTimeSelected(idleTtlUnit);
 
             const idleTtlInSecondsWithoutUnit = executionConfig.idleTtl
               .toString()
               .slice(0, -1);
             setIdleTimeSelected(idleTtlInSecondsWithoutUnit);
           }
-
           if (executionConfig.hasOwnProperty('ttl')) {
             const ttlUnit = executionConfig.idleTtl.slice(-1); // Extracting the last character 's'
 
             setAutoSelected(ttlUnit);
 
             const ttlInSecondsWithoutUnit = executionConfig.ttl
               .toString()
@@ -335,91 +279,311 @@
         }
 
         if (
           peripheralsConfig &&
           peripheralsConfig.metastoreService !== undefined
         ) {
           setServicesSelected(peripheralsConfig.metastoreService);
-          const metastoreDetails =
-            peripheralsConfig?.metastoreService?.split('/');
-          const metaProject = peripheralsConfig?.metastoreService?.split('/')
-            ? metastoreDetails[1]
-            : '';
-          const metaRegion = peripheralsConfig?.metastoreService?.split('/')
-            ? metastoreDetails[3]
-            : '';
-          setProjectId(metaProject);
-          setRegion(metaRegion);
         }
 
         if (
           peripheralsConfig &&
           peripheralsConfig.sparkHistoryServerConfig &&
           peripheralsConfig.sparkHistoryServerConfig.hasOwnProperty(
             'dataprocCluster'
           )
         ) {
           const dataprocCluster =
             peripheralsConfig.sparkHistoryServerConfig.dataprocCluster;
-          /*
+            /*
          Extracting clusterName from dataprocCluster
          Example: "projects/{projectName}/locations/{region}/sessionTemplates/{dataprocCluster}",
       */
           setClusterSelected(dataprocCluster.split('/')[5]);
         }
-        listNetworksFromSubNetworkAPI(executionConfig.subnetworkUri);
       }
     } else {
       displayUserInfo();
       setCreateTime(new Date().toISOString());
     }
   };
+  const listClustersAPI = async () => {
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters?pageSize=100`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { clusters: Cluster[] }) => {
+              let transformClusterListData = [];
+
+              transformClusterListData = responseResult.clusters.filter(
+                (data: Cluster) => {
+                  if (data.status.state === STATUS_RUNNING) {
+                    return {
+                      clusterName: data.clusterName
+                    };
+                  }
+                }
+              );
 
-  const listNetworksFromSubNetworkAPI = async (subnetwork: string) => {
-    await RunTimeSerive.listNetworksFromSubNetworkAPIService(
-      subnetwork,
-      setIsloadingNetwork,
-      setNetworkSelected,
-      setSubNetworkSelected,
-      setDefaultValue
-    );
+              const keyLabelStructure = transformClusterListData.map(obj => ({
+                key: obj.clusterName,
+                value: obj.clusterName,
+                text: obj.clusterName
+              }));
+              setClustersList(keyLabelStructure);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing clusters', err);
+        });
+    }
   };
-  const listClustersAPI = async () => {
-    await RunTimeSerive.listClustersAPIService(setClustersList);
+  const listNetworksAPI = async () => {
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_NETWORKS}/projects/${credentials.project_id}/global/networks`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { items: Network[] }) => {
+              let transformedNetworkList = [];
+              /*
+         Extracting network from items
+         Example: "https://www.googleapis.com/compute/v1/projects/{projectName}/global/networks/",
+      */
+
+              transformedNetworkList = responseResult.items.map(
+                (data: Network) => {
+                  return {
+                    network: data.selfLink.split('/')[9]
+                  };
+                }
+              );
+              const keyLabelStructureNetwork = transformedNetworkList.map(
+                obj => ({
+                  key: obj.network,
+                  value: obj.network,
+                  text: obj.network
+                })
+              );
+              setNetworklist(keyLabelStructureNetwork);
+            })
+
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing Networks', err);
+        });
+    }
+  };
+  type SubnetworkData = {
+    subnetworks: string;
   };
+  const listSubNetworksAPI = async (subnetwork: string) => {
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_NETWORKS}/projects/${credentials.project_id}/global/networks/${subnetwork}`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { subnetworks: string[] }) => {
+              let transformedSubNetworkList = [];
+              /*
+         Extracting  subnetworks from Network
+         Example: "https://www.googleapis.com/compute/v1/projects/{projectName}/global/networks/subnetwork",
+      */
 
-  const listNetworksAPI = async () => {
-    await RunTimeSerive.listNetworksAPIService(
-      setNetworklist,
-      setNetworkSelected,
-      selectedRuntimeClone,
-      setIsloadingNetwork
-    );
+              transformedSubNetworkList = responseResult.subnetworks.map(
+                (data: string) => {
+                  return {
+                    subnetworks: data.split(
+                      `${credentials.region_id}/subnetworks/`
+                    )[1]
+                  };
+                }
+              );
+              const keyLabelStructureSubNetwork = transformedSubNetworkList
+                .filter((obj: SubnetworkData) => obj.subnetworks !== undefined)
+                .map((obj: SubnetworkData) => ({
+                  key: obj.subnetworks,
+                  value: obj.subnetworks,
+                  text: obj.subnetworks
+                }));
+              setSubNetworklist(keyLabelStructureSubNetwork);
+              setDefaultValue(keyLabelStructureSubNetwork[0].value);
+              setSubNetworkSelected(keyLabelStructureSubNetwork[0].value);
+            })
+
+            .catch((e: Error) => {
+              console.log(e);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing Networks', err);
+        });
+    }
   };
 
-  const listSubNetworksAPI = async (subnetwork: string) => {
-    await RunTimeSerive.listSubNetworksAPIService(
-      subnetwork,
-      setSubNetworklist,
-      setSubNetworkSelected,
-      selectedRuntimeClone,
-      setIsloadingNetwork
-    );
+  const listMetaStoreAPI = async (data: undefined) => {
+    setIsLoadingService(true);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL_META}/projects/${projectId}/locations/${data}/services`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { services: Service[] }) => {
+              let transformClusterListData = [];
+
+              transformClusterListData = responseResult.services.filter(
+                (data: Service) => {
+                  return {
+                    name: data.name
+                  };
+                }
+              );
+
+              const keyLabelStructure = transformClusterListData.map(obj => ({
+                key: obj.name,
+                value: obj.name,
+                text: obj.name
+              }));
+              const noneOption = { key: 'None', value: 'None', text: 'None' };
+              setServicesList([noneOption, ...keyLabelStructure]);
+              setIsLoadingService(false);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoadingService(false);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing services', err);
+          setIsLoadingService(false);
+        });
+    }
+  };
+  const projectListAPI = async () => {
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(PROJECT_LIST_URL, {
+        method: 'GET',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { projects: Project[] }) => {
+              let transformedProjectList = [];
+              transformedProjectList = responseResult.projects.map(
+                (data: Project) => {
+                  return {
+                    projectId: data.projectId
+                  };
+                }
+              );
+              const keyLabelStructure = transformedProjectList.map(obj => ({
+                key: obj.projectId,
+                value: obj.projectId,
+                text: obj.projectId
+              }));
+              const noneOption = { key: 'None', value: 'None', text: 'None' };
+              setProjectList([noneOption, ...keyLabelStructure]);
+            })
+            .catch((e: Error) => console.log(e));
+        })
+        .catch((err: Error) => {
+          console.error('Error fetching project list', err);
+        });
+    }
   };
 
-  const regionListAPI = async (
-    projectId: string,
-    network: string | undefined
-  ) => {
-    await RunTimeSerive.regionListAPIService(
-      projectId,
-      network,
-      setIsLoadingService,
-      setServicesList
-    );
+  type Region = {
+    name: string;
+  };
+
+  const regionListAPI = async (projectId: string) => {
+    setIsLoadingRegion(true);
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(`${REGION_URL}${projectId}/regions`, {
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      })
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: { items: Region[] }) => {
+              let transformedRegionList = [];
+              transformedRegionList = responseResult.items.map(
+                (data: Region) => {
+                  return {
+                    value: data.name,
+                    key: data.name,
+                    text: data.name
+                  };
+                }
+              );
+              setRegionList(transformedRegionList);
+              setIsLoadingRegion(false);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoadingRegion(false);
+            });
+        })
+        .catch((err: Error) => {
+          console.error('Error listing regions', err);
+          setIsLoadingRegion(false);
+        });
+    }
   };
 
   const generateRandomHex = () => {
     if (!generationCompleted) {
       const crypto = window.crypto || window.Crypto;
       const array = new Uint32Array(1);
       crypto.getRandomValues(array);
@@ -455,300 +619,160 @@
     event.target.value.length > 0
       ? setVersionValidation(false)
       : setVersionValidation(true);
     const newVersion = event.target.value;
     setVersionSelected(newVersion);
   };
 
-  const handleServiceSelected = (data: string | null) => {
-    if (data !== null) {
-      setServicesSelected(data!.toString());
-    }
+  const handleServiceSelected = (event: any, data: any) => {
+    setServicesSelected(data.value);
   };
-  const handleIdleSelected = (event: React.ChangeEvent<HTMLInputElement>) => {
+  const handleIdleSelected = (event: ChangeEvent<HTMLInputElement>) => {
     const inputValue = event.target.value;
     const numericRegex = /^[0-9]*$/;
 
     if (numericRegex.test(inputValue) || inputValue === '') {
       setIdleValidation(false);
     } else {
       setIdleValidation(true);
     }
+
     setIdleTimeSelected(inputValue);
   };
-  const handletimeSelected = (
-    event: React.SyntheticEvent<HTMLElement, Event>,
-    data: DropdownProps
-  ) => {
-    setTimeSelected(data.value!.toString());
+  const handletimeSelected = (event: any, data: any) => {
+    setTimeSelected(data.value);
   };
   const handleAutoTimeSelected = (event: ChangeEvent<HTMLInputElement>) => {
     const inputValue = event.target.value;
     const numericRegex = /^[0-9]*$/;
 
     if (numericRegex.test(inputValue) || inputValue === '') {
       setAutoValidation(false);
     } else {
       setAutoValidation(true);
     }
 
     setAutoTimeSelected(inputValue);
   };
-  const handleAutoSelected = (
-    event: React.SyntheticEvent<HTMLElement, Event>,
-    data: DropdownProps
-  ) => {
-    setAutoSelected(data.value!.toString());
-  };
-  const handleProjectIdChange = (data: any, network: string | undefined) => {
-    setProjectId(data ?? '');
-    setServicesList([]);
-    setServicesSelected('');
-    regionListAPI(data, network);
-  };
-
-  const handleNetworkChange = async (data: DropdownProps | null) => {
-    if (data !== null) {
-      setNetworkSelected(data!.toString());
-      setSubNetworkSelected(defaultValue);
-      await listSubNetworksAPI(data!.toString());
-      await handleProjectIdChange(projectId, data!.toString());
-    }
+  const handleAutoSelected = (event: any, data: any) => {
+    setAutoSelected(data.value);
   };
-
-  const handleNetworkSharedVpcRadioChange = () => {
-    setSelectedNetworkRadio('sharedVpc');
-    setSubNetworkSelected(subNetworkList[0]!.toString());
-    setNetworkSelected(networkList[0]!.toString());
-  };
-  const handleSubNetworkRadioChange = () => {
-    setSelectedNetworkRadio('projectNetwork');
-    setSharedvpcSelected('');
-  };
-  const handleSubNetworkChange = (data: string | null) => {
-    if (data !== null) {
-      setSubNetworkSelected(data!.toString());
-    }
+  const handleProjectIdChange = (event: any, data: any) => {
+    regionListAPI(data.value);
+    setProjectId(data.value);
+    data.value === 'None' && setRegion('');
+    data.value === 'None' && setServicesSelected('');
+    data.value === 'None' && setRegionList([]);
+    data.value === 'None' && setServicesList([]);
+  };
+  const handleRegionChange = (event: any, data: any) => {
+    setRegion(data.value);
+    listMetaStoreAPI(data.value);
+  };
+  const handleNetworkChange = (event: any, data: any) => {
+    setNetworkSelected(data.value);
+    setSubNetworkSelected(defaultValue);
+    listSubNetworksAPI(data.value);
   };
-  const handleSharedSubNetwork = async (data: string | null) => {
-    if (data !== null) {
-      setSharedvpcSelected(data!.toString());
-      await handleProjectIdChange(projectId, data!.toString());
-    }
+  const handleSubNetworkChange = (event: any, data: any) => {
+    setSubNetworkSelected(data.value);
   };
-  const handleCancelButton = async () => {
+  const handleCancelButton = () => {
     setOpenCreateTemplate(false);
-    if (fromPage === 'launcher') {
-      app.shell.activeWidget?.close();
-    }
+    // const content = new AuthLogin();
+    // const widget = new MainAreaWidget<AuthLogin>({ content });
+    // widget.title.label = 'Config Setup';
+    // //widget.title.icon = iconCluster;
+    // app.shell.add(widget, 'main');
   };
 
-  const handleClusterSelected = (data: string | null) => {
-    setClusterSelected(data ?? '');
-  };
-  const handleNetworkTags = (
-    setDuplicateValidation: (value: boolean) => void,
-    listOfFiles: string[]
-  ) => {
-    setNetworkTagSelected(listOfFiles);
-    handleDuplicateValidation(setDuplicateValidation, listOfFiles);
-  };
-  const handleDuplicateValidation = (
-    setDuplicateValidation: (value: boolean) => void,
-    listOfFiles: string | string[]
-  ) => {
-    if (Array.isArray(listOfFiles)) {
-      const fileNames = listOfFiles.map((fileName: string) =>
-        fileName.toLowerCase()
-      );
-      const uniqueFileNames = new Set<string>();
-      const duplicateFileNames = fileNames.filter((fileName: string) => {
-        const isDuplicate = uniqueFileNames.has(fileName);
-        uniqueFileNames.add(fileName);
-        return isDuplicate;
-      });
-      if (duplicateFileNames.length > 0) {
-        setDuplicateValidation(true);
-      } else {
-        setDuplicateValidation(false);
-      }
-    }
+  const handleClusterSelected = (event: any, data: any) => {
+    setClusterSelected(data.value);
   };
   function isSaveDisabled() {
     return (
       displayNameSelected === '' ||
       runTimeSelected === '' ||
       desciptionSelected === '' ||
       versionSelected === '' ||
       displayNameValidation ||
       versionValidation ||
       descriptionValidation ||
       idleValidation ||
       runTimeValidation ||
-      autoValidation ||
-      duplicateValidation ||
-      (selectedNetworkRadio === 'sharedVpc' &&
-        sharedSubNetworkList.length === 0) ||
-      (selectedNetworkRadio === 'sharedVpc' && sharedvpcSelected === '') ||
-      (selectedNetworkRadio === 'projectNetwork' &&
-        networkList.length !== 0 &&
-        subNetworkList.length === 0)
+      autoValidation
     );
   }
   const createRuntimeApi = async (payload: any) => {
     const credentials = await authApi();
-    const { DATAPROC } = await gcpServiceUrls;
     if (credentials) {
-      loggedFetch(
-        `${DATAPROC}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessionTemplates`,
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessionTemplates`,
         {
           method: 'POST',
           body: JSON.stringify(payload),
           headers: {
             'Content-Type': API_HEADER_CONTENT_TYPE,
             Authorization: API_HEADER_BEARER + credentials.access_token
           }
         }
       )
         .then(async (response: Response) => {
           if (response.ok) {
             const responseResult = await response.json();
             setOpenCreateTemplate(false);
             toast.success(
-              `Runtime Template ${displayNameSelected} successfully created`,
-              toastifyCustomStyle
+              `RuntimeTemplate ${displayNameSelected} successfully submitted`
             );
-            const kernelSpecs = await KernelSpecAPI.getSpecs();
-            const kernels = kernelSpecs.kernelspecs;
-
-            const { commands } = app;
-
-            if (launcher) {
-              Object.values(kernels).forEach((kernelsData, index) => {
-                const commandNameExist = `notebook:create-${kernelsData?.name}`;
-                if (
-                  kernelsData?.resources.endpointParentResource &&
-                  kernelsData?.resources.endpointParentResource.includes(
-                    '/sessions'
-                  ) &&
-                  // Check if the command is already registered
-                  !commands.hasCommand(commandNameExist)
-                ) {
-                  const commandNotebook = `notebook:create-${kernelsData?.name}`;
-                  commands.addCommand(commandNotebook, {
-                    caption: kernelsData?.display_name,
-                    label: kernelsData?.display_name,
-                    icon: iconDisplay(kernelsData),
-                    execute: async () => {
-                      const model = await app.commands.execute(
-                        'docmanager:new-untitled',
-                        {
-                          type: 'notebook',
-                          path: '',
-                          kernel: { name: kernelsData?.name }
-                        }
-                      );
-                      await app.commands.execute('docmanager:open', {
-                        kernel: { name: kernelsData?.name },
-                        path: model.path,
-                        factory: 'notebook'
-                      });
-                    }
-                  });
-
-                  launcher.add({
-                    command: commandNotebook,
-                    category: 'Dataproc Serverless Notebooks',
-                    //@ts-ignore jupyter lab Launcher type issue
-                    metadata: kernelsData?.metadata,
-                    rank: index + 1,
-                    //@ts-ignore jupyter lab Launcher type issue
-                    args: kernelsData?.argv
-                  });
-                }
-              });
-              Object.values(kernels).forEach((kernelsData, index) => {
-                const commandNameExist = `notebook:create-${kernelsData?.name}`;
-                if (
-                  kernelsData?.resources.endpointParentResource &&
-                  !kernelsData?.resources.endpointParentResource.includes(
-                    '/sessions'
-                  ) &&
-                  // Check if the command is already registered
-                  !commands.hasCommand(commandNameExist)
-                ) {
-                  const commandNotebook = `notebook:create-${kernelsData?.name}`;
-                  commands.addCommand(commandNotebook, {
-                    caption: kernelsData?.display_name,
-                    label: kernelsData?.display_name,
-                    icon: iconDisplay(kernelsData),
-                    execute: async () => {
-                      const model = await app.commands.execute(
-                        'docmanager:new-untitled',
-                        {
-                          type: 'notebook',
-                          path: '',
-                          kernel: { name: kernelsData?.name }
-                        }
-                      );
-                      await app.commands.execute('docmanager:open', {
-                        kernel: { name: kernelsData?.name },
-                        path: model.path,
-                        factory: 'notebook'
-                      });
-                    }
-                  });
-
-                  launcher.add({
-                    command: commandNotebook,
-                    category: 'Dataproc Cluster Notebooks',
-                    //@ts-ignore jupyter lab Launcher type issue
-                    metadata: kernelsData?.metadata,
-                    rank: index + 1,
-                    //@ts-ignore jupyter lab Launcher type issue
-                    args: kernelsData?.argv
-                  });
-                }
-              });
-            }
-
-            if (fromPage === 'launcher') {
-              app.shell.activeWidget?.close();
-            }
             console.log(responseResult);
           } else {
             const errorResponse = await response.json();
             console.log(errorResponse);
             setError({ isOpen: true, message: errorResponse.error.message });
-            toast.error(errorResponse?.error?.message, toastifyCustomStyle);
           }
         })
         .catch((err: Error) => {
           console.error('Error Creating template', err);
-          DataprocLoggingService.log(
-            'Error Creating template',
-            LOG_LEVEL.ERROR
-          );
-          toast.error(
-            `Failed to create the template : ${err}`,
-            toastifyCustomStyle
-          );
+          toast.error('Failed to create the template');
         });
     }
   };
   const updateRuntimeApi = async (payload: any) => {
-    await RunTimeSerive.updateRuntimeApiService(
-      payload,
-      app,
-      fromPage,
-      runTimeSelected,
-      displayNameSelected,
-      setError,
-      setOpenCreateTemplate
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessionTemplates/${runTimeSelected}`,
+        {
+          method: 'PATCH',
+          body: JSON.stringify(payload),
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then(async (response: Response) => {
+          if (response.ok) {
+            const responseResult = await response.json();
+            setOpenCreateTemplate(false);
+            toast.success(
+              `RuntimeTemplate ${displayNameSelected} successfully updated`
+            );
+            console.log(responseResult);
+          } else {
+            const errorResponse = await response.json();
+            console.log(errorResponse);
+            setError({ isOpen: true, message: errorResponse.error.message });
+          }
+        })
+        .catch((err: Error) => {
+          console.error('Error updating template', err);
+          toast.error('Failed to update the template');
+        });
+    }
   };
 
   const handleSave = async () => {
     const credentials = await authApi();
     if (credentials) {
       const labelObject: { [key: string]: string } = {};
       labelDetailUpdated.forEach((label: string) => {
@@ -760,95 +784,58 @@
       const propertyObject: { [key: string]: string } = {};
       propertyDetailUpdated.forEach((label: string) => {
         const labelSplit = label.split(':');
         const key = labelSplit[0];
         const value = labelSplit[1];
         propertyObject[key] = value;
       });
-      const inputValueHour = Number(idleTimeSelected) * 3600;
-      const inputValueMin = Number(idleTimeSelected) * 60;
-      const inputValueHourAuto = Number(autoTimeSelected) * 3600;
-      const inputValueMinAuto = Number(autoTimeSelected) * 60;
-
       const payload = {
         name: `projects/${credentials.project_id}/locations/${credentials.region_id}/sessionTemplates/${runTimeSelected}`,
         description: desciptionSelected,
         creator: userInfo,
         createTime: createTime,
         jupyterSession: {
           kernel: 'PYTHON',
           displayName: displayNameSelected
         },
         labels: labelObject,
         runtimeConfig: {
           ...(versionSelected && { version: versionSelected }),
-          ...(containerImageSelected !== '' && {
-            containerImage: containerImageSelected
-          }),
           ...(propertyObject && { properties: propertyObject }),
 
           ...(pythonRepositorySelected && {
             repositoryConfig: {
               pypiRepositoryConfig: {
                 pypiRepository: pythonRepositorySelected
               }
             }
           })
         },
         environmentConfig: {
           executionConfig: {
-            ...(serviceAccountSelected !== '' && {
-              serviceAccount: serviceAccountSelected
-            }),
             ...(networkTagSelected.length > 0 && {
               networkTags: networkTagSelected
             }),
+            // ...(networkSelected && {networkUri:networkSelected}),
+            ...(subNetworkSelected && { subnetworkUri: subNetworkSelected }),
 
-            ...(subNetworkSelected &&
-              selectedNetworkRadio === 'projectNetwork' && {
-                subnetworkUri: subNetworkSelected
-              }),
-            ...(sharedvpcSelected &&
-              selectedNetworkRadio === 'sharedVpc' && {
-                subnetworkUri: `projects/${projectInfo}/regions/${credentials.region_id}/subnetworks/${sharedvpcSelected}`
-              }),
-            ...(timeSelected === 'h' &&
-              idleTimeSelected && {
-                idleTtl: inputValueHour.toString() + 's'
-              }),
-            ...(timeSelected === 'm' &&
-              idleTimeSelected && {
-                idleTtl: inputValueMin.toString() + 's'
-              }),
-            ...(timeSelected === 's' &&
-              idleTimeSelected && {
-                idleTtl: idleTimeSelected + 's'
-              }),
-
-            ...(autoSelected === 'h' &&
-              autoTimeSelected && {
-                ttl: inputValueHourAuto.toString() + 's'
-              }),
-            ...(autoSelected === 'm' &&
-              autoTimeSelected && {
-                ttl: inputValueMinAuto.toString() + 's'
-              }),
-
-            ...(autoSelected === 's' &&
-              autoTimeSelected && {
-                ttl: autoTimeSelected + 's'
-              })
+            ...(idleTimeSelected && {
+              idleTtl: idleTimeSelected + timeSelected
+            }),
+            ...(autoTimeSelected && {
+              ttl: autoTimeSelected + autoSelected
+            })
           },
           peripheralsConfig: {
             ...(servicesSelected !== 'None' && {
               metastoreService: servicesSelected
             }),
             ...(clusterSelected !== '' && {
               sparkHistoryServerConfig: {
-                dataprocCluster: `projects/${credentials.project_id}/regions/${credentials.region_id}/clusters/${clusterSelected}`
+                dataprocCluster: `projects/${credentials.project_id}/locations/${credentials.region_id}/clusters/${clusterSelected}`
               }
             })
           }
         },
 
         updateTime: new Date().toISOString()
       };
@@ -858,560 +845,332 @@
         createRuntimeApi(payload);
       }
     }
   };
 
   return (
     <div>
-      {configLoading && !loggedIn && !configError && !loginError && (
-        <div className="spin-loader-main">
-          <CircularProgress
-            className="spin-loader-custom-style"
-            size={18}
-            aria-label="Loading Spinner"
-            data-testid="loader"
-          />
-          Loading Runtime
+      <div className="scroll-comp">
+        <div className="cluster-details-header">
+          <div className="cluster-details-title">Basics</div>
         </div>
-      )}
-
-      {loggedIn && !configError ? (
-        <>
-          <div className="cluster-details-header">
-            <div className="back-arrow-icon" onClick={handleCancelButton}>
-              <iconLeftArrow.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
+        <div className="submit-job-container">
+          <form>
+            <div className="create-batches-message">Display name*</div>
+            <Input
+              className="create-batch-style "
+              value={displayNameSelected}
+              onChange={e => handleDisplayNameChange(e)}
+              type="text"
+            />
+            {displayNameValidation && (
+              <div className="error-key-parent">
+                <iconError.react tag="div" />
+                <div className="error-key-missing">Name is required</div>
+              </div>
+            )}
+
+            <div className="create-batches-message">Runtime ID*</div>
+
+            <Input
+              className="create-batch-style "
+              value={runTimeSelected}
+              onChange={e => handleInputChange(e)}
+              type="text"
+              disabled={selectedRuntimeClone !== undefined}
+            />
+            {runTimeValidation && (
+              <div className="error-key-parent">
+                <iconError.react tag="div" />
+                <div className="error-key-missing">ID is required</div>
+              </div>
+            )}
+
+            <div className="create-batches-message">Description*</div>
+            <Input
+              className="create-batch-style "
+              value={desciptionSelected}
+              onChange={e => handleDescriptionChange(e)}
+              type="text"
+            />
+            {descriptionValidation && (
+              <div className="error-key-parent">
+                <iconError.react tag="div" />
+                <div className="error-key-missing">Description is required</div>
+              </div>
+            )}
+
+            <div className="create-batches-message">Runtime version*</div>
+
+            <Input
+              className="create-batch-style "
+              value={versionSelected}
+              onChange={e => handleVersionChange(e)}
+              type="text"
+            />
+            {versionValidation && (
+              <div className="error-key-parent">
+                <iconError.react tag="div" />
+                <div className="error-key-missing">Version is required</div>
+              </div>
+            )}
+            <div className="submit-job-label-header">Network Configuration</div>
+            <div className="create-batches-message">
+              Establishes connectivity for the VM instances in this cluster.
             </div>
-            <div className="cluster-details-title">
-              Serverless Runtime Template
+            <div className="create-batches-message">
+              Networks in this project
             </div>
-          </div>
-          <div className="runtime-container">
-            <form>
-              <div className="select-text-overlay">
-                <Input
-                  className="create-runtime-style "
-                  value={displayNameSelected}
-                  onChange={e => handleDisplayNameChange(e)}
-                  type="text"
-                  Label="Display name*"
-                />
-              </div>
-              {displayNameValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">Name is required</div>
-                </div>
-              )}
-
-              <div className="select-text-overlay">
-                <Input
-                  className={`create-runtime-style ${
-                    selectedRuntimeClone !== undefined ? ' disable-text' : ''
-                  }`}
-                  value={runTimeSelected}
-                  onChange={e => handleInputChange(e)}
-                  type="text"
-                  disabled={selectedRuntimeClone !== undefined}
-                  Label="Runtime ID*"
-                />
-              </div>
-
-              {runTimeValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">ID is required</div>
-                </div>
-              )}
-
-              <div className="select-text-overlay">
-                <Input
-                  className="create-runtime-style "
-                  value={desciptionSelected}
-                  onChange={e => handleDescriptionChange(e)}
-                  type="text"
-                  Label="Description*"
-                />
-              </div>
-
-              {descriptionValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Description is required
-                  </div>
-                </div>
-              )}
-
-              <div className="select-text-overlay">
-                <Input
-                  className="create-runtime-style "
-                  value={versionSelected}
-                  onChange={e => handleVersionChange(e)}
-                  type="text"
-                  Label="Runtime version*"
-                />
-              </div>
-
-              {versionValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">Version is required</div>
-                </div>
-              )}
-              <div className="select-text-overlay">
-                <Input
-                  className="create-batch-style "
-                  value={containerImageSelected}
-                  onChange={e => setContainerImageSelected(e.target.value)}
-                  type="text"
-                  placeholder="Enter URI, for example, gcr.io/my-project-id/my-image:1.0.1"
-                  Label="Custom container image"
-                />
-              </div>
-              <div className="create-custom-messagelist">
-                {CUSTOM_CONTAINER_MESSAGE}{' '}
-              </div>
-              <div className="create-container-message">
-                <div className="create-container-image-message">
-                  {CUSTOM_CONTAINER_MESSAGE_PART}
-                </div>
-                <div
-                  className="learn-more-url"
-                  onClick={() => {
-                    window.open(`${CONTAINER_REGISTERY}`, '_blank');
-                  }}
-                >
-                  Container Registry
-                </div>
-                &nbsp; <div className="create-container-image-message">or</div>
-                <div
-                  className="learn-more-url"
-                  onClick={() => {
-                    window.open(`${ARTIFACT_REGISTERY}`, '_blank');
-                  }}
-                >
-                  Artifact Registry
-                </div>
-                {' . '}
-                <div
-                  className="learn-more-url"
-                  onClick={() => {
-                    window.open(`${CUSTOM_CONTAINERS}`, '_blank');
-                  }}
-                >
-                  Learn more
-                </div>
-              </div>
-              <div className="submit-job-label-header">
-                Execution Configuration
-              </div>
-              <div className="select-text-overlay">
-                <Input
-                  className="create-batch-style "
-                  value={serviceAccountSelected}
-                  onChange={e => setServiceAccountSelected(e.target.value)}
-                  type="text"
-                  placeholder=""
-                  Label="Service account"
-                />
-              </div>
-              <div className="create-custom-messagelist">
-                If not provided, the default GCE service account will be used.
-                <div
-                  className="submit-job-learn-more"
-                  onClick={() => {
-                    window.open(`${SERVICE_ACCOUNT}`, '_blank');
-                  }}
-                >
-                  Learn more
-                </div>
-              </div>
-              <div className="submit-job-label-header">
-                Network Configuration
-              </div>
-              <div className="runtime-message">
-                Establishes connectivity for the VM instances in this cluster.
-              </div>
-              <div>
-                <div className="create-runtime-radio">
-                  <Radio
-                    size="small"
-                    className="select-runtime-radio-style"
-                    value="projectNetwork"
-                    checked={selectedNetworkRadio === 'projectNetwork'}
-                    onChange={() => handleSubNetworkRadioChange()}
-                  />
-                  <div className="create-batch-message">
-                    Networks in this project
-                  </div>
-                </div>
-              </div>
-              <div>
-                <div className="create-runtime-radio">
-                  <Radio
-                    size="small"
-                    className="select-runtime-radio-style"
-                    value="sharedVpc"
-                    checked={selectedNetworkRadio === 'sharedVpc'}
-                    onChange={() => handleNetworkSharedVpcRadioChange()}
-                  />
-                  <div className="create-batch-message">
-                    Networks shared from host project: "{projectInfo}"
-                  </div>
-                </div>
-                <div className="create-runtime-sub-message-network">
-                  Choose a shared VPC network from project that is different
-                  from this cluster's project.{' '}
-                  <div
-                    className="submit-job-learn-more"
-                    onClick={() => {
-                      window.open(`${SHARED_VPC}`, '_blank');
-                    }}
-                  >
-                    Learn more
-                  </div>
-                </div>
-              </div>
-
-              <div>
-                {selectedNetworkRadio === 'projectNetwork' && (
-                  <div className="create-batch-network">
-                    {isloadingNetwork ? (
-                      <div className="metastore-loader">
-                        <CircularProgress
-                          size={25}
-                          aria-label="Loading Spinner"
-                          data-testid="loader"
-                        />
-                      </div>
-                    ) : (
-                      <>
-                        <div className="select-text-overlay">
-                          <Autocomplete
-                            options={networkList}
-                            value={networkSelected}
-                            onChange={(_event, val) => handleNetworkChange(val)}
-                            renderInput={params => (
-                              <TextField {...params} label="Primary network*" />
-                            )}
-                          />
-                        </div>
-                        <div className="select-text-overlay subnetwork-style">
-                          <Autocomplete
-                            options={subNetworkList}
-                            value={subNetworkSelected}
-                            onChange={(_event, val) =>
-                              handleSubNetworkChange(val)
-                            }
-                            renderInput={params => (
-                              <TextField {...params} label="subnetwork" />
-                            )}
-                          />
-                        </div>
-                      </>
-                    )}
-                  </div>
-                )}
-                {selectedNetworkRadio === 'projectNetwork' &&
-                  networkList.length === 0 && (
-                    <div className="error-key-parent">
-                      <iconError.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
-                      <div className="error-key-missing">
-                        No local networks are available.
-                      </div>
-                    </div>
-                  )}
-                {!isloadingNetwork &&
-                  selectedNetworkRadio === 'projectNetwork' &&
-                  networkSelected !== '' &&
-                  subNetworkSelected === '' && (
-                    <div className="error-key-parent">
-                      <iconError.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
-                      <div className="error-key-missing">
-                        Please select a valid network and subnetwork.
-                      </div>
-                    </div>
-                  )}
-                {selectedNetworkRadio === 'sharedVpc' && (
-                  <div className="select-text-overlay">
-                    <Autocomplete
-                      options={sharedSubNetworkList}
-                      value={sharedvpcSelected}
-                      onChange={(_event, val) => handleSharedSubNetwork(val)}
-                      renderInput={params => (
-                        <TextField {...params} label="Shared subnetwork" />
-                      )}
-                    />
-                  </div>
-                )}
-                {selectedNetworkRadio === 'sharedVpc' &&
-                  sharedSubNetworkList.length === 0 && (
-                    <div className="error-key-parent">
-                      <iconError.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
-                      <div className="error-key-missing">
-                        No shared subnetworks are available in this region.
-                      </div>
-                    </div>
-                  )}
-              </div>
-
-              <div className="select-text-overlay">
-                <MuiChipsInput
-                  className="select-runtime-style"
-                  onChange={e => handleNetworkTags(setDuplicateValidation, e)}
-                  addOnBlur={true}
-                  value={networkTagSelected}
-                  inputProps={{ placeholder: '' }}
-                  label="Network tags"
-                />
-              </div>
-              {duplicateValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Duplicate paths are not allowed
-                  </div>
-                </div>
-              )}
-
-              {!duplicateValidation && (
-                <div className="create-messagelist">
-                  Network tags are text attributes you can add to make firewall
-                  rules and routes applicable to specific VM instances.
-                </div>
-              )}
-
-              <div className="submit-job-label-header">Metastore</div>
-
-              <div className="select-text-overlay">
-                <DynamicDropdown
-                  value={projectId}
-                  onChange={(_, projectId) =>
-                    handleProjectIdChange(projectId, networkSelected)
-                  }
-                  fetchFunc={projectListAPI}
-                  label="Project ID"
-                  // Always show the clear indicator and hide the dropdown arrow
-                  // make it very clear that this is an autocomplete.
-                  sx={{
-                    '& .MuiAutocomplete-clearIndicator': {
-                      visibility: 'hidden'
-                    }
-                  }}
-                  popupIcon={null}
-                />
+            <div className="create-batch-network">
+              <div className="create-batch-network-message">
+                Primary network
               </div>
-
-              <div className="select-text-overlay">
-                {isLoadingService ? (
-                  <div className="metastore-loader">
-                    <CircularProgress
-                      size={25}
-                      aria-label="Loading Spinner"
-                      data-testid="loader"
-                    />
-                  </div>
-                ) : (
-                  <Autocomplete
-                    options={servicesList}
-                    value={servicesSelected}
-                    onChange={(_event, val) => handleServiceSelected(val)}
-                    renderInput={params => (
-                      <TextField {...params} label="Metastore services" />
-                    )}
-                  />
-                )}
-              </div>
-
-              <div className="single-line">
-                <div className="select-text-overlay">
-                  <Input
-                    className="runtimetemplate-max-idle"
-                    value={idleTimeSelected}
-                    onChange={e => handleIdleSelected(e)}
-                    type="text"
-                    Label="Max idle time"
-                  />
-                </div>
+              <div className="create-batch-network-message">Subnetwork</div>
+            </div>
+            <div>
+              <div className="create-batch-network">
                 <Select
-                  className="runtimetemplate-max-idle-select"
-                  value={timeSelected}
-                  onChange={handletimeSelected}
-                  type="text"
                   search
-                  selection
-                  options={timeList}
+                  className="select-primary-network-style"
+                  value={networkSelected}
+                  onChange={handleNetworkChange}
+                  type="text"
+                  options={networkList}
                 />
-              </div>
-              <div className="create-messagelist">
-                Max notebook idle time before the session is auto-terminated 10
-                mins to 330 hours.
-              </div>
-              {idleValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Only Numeric is allowed
-                  </div>
-                </div>
-              )}
-
-              <div className="single-line">
-                <div className="select-text-overlay">
-                  <Input
-                    className="runtimetemplate-max-idle"
-                    value={autoTimeSelected}
-                    onChange={e => handleAutoTimeSelected(e)}
-                    type="text"
-                    Label="Max session time"
-                  />
-                </div>
 
                 <Select
                   search
-                  selection
-                  className="runtimetemplate-max-idle-select"
-                  value={autoSelected}
-                  onChange={handleAutoSelected}
+                  className="select-sub-network-style"
+                  value={subNetworkSelected}
+                  onChange={handleSubNetworkChange}
                   type="text"
-                  options={timeList}
+                  options={subNetworkList}
+                  placeholder={defaultValue}
                 />
               </div>
-              <div className="create-messagelist">
-                Max lifetime of a session. 10 mins and 330 hours.
-              </div>
-              {autoValidation && (
-                <div className="error-key-parent">
-                  <iconError.react tag="div" className="logo-alignment-style" />
-                  <div className="error-key-missing">
-                    Only Numeric is allowed
-                  </div>
-                </div>
-              )}
+            </div>
+            <div className="create-batches-message">Network tags</div>
+            <TagsInput
+              className="select-job-style"
+              onChange={e => setNetworkTagSelected(e)}
+              addOnBlur={true}
+              value={networkTagSelected}
+              inputProps={{ placeholder: '' }}
+            />
+
+            <div className="create-messagelist">
+              Network tags are text attributes you can add to make firewall
+              rules and routes applicable to specific VM instances.
+            </div>
 
-              <div className="select-text-overlay">
-                <Input
-                  className="create-runtime-style "
-                  value={pythonRepositorySelected}
-                  onChange={e => setPythonRepositorySelected(e.target.value)}
-                  type="text"
-                  Label="Python packages repository"
-                />
-              </div>
-              <div className="create-messagelist">
-                Enter the URI for the repository to install Python packages. By
-                default packages are installed to PyPI pull-through cache on
-                GCP.
-              </div>
+            <div className="submit-job-label-header">Metastore</div>
+            <div className="create-batches-message">Metastore project</div>
+            <Select
+              className="select-job-style"
+              search
+              selection
+              placeholder={projectId}
+              value={projectId}
+              onChange={handleProjectIdChange}
+              options={projectList}
+            />
+            <div className="create-batches-message">Metastore region</div>
+            {isLoadingRegion ? (
+              <ClipLoader
+                loading={true}
+                size={25}
+                aria-label="Loading Spinner"
+                data-testid="loader"
+              />
+            ) : (
+              <Select
+                className="select-job-style"
+                search
+                selection
+                placeholder={region}
+                value={region}
+                onChange={handleRegionChange}
+                options={regionList}
+              />
+            )}
 
-              <div className="submit-job-label-header">
-                Persistent Spark History Server
-              </div>
+            <div className="create-batches-message">Metastore service</div>
+            {isLoadingService ? (
+              <ClipLoader
+                loading={true}
+                size={25}
+                aria-label="Loading Spinner"
+                data-testid="loader"
+              />
+            ) : (
+              <Select
+                className="select-job-style"
+                search
+                selection
+                value={servicesSelected}
+                type="text"
+                options={servicesList}
+                onChange={handleServiceSelected}
+                placeholder={servicesSelected}
+              />
+            )}
+            <div className="single-line">
+              <div className="create-batches-subMessage">Max idle time</div>
+            </div>
+            <div className="single-line">
+              <Input
+                className="runtimetemplate-max-idle"
+                value={idleTimeSelected}
+                onChange={e => handleIdleSelected(e)}
+                type="text"
+              />
 
-              <div className="create-batches-message">
-                Choose a history server cluster to store logs in.{' '}
-              </div>
-              <div className="select-text-overlay">
-                <Autocomplete
-                  options={clustersList}
-                  value={clusterSelected}
-                  onChange={(_event, val) => handleClusterSelected(val)}
-                  noOptionsText="No history server clusters available"
-                  renderInput={params => (
-                    <TextField {...params} label="History server cluster" />
-                  )}
-                />
-              </div>
-              <div className="submit-job-label-header">Spark Properties</div>
-              <LabelProperties
-                labelDetail={propertyDetail}
-                setLabelDetail={setPropertyDetail}
-                labelDetailUpdated={propertyDetailUpdated}
-                setLabelDetailUpdated={setPropertyDetailUpdated}
-                buttonText="ADD PROPERTY"
-                keyValidation={keyValidation}
-                setKeyValidation={setKeyValidation}
-                valueValidation={valueValidation}
-                setValueValidation={setValueValidation}
-                duplicateKeyError={duplicateKeyError}
-                setDuplicateKeyError={setDuplicateKeyError}
-                selectedRuntimeClone={selectedRuntimeClone ? true : false}
+              <Select
+                className="runtimetemplate-max-idle-select"
+                value={timeSelected}
+                onChange={handletimeSelected}
+                type="text"
+                options={timeList}
+              />
+            </div>
+            <div className="create-messagelist">
+              Max notebook idle time before the session is auto-terminated 10
+              mins to 330 hours.
+            </div>
+            {idleValidation && (
+              <div className="error-key-parent">
+                <iconError.react tag="div" />
+                <div className="error-key-missing">Only Numeric is allowed</div>
+              </div>
+            )}
+            <div className="single-line">
+              <div className="create-batches-subMessage">Max session time</div>
+            </div>
+            <div className="single-line">
+              <Input
+                className="runtimetemplate-max-idle"
+                value={autoTimeSelected}
+                onChange={e => handleAutoTimeSelected(e)}
+                type="text"
               />
-              <div className="submit-job-label-header">Labels</div>
-              <LabelProperties
-                labelDetail={labelDetail}
-                setLabelDetail={setLabelDetail}
-                labelDetailUpdated={labelDetailUpdated}
-                setLabelDetailUpdated={setLabelDetailUpdated}
-                buttonText="ADD LABEL"
-                selectedRuntimeClone={selectedRuntimeClone}
-                keyValidation={keyValidation}
-                setKeyValidation={setKeyValidation}
-                valueValidation={valueValidation}
-                setValueValidation={setValueValidation}
-                duplicateKeyError={duplicateKeyError}
-                setDuplicateKeyError={setDuplicateKeyError}
+
+              <Select
+                search
+                selection
+                className="runtimetemplate-max-idle-select"
+                value={autoSelected}
+                onChange={handleAutoSelected}
+                type="text"
+                options={timeList}
               />
-              <div className="job-button-style-parent">
+            </div>
+            <div className="create-messagelist">
+              Max lifetime of a session. 10 mins and 330 hours.
+            </div>
+            {autoValidation && (
+              <div className="error-key-parent">
+                <iconError.react tag="div" />
+                <div className="error-key-missing">Only Numeric is allowed</div>
+              </div>
+            )}
+
+            <div className="create-batches-message">
+              Python packages repository
+            </div>
+            <Input
+              className="create-batch-style "
+              value={pythonRepositorySelected}
+              onChange={e => setPythonRepositorySelected(e.target.value)}
+              type="text"
+            />
+            <div className="create-messagelist">
+              Enter the URI for the repository to install Python packages. By
+              default packages are installed to PyPI mirror on GCP.
+            </div>
+
+            <div className="submit-job-label-header">
+              Persistent Spark History Server
+            </div>
+            <div className="create-batches-message">
+              Choose a history server cluster to store logs in.{' '}
+            </div>
+
+            <Select
+              className="select-job-style"
+              search
+              clearable
+              value={clusterSelected}
+              onChange={handleClusterSelected}
+              options={clustersList}
+              placeholder="History server cluster"
+            />
+            <div className="submit-job-label-header">Spark Properties</div>
+            <LabelProperties
+              labelDetail={propertyDetail}
+              setLabelDetail={setPropertyDetail}
+              labelDetailUpdated={propertyDetailUpdated}
+              setLabelDetailUpdated={setPropertyDetailUpdated}
+              buttonText="ADD PROPERTY"
+              keyValidation={keyValidation}
+              setKeyValidation={setKeyValidation}
+              valueValidation={valueValidation}
+              setValueValidation={setValueValidation}
+              duplicateKeyError={duplicateKeyError}
+              setDuplicateKeyError={setDuplicateKeyError}
+              selectedRuntimeClone={selectedRuntimeClone}
+            />
+            <div className="submit-job-label-header">Labels</div>
+            <LabelProperties
+              labelDetail={labelDetail}
+              setLabelDetail={setLabelDetail}
+              labelDetailUpdated={labelDetailUpdated}
+              setLabelDetailUpdated={setLabelDetailUpdated}
+              buttonText="ADD LABEL"
+              selectedRuntimeClone={selectedRuntimeClone}
+              keyValidation={keyValidation}
+              setKeyValidation={setKeyValidation}
+              valueValidation={valueValidation}
+              setValueValidation={setValueValidation}
+              duplicateKeyError={duplicateKeyError}
+              setDuplicateKeyError={setDuplicateKeyError}
+            />
+            <div className="job-button-style-parent">
+              <div
+                className={
+                  isSaveDisabled()
+                    ? 'submit-button-disable-style'
+                    : 'submit-button-style'
+                }
+                aria-label="submit Batch"
+              >
                 <div
                   onClick={() => {
                     if (!isSaveDisabled()) {
                       handleSave();
                     }
                   }}
-                  className={
-                    isSaveDisabled()
-                      ? 'submit-button-disable-style'
-                      : 'submit-button-style'
-                  }
-                  aria-label="submit Batch"
-                >
-                  <div>SAVE</div>
-                </div>
-                <div
-                  className="job-cancel-button-style"
-                  aria-label="cancel Batch"
-                  onClick={handleCancelButton}
                 >
-                  <div>CANCEL</div>
+                  SAVE
                 </div>
-                {error.isOpen && (
-                  <ErrorPopup
-                    onCancel={() => setError({ isOpen: false, message: '' })}
-                    errorPopupOpen={error.isOpen}
-                    errorMsg={error.message}
-                  />
-                )}
               </div>
-            </form>
-          </div>
-        </>
-      ) : (
-        loginError && (
-          <div role="alert" className="login-error">
-            {LOGIN_ERROR_MESSAGE}
-          </div>
-        )
-      )}
-
-      {configError && (
-        <div role="alert" className="login-error">
-          Please configure gcloud with account, project-id and region
+              <div
+                className="job-cancel-button-style"
+                aria-label="cancel Batch"
+              >
+                <div onClick={handleCancelButton}>CANCEL</div>
+              </div>
+              {error.isOpen && (
+                <ErrorPopup
+                  onCancel={() => setError({ isOpen: false, message: '' })}
+                  errorPopupOpen={error.isOpen}
+                  DeleteMsg={error.message}
+                />
+              )}
+            </div>
+          </form>
         </div>
-      )}
+      </div>
     </div>
   );
 }
 
 export default CreateRunTime;
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/runtime/listRuntimeTemplates.tsx` & `dataproc_jupyter_plugin-0.1.9/src/batches/batches.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -11,353 +11,321 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
+import { ReactWidget } from '@jupyterlab/apputils';
 import React, { useState, useEffect, useRef } from 'react';
-import { useTable, useGlobalFilter, usePagination } from 'react-table';
+import {
+  authApi,
+  checkConfig,
+  elapsedTime,
+  jobTimeFormat,
+  jobTypeDisplay
+} from '../utils/utils';
+import {
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
+  API_HEADER_BEARER,
+  LOGIN_STATE
+} from '../utils/const';
+import ListBatches from './listBatches';
 import { LabIcon } from '@jupyterlab/ui-components';
-import filterIcon from '../../style/icons/filter_icon.svg';
 import deleteIcon from '../../style/icons/delete_icon.svg';
-import GlobalFilter from '../utils/globalFilter';
-import TableData from '../utils/tableData';
-import { ICellProps } from '../utils/utils';
+import BatchDetails from './batchDetails';
+import ListSessions from '../sessions/listSessions';
+import { ClipLoader } from 'react-spinners';
 import DeletePopup from '../utils/deletePopup';
-import { RunTimeSerive } from './runtimeService';
-import { PaginationView } from '../utils/paginationView';
+import { toast, ToastContainer } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
+import { deleteBatchAPI } from '../utils/batchService';
+import CreateBatch from './createBatch';
 import PollingTimer from '../utils/pollingTimer';
-import SubmitJobIcon from '../../style/icons/submit_job_icon.svg';
-import {
-  ISessionTemplate,
-  ISessionTemplateDisplay
-} from '../utils/listRuntimeTemplateInterface';
-import { CircularProgress } from '@mui/material';
-const iconFilter = new LabIcon({
-  name: 'launcher:filter-icon',
-  svgstr: filterIcon
-});
+
 const iconDelete = new LabIcon({
   name: 'launcher:delete-icon',
   svgstr: deleteIcon
 });
-const iconSubmitJob = new LabIcon({
-  name: 'launcher:submit-job-icon',
-  svgstr: SubmitJobIcon
-});
-
-interface IListRuntimeTemplate {
-  openCreateTemplate: boolean;
-  setOpenCreateTemplate: (value: boolean) => void;
-  setSelectedRuntimeClone: (value: ISessionTemplate | undefined) => void;
-}
 
-function ListRuntimeTemplates({
-  openCreateTemplate,
-  setOpenCreateTemplate,
-  setSelectedRuntimeClone
-}: IListRuntimeTemplate) {
-  const [runtimeTemplateslist, setRuntimeTemplateslist] = useState<
-    ISessionTemplateDisplay[]
-  >([]);
+const BatchesComponent = (): React.JSX.Element => {
+  const [batchesList, setBatchesList] = useState([]);
+  const [selectedMode, setSelectedMode] = useState('Batches');
   const [isLoading, setIsLoading] = useState(true);
+  const [batchSelected, setBatchSelected] = useState('');
   const [pollingDisable, setPollingDisable] = useState(false);
+  const [detailedBatchView, setDetailedBatchView] = useState(false);
+  const [loggedIn, setLoggedIn] = useState(false);
+  const [configError, setConfigError] = useState(false);
+  const [loginError, setLoginError] = useState(false);
+  const [configLoading, setConfigLoading] = useState(true);
 
   const [deletePopupOpen, setDeletePopupOpen] = useState(false);
-  const [selectedRuntimeTemplateValue, setSelectedRuntimeTemplateValue] =
-    useState('');
-  const [
-    selectedRuntimeTemplateDisplayName,
-    setSelectedRuntimeTemplateDisplayName
-  ] = useState('');
-  const [runTimeTemplateAllList, setRunTimeTemplateAllList] = useState<
-    ISessionTemplate[]
-  >([
-    {
-      name: '',
-      createTime: '',
-      jupyterSession: {
-        kernel: '',
-        displayName: ''
-      },
-      creator: '',
-      labels: {
-        purpose: ''
-      },
-      environmentConfig: {
-        executionConfig: {
-          subnetworkUri: ''
-        }
-      },
-      description: '',
-      updateTime: ''
-    }
-  ]);
+  const [selectedBatch, setSelectedBatch] = useState('');
+  const [regionName, setRegionName] = useState('');
+  const [projectName, setProjectName] = useState('');
 
+  const [createBatchView, setCreateBatchView] = useState(false);
   const timer = useRef<NodeJS.Timeout | undefined>(undefined);
 
-  const pollingRuntimeTemplates = async (
+  const pollingBatches = async (
     pollingFunction: () => void,
     pollingDisable: boolean
   ) => {
     timer.current = PollingTimer(
       pollingFunction,
       pollingDisable,
       timer.current
     );
   };
 
-  const data = runtimeTemplateslist;
-
-  const columns = React.useMemo(
-    () => [
-      {
-        Header: 'Name',
-        accessor: 'name'
-      },
-      {
-        Header: 'Owner',
-        accessor: 'owner'
-      },
-      {
-        Header: 'Description',
-        accessor: 'description'
-      },
-      {
-        Header: 'Last Modified',
-        accessor: 'lastModified'
-      },
-      {
-        Header: 'Actions',
-        accessor: 'actions'
-      }
-    ],
-    []
-  );
-
-  const listRuntimeTemplatesAPI = async () => {
-    await RunTimeSerive.listRuntimeTemplatesAPIService(
-      renderActions,
-      setIsLoading,
-      setRuntimeTemplateslist,
-      setRunTimeTemplateAllList
-    );
+  const selectedModeChange = (mode: 'Sessions' | 'Batches') => {
+    setSelectedMode(mode);
   };
 
-  const handleDeleteRuntimeTemplate = (
-    runtimeTemplateName: string,
-    runtimeTemplateDisplayName: string
+  const listBatchAPI = async (
+    nextPageToken?: string,
+    previousBatchesList?: object
   ) => {
-    setSelectedRuntimeTemplateValue(runtimeTemplateName);
-    setSelectedRuntimeTemplateDisplayName(runtimeTemplateDisplayName);
+    const credentials = await authApi();
+    const pageToken = nextPageToken ?? '';
+    if (credentials) {
+      setRegionName(credentials.region_id || '');
+      setProjectName(credentials.project_id || '');
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/batches?orderBy=create_time desc&&pageSize=50&pageToken=${pageToken}`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              let transformBatchListData = [];
+              if (responseResult && responseResult.batches) {
+                transformBatchListData = responseResult.batches.map(
+                  (data: any) => {
+                    const startTimeDisplay = jobTimeFormat(data.createTime);
+                    const startTime = new Date(data.createTime);
+                    const elapsedTimeString = elapsedTime(
+                      data.stateTime,
+                      startTime
+                    );
+                    const batchType = Object.keys(data).filter(key =>
+                      key.endsWith('Batch')
+                    );
+                    /*
+                     Extracting batchID, location from batchInfo.name
+                      Example: "projects/{project}/locations/{location}/batches/{batchID}"
+                    */
+                    const batchTypeDisplay = jobTypeDisplay(
+                      batchType[0].split('Batch')[0]
+                    );
+                    return {
+                      batchID: data.name.split('/')[5],
+                      status: data.state,
+                      location: data.name.split('/')[3],
+                      creationTime: startTimeDisplay,
+                      type: batchTypeDisplay,
+                      elapsedTime: elapsedTimeString,
+                      actions: renderActions(data)
+                    };
+                  }
+                );
+              }
+
+              const existingBatchData = previousBatchesList ?? [];
+              //setStateAction never type issue
+              let allBatchesData: any = [
+                ...(existingBatchData as []),
+                ...transformBatchListData
+              ];
+
+              if (responseResult.nextPageToken) {
+                listBatchAPI(responseResult.nextPageToken, allBatchesData);
+              } else {
+                setBatchesList(allBatchesData);
+                setIsLoading(false);
+                setLoggedIn(true);
+              }
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error listing batches', err);
+          toast.error('Failed to fetch batches');
+        });
+    }
+  };
+  const handleBatchDetails = (selectedName: string) => {
+    pollingBatches(listBatchAPI, true);
+    setBatchSelected(selectedName);
+    setDetailedBatchView(true);
+  };
+
+  const handleDeleteBatch = (batch: string) => {
+    setSelectedBatch(batch);
     setDeletePopupOpen(true);
   };
   const handleCancelDelete = () => {
     setDeletePopupOpen(false);
   };
 
   const handleDelete = async () => {
-    await RunTimeSerive.deleteRuntimeTemplateAPI(
-      selectedRuntimeTemplateValue,
-      selectedRuntimeTemplateDisplayName
-    );
+    await deleteBatchAPI(selectedBatch);
+    listBatchAPI();
+    setDetailedBatchView(false);
     setDeletePopupOpen(false);
   };
-  const {
-    getTableProps,
-    getTableBodyProps,
-    headerGroups,
-    rows,
-    prepareRow,
-    state,
-    preGlobalFilteredRows,
-    setGlobalFilter,
-    page,
-    canPreviousPage,
-    canNextPage,
-    nextPage,
-    previousPage,
-    setPageSize,
-    state: { pageIndex, pageSize }
-  } = useTable(
-    //@ts-ignore columns Header, accessor with interface issue
-    { columns, data, autoResetPage: false, initialState: { pageSize: 50 } },
-    useGlobalFilter,
-    usePagination
-  );
-
-  useEffect(() => {
-    listRuntimeTemplatesAPI();
-    if (!openCreateTemplate) {
-      pollingRuntimeTemplates(listRuntimeTemplatesAPI, pollingDisable);
-    }
 
-    return () => {
-      pollingRuntimeTemplates(listRuntimeTemplatesAPI, true);
-    };
-  }, [pollingDisable, openCreateTemplate]);
-
-  const renderActions = (data: ISessionTemplate) => {
-    let runtimeTemplateName = data.name;
-    let runtimeTemplateDisplayName = data?.jupyterSession?.displayName;
+  const renderActions = (data: { name: string }) => {
     return (
-      <div className="actions-icon">
+      <div className="actions-icon" role="button" aria-label="Delete Job">
         <div
-          role="button"
           className="icon-buttons-style"
-          title="Delete Runtime Template"
-          onClick={() =>
-            handleDeleteRuntimeTemplate(
-              runtimeTemplateName,
-              runtimeTemplateDisplayName
-            )
-          }
+          title="Delete Batch"
+          onClick={() => handleDeleteBatch(data.name.split('/')[5])}
         >
-          <iconDelete.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconDelete.react tag="div" />
         </div>
       </div>
     );
   };
 
-  const handleRuntimeTemplatesName = (selectedValue: ICellProps) => {
-    let selectedRunTimeAll: ISessionTemplate[] = [];
-    /*
-         Extracting runtimeId from name
-         Example: "projects/{projectName}/locations/{region}/sessionTemplates/{runtimeid}",
-      */
-
-    runTimeTemplateAllList.forEach((data: ISessionTemplate) => {
-      if (data.name.split('/')[5] === selectedValue.row.original.id) {
-        selectedRunTimeAll.push(data);
-      }
-    });
-
-    pollingRuntimeTemplates(listRuntimeTemplatesAPI, true);
-    setSelectedRuntimeClone(selectedRunTimeAll[0]);
-    setOpenCreateTemplate(true);
-  };
-
-  const handleCreateBatchOpen = () => {
-    setOpenCreateTemplate(true);
-    setSelectedRuntimeClone(undefined);
-  };
-
-  const tableDataCondition = (cell: ICellProps) => {
-    if (cell.column.Header === 'Name') {
-      return (
-        <td
-          role="button"
-          {...cell.getCellProps()}
-          className="cluster-name"
-          onClick={() => handleRuntimeTemplatesName(cell)}
-        >
-          {cell.value}
-        </td>
-      );
+  const toggleStyleSelection = (toggleItem: string) => {
+    if (selectedMode === toggleItem) {
+      return 'selected-header';
     } else {
-      return (
-        <td {...cell.getCellProps()} className="runtime-table-data">
-          {cell.render('Cell')}
-        </td>
-      );
+      return 'unselected-header';
     }
   };
 
+  useEffect(() => {
+    checkConfig(setLoggedIn, setConfigError, setLoginError);
+    const localstorageGetInformation = localStorage.getItem('loginState');
+    setLoggedIn(localstorageGetInformation === LOGIN_STATE);
+    if (loggedIn) {
+      setConfigLoading(false);
+    }
+    listBatchAPI();
+    if (!detailedBatchView && selectedMode === 'Batches') {
+      pollingBatches(listBatchAPI, pollingDisable);
+    }
+
+    return () => {
+      pollingBatches(listBatchAPI, true);
+    };
+  }, [pollingDisable, detailedBatchView, selectedMode]);
+
   return (
-    <div className="list-runtime-template-wrapper">
+    <div className="component-level">
+      {configLoading && !loggedIn && !configError && !loginError && (
+        <div className="spin-loaderMain">
+          <ClipLoader
+            color="#8A8A8A"
+            loading={true}
+            size={18}
+            aria-label="Loading Spinner"
+            data-testid="loader"
+          />
+          Loading Batches
+        </div>
+      )}
       {deletePopupOpen && (
         <DeletePopup
           onCancel={() => handleCancelDelete()}
           onDelete={() => handleDelete()}
           deletePopupOpen={deletePopupOpen}
           DeleteMsg={
-            'This will delete ' +
-            selectedRuntimeTemplateDisplayName +
-            ' and cannot be undone.'
+            'This will delete ' + selectedBatch + ' and cannot be undone.'
           }
         />
       )}
-      <div className="create-runtime-button-wrapper">
-        <div
-          className="create-runtime-overlay"
-          onClick={() => {
-            handleCreateBatchOpen();
-          }}
-        >
-          <div className="create-icon">
-            <iconSubmitJob.react tag="div" className="logo-alignment-style" />
-          </div>
-          <div className="create-text">Create</div>
-        </div>
-      </div>
-      {runtimeTemplateslist.length > 0 && !openCreateTemplate ? (
-        <div>
-          <div className="filter-cluster-overlay">
-            <div className="filter-cluster-icon">
-              <iconFilter.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
-            </div>
-            <div className="filter-cluster-text"></div>
-            <div className="filter-cluster-section">
-              <GlobalFilter
-                preGlobalFilteredRows={preGlobalFilteredRows}
-                globalFilter={state.globalFilter}
-                setGlobalFilter={setGlobalFilter}
-                setPollingDisable={setPollingDisable}
-              />
-            </div>
-          </div>
-          <div className="runtime-list-table-parent">
-            <TableData
-              getTableProps={getTableProps}
-              headerGroups={headerGroups}
-              getTableBodyProps={getTableBodyProps}
-              isLoading={isLoading}
-              rows={rows}
-              page={page}
-              prepareRow={prepareRow}
-              tableDataCondition={tableDataCondition}
-              fromPage="Runtime Templates"
+      {loggedIn && !configError ? (
+        <>
+          {detailedBatchView && (
+            <BatchDetails
+              batchSelected={batchSelected}
+              setDetailedBatchView={setDetailedBatchView}
+            />
+          )}
+          {createBatchView && (
+            <CreateBatch
+              setCreateBatchView={setCreateBatchView}
+              regionName={regionName}
+              projectName={projectName}
             />
-            {runtimeTemplateslist.length > 50 && (
-              <PaginationView
-                pageSize={pageSize}
-                setPageSize={setPageSize}
-                pageIndex={pageIndex}
-                allData={runtimeTemplateslist}
-                previousPage={previousPage}
-                nextPage={nextPage}
-                canPreviousPage={canPreviousPage}
-                canNextPage={canNextPage}
-              />
-            )}
-          </div>
-        </div>
-      ) : (
-        <div>
-          {isLoading && (
-            <div className="spin-loader-runtime">
-              <CircularProgress
-                className = "spin-loader-custom-style"
-                size={18}
-                aria-label="Loading Spinner"
-                data-testid="loader"
-              />
-              Loading Runtime Templates
-            </div>
           )}
-          {!isLoading && !openCreateTemplate && (
-            <div className="no-data-style">No rows to display</div>
+
+          {!detailedBatchView && !createBatchView && (
+            <div className="clusters-list-component" role="tablist">
+              {
+                <div className="clusters-list-overlay" role="tab">
+                  <div
+                    role="tabpanel"
+                    className={toggleStyleSelection('Batches')}
+                    onClick={() => selectedModeChange('Batches')}
+                  >
+                    Batches
+                  </div>
+                  <div
+                    role="tabpanel"
+                    className={toggleStyleSelection('Sessions')}
+                    onClick={() => selectedModeChange('Sessions')}
+                  >
+                    Sessions
+                  </div>
+                </div>
+              }
+              <div>
+                {selectedMode === 'Sessions' ? (
+                  <ListSessions />
+                ) : (
+                  <ListBatches
+                    batchesList={batchesList}
+                    isLoading={isLoading}
+                    setPollingDisable={setPollingDisable}
+                    listBatchAPI={listBatchAPI}
+                    handleBatchDetails={handleBatchDetails}
+                    setCreateBatchView={setCreateBatchView}
+                    createBatchView={createBatchView}
+                  />
+                )}
+              </div>
+              <ToastContainer />
+            </div>
           )}
+        </>
+      ) : (
+        loginError && (
+          <div role="alert" className="login-error">
+            Please login to continue
+          </div>
+        )
+      )}
+      {configError && (
+        <div role="alert" className="login-error">
+          Please configure gcloud with account, project-id and region
         </div>
       )}
     </div>
   );
-}
+};
 
-export default ListRuntimeTemplates;
+export class Batches extends ReactWidget {
+  constructor() {
+    super();
+  }
+
+  render(): React.JSX.Element {
+    return <BatchesComponent />;
+  }
+}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/sessions/listSessions.tsx` & `dataproc_jupyter_plugin-0.1.9/src/sessions/listSessions.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -11,43 +11,53 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
+import React, { useState, useEffect, useRef } from 'react';
+import { useTable, useGlobalFilter, usePagination } from 'react-table';
 import { LabIcon } from '@jupyterlab/ui-components';
-import React, { useEffect, useRef, useState } from 'react';
-import { useGlobalFilter, usePagination, useTable } from 'react-table';
-import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
-import deleteIcon from '../../style/icons/delete_icon.svg';
 import filterIcon from '../../style/icons/filter_icon.svg';
-import stopDisableIcon from '../../style/icons/stop_disable_icon.svg';
-import stopIcon from '../../style/icons/stop_icon.svg';
 import SucceededIcon from '../../style/icons/succeeded_icon.svg';
+import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
+import stopIcon from '../../style/icons/stop_icon.svg';
+import stopDisableIcon from '../../style/icons/stop_disable_icon.svg';
+import deleteIcon from '../../style/icons/delete_icon.svg';
+import { ClipLoader } from 'react-spinners';
+import GlobalFilter from '../utils/globalFilter';
 import {
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
   ClusterStatus,
   STATUS_ACTIVE,
   STATUS_CREATING,
   STATUS_DELETING,
   STATUS_FAIL,
   STATUS_PENDING,
   STATUS_PROVISIONING,
   STATUS_TERMINATED,
   STATUS_TERMINATING
 } from '../utils/const';
+import TableData from '../utils/tableData';
+import {
+  ICellProps,
+  authApi,
+  elapsedTime,
+  jobTimeFormat
+} from '../utils/utils';
+import SessionDetails from './sessionDetails';
 import DeletePopup from '../utils/deletePopup';
-import GlobalFilter from '../utils/globalFilter';
+import { toast, ToastContainer } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
+import { deleteSessionAPI, terminateSessionAPI } from '../utils/sessionService';
 import { PaginationView } from '../utils/paginationView';
 import PollingTimer from '../utils/pollingTimer';
-import { SessionService } from './sessionService';
-import TableData from '../utils/tableData';
-import { ICellProps } from '../utils/utils';
-import SessionDetails from './sessionDetails';
-import { CircularProgress } from '@mui/material';
 
 const iconFilter = new LabIcon({
   name: 'launcher:filter-icon',
   svgstr: filterIcon
 });
 const iconSucceeded = new LabIcon({
   name: 'launcher:succeeded-icon',
@@ -67,14 +77,15 @@
   svgstr: stopDisableIcon
 });
 const iconDelete = new LabIcon({
   name: 'launcher:delete-icon',
   svgstr: deleteIcon
 });
 
+
 function ListSessions() {
   const [sessionsList, setSessionsList] = useState([]);
   const [isLoading, setIsLoading] = useState(true);
   const [pollingDisable, setPollingDisable] = useState(false);
   const [sessionSelected, setSessionSelected] = useState('');
   const [detailedSessionView, setDetailedSessionView] = useState(false);
 
@@ -125,35 +136,109 @@
         Header: 'Actions',
         accessor: 'actions'
       }
     ],
     []
   );
 
-  const listSessionsAPI = async () => {
-    await SessionService.listSessionsAPIService(
-      renderActions,
-      setIsLoading,
-      setSessionsList
-    );
+  const listSessionsAPI = async (
+    nextPageToken?: string,
+    previousSessionsList?: object
+  ) => {
+    const credentials = await authApi();
+    const pageToken = nextPageToken ?? '';
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessions?pageSize=50&pageToken=${pageToken}`,
+        {
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              let transformSessionListData = [];
+              if (responseResult && responseResult.sessions) {
+                let sessionsListNew = responseResult.sessions;
+                sessionsListNew.sort(
+                  (a: { createTime: string }, b: { createTime: string }) => {
+                    const dateA = new Date(a.createTime);
+                    const dateB = new Date(b.createTime);
+                    return Number(dateB) - Number(dateA);
+                  }
+                );
+                transformSessionListData = sessionsListNew.map((data: any) => {
+                  const startTimeDisplay = jobTimeFormat(data.createTime);
+                  const startTime = new Date(data.createTime);
+                  let elapsedTimeString = '';
+                  if (
+                    data.state === STATUS_TERMINATED ||
+                    data.state === STATUS_FAIL
+                  ) {
+                    elapsedTimeString = elapsedTime(data.stateTime, startTime);
+                  }
+                  /*
+                    Extracting sessionID, location from sessionInfo.name
+                    Example: "projects/{project}/locations/{location}/sessions/{sessionID}"
+                  */
+                  return {
+                    sessionID: data.name.split('/')[5],
+                    status: data.state,
+                    location: data.name.split('/')[3],
+                    creator: data.creator,
+                    creationTime: startTimeDisplay,
+                    elapsedTime: elapsedTimeString,
+                    actions: renderActions(data)
+                  };
+                });
+              }
+
+              const existingSessionsData = previousSessionsList ?? [];
+              //setStateAction never type issue
+              let allSessionsData: any = [
+                ...(existingSessionsData as []),
+                ...transformSessionListData
+              ];
+
+              if (responseResult.nextPageToken) {
+                listSessionsAPI(responseResult.nextPageToken, allSessionsData);
+              } else {
+                setSessionsList(allSessionsData);
+                setIsLoading(false);
+              }
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error listing Sessions', err);
+          toast.error('Failed to fetch sessions');
+        });
+    }
   };
 
   const handleDeleteSession = (session: string) => {
     setSelectedSessionValue(session);
     setDeletePopupOpen(true);
   };
   const handleCancelDelete = () => {
     setDeletePopupOpen(false);
   };
 
   const handleDelete = async () => {
-    await SessionService.deleteSessionAPI(selectedSessionValue);
+    await deleteSessionAPI(selectedSessionValue);
     setDeletePopupOpen(false);
   };
-
   const {
     getTableProps,
     getTableBodyProps,
     headerGroups,
     rows,
     prepareRow,
     state,
@@ -169,26 +254,24 @@
   } = useTable(
     { columns, data, autoResetPage: false, initialState: { pageSize: 50 } },
     useGlobalFilter,
     usePagination
   );
 
   useEffect(() => {
-    if (!pollingDisable) {
-      listSessionsAPI();
+    listSessionsAPI();
+    if (!detailedSessionView) {
+      pollingSessions(listSessionsAPI, pollingDisable);
     }
+
     return () => {
       pollingSessions(listSessionsAPI, true);
     };
   }, [pollingDisable, detailedSessionView]);
-  useEffect(() => {
-    if (!detailedSessionView && !isLoading) {
-      pollingSessions(listSessionsAPI, pollingDisable);
-    }
-  }, [isLoading]);
+
   const renderActions = (data: { state: ClusterStatus; name: string }) => {
     /*
       Extracting sessionId from sessionInfo
       Example: "projects/{project}/locations/{location}/sessions/{name}"
     */
     let sessionValue = data.name.split('/')[5];
 
@@ -201,40 +284,31 @@
             data.state === ClusterStatus.STATUS_ACTIVE
               ? 'icon-buttons-style'
               : 'icon-buttons-style-disable'
           }
           title="Terminate Session"
           onClick={
             data.state === ClusterStatus.STATUS_ACTIVE
-              ? () => SessionService.terminateSessionAPI(sessionValue)
+              ? () => terminateSessionAPI(sessionValue)
               : undefined
           }
         >
           {data.state === ClusterStatus.STATUS_ACTIVE ? (
-            <iconStop.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
+            <iconStop.react tag="div" />
           ) : (
-            <iconStopDisable.react
-              tag="div"
-              className="icon-white logo-alignment-style"
-            />
+            <iconStopDisable.react tag="div" />
           )}
         </div>
         <div
           role="button"
           className="icon-buttons-style"
           title="Delete Session"
           onClick={() => handleDeleteSession(sessionValue)}
         >
-          <iconDelete.react
-            tag="div"
-            className="icon-white logo-alignment-style"
-          />
+          <iconDelete.react tag="div" />
         </div>
       </div>
     );
   };
   const handleSessionDetails = (selectedName: string) => {
     pollingSessions(listSessionsAPI, true);
     setSessionSelected(selectedName);
@@ -254,32 +328,27 @@
         </td>
       );
     }
     if (cell.column.Header === 'Status') {
       return (
         <td {...cell.getCellProps()} className="clusters-table-data">
           <div key="Status" className="cluster-status-parent">
-            {cell.value === STATUS_FAIL && (
-              <iconClusterError.react
-                tag="div"
-                className="logo-alignment-style"
-              />
-            )}
+            {cell.value === STATUS_FAIL && <iconClusterError.react tag="div" />}
             {cell.value === STATUS_TERMINATED && (
-              <iconSucceeded.react tag="div" className="logo-alignment-style" />
-            )}
-            {cell.value === STATUS_ACTIVE && (
-              <iconSucceeded.react tag="div" className="logo-alignment-style" />
+              <iconSucceeded.react tag="div" />
             )}
+            {cell.value === STATUS_ACTIVE && <iconSucceeded.react tag="div" />}
             {(cell.value === STATUS_PROVISIONING ||
               cell.value === STATUS_CREATING ||
               cell.value === STATUS_PENDING ||
               cell.value === STATUS_TERMINATING ||
               cell.value === STATUS_DELETING) && (
-              <CircularProgress
+              <ClipLoader
+                color="#8A8A8A"
+                loading={true}
                 size={15}
                 aria-label="Loading Spinner"
                 data-testid="loader"
               />
             )}
             <div className="cluster-status">
               {cell.value && cell.value.toLowerCase()}
@@ -294,14 +363,15 @@
         </td>
       );
     }
   };
 
   return (
     <div>
+      <ToastContainer />
       {deletePopupOpen && (
         <DeletePopup
           onCancel={() => handleCancelDelete()}
           onDelete={() => handleDelete()}
           deletePopupOpen={deletePopupOpen}
           DeleteMsg={
             'This will delete ' +
@@ -317,18 +387,15 @@
           detailedSessionView={detailedSessionView}
         />
       )}
       {sessionsList.length > 0 && !detailedSessionView ? (
         <div>
           <div className="filter-cluster-overlay">
             <div className="filter-cluster-icon">
-              <iconFilter.react
-                tag="div"
-                className="icon-white logo-alignment-style"
-              />
+              <iconFilter.react tag="div" />
             </div>
             <div className="filter-cluster-text"></div>
             <div className="filter-cluster-section">
               <GlobalFilter
                 preGlobalFilteredRows={preGlobalFilteredRows}
                 globalFilter={state.globalFilter}
                 setGlobalFilter={setGlobalFilter}
@@ -361,17 +428,18 @@
               />
             )}
           </div>
         </div>
       ) : (
         <div>
           {isLoading && (
-            <div className="spin-loader-main">
-              <CircularProgress
-                className = "spin-loader-custom-style"
+            <div className="spin-loaderMain">
+              <ClipLoader
+                color="#8A8A8A"
+                loading={true}
                 size={18}
                 aria-label="Loading Spinner"
                 data-testid="loader"
               />
               Loading Sessions
             </div>
           )}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/sessions/sessionDetails.tsx` & `dataproc_jupyter_plugin-0.1.9/src/sessions/sessionDetails.tsx`

 * *Files 27% similar despite different names*

```diff
@@ -18,47 +18,42 @@
 import React, { useState, useEffect, useRef } from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
 import LeftArrowIcon from '../../style/icons/left_arrow_icon.svg';
 import StopClusterIcon from '../../style/icons/stop_cluster_icon.svg';
 import StopClusterDisableIcon from '../../style/icons/stop_cluster_disable_icon.svg';
 import SucceededIcon from '../../style/icons/succeeded_icon.svg';
 import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
-import errorIcon from '../../style/icons/error_icon.svg';
 import {
-  DATAPROC_CLUSTER_KEY,
-  DATAPROC_CLUSTER_LABEL,
-  METASTORE_SERVICE_KEY,
-  METASTORE_SERVICE_LABEL,
+  API_HEADER_BEARER,
+  API_HEADER_CONTENT_TYPE,
+  BASE_URL,
   NETWORK_KEY,
   NETWORK_LABEL,
-  NETWORK_TAGS_KEY,
-  NETWORK_TAGS_LABEL,
   SERVICE_ACCOUNT_KEY,
   SERVICE_ACCOUNT_LABEL,
-  SPARK_HISTORY_SERVER,
-  SPARK_HISTORY_SERVER_KEY,
   STATUS_ACTIVE,
   STATUS_CREATING,
   STATUS_DELETING,
   STATUS_ERROR,
   STATUS_FAIL,
   STATUS_PROVISIONING,
   STATUS_STARTING,
   STATUS_STOPPING,
   STATUS_TERMINATED,
   STATUS_TERMINATING,
   SUBNETWORK_KEY,
   SUBNETWORK_LABEL
 } from '../utils/const';
-import { elapsedTime, jobTimeFormat } from '../utils/utils';
+import { authApi, elapsedTime, jobTimeFormat } from '../utils/utils';
+import ClipLoader from 'react-spinners/ClipLoader';
 import ViewLogs from '../utils/viewLogs';
-import { SessionService } from './sessionService';
+import { toast, ToastContainer } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
+import { terminateSessionAPI } from '../utils/sessionService';
 import PollingTimer from '../utils/pollingTimer';
-import { JupyterLab } from '@jupyterlab/application';
-import { CircularProgress } from '@mui/material';
 
 const iconLeftArrow = new LabIcon({
   name: 'launcher:left-arrow-icon',
   svgstr: LeftArrowIcon
 });
 const iconStopCluster = new LabIcon({
   name: 'launcher:stop-cluster-icon',
@@ -73,90 +68,97 @@
   svgstr: SucceededIcon
 });
 
 const iconClusterError = new LabIcon({
   name: 'launcher:cluster-error-icon',
   svgstr: clusterErrorIcon
 });
-const iconError = new LabIcon({
-  name: 'launcher:error-icon',
-  svgstr: errorIcon
-});
 
 interface ISessionDetailsProps {
   sessionSelected: string;
   setDetailedSessionView: (value: boolean) => void;
   detailedSessionView: boolean;
-  fromPage?: string;
-  app?: JupyterLab;
 }
 function SessionDetails({
   sessionSelected,
   setDetailedSessionView,
-  detailedSessionView,
-  fromPage,
-  app
+  detailedSessionView
 }: ISessionDetailsProps) {
   const [sessionInfo, setSessionInfo] = useState({
     state: '',
     name: '',
     uuid: '',
     elapsedTime: '',
     createTime: '',
     stateTime: '',
     stateHistory: [{ stateStartTime: '' }],
     runtimeConfig: { properties: [] },
-    stateMessage: '',
     environmentConfig: {
-      executionConfig: {
-        serviceAccount: '',
-        subnetworkUri: '',
-        networkTags: [],
-        kmsKey: ''
-      },
-      peripheralsConfig: {
-        metastoreService: '',
-        sparkHistoryServerConfig: {
-          dataprocCluster: ''
-        }
-      }
+      executionConfig: []
     }
   });
   const [isLoading, setIsLoading] = useState(true);
   const [labelDetail, setLabelDetail] = useState(['']);
   const timer = useRef<NodeJS.Timeout | undefined>(undefined);
-  const [errorView, setErrorView] = useState(false);
 
   const pollingSessionDetails = async (
     pollingFunction: () => void,
     pollingDisable: boolean
   ) => {
     timer.current = PollingTimer(
       pollingFunction,
       pollingDisable,
       timer.current
     );
   };
 
   const handleDetailedView = () => {
-    if (fromPage === 'Launcher') {
-      app?.shell.activeWidget?.close();
-    } else {
-      pollingSessionDetails(getSessionDetails, true);
-      setDetailedSessionView(false);
-    }
+    pollingSessionDetails(getSessionDetails, true);
+    setDetailedSessionView(false);
   };
   const getSessionDetails = async () => {
-    await SessionService.getSessionDetailsService(
-      sessionSelected,
-      setErrorView,
-      setIsLoading,
-      setLabelDetail,
-      setSessionInfo
-    );
+    const credentials = await authApi();
+    if (credentials) {
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessions/${sessionSelected}`,
+        {
+          method: 'GET',
+          headers: {
+            'Content-Type': API_HEADER_CONTENT_TYPE,
+            Authorization: API_HEADER_BEARER + credentials.access_token
+          }
+        }
+      )
+        .then((response: Response) => {
+          response
+            .json()
+            .then((responseResult: any) => {
+              setSessionInfo(responseResult);
+              const labelValue: string[] = [];
+              if (responseResult.labels) {
+                for (const [key, value] of Object.entries(
+                  responseResult.labels
+                )) {
+                  labelValue.push(`${key}:${value}`);
+                }
+              }
+              setLabelDetail(labelValue);
+              setIsLoading(false);
+            })
+            .catch((e: Error) => {
+              console.log(e);
+              setIsLoading(false);
+            });
+        })
+        .catch((err: Error) => {
+          setIsLoading(false);
+          console.error('Error loading session details', err);
+          toast.error(`Failed to fetch session details ${sessionSelected}`);
+        });
+    }
   };
 
   useEffect(() => {
     getSessionDetails();
     pollingSessionDetails(getSessionDetails, false);
 
     return () => {
@@ -186,76 +188,45 @@
   if (sessionActiveTime !== '') {
     const sessionInfoStateTime = new Date(sessionInfo.stateTime);
     runTimeString = elapsedTime(sessionInfoStateTime, sessionActiveTime);
   }
 
   return (
     <div>
-      {errorView && (
-        <div className="error-view-parent">
-          <div
-            role="button"
-            aria-label="back-arrow-icon"
-            className="back-arrow-icon"
-            onClick={() => handleDetailedView()}
-          >
-            <iconLeftArrow.react tag="div" className="logo-alignment-style" />
-          </div>
-          <div className="error-view-message-parent">
-            <iconError.react tag="div" className="logo-alignment-style" />
-            <div role="alert" className="error-view-message">
-              Unable to find the resource you requested
-            </div>
-          </div>
-        </div>
-      )}
-      {sessionInfo.name !== '' && !errorView ? (
-        <div className="scroll">
+      <ToastContainer />
+      {sessionInfo.name !== '' ? (
+        <div className="scroll-comp">
           {detailedSessionView && (
             <div>
-              <div className="scroll-fix-header cluster-details-header">
+              <div className="cluster-details-header">
                 <div
                   role="button"
                   className="back-arrow-icon"
                   onClick={() => handleDetailedView()}
                 >
-                  <iconLeftArrow.react
-                    tag="div"
-                    className="icon-white logo-alignment-style"
-                  />
+                  <iconLeftArrow.react tag="div" />
                 </div>
                 <div className="cluster-details-title">Session details</div>
                 <div
                   role="button"
                   className={
-                    sessionInfo.state === STATUS_ACTIVE ||
-                    sessionInfo.state === STATUS_CREATING
+                    sessionInfo.state === STATUS_ACTIVE
                       ? 'action-cluster-section'
                       : 'action-cluster-section disabled'
                   }
                   onClick={() =>
-                    sessionInfo.state === STATUS_ACTIVE ||
-                    (sessionInfo.state === STATUS_CREATING &&
-                      SessionService.terminateSessionAPI(
-                        sessionInfo.name.split('/')[5]
-                      ))
+                    sessionInfo.state === STATUS_ACTIVE &&
+                    terminateSessionAPI(sessionInfo.name.split('/')[5])
                   }
                 >
                   <div className="action-cluster-icon">
-                    {sessionInfo.state === STATUS_ACTIVE ||
-                    sessionInfo.state === STATUS_CREATING ? (
-                      <iconStopCluster.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                    {sessionInfo.state === STATUS_ACTIVE ? (
+                      <iconStopCluster.react tag="div" />
                     ) : (
-                      <iconStopClusterDisable.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                      <iconStopClusterDisable.react tag="div" />
                     )}
                   </div>
                   <div className="action-cluster-text">TERMINATE</div>
                 </div>
                 <ViewLogs sessionInfo={sessionInfo} />
               </div>
               <div className="cluster-details-container">
@@ -272,66 +243,48 @@
                     {sessionInfo.uuid}
                   </div>
                 </div>
                 <div className="row-details">
                   <div className="cluster-details-label">Status</div>
                   <div className="session-detail-status-parent">
                     {sessionInfo.state === STATUS_ACTIVE && (
-                      <iconSucceeded.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                      <iconSucceeded.react tag="div" />
                     )}
                     {sessionInfo.state === STATUS_TERMINATED && (
-                      <iconSucceeded.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                      <iconSucceeded.react tag="div" />
                     )}
                     {sessionInfo.state === STATUS_ERROR && (
-                      <iconClusterError.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                      <iconClusterError.react tag="div" />
                     )}
                     {sessionInfo.state === STATUS_FAIL && (
-                      <iconClusterError.react
-                        tag="div"
-                        className="logo-alignment-style"
-                      />
+                      <iconClusterError.react tag="div" />
                     )}
                     {(sessionInfo.state === STATUS_PROVISIONING ||
                       sessionInfo.state === STATUS_CREATING ||
                       sessionInfo.state === STATUS_STARTING ||
                       sessionInfo.state === STATUS_STOPPING ||
                       sessionInfo.state === STATUS_TERMINATING ||
                       sessionInfo.state === STATUS_DELETING) && (
                       <div>
-                        <CircularProgress
+                        <ClipLoader
+                          color="#8A8A8A"
+                          loading={true}
                           size={15}
                           aria-label="Loading Spinner"
                           data-testid="loader"
                         />
                       </div>
                     )}
                     <div className="cluster-status">
                       {sessionInfo.state === STATUS_CREATING
                         ? STATUS_PROVISIONING
                         : sessionInfo.state.toLowerCase()}
                     </div>
                   </div>
                 </div>
-                {sessionInfo.state === STATUS_FAIL && (
-                  <div className="row-details">
-                    <div className="cluster-details-label">Status Message</div>
-                    <div className="session-details-value">
-                      {sessionInfo.stateMessage}
-                    </div>
-                  </div>
-                )}
                 <div className="row-details">
                   <div className="cluster-details-label">Create time</div>
                   <div className="session-details-value">
                     {createTimeString}
                   </div>
                 </div>
               </div>
@@ -377,144 +330,43 @@
                   let label;
                   if (key === SERVICE_ACCOUNT_KEY) {
                     label = SERVICE_ACCOUNT_LABEL;
                   } else if (key === NETWORK_KEY) {
                     label = NETWORK_LABEL;
                   } else if (key === SUBNETWORK_KEY) {
                     label = SUBNETWORK_LABEL;
-                  } else if (key === NETWORK_TAGS_KEY) {
-                    label = NETWORK_TAGS_LABEL;
                   } else {
                     label = '';
                   }
                   if (
                     key === SERVICE_ACCOUNT_KEY ||
                     key === NETWORK_KEY ||
                     key === SUBNETWORK_KEY
                   ) {
                     return (
                       <div className="row-details" key={key}>
                         <div className="session-env-details-label">{label}</div>
                         <div className="session-env-details-value">{value}</div>
                       </div>
                     );
-                  } else if (key === NETWORK_TAGS_KEY) {
-                    return (
-                      <div className="row-details" key={key}>
-                        <div className="session-env-details-label">{label}</div>
-                        <div className="session-env-details-value">
-                          {
-                            //@ts-ignore value type issue
-                            value.map((item: string) => {
-                              return <div>{item}</div>;
-                            })
-                          }
-                        </div>
-                      </div>
-                    );
                   }
                 })}
-                {(sessionInfo?.environmentConfig?.peripheralsConfig
-                  ?.metastoreService ||
-                  sessionInfo?.environmentConfig?.peripheralsConfig
-                    ?.sparkHistoryServerConfig?.dataprocCluster) && (
-                  <div className="row-details">
-                    <div className="session-env-details-label">
-                      Peripherals config
-                    </div>
-                    <div className="session-env-details-value"></div>
-                  </div>
-                )}
-                {Object.entries(
-                  sessionInfo.environmentConfig.peripheralsConfig
-                ).map(([key, value]) => {
-                  let label;
-                  if (key === METASTORE_SERVICE_KEY) {
-                    label = METASTORE_SERVICE_LABEL;
-                  } else if (key === SPARK_HISTORY_SERVER_KEY) {
-                    label = SPARK_HISTORY_SERVER;
-                  } else {
-                    label = '';
-                  }
-                  <div className="row-details">
-                    <div className="session-env-details-label">
-                      Peripherals config
-                    </div>
-                    <div className="session-env-details-value"></div>
-                  </div>;
-                  if (key === METASTORE_SERVICE_KEY) {
-                    return (
-                      <div className="row-details" key={key}>
-                        <div className="session-env-details-label">{label}</div>
-                        <div className="session-env-details-value">
-                          {
-                            sessionInfo.environmentConfig.peripheralsConfig[
-                              METASTORE_SERVICE_KEY
-                            ]
-                          }
-                        </div>
-                      </div>
-                    );
-                  } else if (
-                    key === SPARK_HISTORY_SERVER_KEY &&
-                    sessionInfo?.environmentConfig?.peripheralsConfig
-                      ?.sparkHistoryServerConfig?.dataprocCluster
-                  ) {
-                    return (
-                      <div>
-                        <div className="row-details" key={key}>
-                          <div className="batch-details-label-level-two">
-                            {label}
-                          </div>
-                        </div>
-                        <div className="row-details" key={DATAPROC_CLUSTER_KEY}>
-                          <div className="batch-details-label-level-three">
-                            {DATAPROC_CLUSTER_LABEL}
-                          </div>
-                          <div className="session-env-details-value">
-                            {
-                              sessionInfo.environmentConfig.peripheralsConfig
-                                .sparkHistoryServerConfig[DATAPROC_CLUSTER_KEY]
-                            }
-                          </div>
-                        </div>
-                      </div>
-                    );
-                  }
-                })}
-
                 <div className="row-details">
-                  <div className="session-env-details-label">
-                    Encryption type
-                  </div>
-                  <div className="session-env-details-value">
-                    {sessionInfo?.environmentConfig?.executionConfig?.kmsKey
-                      ? 'Customer-managed'
-                      : 'Google-managed'}
-                  </div>
+                  <div className="session-env-details-label">Network tags</div>
+                  <div className="session-env-details-value"></div>
                 </div>
-                {sessionInfo?.environmentConfig?.executionConfig?.kmsKey && (
-                  <div className="row-details">
-                    <div className="session-env-details-label">
-                      Encryption key
-                    </div>
-                    <div className="session-env-details-value">
-                      {sessionInfo.environmentConfig.executionConfig.kmsKey}
-                    </div>
-                  </div>
-                )}
                 <div className="row-details">
                   <div className="cluster-details-label">Labels</div>
                   <div className="session-label-style-parent">
                     {labelDetail.length > 0
                       ? labelDetail.map(label => {
                           /*
-                          Extracting key, value from label
-                             Example: "{client:dataproc_jupyter_plugin}"
-                       */
+                            Extracting key, value from label
+                               Example: "{client:dataproc_jupyter_plugin}"
+                         */
                           const labelParts = label.split(':');
 
                           return (
                             <div key={label} className="job-label-style">
                               {labelParts[0]} : {labelParts[1]}
                             </div>
                           );
@@ -523,26 +375,27 @@
                   </div>
                 </div>
               </div>
             </div>
           )}
         </div>
       ) : (
-        <>
+        <div className="loader-full-style">
           {isLoading && (
-            <div className="spin-loader-main">
-              <CircularProgress
-                className = "spin-loader-custom-style"
-                size={18}
+            <div className="session-loader">
+              <ClipLoader
+                color="#8A8A8A"
+                loading={true}
+                size={20}
                 aria-label="Loading Spinner"
                 data-testid="loader"
               />
               Loading Session Details
             </div>
           )}
-        </>
+        </div>
       )}
     </div>
   );
 }
 
 export default SessionDetails;
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/globalFilter.tsx` & `dataproc_jupyter_plugin-0.1.9/src/utils/globalFilter.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -16,44 +16,38 @@
  */
 
 import React from 'react';
 
 function GlobalFilter({
   globalFilter,
   setGlobalFilter,
-  setPollingDisable,
-  gcsBucket,
-  fromPage
+  setPollingDisable
 }: any) {
   const [value, setValue] = React.useState(globalFilter);
   const onChange = (value: string) => {
     setGlobalFilter(value || undefined);
   };
-  if (fromPage !== 'notebook-templates') {
-    if (value !== undefined) {
-      if (value.length !== 0) {
-        setPollingDisable(true);
-      } else {
-        setPollingDisable(false);
-      }
+  if (value !== undefined) {
+    if (value.length !== 0) {
+      setPollingDisable(true);
+    } else {
+      setPollingDisable(false);
     }
   }
 
   return (
     <span>
       <input
         value={value || ''}
         onChange={e => {
           setValue(e.target.value);
           onChange(e.target.value);
         }}
-        placeholder={gcsBucket ? 'Filter files by name' : 'Filter Table'}
+        placeholder={'Filter Table'}
         aria-label="filterd value"
-        className={
-          gcsBucket ? 'gcs-filter-section-part' : 'filter-section-part'
-        }
+        className="filter-section-part"
       />
     </span>
   );
 }
 
 export default GlobalFilter;
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/jobDetailsInterface.ts` & `dataproc_jupyter_plugin-0.1.9/src/utils/jobDetailsInterface.ts`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/listRuntimeTemplateInterface.ts` & `dataproc_jupyter_plugin-0.1.9/src/utils/listRuntimeTemplateInterface.ts`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-export interface ISessionTemplateRoot {
-  error: {
-    code: number;
-    message: string;
-  };
-  sessionTemplates: ISessionTemplate[];
+export interface SessionTemplateRoot {
+  sessionTemplates: SessionTemplate[];
   nextPageToken: string;
 }
 
-export interface ISessionTemplate {
+export interface SessionTemplate {
   name: string;
   createTime: string;
-  jupyterSession: IJupyterSession;
+  jupyterSession: JupyterSession;
   creator: string;
-  labels: ILabels;
-  environmentConfig: IEnvironmentConfig;
+  labels: Labels;
+  environmentConfig: EnvironmentConfig;
   description: string;
   updateTime: string;
 }
 
-export interface IJupyterSession {
+export interface JupyterSession {
   kernel: string;
   displayName: string;
 }
 
-export interface ILabels {
+export interface Labels {
   purpose: string;
 }
 
-export interface IEnvironmentConfig {
-  executionConfig: IExecutionConfig;
+export interface EnvironmentConfig {
+  executionConfig: ExecutionConfig;
 }
 
-export interface IExecutionConfig {
+export interface ExecutionConfig {
   subnetworkUri: string;
 }
 
-export interface ISessionTemplateDisplay {
+export interface SessionTemplateDisplay {
   name: string;
   owner: string;
   description: string;
   lastModified: string;
-  id: string;
+  id:string
 }
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/metastoreService.ts` & `dataproc_jupyter_plugin-0.1.9/src/utils/projectService.ts`

 * *Files 18% similar despite different names*

```diff
@@ -11,41 +11,64 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
+import { useEffect, useRef, useState } from 'react';
 import {
   API_HEADER_BEARER,
   API_HEADER_CONTENT_TYPE,
-  gcpServiceUrls
-} from './const';
-import { authApi, loggedFetch } from './utils';
+  PROJECT_LIST_URL
+} from '../utils/const';
+import { authApi } from '../utils/utils';
 
-export const metastoreServiceListAPI = async (
-  projectId: string,
-  prefix: string
-): Promise<string[]> => {
+interface Project {
+  projectId: string;
+  name: string;
+}
+
+const projectListAPI = async (prefix: string): Promise<Project[]> => {
   const credentials = await authApi();
-  const { METASTORE } = await gcpServiceUrls;
   if (!credentials) {
     return [];
   }
-  const requestUrl = new URL(
-    `${METASTORE}/projects/${projectId}/locations/${credentials.region_id}/services`
-  );
+  const requestUrl = new URL(PROJECT_LIST_URL);
   if (prefix.length > 0) {
     requestUrl.searchParams.append('filter', `name:${prefix}*`);
   }
   requestUrl.searchParams.append('pageSize', '200');
-  const resp = await loggedFetch(requestUrl.toString(), {
+  const resp = await fetch(requestUrl.toString(), {
     method: 'GET',
     headers: {
       'Content-Type': API_HEADER_CONTENT_TYPE,
       Authorization: API_HEADER_BEARER + credentials.access_token
     }
   });
-
-  const json = (await resp.json()) as { services: { name: string }[] };
-  return json.services.map(service => service.name);
+  const { projects } = (await resp.json()) as { projects: Project[] };
+  return projects;
 };
+
+/**
+ * Hook for returning a list of Cloud Project Names with the prefix
+ * specified.
+ * @param prefix The prefix string to search for.
+ * @returns List of projects that matches the prefix.  If the results
+ *   are pending, an empty list is returned.
+ */
+export function useProjectList(prefix: string) {
+  const [projects, setProjects] = useState<Project[]>([]);
+  const currentPrefix = useRef(prefix);
+  useEffect(() => {
+    currentPrefix.current = prefix;
+    projectListAPI(prefix).then(projects => {
+      if (currentPrefix.current != prefix) {
+        // The prefix changed while the network request was pending
+        // so we should throw away these results.
+        return;
+      }
+      setProjects(projects);
+    });
+  }, [prefix]);
+  return projects;
+}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/networkService.ts` & `dataproc_jupyter_plugin-0.1.9/src/utils/sessionService.tsx`

 * *Files 27% similar despite different names*

```diff
@@ -12,68 +12,64 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 import {
-  API_HEADER_BEARER,
   API_HEADER_CONTENT_TYPE,
-  gcpServiceUrls
-} from './const';
-import { authApi, loggedFetch } from './utils';
+  BASE_URL,
+  API_HEADER_BEARER
+} from '../utils/const';
+import { authApi } from '../utils/utils';
+import { toast } from 'react-toastify';
+import 'react-toastify/dist/ReactToastify.css';
 
-type Network = {
-  selfLink: string;
-  network: string;
-  subnetworks: string;
-};
-
-/**
- * Return a list of VPC Networks that matches the search term specified
- * for the current project.
- * @param search Search to feed to the name filter
- * @returns List of Networks that matches the search term.
- */
-export const listNetworksAPI = async (search: string) => {
+export const deleteSessionAPI = async (selectedSession: string) => {
   const credentials = await authApi();
-  const { COMPUTE } = await gcpServiceUrls;
-  if (!credentials) {
-    return [];
-  }
-  const requestUrl = new URL(
-    `${COMPUTE}/projects/${credentials.project_id}/global/networks`
-  );
-  if (search.length > 0) {
-    requestUrl.searchParams.append('filter', `name:${search}*`);
+  if (credentials) {
+    fetch(
+      `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessions/${selectedSession}`,
+      {
+        method: 'DELETE',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      }
+    )
+      .then((response: Response) => {
+        console.log(response);
+      })
+      .catch((err: Error) => {
+        console.error('Error deleting session', err);
+        toast.error(`Failed to delete the session ${selectedSession}`);
+      });
   }
-  const resp = await loggedFetch(requestUrl.toString(), {
-    headers: {
-      'Content-Type': API_HEADER_CONTENT_TYPE,
-      Authorization: API_HEADER_BEARER + credentials.access_token
-    }
-  });
-  const json = (await resp.json()) as { items: Network[] };
-  return json.items;
 };
-
-/**
- * Fetches all the subnetwork URIs for a given network.
- * @param network The networkURI to fetch all the subnetworks for.
- * @returns A list of subnetworksURI.
- */
-export const listSubNetworksAPI = async (network: string) => {
+export const terminateSessionAPI = async (selectedSession: string) => {
   const credentials = await authApi();
-  const { COMPUTE } = await gcpServiceUrls;
-  if (!credentials) return [];
-  const resp = await loggedFetch(
-    `${COMPUTE}/projects/${credentials.project_id}/global/networks/${network}`,
-    {
-      headers: {
-        'Content-Type': API_HEADER_CONTENT_TYPE,
-        Authorization: API_HEADER_BEARER + credentials.access_token
+  if (credentials) {
+    fetch(
+      `${BASE_URL}/projects/${credentials.project_id}/locations/${credentials.region_id}/sessions/${selectedSession}:terminate`,
+      {
+        method: 'POST',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
       }
-    }
-  );
-  const json: { subnetworks: string[] | null | undefined } = await resp.json();
-  return json.subnetworks ?? [];
+    )
+      .then((response: Response) => {
+        response
+          .json()
+          .then((responseResult: Response) => {
+            console.log(responseResult);
+          })
+          .catch((e: Error) => console.log(e));
+      })
+      .catch((err: Error) => {
+        console.error('Error terminating session', err);
+        toast.error(`Failed to terminate session ${selectedSession}`);
+      });
+  }
 };
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/paginationView.tsx` & `dataproc_jupyter_plugin-0.1.9/src/utils/paginationView.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -12,124 +12,94 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 import React from 'react';
-import { ISessionTemplateDisplay } from './listRuntimeTemplateInterface';
-import { Select } from '../controls/MuiWrappedSelect';
-import { LabIcon } from '@jupyterlab/ui-components';
-import PreviousIcon from '../../style/icons/previous_page.svg';
-import NextIcon from '../../style/icons/next_page.svg';
+import { SessionTemplateDisplay } from './listRuntimeTemplateInterface';
+
 interface IBatch {
   batchID: string;
   status: string;
   location: string;
   creationTime: string;
   elapsedTime: string;
-  type: string | undefined;
+  type: string;
   actions: JSX.Element;
 }
-interface ITemplate {
-  title: string;
-  category: string;
-  description: string;
-}
 interface ICluster {
   clusterName: string;
   status: string;
   clusterImage: string;
   region: string;
   zone: string;
   totalWorkersNode: string;
   schedulesDeletion: string;
   actions: React.ReactNode;
 }
-interface IDagList {
-  jobid: string;
-  notebookname: string;
-  schedule: string;
-  scheduleInterval: string;
-}
-
 interface IPaginationViewProps {
   pageSize: number;
   setPageSize: (value: number) => void;
   pageIndex: number;
-  allData:
-    | IBatch[]
-    | ITemplate[]
-    | ICluster[]
-    | ISessionTemplateDisplay[]
-    | IDagList[];
+  allData: IBatch[] | ICluster[] | SessionTemplateDisplay[];
   previousPage: () => void;
-  nextPage: () => void;
+  nextPage:  () => void;
   canPreviousPage: boolean;
   canNextPage: boolean;
 }
-const iconPrevious = new LabIcon({
-  name: 'launcher:previous-icon',
-  svgstr: PreviousIcon
-});
-const iconNext = new LabIcon({
-  name: 'launcher:next-icon',
-  svgstr: NextIcon
-});
 
 export const PaginationView = ({
   pageSize,
   setPageSize,
   pageIndex,
   allData,
   previousPage,
   nextPage,
   canPreviousPage,
   canNextPage
 }: IPaginationViewProps) => {
   return (
     <div className="pagination-parent-view">
       <div>Rows per page: </div>
-      <Select
+      <select
         className="page-size-selection"
-        value={pageSize.toString()} // Convert pageSize to string for compatibility
-        onChange={(e, { value }) => {
-          const selectedPageSize = parseInt(value as string, 10); // Parse the value to a number
-          setPageSize(selectedPageSize); // Use the parsed number as the new pageSize
+        value={pageSize}
+        onChange={e => {
+          setPageSize(Number(e.target.value));
         }}
-        options={[
-          { key: '50', value: '50', text: '50' },
-          { key: '100', value: '100', text: '100' },
-          { key: '200', value: '200', text: '200' }
-        ]}
-      />
+      >
+        {[50, 100, 200].map(pageSize => (
+          <option key={pageSize} value={pageSize}>
+            {pageSize}
+          </option>
+        ))}
+      </select>
       {(pageIndex + 1) * pageSize > allData.length ? (
         <div className="page-display-part">
-          {pageIndex * pageSize + 1} - {allData.length} of {allData.length}
+          {pageIndex * pageSize + 1} -{' '} {allData.length} of {allData.length}
         </div>
       ) : (
         <div className="page-display-part">
-          {pageIndex * pageSize + 1} - {(pageIndex + 1) * pageSize} of{' '}
+          {pageIndex * pageSize + 1} -{' '} {(pageIndex + 1) * pageSize} of{' '}
           {allData.length}
         </div>
       )}
-      <div
-        role="button"
+      <div role="button"
         className={
           !canPreviousPage ? 'page-move-button disabled' : 'page-move-button'
         }
         onClick={() => previousPage()}
       >
-        <iconPrevious.react tag="div" className="icon-white logo-alignment-style" />
+        {'<'}
       </div>
-      <div
-        role="button"
+      <div role="button"
         onClick={() => nextPage()}
         className={
           !canNextPage ? 'page-move-button disabled' : 'page-move-button'
         }
       >
-        <iconNext.react tag="div" className="icon-white logo-alignment-style" />
+        {'>'}
       </div>
     </div>
   );
 };
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/regionService.tsx` & `dataproc_jupyter_plugin-0.1.9/src/utils/jobServices.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -11,70 +11,65 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-
-import { useEffect, useRef, useState } from 'react';
-import { API_HEADER_BEARER, API_HEADER_CONTENT_TYPE, gcpServiceUrls } from '../utils/const';
-import { authApi, toastifyCustomStyle } from '../utils/utils';
 import { toast } from 'react-toastify';
+import { BASE_URL, API_HEADER_CONTENT_TYPE, API_HEADER_BEARER } from './const';
+import { authApi } from './utils';
 
-interface IRegions {
-  name: string;
-}
-
-const regionListAPI = async (projectId: string, credentials: any) => {
-  const { REGION_URL } = await gcpServiceUrls;
-  if(projectId !== ''){
-  try {
-    const resp = await fetch(`${REGION_URL}/${projectId}/regions`, {
-      method: 'GET',
-      headers: {
-        'Content-Type': API_HEADER_CONTENT_TYPE,
-        Authorization: API_HEADER_BEARER + credentials.access_token,
-      },
-    });
-   const responseResult = await resp.json()
-    if (responseResult?.error?.code)
-   {
-      throw new Error(responseResult?.error?.message);
-    }
-
-    const { items } = (responseResult) as { items: IRegions[] | undefined };
-    return items ?? [];
-  } catch (error) {
-    console.error(error);
-    throw error; 
-  }
-  }
-  else{
-    return [];
+export const stopJobApi = async (jobId: string) => {
+  const credentials = await authApi();
+  if (credentials) {
+    fetch(
+      `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/jobs/${jobId}:cancel`,
+      {
+        method: 'POST',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
+        }
+      }
+    )
+      .then((response: Response) => {
+        response
+          .json()
+          .then((responseResult: Response) => {
+            console.log(responseResult);
+          })
+          .catch((e: Error) => console.log(e));
+      })
+      .catch((err: Error) => {
+        console.error('Error to  stop job', err);
+        toast.error(`Failed to stop job ${jobId}`);
+      });
   }
 };
-
-export function useRegion(projectId: string) {
-  const [regions, setRegions] = useState<IRegions[]>([]);
-  const currentRegion = useRef(projectId);
-
-  useEffect(() => {
-    currentRegion.current = projectId;
-    authApi()
-      .then((credentials) => regionListAPI(projectId, credentials))
-      .then((items) => {
-        if (currentRegion.current !== projectId) {
-          // The project changed while the network request was pending
-          // so we should throw away these results.
-          return;
+export const deleteJobApi = async (jobId: string) => {
+  const credentials = await authApi();
+  if (credentials) {
+    fetch(
+      `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/jobs/${jobId}`,
+      {
+        method: 'DELETE',
+        headers: {
+          'Content-Type': API_HEADER_CONTENT_TYPE,
+          Authorization: API_HEADER_BEARER + credentials.access_token
         }
-        setRegions(items);
+      }
+    )
+      .then((response: Response) => {
+        response
+          .json()
+          .then((responseResult: Response) => {
+            console.log(responseResult);
+          })
+          .catch((e: Error) => console.log(e));
       })
-      .catch((error) => {
-        console.error(error);
-        toast.error(error.message,toastifyCustomStyle)
+      .catch((err: Error) => {
+        console.error('Error Deleting Job', err);
+        toast.error(`Failed to delete the job ${jobId}`);
       });
-  }, [projectId]);
-
-  return regions;
-}
+  }
+};
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/statusDisplay.tsx` & `dataproc_jupyter_plugin-0.1.9/src/utils/statusDisplay.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 import React from 'react';
+import { ClipLoader } from 'react-spinners';
 import {
   STATUS_CREATING,
   STATUS_DELETING,
   STATUS_FAIL,
   STATUS_PROVISIONING,
   STATUS_RUNNING,
   STATUS_STARTING,
@@ -29,15 +30,14 @@
   STATUS_SUCCESS
 } from '../utils/const';
 import { LabIcon } from '@jupyterlab/ui-components';
 import stopIcon from '../../style/icons/stop_icon.svg';
 import clusterRunningIcon from '../../style/icons/cluster_running_icon.svg';
 import clusterErrorIcon from '../../style/icons/cluster_error_icon.svg';
 import SucceededIcon from '../../style/icons/succeeded_icon.svg';
-import { CircularProgress } from '@mui/material';
 
 export const statusDisplay = (statusMsg: string) => {
   const iconClusterRunning = new LabIcon({
     name: 'launcher:cluster-running-icon',
     svgstr: clusterRunningIcon
   });
   const iconClusterError = new LabIcon({
@@ -51,33 +51,27 @@
   const iconStop = new LabIcon({
     name: 'launcher:stop-icon',
     svgstr: stopIcon
   });
 
   return (
     <div className="cluster-detail-status-parent">
-      {statusMsg === STATUS_CANCELLED && (
-        <iconStop.react tag="div" className="logo-alignment-style" />
-      )}
-      {statusMsg === STATUS_RUNNING && (
-        <iconClusterRunning.react tag="div" className="logo-alignment-style" />
-      )}
-      {statusMsg === STATUS_SUCCESS && (
-        <iconSucceeded.react tag="div" className="logo-alignment-style" />
-      )}
-      {statusMsg === STATUS_FAIL && (
-        <iconClusterError.react tag="div" className="logo-alignment-style" />
-      )}
+      {statusMsg === STATUS_CANCELLED && <iconStop.react tag="div" />}
+      {statusMsg === STATUS_RUNNING && <iconClusterRunning.react tag="div" />}
+      {statusMsg === STATUS_SUCCESS && <iconSucceeded.react tag="div" />}
+      {statusMsg === STATUS_FAIL && <iconClusterError.react tag="div" />}
       {(statusMsg === STATUS_PROVISIONING ||
         statusMsg === STATUS_CREATING ||
         statusMsg === STATUS_STARTING ||
         statusMsg === STATUS_STOPPING ||
         statusMsg === STATUS_PENDING ||
         statusMsg === STATUS_DELETING) && (
-        <CircularProgress
+        <ClipLoader
+          color="#8A8A8A"
+          loading={true}
           size={15}
           aria-label="Loading Spinner"
           data-testid="loader"
         />
       )}
       <div className="cluster-status">{statusMsg.toLowerCase()}</div>
     </div>
```

### Comparing `dataproc_jupyter_plugin-0.1.78/src/utils/viewLogs.tsx` & `dataproc_jupyter_plugin-0.1.9/src/utils/viewLogs.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -17,107 +17,53 @@
 
 import React from 'react';
 import { LabIcon } from '@jupyterlab/ui-components';
 import ViewLogsIcon from '../../style/icons/view_logs_icon.svg';
 import {
   API_HEADER_BEARER,
   API_HEADER_CONTENT_TYPE,
+  BASE_URL,
   SPARK_HISTORY_SERVER,
   VIEW_LOGS_BATCH_URL,
   VIEW_LOGS_CLUSTER_URL,
-  VIEW_LOGS_SESSION_URL,
-  gcpServiceUrls
+  VIEW_LOGS_SESSION_URL
 } from './const';
-import { authApi, loggedFetch } from './utils';
-import { DataprocLoggingService, LOG_LEVEL } from '../utils/loggingService';
+import { authApi } from './utils';
 
 const iconViewLogs = new LabIcon({
   name: 'launcher:view-logs-icon',
   svgstr: ViewLogsIcon
 });
-export interface IViewLogs {
-  config: IConfig;
-}
-
-export interface IConfig {
-  endpointConfig: IEndpointConfig;
-}
-
-export interface IEndpointConfig {
-  httpPorts: IHttpPorts;
-}
-
-export interface IHttpPorts {
-  config: IConfig;
-  error: {
-    code: number;
-  };
-  'Spark History Server': string;
-}
-interface IViewLogsProps {
-  clusterInfo?: {
-    clusterUuid: string;
-    clusterName: string;
-  };
-  projectName?: string;
-  clusterName?: string;
-  setErrorView?: (value: boolean) => void;
-  batchInfoResponse?:
-    | {
-        runtimeInfo?: {
-          endpoints?: {
-            [key: string]: string;
-          };
-        };
-        name?: string;
-        createTime?: string;
-      }
-    | undefined;
-  sessionInfo?: {
-    runtimeInfo?: {
-      endpoints?: {
-        [key: string]: string;
-      };
-    };
-    name: string;
-    createTime: string;
-  };
-}
 
 function ViewLogs({
   clusterInfo,
   projectName,
   clusterName,
   setErrorView,
   batchInfoResponse,
   sessionInfo
-}: IViewLogsProps) {
+}: any) {
   const handleJobDetailsViewLogs = async (clusterName: string) => {
     const credentials = await authApi();
-    const { DATAPROC } = await gcpServiceUrls;
     if (credentials) {
-      loggedFetch(
-        `${DATAPROC}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters/${clusterName}`,
+      fetch(
+        `${BASE_URL}/projects/${credentials.project_id}/regions/${credentials.region_id}/clusters/${clusterName}`,
         {
           method: 'GET',
           headers: {
             'Content-Type': API_HEADER_CONTENT_TYPE,
             Authorization: API_HEADER_BEARER + credentials.access_token
           }
         }
       )
         .then((response: Response) => {
           response
             .json()
-            .then((responseResult: IHttpPorts) => {
-              if (
-                responseResult.error &&
-                responseResult.error.code === 404 &&
-                setErrorView
-              ) {
+            .then((responseResult: any) => {
+              if (responseResult.error && responseResult.error.code === 404) {
                 setErrorView(true);
               } else {
                 window.open(
                   responseResult.config.endpointConfig.httpPorts[
                     SPARK_HISTORY_SERVER
                   ]
                 );
@@ -125,31 +71,29 @@
             })
             .catch((e: Error) => {
               console.error(e);
             });
         })
         .catch((err: Error) => {
           console.error('Error listing clusters Details', err);
-          DataprocLoggingService.log('Error listing clusters Details', LOG_LEVEL.ERROR);
-          
         });
     }
   };
 
   return (
     <>
       <div
         role="button"
         className={
           (batchInfoResponse?.runtimeInfo?.endpoints &&
             batchInfoResponse?.runtimeInfo?.endpoints[SPARK_HISTORY_SERVER]) ||
           (sessionInfo?.runtimeInfo?.endpoints &&
             sessionInfo?.runtimeInfo?.endpoints[SPARK_HISTORY_SERVER]) ||
-          clusterName ||
-          clusterInfo
+          (clusterName) ||
+          (clusterInfo)
             ? 'action-cluster-section'
             : 'action-disabled action-cluster-section'
         }
         onClick={() => {
           if (clusterInfo) {
             window.open(
               `${VIEW_LOGS_CLUSTER_URL}"${clusterInfo.clusterName}" resource.labels.cluster_uuid="${clusterInfo.clusterUuid}"?project=${projectName}`,
@@ -175,15 +119,15 @@
             );
           } else if (clusterName) {
             handleJobDetailsViewLogs(clusterName);
           }
         }}
       >
         <div className="action-cluster-icon">
-          <iconViewLogs.react tag="div" className="logo-alignment-style" />
+          <iconViewLogs.react tag="div" />
         </div>
         {clusterInfo ? (
           <div className="action-cluster-text">VIEW CLOUD LOGS</div>
         ) : (
           <div className="action-cluster-text">VIEW SPARK LOGS</div>
         )}
       </div>
@@ -191,50 +135,39 @@
         role="button"
         className="action-cluster-section"
         onClick={() => {
           /*
             Extracting project, location, session_id from sessionInfo.name
             Example: "projects/{project}/locations/{location}/sessionTemplates/{session_id}"
             */
-          if (sessionInfo) {
-            const sessionValueUri = sessionInfo.name.split('/');
+          const sessionValueUri = sessionInfo.name.split('/');
 
+          if (sessionInfo) {
             window.open(
               `${VIEW_LOGS_SESSION_URL} resource.labels.project_id="${sessionValueUri[1]}" resource.labels.location="${sessionValueUri[3]}" resource.labels.session_id="${sessionValueUri[5]}";cursorTimestamp=${sessionInfo.createTime};?project=${sessionValueUri[1]}`,
               '_blank'
             );
           } else {
             /*
-            Extracting project, location, batch_id from batchInfoResponse.name
+            Extracting project, location, batch_id from batchInfoResponse.name 
             Example: "projects/{project}/locations/{location}/batches/{batch_id}"
             */
-            const batchValueUri: string[] | undefined =
-              batchInfoResponse?.name?.split('/');
+            const batchValueUri = batchInfoResponse.name.split('/');
 
-            if (
-              batchValueUri &&
-              batchValueUri.length >= 6 &&
-              batchInfoResponse?.createTime
-            ) {
-              const project_id = batchValueUri[1];
-              const location = batchValueUri[3];
-              const batch_id = batchValueUri[5];
-              const cursorTimestamp = batchInfoResponse.createTime;
-
-              const url = `${VIEW_LOGS_BATCH_URL} resource.labels.project_id="${project_id}" resource.labels.location="${location}" resource.labels.batch_id="${batch_id}";cursorTimestamp=${cursorTimestamp};?project=${project_id}`;
-
-              window.open(url, '_blank');
-            }
+            window.open(
+              `${VIEW_LOGS_BATCH_URL} resource.labels.project_id="${batchValueUri[1]}" resource.labels.location="${batchValueUri[3]}" resource.labels.batch_id="${batchValueUri[5]}";cursorTimestamp=${batchInfoResponse.createTime};?project=${batchValueUri[1]}`,
+              '_blank'
+            );
           }
         }}
       >
         {!clusterInfo && !clusterName && (
           <>
             <div className="action-cluster-icon">
-              <iconViewLogs.react tag="div" className="logo-alignment-style" />
+              <iconViewLogs.react tag="div" />
             </div>
             <div className="action-cluster-text">VIEW CLOUD LOGS</div>
           </>
         )}
       </div>
     </>
   );
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/authLogin.css` & `dataproc_jupyter_plugin-0.1.9/style/authLogin.css`

 * *Files 16% similar despite different names*

```diff
@@ -3,85 +3,76 @@
 .signin-google-icon {
   align-items: center;
   display: flex;
   justify-content: center;
   margin-top: -20px;
   cursor: pointer;
 }
-
 .signin-google-icon:disabled {
   opacity: 0.5;
 }
-
 .settings-overlay {
   width: 100%;
   height: 80px;
   display: flex;
   flex-direction: row;
   align-items: flex-end;
   padding-bottom: 10px;
-  padding-left: 5px;
 }
 
 .settings-text {
   font-style: normal;
   font-weight: 400;
   font-size: 18px;
   line-height: 22px;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   padding-left: 10px;
   padding-bottom: 5px;
 }
 
-.settings-separator {
-  border-bottom: 1px solid var(--jp-layout-color3);
+.settings-seperator {
+  border: 1px solid #e0e0e0;
   width: 100%;
   height: 0px;
-  margin-left: 5px;
 }
-
 .config-form {
   display: flex;
   flex-direction: column;
-  padding-top: 30px;
-  padding-left: 5px;
-  padding-right: 20px;
+  padding-top: 60px;
   width: 100%;
   width: 630px;
 }
-
 .project-overlay {
   position: relative;
 }
-
 .region-overlay {
   position: relative;
   margin-top: 50px;
 }
-
 .project-text {
+  width: 60px;
   height: 13px;
   font-style: normal;
   font-weight: 1000;
   font-size: 12px;
   line-height: 13px;
   display: flex;
   align-items: center;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   position: absolute;
-  background-color: var(--jp-layout-color0);
+  background-color: #fff;
   bottom: 32px;
   padding-left: 2px;
   left: 7px;
 }
 
 .project-select {
   box-sizing: border-box;
-  background: var(--jp-layout-color0) !important;
-  border: 1px solid var(--jp-ui-font-color2) !important;
+  background: #ffffff !important;
+  border: 1px solid rgba(0, 0, 0, 0.38) !important;
   display: block !important;
   height: 36px;
   width: 100%;
   border-radius: 4px !important;
   appearance: none !important;
   -webkit-appearance: none !important;
   -moz-appearance: none;
@@ -93,217 +84,199 @@
   height: 13px;
   font-style: normal;
   font-weight: 1000;
   font-size: 12px;
   line-height: 13px;
   display: flex;
   align-items: center;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   position: absolute;
-  background-color: var(--jp-layout-color0);
+  background-color: #fff;
   padding-right: 4px;
   bottom: 34px;
   padding-left: 2px;
   left: 7px;
-  z-index: 3;
 }
 
-.project-region-select {
+.region-select {
   box-sizing: border-box;
-  background: var(--jp-layout-color0) !important;
+  background: #ffffff !important;
+  border: 1px solid rgba(0, 0, 0, 0.38) !important;
   display: block !important;
-  min-height: 36px;
+  height: 40px;
   width: 100%;
   border-radius: 4px !important;
   appearance: none !important;
   -webkit-appearance: none !important;
   -moz-appearance: none;
   transform: none !important;
+  position: unset !important;
 }
-
 .region-loader {
   margin-left: 1px;
   margin-top: 160px;
 }
-
 .save-overlay {
   display: flex;
   flex-direction: row;
   align-items: flex-start;
   padding: 32px 0px 0px;
   gap: 12px;
   height: 64px;
 }
-
+.save-button {
+  height: 32px;
+  background: #3367d6;
+  box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.12), 0px 2px 2px rgba(0, 0, 0, 0.2),
+    0px 1px 1px rgba(0, 0, 0, 0.14);
+  border-radius: 4px;
+  flex: none;
+  width: 65px;
+  font-style: normal;
+  font-weight: 500;
+  font-size: 13px;
+  line-height: 32px;
+  align-items: center;
+  text-align: center;
+  text-transform: uppercase;
+  color: #ffffff;
+  border: none;
+  cursor: pointer;
+}
+.save-button:disabled {
+  background: lightgrey;
+  color: black;
+}
 .save-loader {
   margin-top: 5px;
 }
-
 .user-info-card {
   box-sizing: border-box;
   width: 344px;
   height: fit-content;
-  background: var(--jp-layout-color0);
+  background: #ffffff;
   border: 1px solid #b0b0b0;
   border-radius: 27px;
+  margin-left: 21%;
   margin-top: 30px;
   display: flex;
   flex-direction: column;
   margin-right: 25px;
 }
-
 .user-image-overlay {
   width: 63px;
   height: 62px;
   border-radius: 33.5px;
 }
-
 .user-image {
   height: 62px;
   border-radius: 33.5px;
 }
-
 .config-overlay {
   display: flex;
   flex-direction: row;
   margin-bottom: 25px;
-  justify-content: space-between;
 }
-
 .google-header {
   align-items: center;
   justify-content: center;
   padding-top: 8px;
   padding-bottom: 8px;
   display: flex;
   font-size: 12px;
 }
-
-.separator {
-  width: 100%;
-  height: 0;
-  border-bottom: 1px solid var(--jp-layout-color3);
+.seperator {
+  width: 344px;
+  height: 0px;
+  left: 1316.5px;
+  top: 217px;
+  border: 1px solid #e1e3e1;
 }
-
 .user-overlay {
   display: flex;
   padding: 30px 30px;
 }
 
 .google-footer {
   width: 344px;
   height: 0px;
   border: 1px solid #e1e3e1;
   text-align: center;
 }
-
 .user-details {
   font-style: normal;
   font-weight: 500;
   font-size: 12px;
   line-height: 17px;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   padding-left: 30px;
   padding-top: 20px;
   justify-content: center;
   align-items: center;
   overflow-wrap: anywhere;
 }
-
 .add-account {
   display: flex;
   justify-content: center;
   height: 32px;
 }
-
 .account-icon {
   padding-left: 20px;
   margin-top: 5px;
 }
-
 .account-dropdown {
   width: 250px;
   height: 32px;
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 32px;
   display: flex;
   align-items: center;
   text-align: center;
   text-transform: uppercase;
   color: #1f1f1f;
   border: none;
 }
-
 .footer-text {
   padding-top: 15px;
 }
 
 .privacy-terms {
   margin: 0 5px;
 }
-
 .ui.selection.active.dropdown .menu {
   border: none !important;
 }
-
 .ui.dropdown .menu .selected.item,
 .ui.dropdown.selected {
-  background: var(--jp-layout-color0) !important;
-  color: var(--jp-brand-color0) !important;
+  background: rgb(230, 236, 250) !important;
+  color: rgb(28, 58, 169) !important;
 }
-
-.dataproc-settings-header {
-  padding-bottom: 15px;
-  font-style: normal;
-  font-weight: 500;
-  font-size: 20px;
-  color: var(--jp-ui-font-color0);
-}
-
 .runtime-title-section {
   display: flex;
   justify-content: space-between;
-  color: var(--jp-ui-font-color0);
-  font-size: 16px;
+  color: #000;
+  font-size: 20px;
   font-style: normal;
   font-weight: 500;
   margin-right: 20px;
   line-height: 28px;
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid #e0e0e0;
 }
 
 .settings-component {
+  height: 84vh;
+  overflow-y: auto;
   margin-left: 40px;
-  font-family: 'Roboto';
 }
 
 .expand-icon {
   cursor: pointer;
 }
 
 .runtime-title-part {
   margin-bottom: 5px;
 }
-.footer-divider {
+.footer-divider{
   margin: 0 5px;
-}
-
-.feedback-container {
-  color: #3367d6 !important;
-  font-weight: bold;
-}
-
-.feedback-version-container {
-  margin-right: 25px;
-}
-
-.project-header,
-.bigquery-region-header {
-  padding-top: 40px;
-  padding-left: 5px;
-  font-style: normal;
-  font-weight: 500;
-  font-size: 20px;
-  color: var(--jp-ui-font-color0);
-}
+}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/batches.css` & `dataproc_jupyter_plugin-0.1.9/style/batches.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .batch-header-part {
   display: flex;
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
 }
 
 .create-batch-overlay {
   height: 48px;
   padding-left: 15px;
   display: flex;
   align-items: center;
@@ -14,92 +14,70 @@
 .batch-details-label-level-two {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
   padding-left: 30px;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   overflow-wrap: anywhere;
 }
-.learn-more-url {
-  color: var(--jp-brand-color1);
-  text-decoration: underline;
-  cursor: pointer;
-  padding-left: 3px;
-  font-size: 10px;
-  margin-top: 2px;
-}
 
 .batch-details-label-level-three {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
   padding-left: 45px;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   overflow-wrap: anywhere;
 }
-.scroll-comp-batchdetails {
-  overflow-y: auto;
-  max-height: 90.1vh;
-}
-.create-batch-wrapper {
-  height: 48px;
-  /* padding-left: 15px; */
-  border-bottom: 1px solid var(--jp-layout-color3);
-  display: flex;
-  align-items: center;
-}
 
 .batch-details-container {
   width: 80%;
   padding-left: 15px;
 }
-
 .batch-details-container-top {
   width: 50%;
   padding-left: 15px;
 }
-
 .details-label {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
 }
-
 .batch-details-label-level-one {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
   padding-left: 15px;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   overflow-wrap: anywhere;
 }
-
 .details-value {
   font-style: normal;
   font-weight: 400;
   font-size: 13px;
   line-height: 20px;
   width: 35%;
-  color: var(--jp-ui-font-color2);
+  color: rgba(0, 0, 0, 0.66);
 }
-
 .batch-details-row-label {
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
   display: flex;
   justify-content: flex-start;
   align-items: flex-start;
   min-height: 18px;
   margin-bottom: 6px;
 }
-.scroll-comp-batch {
-  overflow-y: auto;
-  max-height: 85vh;
-}
+.scroll-comp-batch{
+ 
+    overflow-y: auto;
+    max-height: 85vh;
+  
+}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/clusterDetails.css` & `dataproc_jupyter_plugin-0.1.9/style/clusterDetails.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 @import url(https://fonts.googleapis.com/css?family=Roboto);
 
 .cluster-details-header {
   height: 48px;
   display: flex;
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
 }
-
 .scrollable-content {
   overflow: auto;
   max-height: calc(100vh - 48px);
 }
 
 .cluster-details-title {
   padding: 0px 15px;
   height: 48px;
   font-style: normal;
   font-weight: 400;
   font-size: 18px;
   line-height: 24px;
-
+  
   display: flex;
   align-items: center;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
 }
 
 .action-cluster-text {
   padding-left: 5px;
 }
 
 .action-cluster-section.disabled {
-  color: var(--jp-ui-font-color2);
+  color: rgba(0, 0, 0, 0.54);
   cursor: context-menu;
 }
 
 .loader-full-style {
   display: flex;
   align-items: center;
   text-align: center;
@@ -50,76 +49,72 @@
 }
 
 .action-cluster-icon {
   display: flex;
   align-items: center;
   justify-content: center;
 }
-
 .action-disabled {
   opacity: 0.5;
   cursor: context-menu !important;
 }
-
 .action-cluster-section {
   cursor: pointer;
   padding-left: 20px;
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 32px;
-
+  
   display: flex;
   align-items: center;
   text-align: center;
-  color: #3367d6;
+  color: #3367D6;
 }
 
 .cluster-details-container {
   width: 50%;
   padding-left: 15px;
-  margin-top: 7px;
 }
 
 .cluster-details-label {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 18px;
   min-width: 35%;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   overflow-wrap: anywhere;
 }
 
 .cluster-details-value {
   font-style: normal;
   font-weight: 400;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
-  color: var(--jp-ui-font-color2);
+  color: rgba(0, 0, 0, 0.66);
 }
 
 .row-details {
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
   display: flex;
   justify-content: flex-start;
   align-items: flex-start;
   min-height: 18px;
   margin-bottom: 6px;
 }
-
 .cluster-details-value-job {
   font-style: normal;
   font-weight: 400;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
-  color: #3367d6;
+  color: #3367D6;
   text-decoration: underline;
   cursor: pointer;
   height: 20px;
 }
 
-.cluster-details-action-parent {
+.cluster-details-action-parent{
   display: flex;
-}
+}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/databaseInfo.css` & `dataproc_jupyter_plugin-0.1.9/style/databaseInfo.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,89 @@
 @import url(https://fonts.googleapis.com/css?family=Roboto);
 
-.db-title {
-  height: 28px;
-  font-size: 20px;
-  line-height: 28px;
-  font-weight: 600;
-  margin-top: 50px;
-  margin-left: 20px;
+.db-title{
+    width: 124px;
+    height: 28px;
+    font-size: 20px;
+    line-height: 28px;
+    font-weight: 600;
+    margin-top: 50px;
+    margin-left: 20px;
 }
 
-.title-overlay {
+.title-overlay{
   height: 37px;
   display: flex;
   flex-direction: row;
   align-items: center;
   padding: 0px;
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
   padding-left: 20px;
   font-size: 15px;
   font-weight: 600;
 }
-
-.tr-row:nth-child(odd) {
-  background-color: var(--jp-layout-color2);
-}
-
-.tr-row:nth-child(even) {
-  background-color: var(--jp-layout-color1);
-}
-
-.db-table {
-  width: 100%;
-  border-collapse: collapse;
-}
-
-.db-table td {
-  padding-left: 10px;
-  height: 29px;
-  width: 10px;
-  font-size: 13px;
-  line-height: 20px;
-}
-.table-container {
-  width: 100%;
-  overflow-y: auto;
-  margin-top: 25px;
-  margin-left: 20px;
-  padding-right: 30px;
-  display: flex;
-}
-.big-query-schema-table-container {
-  width: 100%;
-  overflow-y: auto;
-  margin: 25px 0;
-  display: flex;
-}
+.tr-row-even {
+    background-color: #F5F5F5;
+  }
+  
+  .tr-row-odd {
+    background-color: white;
+  }
+  .db-table {
+    width: 100%;
+    border-collapse: collapse; 
+  }
+  
+  .db-table td {
+    padding-left: 10px;
+    height: 29px;
+    width: 10px;
+    font-size: 13px;
+    line-height: 20px;
+  }
+  .table-container {
+    width: 100%;
+    overflow-y: auto;
+    margin-top: 25px;
+    margin-left: 20px;
+    padding-right: 30px;
+    display: flex;
+  }
 .db-table td:nth-child(2) {
   width: 70%;
 }
 
 .db-table th {
   padding-left: 10px;
   text-align: left;
-  background-color: #f5f5f5;
-}
-.schema-td {
-  border-bottom: 1px solid var(--jp-layout-color3);
+  background-color: #F5F5F5;
 }
-
-.big-query-schema-table {
-  width: 100%;
-  border-collapse: collapse;
+ .schema-td {
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
 }
-
 .schema-table {
   width: 50%;
   border-collapse: collapse;
 }
 
-.schema-table td,
-.big-query-schema-table td {
-  padding-left: 10px;
+.schema-table td {
+  padding-left: 10px; 
   height: 29px;
   font-size: 13px;
   line-height: 18px;
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
 }
-
-.schema-table th,
-.big-query-schema-table th {
+.schema-table th {
   padding-left: 10px;
   text-align: left;
-  background-color: #f5f5f5;
+  background-color: #F5F5F5;
   line-height: 30px;
 }
-
 .bold-column {
-  font-weight: 700;
+  font-weight: 700; 
 }
-.table-info-overlay {
+.table-info-overlay{
   max-height: 100%;
-  overflow-y: auto;
-  overflow-x: hidden;
+overflow-y: auto;
+overflow-x: hidden;
 }
+
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/index.js` & `dataproc_jupyter_plugin-0.1.9/style/index.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -25,11 +25,8 @@
 import './sessionDetails.css';
 import './popup.css';
 import './createBatch.css';
 import './popup.css';
 import './dpms.css';
 import './databaseInfo.css';
 import './paginationView.css';
-import './runtimeTemplate.css';
-import './gcsBucket.css';
-import './notebookScheduler.css';
-import './notebookTemplates.css';
+import './runtimeTemplate.css';
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/job.css` & `dataproc_jupyter_plugin-0.1.9/style/job.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 @import url(https://fonts.googleapis.com/css?family=Roboto);
-
 .cluster-details-value-job {
   font-style: normal;
   font-weight: 400;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
   color: #3367d6;
@@ -12,166 +11,170 @@
   height: 29px;
 }
 
 .job-label-style {
   background-color: rgba(0, 0, 0, 0.08);
   padding: 0px 10px;
   border-radius: 10px;
+  color: rgb(0, 0, 0);
   font-weight: 400;
   line-height: 20px;
   margin: 3px 0px;
   margin-right: 5px;
 }
 
 .job-argument-style {
   padding: 2px;
 }
 
 .edit-input-style {
   margin-right: 20px;
   width: 90%;
-  height: 36px;
 }
 
 .key-message-wrapper {
   width: 90%;
 }
 
 .job-label-edit-parent {
   font-style: normal;
   font-weight: 400;
   font-size: 13px;
   line-height: 18px;
-  width: 512px;
-  color: var(--jp-ui-font-color2);
-  padding-bottom: 20px;
+  width: 50%;
+  color: rgba(0, 0, 0, 0.66);
+  padding: 10px;
 }
 
 .job-label-edit-row {
   display: flex;
-  margin: 15px 0px;
+  margin: 5px 0px;
   padding-bottom: 18px;
 }
 
 .job-label-style-parent {
   display: flex;
   font-style: normal;
   font-weight: 400;
   font-size: 13px;
   line-height: 18px;
   width: 65%;
   flex-wrap: wrap;
-  color: var(--jp-ui-font-color2);
+  color: rgba(0, 0, 0, 0.66);
 }
 
 .job-edit-header {
   padding: 0px 15px;
   height: 48px;
   display: flex;
   align-items: center;
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
 }
 
 .job-save-button-style {
   margin-right: 10px;
   background: #3367d6;
-  color: var(--jp-layout-color0);
+  color: #ffffff;
   height: 30px;
   font-size: 13px;
   width: 55px;
   cursor: pointer;
   display: flex;
   justify-content: center;
   align-items: center;
   border-radius: 4px;
 }
 
 .job-button-style-parent {
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
   display: flex;
   justify-content: flex-start;
   align-items: center;
   min-height: 55px;
 }
 
 .job-cancel-button-style {
   margin-right: 10px;
-  background: var(--jp-layout-color1);
-  color: var(--jp-ui-font-color0);
+  background: white;
+  color: #000000;
   height: 30px;
   width: 75px;
   font-size: 13px;
   cursor: pointer;
   display: flex;
   justify-content: center;
   align-items: center;
   border-radius: 4px;
   font-weight: 600;
 }
-
 .job-cancel-button-style:hover {
   background-color: #d3d3d3;
 }
 
 .job-add-label-button-disabled {
   display: flex;
   flex-direction: row;
   align-items: center;
   padding: 0px 12px;
   gap: 4px;
 
   width: 110px;
   height: 32px;
 
-  background: var(--jp-layout-color0);
-  color: var(--jp-ui-font-color2);
+  background: #ffffff;
+  color: rgba(0, 0, 0, 0.54);
 }
 
 .job-add-label-button {
   cursor: pointer;
   display: flex;
   flex-direction: row;
   align-items: center;
   padding: 0px 12px;
   gap: 4px;
+
+  width: 110px;
   height: 32px;
-  background: var(--jp-layout-color0);
-  box-shadow: 0px 1px 5px var(--jp-shadow-umbra-color),
-    0px 2px 2px var(--jp-shadow-umbra-color),
-    0px 1px 1px var(--jp-shadow-umbra-color);
+
+  background: #ffffff;
+  box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.12), 0px 2px 2px rgba(0, 0, 0, 0.2),
+    0px 1px 1px rgba(0, 0, 0, 0.14);
   border-radius: 4px;
-  border-style: none;
 }
 
 .job-edit-button {
   cursor: pointer;
   display: flex;
   flex-direction: row;
   align-items: center;
   padding: 0px 12px;
   gap: 4px;
+
+  width: 75px;
   height: 32px;
-  background: var(--jp-layout-color0);
-  box-shadow: 0px 1px 5px var(--jp-shadow-umbra-color),
-  0px 2px 2px var(--jp-shadow-umbra-color),
-  0px 1px 1px var(--jp-shadow-umbra-color);
+
+  background: #ffffff;
+  box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.12), 0px 2px 2px rgba(0, 0, 0, 0.2),
+    0px 1px 1px rgba(0, 0, 0, 0.14);
   border-radius: 4px;
 }
 
 .job-edit-button-disabled {
   display: flex;
   flex-direction: row;
   align-items: center;
   padding: 0px 12px;
   gap: 4px;
-  color: var(--jp-ui-font-color2);
+  color: rgba(0, 0, 0, 0.54);
+
+  width: 75px;
   height: 32px;
-  background: var(--jp-layout-color0);
+
+  background: #ffffff;
   opacity: 0.5;
-  border-radius: 4px;
 }
 
 .job-edit-text-disabled {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 32px;
@@ -180,33 +183,32 @@
   display: flex;
   align-items: center;
   text-align: center;
   text-transform: uppercase;
 
   /* Quick Selection/Blue 700 */
 
-  color: var(--jp-ui-font-color2);
+  color: rgba(0, 0, 0, 0.54);
 }
 
 .color-icon {
   color: #3367d6;
   display: flex;
 }
 
 .color-icon-disabled {
-  color: var(--jp-ui-font-color2);
+  color: rgba(0, 0, 0, 0.54);
   display: flex;
 }
 
 .job-edit-text {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 32px;
-  font-family: 'Roboto';
   /* identical to box height, or 246% */
 
   display: flex;
   align-items: center;
   text-align: center;
   text-transform: uppercase;
 
@@ -221,44 +223,41 @@
 }
 
 .job-label-style-list {
   background-color: rgba(0, 0, 0, 0.08);
   padding: 0px 10px;
   width: fit-content;
   border-radius: 10px;
+  color: rgb(0, 0, 0);
   font-weight: 400;
   line-height: 20px;
   margin: 3px 0px;
 }
 
 .jobs-list-table-parent {
-  height: 100%;
+  height: 63vh;
   overflow: auto;
 }
-.scroll-comp-jobdetails {
-  overflow-y: auto;
-  max-height: 90vh;
-}
+
 .jobs-list-table-parent-small {
-  height: 55vh;
+  height: 49vh;
   overflow: auto;
 }
-
 .job-details-label-row {
-  border-bottom: 1px solid var(--jp-layout-color3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.12);
   display: flex;
   justify-content: flex-start;
   align-items: flex-start;
   min-height: 18px;
   margin-bottom: 6px;
 }
 
 .job-details-label-level-one {
   font-style: normal;
   font-weight: 500;
   font-size: 13px;
   line-height: 18px;
   width: 35%;
   padding-left: 15px;
-  color: var(--jp-ui-font-color0);
+  color: #000000;
   overflow-wrap: anywhere;
-}
+}
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/add_account_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/add_account_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/clone_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/clone_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/clone_icon_disable.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/clone_icon_disable.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/cluster_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/cluster_icon.svg`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,131 @@
 00000000: 3c73 7667 2077 6964 7468 3d22 3532 2220  <svg width="52" 
 00000010: 6865 6967 6874 3d22 3532 2220 7669 6577  height="52" view
 00000020: 426f 783d 2230 2030 2035 3220 3532 2220  Box="0 0 52 52" 
 00000030: 6669 6c6c 3d22 6e6f 6e65 2220 786d 6c6e  fill="none" xmln
 00000040: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
 00000050: 2e6f 7267 2f32 3030 302f 7376 6722 3e0a  .org/2000/svg">.
-00000060: 3c70 6174 6820 6669 6c6c 2d72 756c 653d  <path fill-rule=
-00000070: 2265 7665 6e6f 6464 2220 636c 6970 2d72  "evenodd" clip-r
-00000080: 756c 653d 2265 7665 6e6f 6464 2220 643d  ule="evenodd" d=
-00000090: 224d 3330 2e32 3232 3220 3135 2e34 3434  "M30.2222 15.444
-000000a0: 3543 3330 2e32 3232 3220 3137 2e37 3736  5C30.2222 17.776
-000000b0: 3320 3238 2e33 3331 3820 3139 2e36 3636  3 28.3318 19.666
-000000c0: 3720 3235 2e39 3939 3920 3139 2e36 3636  7 25.9999 19.666
-000000d0: 3743 3233 2e36 3638 3120 3139 2e36 3636  7C23.6681 19.666
-000000e0: 3720 3231 2e37 3737 3720 3137 2e37 3736  7 21.7777 17.776
-000000f0: 3320 3231 2e37 3737 3720 3135 2e34 3434  3 21.7777 15.444
-00000100: 3543 3231 2e37 3737 3720 3133 2e31 3132  5C21.7777 13.112
-00000110: 3620 3233 2e36 3638 3120 3131 2e32 3232  6 23.6681 11.222
-00000120: 3220 3235 2e39 3939 3920 3131 2e32 3232  2 25.9999 11.222
-00000130: 3243 3238 2e33 3331 3820 3131 2e32 3232  2C28.3318 11.222
-00000140: 3220 3330 2e32 3232 3220 3133 2e31 3132  2 30.2222 13.112
-00000150: 3620 3330 2e32 3232 3220 3135 2e34 3434  6 30.2222 15.444
-00000160: 355a 4d31 352e 3434 3434 2033 302e 3232  5ZM15.4444 30.22
-00000170: 3232 4331 372e 3737 3633 2033 302e 3232  22C17.7763 30.22
-00000180: 3232 2031 392e 3636 3636 2032 382e 3333  22 19.6666 28.33
-00000190: 3139 2031 392e 3636 3636 2032 3643 3139  19 19.6666 26C19
-000001a0: 2e36 3636 3620 3233 2e36 3638 3120 3137  .6666 23.6681 17
-000001b0: 2e37 3736 3320 3231 2e37 3737 3820 3135  .7763 21.7778 15
-000001c0: 2e34 3434 3420 3231 2e37 3737 3843 3133  .4444 21.7778C13
-000001d0: 2e31 3132 3520 3231 2e37 3737 3820 3131  .1125 21.7778 11
-000001e0: 2e32 3232 3220 3233 2e36 3638 3120 3131  .2222 23.6681 11
-000001f0: 2e32 3232 3220 3236 4331 312e 3232 3232  .2222 26C11.2222
-00000200: 2032 382e 3333 3139 2031 332e 3131 3235   28.3319 13.1125
-00000210: 2033 302e 3232 3232 2031 352e 3434 3434   30.2222 15.4444
-00000220: 2033 302e 3232 3232 5a4d 3336 2e35 3535   30.2222ZM36.555
-00000230: 3520 3330 2e32 3232 3243 3338 2e38 3837  5 30.2222C38.887
-00000240: 3420 3330 2e32 3232 3220 3430 2e37 3737  4 30.2222 40.777
-00000250: 3720 3238 2e33 3331 3920 3430 2e37 3737  7 28.3319 40.777
-00000260: 3720 3236 4334 302e 3737 3737 2032 332e  7 26C40.7777 23.
-00000270: 3636 3831 2033 382e 3838 3734 2032 312e  6681 38.8874 21.
-00000280: 3737 3738 2033 362e 3535 3535 2032 312e  7778 36.5555 21.
-00000290: 3737 3738 4333 342e 3232 3336 2032 312e  7778C34.2236 21.
-000002a0: 3737 3738 2033 322e 3333 3333 2032 332e  7778 32.3333 23.
-000002b0: 3636 3831 2033 322e 3333 3333 2032 3643  6681 32.3333 26C
-000002c0: 3332 2e33 3333 3320 3238 2e33 3331 3920  32.3333 28.3319 
-000002d0: 3334 2e32 3233 3620 3330 2e32 3232 3220  34.2236 30.2222 
-000002e0: 3336 2e35 3535 3520 3330 2e32 3232 325a  36.5555 30.2222Z
-000002f0: 4d32 352e 3939 3939 2034 302e 3737 3738  M25.9999 40.7778
-00000300: 4332 382e 3333 3138 2034 302e 3737 3738  C28.3318 40.7778
-00000310: 2033 302e 3232 3232 2033 382e 3838 3734   30.2222 38.8874
-00000320: 2033 302e 3232 3232 2033 362e 3535 3536   30.2222 36.5556
-00000330: 4333 302e 3232 3232 2033 342e 3232 3337  C30.2222 34.2237
-00000340: 2032 382e 3333 3138 2033 322e 3333 3333   28.3318 32.3333
-00000350: 2032 352e 3939 3939 2033 322e 3333 3333   25.9999 32.3333
-00000360: 4332 332e 3636 3831 2033 322e 3333 3333  C23.6681 32.3333
-00000370: 2032 312e 3737 3737 2033 342e 3232 3337   21.7777 34.2237
-00000380: 2032 312e 3737 3737 2033 362e 3535 3536   21.7777 36.5556
-00000390: 4332 312e 3737 3737 2033 382e 3838 3734  C21.7777 38.8874
-000003a0: 2032 332e 3636 3831 2034 302e 3737 3738   23.6681 40.7778
-000003b0: 2032 352e 3939 3939 2034 302e 3737 3738   25.9999 40.7778
-000003c0: 5a4d 3239 2e31 3636 3620 3236 4332 392e  ZM29.1666 26C29.
-000003d0: 3136 3636 2032 372e 3734 3839 2032 372e  1666 27.7489 27.
-000003e0: 3734 3838 2032 392e 3136 3637 2032 352e  7488 29.1667 25.
-000003f0: 3939 3939 2032 392e 3136 3637 4332 342e  9999 29.1667C24.
-00000400: 3235 3120 3239 2e31 3636 3720 3232 2e38  251 29.1667 22.8
-00000410: 3333 3320 3237 2e37 3438 3920 3232 2e38  333 27.7489 22.8
-00000420: 3333 3320 3236 4332 322e 3833 3333 2032  333 26C22.8333 2
-00000430: 342e 3235 3131 2032 342e 3235 3120 3232  4.2511 24.251 22
-00000440: 2e38 3333 3320 3235 2e39 3939 3920 3232  .8333 25.9999 22
-00000450: 2e38 3333 3343 3237 2e37 3438 3820 3232  .8333C27.7488 22
-00000460: 2e38 3333 3320 3239 2e31 3636 3620 3234  .8333 29.1666 24
-00000470: 2e32 3531 3120 3239 2e31 3636 3620 3236  .2511 29.1666 26
-00000480: 5a4d 3137 2e35 3535 3520 3139 2e36 3636  ZM17.5555 19.666
-00000490: 3743 3138 2e37 3231 3420 3139 2e36 3636  7C18.7214 19.666
-000004a0: 3720 3139 2e36 3636 3620 3138 2e37 3231  7 19.6666 18.721
-000004b0: 3520 3139 2e36 3636 3620 3137 2e35 3535  5 19.6666 17.555
-000004c0: 3643 3139 2e36 3636 3620 3136 2e33 3839  6C19.6666 16.389
-000004d0: 3620 3138 2e37 3231 3420 3135 2e34 3434  6 18.7214 15.444
-000004e0: 3520 3137 2e35 3535 3520 3135 2e34 3434  5 17.5555 15.444
-000004f0: 3543 3136 2e33 3839 3620 3135 2e34 3434  5C16.3896 15.444
-00000500: 3520 3135 2e34 3434 3420 3136 2e33 3839  5 15.4444 16.389
-00000510: 3620 3135 2e34 3434 3420 3137 2e35 3535  6 15.4444 17.555
-00000520: 3643 3135 2e34 3434 3420 3138 2e37 3231  6C15.4444 18.721
-00000530: 3520 3136 2e33 3839 3620 3139 2e36 3636  5 16.3896 19.666
-00000540: 3720 3137 2e35 3535 3520 3139 2e36 3636  7 17.5555 19.666
-00000550: 375a 4d31 392e 3636 3636 2033 342e 3434  7ZM19.6666 34.44
-00000560: 3435 4331 392e 3636 3636 2033 352e 3631  45C19.6666 35.61
-00000570: 3034 2031 382e 3732 3134 2033 362e 3535  04 18.7214 36.55
-00000580: 3536 2031 372e 3535 3535 2033 362e 3535  56 17.5555 36.55
-00000590: 3536 4331 362e 3338 3936 2033 362e 3535  56C16.3896 36.55
-000005a0: 3536 2031 352e 3434 3434 2033 352e 3631  56 15.4444 35.61
-000005b0: 3034 2031 352e 3434 3434 2033 342e 3434  04 15.4444 34.44
-000005c0: 3435 4331 352e 3434 3434 2033 332e 3237  45C15.4444 33.27
-000005d0: 3835 2031 362e 3338 3936 2033 322e 3333  85 16.3896 32.33
-000005e0: 3333 2031 372e 3535 3535 2033 322e 3333  33 17.5555 32.33
-000005f0: 3333 4331 382e 3732 3134 2033 322e 3333  33C18.7214 32.33
-00000600: 3333 2031 392e 3636 3636 2033 332e 3237  33 19.6666 33.27
-00000610: 3835 2031 392e 3636 3636 2033 342e 3434  85 19.6666 34.44
-00000620: 3435 5a4d 3334 2e34 3434 3420 3139 2e36  45ZM34.4444 19.6
-00000630: 3636 3743 3335 2e36 3130 3320 3139 2e36  667C35.6103 19.6
-00000640: 3636 3720 3336 2e35 3535 3520 3138 2e37  667 36.5555 18.7
-00000650: 3231 3520 3336 2e35 3535 3520 3137 2e35  215 36.5555 17.5
-00000660: 3535 3643 3336 2e35 3535 3520 3136 2e33  556C36.5555 16.3
-00000670: 3839 3620 3335 2e36 3130 3320 3135 2e34  896 35.6103 15.4
-00000680: 3434 3520 3334 2e34 3434 3420 3135 2e34  445 34.4444 15.4
-00000690: 3434 3543 3333 2e32 3738 3520 3135 2e34  445C33.2785 15.4
-000006a0: 3434 3520 3332 2e33 3333 3320 3136 2e33  445 32.3333 16.3
-000006b0: 3839 3620 3332 2e33 3333 3320 3137 2e35  896 32.3333 17.5
-000006c0: 3535 3643 3332 2e33 3333 3320 3138 2e37  556C32.3333 18.7
-000006d0: 3231 3520 3333 2e32 3738 3520 3139 2e36  215 33.2785 19.6
-000006e0: 3636 3720 3334 2e34 3434 3420 3139 2e36  667 34.4444 19.6
-000006f0: 3636 375a 4d33 362e 3535 3535 2033 342e  667ZM36.5555 34.
-00000700: 3434 3435 4333 362e 3535 3535 2033 352e  4445C36.5555 35.
-00000710: 3631 3034 2033 352e 3631 3033 2033 362e  6104 35.6103 36.
-00000720: 3535 3536 2033 342e 3434 3434 2033 362e  5556 34.4444 36.
-00000730: 3535 3536 4333 332e 3237 3835 2033 362e  5556C33.2785 36.
-00000740: 3535 3536 2033 322e 3333 3333 2033 352e  5556 32.3333 35.
-00000750: 3631 3034 2033 322e 3333 3333 2033 342e  6104 32.3333 34.
-00000760: 3434 3435 4333 322e 3333 3333 2033 332e  4445C32.3333 33.
-00000770: 3237 3835 2033 332e 3237 3835 2033 322e  2785 33.2785 32.
-00000780: 3333 3333 2033 342e 3434 3434 2033 322e  3333 34.4444 32.
-00000790: 3333 3333 4333 352e 3631 3033 2033 322e  3333C35.6103 32.
-000007a0: 3333 3333 2033 362e 3535 3535 2033 332e  3333 36.5555 33.
-000007b0: 3237 3835 2033 362e 3535 3535 2033 342e  2785 36.5555 34.
-000007c0: 3434 3435 5a22 2066 696c 6c3d 2223 3333  4445Z" fill="#33
-000007d0: 3637 4436 222f 3e0a 3c2f 7376 673e 0a    67D6"/>.</svg>.
+00000060: 3c72 6563 7420 7769 6474 683d 2235 3222  <rect width="52"
+00000070: 2068 6569 6768 743d 2235 3222 2066 696c   height="52" fil
+00000080: 6c3d 2277 6869 7465 222f 3e0a 3c70 6174  l="white"/>.<pat
+00000090: 6820 6669 6c6c 2d72 756c 653d 2265 7665  h fill-rule="eve
+000000a0: 6e6f 6464 2220 636c 6970 2d72 756c 653d  nodd" clip-rule=
+000000b0: 2265 7665 6e6f 6464 2220 643d 224d 3330  "evenodd" d="M30
+000000c0: 2e32 3232 3220 3135 2e34 3434 3443 3330  .2222 15.4444C30
+000000d0: 2e32 3232 3220 3137 2e37 3736 3320 3238  .2222 17.7763 28
+000000e0: 2e33 3331 3820 3139 2e36 3636 3620 3235  .3318 19.6666 25
+000000f0: 2e39 3939 3920 3139 2e36 3636 3643 3233  .9999 19.6666C23
+00000100: 2e36 3638 3120 3139 2e36 3636 3620 3231  .6681 19.6666 21
+00000110: 2e37 3737 3720 3137 2e37 3736 3320 3231  .7777 17.7763 21
+00000120: 2e37 3737 3720 3135 2e34 3434 3443 3231  .7777 15.4444C21
+00000130: 2e37 3737 3720 3133 2e31 3132 3520 3233  .7777 13.1125 23
+00000140: 2e36 3638 3120 3131 2e32 3232 3220 3235  .6681 11.2222 25
+00000150: 2e39 3939 3920 3131 2e32 3232 3243 3238  .9999 11.2222C28
+00000160: 2e33 3331 3820 3131 2e32 3232 3220 3330  .3318 11.2222 30
+00000170: 2e32 3232 3220 3133 2e31 3132 3520 3330  .2222 13.1125 30
+00000180: 2e32 3232 3220 3135 2e34 3434 345a 4d31  .2222 15.4444ZM1
+00000190: 352e 3434 3434 2033 302e 3232 3232 4331  5.4444 30.2222C1
+000001a0: 372e 3737 3633 2033 302e 3232 3232 2031  7.7763 30.2222 1
+000001b0: 392e 3636 3636 2032 382e 3333 3138 2031  9.6666 28.3318 1
+000001c0: 392e 3636 3636 2032 352e 3939 3939 4331  9.6666 25.9999C1
+000001d0: 392e 3636 3636 2032 332e 3636 3831 2031  9.6666 23.6681 1
+000001e0: 372e 3737 3633 2032 312e 3737 3737 2031  7.7763 21.7777 1
+000001f0: 352e 3434 3434 2032 312e 3737 3737 4331  5.4444 21.7777C1
+00000200: 332e 3131 3235 2032 312e 3737 3737 2031  3.1125 21.7777 1
+00000210: 312e 3232 3232 2032 332e 3636 3831 2031  1.2222 23.6681 1
+00000220: 312e 3232 3232 2032 352e 3939 3939 4331  1.2222 25.9999C1
+00000230: 312e 3232 3232 2032 382e 3333 3138 2031  1.2222 28.3318 1
+00000240: 332e 3131 3235 2033 302e 3232 3232 2031  3.1125 30.2222 1
+00000250: 352e 3434 3434 2033 302e 3232 3232 5a4d  5.4444 30.2222ZM
+00000260: 3336 2e35 3535 3520 3330 2e32 3232 3243  36.5555 30.2222C
+00000270: 3338 2e38 3837 3420 3330 2e32 3232 3220  38.8874 30.2222 
+00000280: 3430 2e37 3737 3720 3238 2e33 3331 3820  40.7777 28.3318 
+00000290: 3430 2e37 3737 3720 3235 2e39 3939 3943  40.7777 25.9999C
+000002a0: 3430 2e37 3737 3720 3233 2e36 3638 3120  40.7777 23.6681 
+000002b0: 3338 2e38 3837 3420 3231 2e37 3737 3720  38.8874 21.7777 
+000002c0: 3336 2e35 3535 3520 3231 2e37 3737 3743  36.5555 21.7777C
+000002d0: 3334 2e32 3233 3620 3231 2e37 3737 3720  34.2236 21.7777 
+000002e0: 3332 2e33 3333 3320 3233 2e36 3638 3120  32.3333 23.6681 
+000002f0: 3332 2e33 3333 3320 3235 2e39 3939 3943  32.3333 25.9999C
+00000300: 3332 2e33 3333 3320 3238 2e33 3331 3820  32.3333 28.3318 
+00000310: 3334 2e32 3233 3620 3330 2e32 3232 3220  34.2236 30.2222 
+00000320: 3336 2e35 3535 3520 3330 2e32 3232 325a  36.5555 30.2222Z
+00000330: 4d32 352e 3939 3939 2034 302e 3737 3737  M25.9999 40.7777
+00000340: 4332 382e 3333 3138 2034 302e 3737 3737  C28.3318 40.7777
+00000350: 2033 302e 3232 3232 2033 382e 3838 3734   30.2222 38.8874
+00000360: 2033 302e 3232 3232 2033 362e 3535 3535   30.2222 36.5555
+00000370: 4333 302e 3232 3232 2033 342e 3232 3336  C30.2222 34.2236
+00000380: 2032 382e 3333 3138 2033 322e 3333 3333   28.3318 32.3333
+00000390: 2032 352e 3939 3939 2033 322e 3333 3333   25.9999 32.3333
+000003a0: 4332 332e 3636 3831 2033 322e 3333 3333  C23.6681 32.3333
+000003b0: 2032 312e 3737 3737 2033 342e 3232 3336   21.7777 34.2236
+000003c0: 2032 312e 3737 3737 2033 362e 3535 3535   21.7777 36.5555
+000003d0: 4332 312e 3737 3737 2033 382e 3838 3734  C21.7777 38.8874
+000003e0: 2032 332e 3636 3831 2034 302e 3737 3737   23.6681 40.7777
+000003f0: 2032 352e 3939 3939 2034 302e 3737 3737   25.9999 40.7777
+00000400: 5a4d 3239 2e31 3636 3620 3235 2e39 3939  ZM29.1666 25.999
+00000410: 3943 3239 2e31 3636 3620 3237 2e37 3438  9C29.1666 27.748
+00000420: 3820 3237 2e37 3438 3820 3239 2e31 3636  8 27.7488 29.166
+00000430: 3620 3235 2e39 3939 3920 3239 2e31 3636  6 25.9999 29.166
+00000440: 3643 3234 2e32 3531 2032 392e 3136 3636  6C24.251 29.1666
+00000450: 2032 322e 3833 3333 2032 372e 3734 3838   22.8333 27.7488
+00000460: 2032 322e 3833 3333 2032 352e 3939 3939   22.8333 25.9999
+00000470: 4332 322e 3833 3333 2032 342e 3235 3120  C22.8333 24.251 
+00000480: 3234 2e32 3531 2032 322e 3833 3333 2032  24.251 22.8333 2
+00000490: 352e 3939 3939 2032 322e 3833 3333 4332  5.9999 22.8333C2
+000004a0: 372e 3734 3838 2032 322e 3833 3333 2032  7.7488 22.8333 2
+000004b0: 392e 3136 3636 2032 342e 3235 3120 3239  9.1666 24.251 29
+000004c0: 2e31 3636 3620 3235 2e39 3939 395a 4d31  .1666 25.9999ZM1
+000004d0: 372e 3535 3535 2031 392e 3636 3636 4331  7.5555 19.6666C1
+000004e0: 382e 3732 3134 2031 392e 3636 3636 2031  8.7214 19.6666 1
+000004f0: 392e 3636 3636 2031 382e 3732 3134 2031  9.6666 18.7214 1
+00000500: 392e 3636 3636 2031 372e 3535 3535 4331  9.6666 17.5555C1
+00000510: 392e 3636 3636 2031 362e 3338 3936 2031  9.6666 16.3896 1
+00000520: 382e 3732 3134 2031 352e 3434 3434 2031  8.7214 15.4444 1
+00000530: 372e 3535 3535 2031 352e 3434 3434 4331  7.5555 15.4444C1
+00000540: 362e 3338 3936 2031 352e 3434 3434 2031  6.3896 15.4444 1
+00000550: 352e 3434 3434 2031 362e 3338 3936 2031  5.4444 16.3896 1
+00000560: 352e 3434 3434 2031 372e 3535 3535 4331  5.4444 17.5555C1
+00000570: 352e 3434 3434 2031 382e 3732 3134 2031  5.4444 18.7214 1
+00000580: 362e 3338 3936 2031 392e 3636 3636 2031  6.3896 19.6666 1
+00000590: 372e 3535 3535 2031 392e 3636 3636 5a4d  7.5555 19.6666ZM
+000005a0: 3139 2e36 3636 3620 3334 2e34 3434 3443  19.6666 34.4444C
+000005b0: 3139 2e36 3636 3620 3335 2e36 3130 3320  19.6666 35.6103 
+000005c0: 3138 2e37 3231 3420 3336 2e35 3535 3520  18.7214 36.5555 
+000005d0: 3137 2e35 3535 3520 3336 2e35 3535 3543  17.5555 36.5555C
+000005e0: 3136 2e33 3839 3620 3336 2e35 3535 3520  16.3896 36.5555 
+000005f0: 3135 2e34 3434 3420 3335 2e36 3130 3320  15.4444 35.6103 
+00000600: 3135 2e34 3434 3420 3334 2e34 3434 3443  15.4444 34.4444C
+00000610: 3135 2e34 3434 3420 3333 2e32 3738 3520  15.4444 33.2785 
+00000620: 3136 2e33 3839 3620 3332 2e33 3333 3320  16.3896 32.3333 
+00000630: 3137 2e35 3535 3520 3332 2e33 3333 3343  17.5555 32.3333C
+00000640: 3138 2e37 3231 3420 3332 2e33 3333 3320  18.7214 32.3333 
+00000650: 3139 2e36 3636 3620 3333 2e32 3738 3520  19.6666 33.2785 
+00000660: 3139 2e36 3636 3620 3334 2e34 3434 345a  19.6666 34.4444Z
+00000670: 4d33 342e 3434 3434 2031 392e 3636 3636  M34.4444 19.6666
+00000680: 4333 352e 3631 3033 2031 392e 3636 3636  C35.6103 19.6666
+00000690: 2033 362e 3535 3535 2031 382e 3732 3134   36.5555 18.7214
+000006a0: 2033 362e 3535 3535 2031 372e 3535 3535   36.5555 17.5555
+000006b0: 4333 362e 3535 3535 2031 362e 3338 3936  C36.5555 16.3896
+000006c0: 2033 352e 3631 3033 2031 352e 3434 3434   35.6103 15.4444
+000006d0: 2033 342e 3434 3434 2031 352e 3434 3434   34.4444 15.4444
+000006e0: 4333 332e 3237 3835 2031 352e 3434 3434  C33.2785 15.4444
+000006f0: 2033 322e 3333 3333 2031 362e 3338 3936   32.3333 16.3896
+00000700: 2033 322e 3333 3333 2031 372e 3535 3535   32.3333 17.5555
+00000710: 4333 322e 3333 3333 2031 382e 3732 3134  C32.3333 18.7214
+00000720: 2033 332e 3237 3835 2031 392e 3636 3636   33.2785 19.6666
+00000730: 2033 342e 3434 3434 2031 392e 3636 3636   34.4444 19.6666
+00000740: 5a4d 3336 2e35 3535 3520 3334 2e34 3434  ZM36.5555 34.444
+00000750: 3443 3336 2e35 3535 3520 3335 2e36 3130  4C36.5555 35.610
+00000760: 3320 3335 2e36 3130 3320 3336 2e35 3535  3 35.6103 36.555
+00000770: 3520 3334 2e34 3434 3420 3336 2e35 3535  5 34.4444 36.555
+00000780: 3543 3333 2e32 3738 3520 3336 2e35 3535  5C33.2785 36.555
+00000790: 3520 3332 2e33 3333 3320 3335 2e36 3130  5 32.3333 35.610
+000007a0: 3320 3332 2e33 3333 3320 3334 2e34 3434  3 32.3333 34.444
+000007b0: 3443 3332 2e33 3333 3320 3333 2e32 3738  4C32.3333 33.278
+000007c0: 3520 3333 2e32 3738 3520 3332 2e33 3333  5 33.2785 32.333
+000007d0: 3320 3334 2e34 3434 3420 3332 2e33 3333  3 34.4444 32.333
+000007e0: 3343 3335 2e36 3130 3320 3332 2e33 3333  3C35.6103 32.333
+000007f0: 3320 3336 2e35 3535 3520 3333 2e32 3738  3 36.5555 33.278
+00000800: 3520 3336 2e35 3535 3520 3334 2e34 3434  5 36.5555 34.444
+00000810: 345a 2220 6669 6c6c 3d22 2333 3336 3744  4Z" fill="#3367D
+00000820: 3622 2f3e 0a3c 2f73 7667 3e0a            6"/>.</svg>.
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/cluster_running_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/cluster_running_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/database_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/database_widget_icon.svg`

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,148 @@
 00000000: 3c73 7667 2077 6964 7468 3d22 3138 2220  <svg width="18" 
 00000010: 6865 6967 6874 3d22 3138 2220 7669 6577  height="18" view
 00000020: 426f 783d 2230 2030 2031 3820 3138 2220  Box="0 0 18 18" 
 00000030: 6669 6c6c 3d22 6e6f 6e65 2220 786d 6c6e  fill="none" xmln
 00000040: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
 00000050: 2e6f 7267 2f32 3030 302f 7376 6722 3e0a  .org/2000/svg">.
-00000060: 3c70 6174 6820 643d 224d 3920 3135 2e33  <path d="M9 15.3
-00000070: 4337 2e32 3337 3520 3135 2e33 2035 2e37  C7.2375 15.3 5.7
-00000080: 3433 3735 2031 352e 3033 3735 2034 2e35  4375 15.0375 4.5
-00000090: 3138 3735 2031 342e 3531 3235 4333 2e33  1875 14.5125C3.3
-000000a0: 3036 3235 2031 332e 3938 3735 2032 2e37  0625 13.9875 2.7
-000000b0: 2031 332e 3335 2032 2e37 2031 322e 3656   13.35 2.7 12.6V
-000000c0: 352e 3443 322e 3720 342e 3635 2033 2e33  5.4C2.7 4.65 3.3
-000000d0: 3132 3520 342e 3031 3235 2034 2e35 3337  125 4.0125 4.537
-000000e0: 3520 332e 3438 3735 4335 2e37 3632 3520  5 3.4875C5.7625 
-000000f0: 322e 3936 3235 2037 2e32 3520 322e 3720  2.9625 7.25 2.7 
-00000100: 3920 322e 3743 3130 2e37 3337 3520 322e  9 2.7C10.7375 2.
-00000110: 3720 3132 2e32 3138 3720 322e 3936 3235  7 12.2187 2.9625
-00000120: 2031 332e 3434 3337 2033 2e34 3837 3543   13.4437 3.4875C
-00000130: 3134 2e36 3831 3220 342e 3031 3235 2031  14.6812 4.0125 1
-00000140: 352e 3320 342e 3635 2031 352e 3320 352e  5.3 4.65 15.3 5.
-00000150: 3456 3132 2e36 4331 352e 3320 3133 2e33  4V12.6C15.3 13.3
-00000160: 3520 3134 2e36 3837 3520 3133 2e39 3837  5 14.6875 13.987
-00000170: 3520 3133 2e34 3632 3520 3134 2e35 3132  5 13.4625 14.512
-00000180: 3543 3132 2e32 3337 3520 3135 2e30 3337  5C12.2375 15.037
-00000190: 3520 3130 2e37 3520 3135 2e33 2039 2031  5 10.75 15.3 9 1
-000001a0: 352e 335a 4d39 2036 2e37 3543 3130 2e30  5.3ZM9 6.75C10.0
-000001b0: 3735 2036 2e37 3520 3131 2e31 3132 3520  75 6.75 11.1125 
-000001c0: 362e 3631 3837 3520 3132 2e31 3132 3520  6.61875 12.1125 
-000001d0: 362e 3335 3632 3543 3133 2e31 3132 3520  6.35625C13.1125 
-000001e0: 362e 3038 3132 3520 3133 2e37 3235 2035  6.08125 13.725 5
-000001f0: 2e37 3632 3520 3133 2e39 3520 352e 3443  .7625 13.95 5.4C
-00000200: 3133 2e37 3235 2035 2e30 3520 3133 2e31  13.725 5.05 13.1
-00000210: 3036 3220 342e 3733 3735 2031 322e 3039  062 4.7375 12.09
-00000220: 3337 2034 2e34 3632 3543 3131 2e30 3933  37 4.4625C11.093
-00000230: 3720 342e 3138 3735 2031 302e 3036 3235  7 4.1875 10.0625
-00000240: 2034 2e30 3520 3920 342e 3035 4337 2e39   4.05 9 4.05C7.9
-00000250: 3235 2034 2e30 3520 362e 3838 3132 3520  25 4.05 6.88125 
-00000260: 342e 3138 3735 2035 2e38 3638 3735 2034  4.1875 5.86875 4
-00000270: 2e34 3632 3543 342e 3836 3837 3520 342e  .4625C4.86875 4.
-00000280: 3733 3735 2034 2e32 3632 3520 352e 3035  7375 4.2625 5.05
-00000290: 2034 2e30 3520 352e 3443 342e 3236 3235   4.05 5.4C4.2625
-000002a0: 2035 2e37 3632 3520 342e 3836 3235 2036   5.7625 4.8625 6
-000002b0: 2e30 3831 3235 2035 2e38 3520 362e 3335  .08125 5.85 6.35
-000002c0: 3632 3543 362e 3835 2036 2e36 3138 3735  625C6.85 6.61875
-000002d0: 2037 2e39 2036 2e37 3520 3920 362e 3735   7.9 6.75 9 6.75
-000002e0: 5a4d 3920 3130 2e33 3543 392e 3532 3520  ZM9 10.35C9.525 
-000002f0: 3130 2e33 3520 3130 2e30 3235 2031 302e  10.35 10.025 10.
-00000300: 3332 3520 3130 2e35 2031 302e 3237 3543  325 10.5 10.275C
-00000310: 3130 2e39 3735 2031 302e 3231 3235 2031  10.975 10.2125 1
-00000320: 312e 3431 3837 2031 302e 3133 3132 2031  1.4187 10.1312 1
-00000330: 312e 3833 3132 2031 302e 3033 3132 4331  1.8312 10.0312C1
-00000340: 322e 3235 3632 2039 2e39 3331 3235 2031  2.2562 9.93125 1
-00000350: 322e 3634 3337 2039 2e38 3036 3235 2031  2.6437 9.80625 1
-00000360: 322e 3939 3337 2039 2e36 3536 3235 4331  2.9937 9.65625C1
-00000370: 332e 3335 3632 2039 2e34 3933 3735 2031  3.3562 9.49375 1
-00000380: 332e 3637 3520 392e 3331 3235 2031 332e  3.675 9.3125 13.
-00000390: 3935 2039 2e31 3132 3556 372e 3036 3837  95 9.1125V7.0687
-000003a0: 3543 3133 2e36 3520 372e 3233 3132 3520  5C13.65 7.23125 
-000003b0: 3133 2e33 3132 3520 372e 3338 3132 3520  13.3125 7.38125 
-000003c0: 3132 2e39 3337 3520 372e 3531 3837 3543  12.9375 7.51875C
-000003d0: 3132 2e35 3735 2037 2e36 3433 3735 2031  12.575 7.64375 1
-000003e0: 322e 3138 3132 2037 2e37 3520 3131 2e37  2.1812 7.75 11.7
-000003f0: 3536 3220 372e 3833 3735 4331 312e 3333  562 7.8375C11.33
-00000400: 3132 2037 2e39 3235 2031 302e 3838 3735  12 7.925 10.8875
-00000410: 2037 2e39 3933 3735 2031 302e 3432 3520   7.99375 10.425 
-00000420: 382e 3034 3337 3543 392e 3936 3235 2038  8.04375C9.9625 8
-00000430: 2e30 3831 3235 2039 2e34 3837 3520 382e  .08125 9.4875 8.
-00000440: 3120 3920 382e 3143 382e 3520 382e 3120  1 9 8.1C8.5 8.1 
-00000450: 382e 3031 3235 2038 2e30 3831 3235 2037  8.0125 8.08125 7
-00000460: 2e35 3337 3520 382e 3034 3337 3543 372e  .5375 8.04375C7.
-00000470: 3037 3520 372e 3939 3337 3520 362e 3633  075 7.99375 6.63
-00000480: 3132 3520 372e 3932 3520 362e 3230 3632  125 7.925 6.2062
-00000490: 3520 372e 3833 3735 4335 2e37 3933 3735  5 7.8375C5.79375
-000004a0: 2037 2e37 3520 352e 3420 372e 3634 3337   7.75 5.4 7.6437
-000004b0: 3520 352e 3032 3520 372e 3531 3837 3543  5 5.025 7.51875C
-000004c0: 342e 3636 3235 2037 2e33 3831 3235 2034  4.6625 7.38125 4
-000004d0: 2e33 3337 3520 372e 3233 3132 3520 342e  .3375 7.23125 4.
-000004e0: 3035 2037 2e30 3638 3735 5639 2e31 3132  05 7.06875V9.112
-000004f0: 3543 342e 3332 3520 392e 3331 3235 2034  5C4.325 9.3125 4
-00000500: 2e36 3337 3520 392e 3439 3337 3520 342e  .6375 9.49375 4.
-00000510: 3938 3735 2039 2e36 3536 3235 4335 2e33  9875 9.65625C5.3
-00000520: 3337 3520 392e 3830 3632 3520 352e 3731  375 9.80625 5.71
-00000530: 3837 3520 392e 3933 3132 3520 362e 3133  875 9.93125 6.13
-00000540: 3132 3520 3130 2e30 3331 3243 362e 3535  125 10.0312C6.55
-00000550: 3632 3520 3130 2e31 3331 3220 372e 3030  625 10.1312 7.00
-00000560: 3632 3520 3130 2e32 3132 3520 372e 3438  625 10.2125 7.48
-00000570: 3132 3520 3130 2e32 3735 4337 2e39 3638  125 10.275C7.968
-00000580: 3735 2031 302e 3332 3520 382e 3437 3520  75 10.325 8.475 
-00000590: 3130 2e33 3520 3920 3130 2e33 355a 4d39  10.35 9 10.35ZM9
-000005a0: 2031 332e 3935 4339 2e35 3520 3133 2e39   13.95C9.55 13.9
-000005b0: 3520 3130 2e31 2031 332e 3931 3235 2031  5 10.1 13.9125 1
-000005c0: 302e 3635 2031 332e 3833 3735 4331 312e  0.65 13.8375C11.
-000005d0: 3231 3235 2031 332e 3735 2031 312e 3732  2125 13.75 11.72
-000005e0: 3520 3133 2e36 3433 3720 3132 2e31 3837  5 13.6437 12.187
-000005f0: 3520 3133 2e35 3138 3743 3132 2e36 3632  5 13.5187C12.662
-00000600: 3520 3133 2e33 3831 3220 3133 2e30 3536  5 13.3812 13.056
-00000610: 3220 3133 2e32 3331 3220 3133 2e33 3638  2 13.2312 13.368
-00000620: 3720 3133 2e30 3638 3743 3133 2e36 3933  7 13.0687C13.693
-00000630: 3720 3132 2e39 3036 3220 3133 2e38 3837  7 12.9062 13.887
-00000640: 3520 3132 2e37 3337 3520 3133 2e39 3520  5 12.7375 13.95 
-00000650: 3132 2e35 3632 3556 3130 2e36 3638 3743  12.5625V10.6687C
-00000660: 3133 2e36 3520 3130 2e38 3331 3220 3133  13.65 10.8312 13
-00000670: 2e33 3132 3520 3130 2e39 3831 3220 3132  .3125 10.9812 12
-00000680: 2e39 3337 3520 3131 2e31 3138 3743 3132  .9375 11.1187C12
-00000690: 2e35 3735 2031 312e 3234 3337 2031 322e  .575 11.2437 12.
-000006a0: 3138 3132 2031 312e 3335 2031 312e 3735  1812 11.35 11.75
-000006b0: 3632 2031 312e 3433 3735 4331 312e 3333  62 11.4375C11.33
-000006c0: 3132 2031 312e 3532 3520 3130 2e38 3837  12 11.525 10.887
-000006d0: 3520 3131 2e35 3933 3720 3130 2e34 3235  5 11.5937 10.425
-000006e0: 2031 312e 3634 3337 4339 2e39 3632 3520   11.6437C9.9625 
-000006f0: 3131 2e36 3831 3220 392e 3438 3735 2031  11.6812 9.4875 1
-00000700: 312e 3720 3920 3131 2e37 4338 2e35 2031  1.7 9 11.7C8.5 1
-00000710: 312e 3720 382e 3031 3235 2031 312e 3638  1.7 8.0125 11.68
-00000720: 3132 2037 2e35 3337 3520 3131 2e36 3433  12 7.5375 11.643
-00000730: 3743 372e 3037 3520 3131 2e35 3933 3720  7C7.075 11.5937 
-00000740: 362e 3633 3132 3520 3131 2e35 3235 2036  6.63125 11.525 6
-00000750: 2e32 3036 3235 2031 312e 3433 3735 4335  .20625 11.4375C5
-00000760: 2e37 3933 3735 2031 312e 3335 2035 2e34  .79375 11.35 5.4
-00000770: 2031 312e 3234 3337 2035 2e30 3235 2031   11.2437 5.025 1
-00000780: 312e 3131 3837 4334 2e36 3632 3520 3130  1.1187C4.6625 10
-00000790: 2e39 3831 3220 342e 3333 3735 2031 302e  .9812 4.3375 10.
-000007a0: 3833 3132 2034 2e30 3520 3130 2e36 3638  8312 4.05 10.668
-000007b0: 3756 3132 2e36 4334 2e31 3132 3520 3132  7V12.6C4.1125 12
-000007c0: 2e37 3632 3520 342e 3320 3132 2e39 3235  .7625 4.3 12.925
-000007d0: 2034 2e36 3132 3520 3133 2e30 3837 3543   4.6125 13.0875C
-000007e0: 342e 3933 3735 2031 332e 3235 2035 2e33  4.9375 13.25 5.3
-000007f0: 3331 3235 2031 332e 3339 3337 2035 2e37  3125 13.3937 5.7
-00000800: 3933 3735 2031 332e 3531 3837 4336 2e32  9375 13.5187C6.2
-00000810: 3638 3735 2031 332e 3634 3337 2036 2e37  6875 13.6437 6.7
-00000820: 3837 3520 3133 2e37 3520 372e 3335 2031  875 13.75 7.35 1
-00000830: 332e 3833 3735 4337 2e39 3132 3520 3133  3.8375C7.9125 13
-00000840: 2e39 3132 3520 382e 3436 3235 2031 332e  .9125 8.4625 13.
-00000850: 3935 2039 2031 332e 3935 5a22 2066 696c  95 9 13.95Z" fil
-00000860: 6c3d 2223 3631 3631 3631 222f 3e0a 3c2f  l="#616161"/>.</
-00000870: 7376 673e 0a                             svg>.
+00000060: 3c67 2063 6c69 702d 7061 7468 3d22 7572  <g clip-path="ur
+00000070: 6c28 2363 6c69 7030 5f32 3930 385f 3233  l(#clip0_2908_23
+00000080: 3131 3329 223e 0a3c 7265 6374 2077 6964  113)">.<rect wid
+00000090: 7468 3d22 3138 2220 6865 6967 6874 3d22  th="18" height="
+000000a0: 3138 2220 6669 6c6c 3d22 7768 6974 6522  18" fill="white"
+000000b0: 2f3e 0a3c 7061 7468 2064 3d22 4d39 2031  />.<path d="M9 1
+000000c0: 352e 3343 372e 3233 3735 2031 352e 3320  5.3C7.2375 15.3 
+000000d0: 352e 3734 3337 3520 3135 2e30 3337 3520  5.74375 15.0375 
+000000e0: 342e 3531 3837 3520 3134 2e35 3132 3543  4.51875 14.5125C
+000000f0: 332e 3330 3632 3520 3133 2e39 3837 3520  3.30625 13.9875 
+00000100: 322e 3720 3133 2e33 3520 322e 3720 3132  2.7 13.35 2.7 12
+00000110: 2e36 5635 2e34 4332 2e37 2034 2e36 3520  .6V5.4C2.7 4.65 
+00000120: 332e 3331 3235 2034 2e30 3132 3520 342e  3.3125 4.0125 4.
+00000130: 3533 3735 2033 2e34 3837 3543 352e 3736  5375 3.4875C5.76
+00000140: 3235 2032 2e39 3632 3520 372e 3235 2032  25 2.9625 7.25 2
+00000150: 2e37 2039 2032 2e37 4331 302e 3733 3735  .7 9 2.7C10.7375
+00000160: 2032 2e37 2031 322e 3231 3838 2032 2e39   2.7 12.2188 2.9
+00000170: 3632 3520 3133 2e34 3433 3820 332e 3438  625 13.4438 3.48
+00000180: 3735 4331 342e 3638 3133 2034 2e30 3132  75C14.6813 4.012
+00000190: 3520 3135 2e33 2034 2e36 3520 3135 2e33  5 15.3 4.65 15.3
+000001a0: 2035 2e34 5631 322e 3643 3135 2e33 2031   5.4V12.6C15.3 1
+000001b0: 332e 3335 2031 342e 3638 3735 2031 332e  3.35 14.6875 13.
+000001c0: 3938 3735 2031 332e 3436 3235 2031 342e  9875 13.4625 14.
+000001d0: 3531 3235 4331 322e 3233 3735 2031 352e  5125C12.2375 15.
+000001e0: 3033 3735 2031 302e 3735 2031 352e 3320  0375 10.75 15.3 
+000001f0: 3920 3135 2e33 5a4d 3920 362e 3735 4331  9 15.3ZM9 6.75C1
+00000200: 302e 3037 3520 362e 3735 2031 312e 3131  0.075 6.75 11.11
+00000210: 3235 2036 2e36 3138 3735 2031 322e 3131  25 6.61875 12.11
+00000220: 3235 2036 2e33 3536 3235 4331 332e 3131  25 6.35625C13.11
+00000230: 3235 2036 2e30 3831 3235 2031 332e 3732  25 6.08125 13.72
+00000240: 3520 352e 3736 3235 2031 332e 3935 2035  5 5.7625 13.95 5
+00000250: 2e34 4331 332e 3732 3520 352e 3035 2031  .4C13.725 5.05 1
+00000260: 332e 3130 3633 2034 2e37 3337 3520 3132  3.1063 4.7375 12
+00000270: 2e30 3933 3820 342e 3436 3235 4331 312e  .0938 4.4625C11.
+00000280: 3039 3338 2034 2e31 3837 3520 3130 2e30  0938 4.1875 10.0
+00000290: 3632 3520 342e 3035 2039 2034 2e30 3543  625 4.05 9 4.05C
+000002a0: 372e 3932 3520 342e 3035 2036 2e38 3831  7.925 4.05 6.881
+000002b0: 3235 2034 2e31 3837 3520 352e 3836 3837  25 4.1875 5.8687
+000002c0: 3520 342e 3436 3235 4334 2e38 3638 3735  5 4.4625C4.86875
+000002d0: 2034 2e37 3337 3520 342e 3236 3235 2035   4.7375 4.2625 5
+000002e0: 2e30 3520 342e 3035 2035 2e34 4334 2e32  .05 4.05 5.4C4.2
+000002f0: 3632 3520 352e 3736 3235 2034 2e38 3632  625 5.7625 4.862
+00000300: 3520 362e 3038 3132 3520 352e 3835 2036  5 6.08125 5.85 6
+00000310: 2e33 3536 3235 4336 2e38 3520 362e 3631  .35625C6.85 6.61
+00000320: 3837 3520 372e 3920 362e 3735 2039 2036  875 7.9 6.75 9 6
+00000330: 2e37 355a 4d39 2031 302e 3335 4339 2e35  .75ZM9 10.35C9.5
+00000340: 3235 2031 302e 3335 2031 302e 3032 3520  25 10.35 10.025 
+00000350: 3130 2e33 3235 2031 302e 3520 3130 2e32  10.325 10.5 10.2
+00000360: 3735 4331 302e 3937 3520 3130 2e32 3132  75C10.975 10.212
+00000370: 3520 3131 2e34 3138 3820 3130 2e31 3331  5 11.4188 10.131
+00000380: 3220 3131 2e38 3331 3320 3130 2e30 3331  2 11.8313 10.031
+00000390: 3243 3132 2e32 3536 3320 392e 3933 3132  2C12.2563 9.9312
+000003a0: 3520 3132 2e36 3433 3820 392e 3830 3632  5 12.6438 9.8062
+000003b0: 3520 3132 2e39 3933 3820 392e 3635 3632  5 12.9938 9.6562
+000003c0: 3543 3133 2e33 3536 3320 392e 3439 3337  5C13.3563 9.4937
+000003d0: 3520 3133 2e36 3735 2039 2e33 3132 3520  5 13.675 9.3125 
+000003e0: 3133 2e39 3520 392e 3131 3235 5637 2e30  13.95 9.1125V7.0
+000003f0: 3638 3735 4331 332e 3635 2037 2e32 3331  6875C13.65 7.231
+00000400: 3235 2031 332e 3331 3235 2037 2e33 3831  25 13.3125 7.381
+00000410: 3235 2031 322e 3933 3735 2037 2e35 3138  25 12.9375 7.518
+00000420: 3735 4331 322e 3537 3520 372e 3634 3337  75C12.575 7.6437
+00000430: 3520 3132 2e31 3831 3320 372e 3735 2031  5 12.1813 7.75 1
+00000440: 312e 3735 3633 2037 2e38 3337 3543 3131  1.7563 7.8375C11
+00000450: 2e33 3331 3320 372e 3932 3520 3130 2e38  .3313 7.925 10.8
+00000460: 3837 3520 372e 3939 3337 3520 3130 2e34  875 7.99375 10.4
+00000470: 3235 2038 2e30 3433 3735 4339 2e39 3632  25 8.04375C9.962
+00000480: 3520 382e 3038 3132 3520 392e 3438 3735  5 8.08125 9.4875
+00000490: 2038 2e31 2039 2038 2e31 4338 2e35 2038   8.1 9 8.1C8.5 8
+000004a0: 2e31 2038 2e30 3132 3520 382e 3038 3132  .1 8.0125 8.0812
+000004b0: 3520 372e 3533 3735 2038 2e30 3433 3735  5 7.5375 8.04375
+000004c0: 4337 2e30 3735 2037 2e39 3933 3735 2036  C7.075 7.99375 6
+000004d0: 2e36 3331 3235 2037 2e39 3235 2036 2e32  .63125 7.925 6.2
+000004e0: 3036 3235 2037 2e38 3337 3543 352e 3739  0625 7.8375C5.79
+000004f0: 3337 3520 372e 3735 2035 2e34 2037 2e36  375 7.75 5.4 7.6
+00000500: 3433 3735 2035 2e30 3235 2037 2e35 3138  4375 5.025 7.518
+00000510: 3735 4334 2e36 3632 3520 372e 3338 3132  75C4.6625 7.3812
+00000520: 3520 342e 3333 3735 2037 2e32 3331 3235  5 4.3375 7.23125
+00000530: 2034 2e30 3520 372e 3036 3837 3556 392e   4.05 7.06875V9.
+00000540: 3131 3235 4334 2e33 3235 2039 2e33 3132  1125C4.325 9.312
+00000550: 3520 342e 3633 3735 2039 2e34 3933 3735  5 4.6375 9.49375
+00000560: 2034 2e39 3837 3520 392e 3635 3632 3543   4.9875 9.65625C
+00000570: 352e 3333 3735 2039 2e38 3036 3235 2035  5.3375 9.80625 5
+00000580: 2e37 3138 3735 2039 2e39 3331 3235 2036  .71875 9.93125 6
+00000590: 2e31 3331 3235 2031 302e 3033 3132 4336  .13125 10.0312C6
+000005a0: 2e35 3536 3235 2031 302e 3133 3132 2037  .55625 10.1312 7
+000005b0: 2e30 3036 3235 2031 302e 3231 3235 2037  .00625 10.2125 7
+000005c0: 2e34 3831 3235 2031 302e 3237 3543 372e  .48125 10.275C7.
+000005d0: 3936 3837 3520 3130 2e33 3235 2038 2e34  96875 10.325 8.4
+000005e0: 3735 2031 302e 3335 2039 2031 302e 3335  75 10.35 9 10.35
+000005f0: 5a4d 3920 3133 2e39 3543 392e 3535 2031  ZM9 13.95C9.55 1
+00000600: 332e 3935 2031 302e 3120 3133 2e39 3132  3.95 10.1 13.912
+00000610: 3520 3130 2e36 3520 3133 2e38 3337 3543  5 10.65 13.8375C
+00000620: 3131 2e32 3132 3520 3133 2e37 3520 3131  11.2125 13.75 11
+00000630: 2e37 3235 2031 332e 3634 3337 2031 322e  .725 13.6437 12.
+00000640: 3138 3735 2031 332e 3531 3837 4331 322e  1875 13.5187C12.
+00000650: 3636 3235 2031 332e 3338 3132 2031 332e  6625 13.3812 13.
+00000660: 3035 3633 2031 332e 3233 3132 2031 332e  0563 13.2312 13.
+00000670: 3336 3838 2031 332e 3036 3837 4331 332e  3688 13.0687C13.
+00000680: 3639 3338 2031 322e 3930 3632 2031 332e  6938 12.9062 13.
+00000690: 3838 3735 2031 322e 3733 3735 2031 332e  8875 12.7375 13.
+000006a0: 3935 2031 322e 3536 3235 5631 302e 3636  95 12.5625V10.66
+000006b0: 3837 4331 332e 3635 2031 302e 3833 3132  87C13.65 10.8312
+000006c0: 2031 332e 3331 3235 2031 302e 3938 3132   13.3125 10.9812
+000006d0: 2031 322e 3933 3735 2031 312e 3131 3837   12.9375 11.1187
+000006e0: 4331 322e 3537 3520 3131 2e32 3433 3720  C12.575 11.2437 
+000006f0: 3132 2e31 3831 3320 3131 2e33 3520 3131  12.1813 11.35 11
+00000700: 2e37 3536 3320 3131 2e34 3337 3543 3131  .7563 11.4375C11
+00000710: 2e33 3331 3320 3131 2e35 3235 2031 302e  .3313 11.525 10.
+00000720: 3838 3735 2031 312e 3539 3337 2031 302e  8875 11.5937 10.
+00000730: 3432 3520 3131 2e36 3433 3743 392e 3936  425 11.6437C9.96
+00000740: 3235 2031 312e 3638 3132 2039 2e34 3837  25 11.6812 9.487
+00000750: 3520 3131 2e37 2039 2031 312e 3743 382e  5 11.7 9 11.7C8.
+00000760: 3520 3131 2e37 2038 2e30 3132 3520 3131  5 11.7 8.0125 11
+00000770: 2e36 3831 3220 372e 3533 3735 2031 312e  .6812 7.5375 11.
+00000780: 3634 3337 4337 2e30 3735 2031 312e 3539  6437C7.075 11.59
+00000790: 3337 2036 2e36 3331 3235 2031 312e 3532  37 6.63125 11.52
+000007a0: 3520 362e 3230 3632 3520 3131 2e34 3337  5 6.20625 11.437
+000007b0: 3543 352e 3739 3337 3520 3131 2e33 3520  5C5.79375 11.35 
+000007c0: 352e 3420 3131 2e32 3433 3720 352e 3032  5.4 11.2437 5.02
+000007d0: 3520 3131 2e31 3138 3743 342e 3636 3235  5 11.1187C4.6625
+000007e0: 2031 302e 3938 3132 2034 2e33 3337 3520   10.9812 4.3375 
+000007f0: 3130 2e38 3331 3220 342e 3035 2031 302e  10.8312 4.05 10.
+00000800: 3636 3837 5631 322e 3643 342e 3131 3235  6687V12.6C4.1125
+00000810: 2031 322e 3736 3235 2034 2e33 2031 322e   12.7625 4.3 12.
+00000820: 3932 3520 342e 3631 3235 2031 332e 3038  925 4.6125 13.08
+00000830: 3735 4334 2e39 3337 3520 3133 2e32 3520  75C4.9375 13.25 
+00000840: 352e 3333 3132 3520 3133 2e33 3933 3720  5.33125 13.3937 
+00000850: 352e 3739 3337 3520 3133 2e35 3138 3743  5.79375 13.5187C
+00000860: 362e 3236 3837 3520 3133 2e36 3433 3720  6.26875 13.6437 
+00000870: 362e 3738 3735 2031 332e 3735 2037 2e33  6.7875 13.75 7.3
+00000880: 3520 3133 2e38 3337 3543 372e 3931 3235  5 13.8375C7.9125
+00000890: 2031 332e 3931 3235 2038 2e34 3632 3520   13.9125 8.4625 
+000008a0: 3133 2e39 3520 3920 3133 2e39 355a 2220  13.95 9 13.95Z" 
+000008b0: 6669 6c6c 3d22 2333 4237 3845 3722 2f3e  fill="#3B78E7"/>
+000008c0: 0a3c 2f67 3e0a 3c64 6566 733e 0a3c 636c  .</g>.<defs>.<cl
+000008d0: 6970 5061 7468 2069 643d 2263 6c69 7030  ipPath id="clip0
+000008e0: 5f32 3930 385f 3233 3131 3322 3e0a 3c72  _2908_23113">.<r
+000008f0: 6563 7420 7769 6474 683d 2231 3822 2068  ect width="18" h
+00000900: 6569 6768 743d 2231 3822 2066 696c 6c3d  eight="18" fill=
+00000910: 2277 6869 7465 222f 3e0a 3c2f 636c 6970  "white"/>.</clip
+00000920: 5061 7468 3e0a 3c2f 6465 6673 3e0a 3c2f  Path>.</defs>.</
+00000930: 7376 673e 0a                             svg>.
```

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/dataproc_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/dataproc_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/delete_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/delete_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/edit_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/edit_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/edit_icon_disable.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/edit_icon_disable.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/restart_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/restart_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/restart_icon_disable.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/restart_icon_disable.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/settings_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/settings_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/signin_google_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/signin_google_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/start_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/start_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/start_icon_disable.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/start_icon_disable.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/stop_disable_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/stop_disable_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/stop_icon.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/stop_icon.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/style/icons/stop_icon_disable.svg` & `dataproc_jupyter_plugin-0.1.9/style/icons/stop_icon_disable.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/third_party/icons/pyspark_logo.svg` & `dataproc_jupyter_plugin-0.1.9/third_party/icons/pyspark_logo.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/third_party/icons/scala_logo.svg` & `dataproc_jupyter_plugin-0.1.9/third_party/icons/scala_logo.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/third_party/icons/sparkr_logo.svg` & `dataproc_jupyter_plugin-0.1.9/third_party/icons/sparkr_logo.svg`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/.gitignore` & `dataproc_jupyter_plugin-0.1.9/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 dataproc_jupyter_plugin/labextension
 # Version file is handled by hatchling
 dataproc_jupyter_plugin/_version.py
 
 # Integration tests
 ui-tests/test-results/
 ui-tests/playwright-report/
-ui-tests-3.6.6/test-results/
-ui-tests-3.6.6/playwright-report/
 
 # Created by https://www.gitignore.io/api/python
 # Edit at https://www.gitignore.io/?templates=python
 
 ### Python ###
 # Byte-compiled / optimized / DLL files
 __pycache__/
```

### Comparing `dataproc_jupyter_plugin-0.1.78/LICENSE` & `dataproc_jupyter_plugin-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/README.md` & `dataproc_jupyter_plugin-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dataproc_jupyter_plugin-0.1.78/pyproject.toml` & `dataproc_jupyter_plugin-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.5.0", "jupyterlab>=3.6.0,<5", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dataproc_jupyter_plugin"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
@@ -18,21 +18,17 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=2.7.3,<3",
-    "cachetools>=4.2.4",
-    "google-cloud-jupyter-config>=0.0.10",
-    "kernels-mixer>=0.0.12",
-    "pendulum>=3.0.0",
-    "pydantic~=1.10.0",
-    "bigframes~=0.22.0"
+    "jupyter_server>=2.0.1,<3",
+    "cachetools>=5.0.0",
+    "kernels-mixer",
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
@@ -83,15 +79,15 @@
 build_dir = "dataproc_jupyter_plugin/labextension"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
 before-build-npm = [
-    "python -m pip install 'jupyterlab>=3.6.0,<5'",
+    "python -m pip install 'jupyterlab>=4.0.0,<5'",
     "jlpm",
     "jlpm build:prod"
 ]
 before-build-python = ["jlpm clean:all"]
 
 [tool.check-wheel-contents]
 ignore = ["W002"]
```

### Comparing `dataproc_jupyter_plugin-0.1.78/PKG-INFO` & `dataproc_jupyter_plugin-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: dataproc_jupyter_plugin
-Version: 0.1.78
-Dynamic: Keywords
+Version: 0.1.9
 Summary: It is a plugin to work with dataproc services in Jupyterlab
 Project-URL: Homepage, https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin
 Project-URL: Bug Tracker, https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin/issues
 Project-URL: Repository, https://github.com/GoogleCloudDataproc/dataproc-jupyter-plugin.git
 Author-email: google <dataproc-plugins@google.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -218,21 +217,17 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: bigframes~=0.22.0
-Requires-Dist: cachetools>=4.2.4
-Requires-Dist: google-cloud-jupyter-config>=0.0.10
-Requires-Dist: jupyter-server<3,>=2.7.3
-Requires-Dist: kernels-mixer>=0.0.12
-Requires-Dist: pendulum>=3.0.0
-Requires-Dist: pydantic~=1.10.0
+Requires-Dist: cachetools>=5.0.0
+Requires-Dist: jupyter-server<3,>=2.0.1
+Requires-Dist: kernels-mixer
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-jupyter[server]>=0.6.0; extra == 'test'
 Description-Content-Type: text/markdown
```

