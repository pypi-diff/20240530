# Comparing `tmp/etiket_client-0.2.14-py3-none-any.whl.zip` & `tmp/etiket_client-0.2.15-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 117514 bytes, number of entries: 149
--rw-r--r--  2.0 unx      241 b- defN 24-May-23 13:12 etiket_client/__init__.py
+Zip file size: 139973 bytes, number of entries: 178
+-rw-r--r--  2.0 unx      572 b- defN 24-May-30 09:13 etiket_client/__init__.py
 -rw-r--r--  2.0 unx      256 b- defN 23-Dec-13 10:03 etiket_client/exceptions.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/__init__.py
 -rw-r--r--  2.0 unx     1845 b- defN 24-Mar-14 16:06 etiket_client/GUI/app.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/models/__init__.py
 -rw-r--r--  2.0 unx     1362 b- defN 23-Dec-13 10:03 etiket_client/GUI/models/login_mgmt.py
 -rw-r--r--  2.0 unx     1399 b- defN 23-Dec-13 10:03 etiket_client/GUI/models/schema_mgmt.py
 -rw-r--r--  2.0 unx     2112 b- defN 24-Mar-18 07:04 etiket_client/GUI/models/scope_mgmt.py
@@ -19,133 +19,162 @@
 -rw-r--r--  2.0 unx      577 b- defN 23-Dec-13 10:03 etiket_client/GUI/qml/icons/logout.svg
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/qml/settings_pages/__init__.py
 -rw-r--r--  2.0 unx     7366 b- defN 23-Dec-13 10:03 etiket_client/GUI/qml/settings_pages/scope_settings.qml
 -rw-r--r--  2.0 unx    18481 b- defN 24-Mar-14 16:52 etiket_client/GUI/qml/settings_pages/sync_add_new_source.qml
 -rw-r--r--  2.0 unx     7175 b- defN 24-Mar-24 09:35 etiket_client/GUI/qml/settings_pages/sync_settings.qml
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/resources/__init__.py
 -rw-r--r--  2.0 unx     1434 b- defN 23-Dec-13 10:03 etiket_client/GUI/resources/resource_rc.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:54 etiket_client/GUI/sync/__init__.py
+-rw-r--r--  2.0 unx     1880 b- defN 24-May-30 15:56 etiket_client/GUI/sync/app.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/models/__init__.py
+-rw-r--r--  2.0 unx     1362 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/models/login_mgmt.py
+-rw-r--r--  2.0 unx     1399 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/models/schema_mgmt.py
+-rw-r--r--  2.0 unx     2102 b- defN 24-May-30 15:57 etiket_client/GUI/sync/models/scope_mgmt.py
+-rw-r--r--  2.0 unx     1314 b- defN 24-Mar-18 07:03 etiket_client/GUI/sync/models/sync_def_scope.py
+-rw-r--r--  2.0 unx     8340 b- defN 24-Apr-26 10:18 etiket_client/GUI/sync/models/sync_mgmt.py
+-rw-r--r--  2.0 unx     1195 b- defN 24-Jan-11 16:31 etiket_client/GUI/sync/models/sync_proc_mgmt.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/__init__.py
+-rw-r--r--  2.0 unx     2748 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/login.qml
+-rw-r--r--  2.0 unx      921 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/main.qml
+-rw-r--r--  2.0 unx      970 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/settings_index.qml
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/icons/__init__.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/icons/delete.svg
+-rw-r--r--  2.0 unx      577 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/icons/logout.svg
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/settings_pages/__init__.py
+-rw-r--r--  2.0 unx     7366 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/qml/settings_pages/scope_settings.qml
+-rw-r--r--  2.0 unx    18481 b- defN 24-Mar-14 16:52 etiket_client/GUI/sync/qml/settings_pages/sync_add_new_source.qml
+-rw-r--r--  2.0 unx     7382 b- defN 24-May-30 07:26 etiket_client/GUI/sync/qml/settings_pages/sync_settings.qml
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/resources/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 23-Dec-13 10:03 etiket_client/GUI/sync/resources/resource_rc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/local/__init__.py
 -rw-r--r--  2.0 unx     1213 b- defN 24-May-09 07:04 etiket_client/local/database.py
 -rw-r--r--  2.0 unx     1144 b- defN 23-Dec-13 10:03 etiket_client/local/exceptions.py
--rw-r--r--  2.0 unx     6109 b- defN 24-May-16 13:13 etiket_client/local/model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 13:03 etiket_client/local/types.py
+-rw-r--r--  2.0 unx     6491 b- defN 24-May-29 10:33 etiket_client/local/model.py
+-rw-r--r--  2.0 unx      134 b- defN 24-May-29 06:36 etiket_client/local/types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/local/alembic/__init__.py
 -rw-r--r--  2.0 unx     2239 b- defN 24-Mar-13 10:58 etiket_client/local/alembic/env.py
 -rw-r--r--  2.0 unx      850 b- defN 24-Apr-16 18:25 etiket_client/local/alembic/versions/24b0115d4cc7_adding_delete_cache_table.py
 -rw-r--r--  2.0 unx     8187 b- defN 23-Dec-13 13:01 etiket_client/local/alembic/versions/4000a8b9703a_qdrive_v_0_1_0.py
+-rw-r--r--  2.0 unx     2433 b- defN 24-May-27 08:23 etiket_client/local/alembic/versions/4b200763b2ff_fix_datatype.py
 -rw-r--r--  2.0 unx      802 b- defN 23-Dec-13 10:03 etiket_client/local/alembic/versions/6e8777d1c9f3_etiket_client_v_0_1_1.py
 -rw-r--r--  2.0 unx     3913 b- defN 24-Apr-04 06:47 etiket_client/local/alembic/versions/716ce37a1bc1_etiket_client_v_0_1_3.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/local/alembic/versions/__init__.py
 -rw-r--r--  2.0 unx     4611 b- defN 24-Apr-10 12:54 etiket_client/local/alembic/versions/bec34208dd87_update_uniqueness_of_alt_uuid.py
 -rw-r--r--  2.0 unx     1272 b- defN 24-May-15 09:36 etiket_client/local/alembic/versions/c077798e06b9_adding_sync_attr_to_files.py
 -rw-r--r--  2.0 unx     1289 b- defN 24-Jan-12 10:00 etiket_client/local/alembic/versions/c5d93c68feda_etiket_client_v0_1_5.py
 -rw-r--r--  2.0 unx     1812 b- defN 24-May-16 14:39 etiket_client/local/alembic/versions/c867b432fc6a_convert_time_to_utc.py
--rw-r--r--  2.0 unx     4790 b- defN 24-Mar-24 09:35 etiket_client/local/alembic/versions/fe8c0d015ba2_update_sync_tables.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-29 07:13 etiket_client/local/alembic/versions/f8337520d10d_add_app_register_table.py
+-rw-r--r--  2.0 unx     4790 b- defN 24-May-27 08:13 etiket_client/local/alembic/versions/fe8c0d015ba2_update_sync_tables.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/local/dao/__init__.py
+-rw-r--r--  2.0 unx      940 b- defN 24-May-29 10:49 etiket_client/local/dao/app.py
 -rw-r--r--  2.0 unx     2060 b- defN 24-May-03 11:27 etiket_client/local/dao/base.py
--rw-r--r--  2.0 unx    10377 b- defN 24-May-09 10:33 etiket_client/local/dao/dataset.py
+-rw-r--r--  2.0 unx    10377 b- defN 24-May-27 09:28 etiket_client/local/dao/dataset.py
 -rw-r--r--  2.0 unx     3790 b- defN 24-May-14 14:50 etiket_client/local/dao/file.py
 -rw-r--r--  2.0 unx     2153 b- defN 23-Dec-13 10:03 etiket_client/local/dao/schema.py
 -rw-r--r--  2.0 unx     6113 b- defN 24-May-09 07:05 etiket_client/local/dao/scope.py
 -rw-r--r--  2.0 unx     2397 b- defN 23-Dec-13 10:03 etiket_client/local/dao/user.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/local/models/__init__.py
+-rw-r--r--  2.0 unx      486 b- defN 24-May-29 06:41 etiket_client/local/models/app.py
 -rw-r--r--  2.0 unx     3441 b- defN 24-May-16 12:29 etiket_client/local/models/dataset.py
 -rw-r--r--  2.0 unx     2904 b- defN 24-May-16 12:47 etiket_client/local/models/file.py
 -rw-r--r--  2.0 unx     1427 b- defN 24-May-16 12:43 etiket_client/local/models/schema.py
 -rw-r--r--  2.0 unx     1342 b- defN 24-May-16 12:47 etiket_client/local/models/scope.py
 -rw-r--r--  2.0 unx      900 b- defN 24-May-16 12:46 etiket_client/local/models/user.py
 -rw-r--r--  2.0 unx     1292 b- defN 24-May-16 12:47 etiket_client/local/models/user_base.py
 -rw-r--r--  2.0 unx      453 b- defN 24-May-16 14:00 etiket_client/local/models/utility.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/python_api/__init__.py
--rw-r--r--  2.0 unx     1028 b- defN 24-May-15 15:05 etiket_client/python_api/dataset.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 10:42 etiket_client/python_api/__init__.py
+-rw-r--r--  2.0 unx     1028 b- defN 24-May-24 09:47 etiket_client/python_api/dataset.py
 -rw-r--r--  2.0 unx       51 b- defN 23-Dec-13 10:03 etiket_client/python_api/exceptions.py
 -rw-r--r--  2.0 unx      465 b- defN 23-Dec-13 10:03 etiket_client/python_api/schema.py
 -rw-r--r--  2.0 unx      739 b- defN 24-Mar-13 10:58 etiket_client/python_api/scopes.py
 -rw-r--r--  2.0 unx      227 b- defN 23-Dec-13 10:03 etiket_client/python_api/user.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/python_api/dataset_model/__init__.py
 -rw-r--r--  2.0 unx     3280 b- defN 24-May-09 08:38 etiket_client/python_api/dataset_model/dataset.py
 -rw-r--r--  2.0 unx    11710 b- defN 24-May-09 09:03 etiket_client/python_api/dataset_model/files.py
 -rw-r--r--  2.0 unx     2060 b- defN 23-Dec-13 10:03 etiket_client/python_api/dataset_model/utility.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/remote/__init__.py
 -rw-r--r--  2.0 unx     1943 b- defN 24-Apr-09 10:33 etiket_client/remote/authenticate.py
--rw-r--r--  2.0 unx     6517 b- defN 24-May-15 07:27 etiket_client/remote/client.py
+-rw-r--r--  2.0 unx     6517 b- defN 24-May-29 14:07 etiket_client/remote/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/remote/endpoints/__init__.py
--rw-r--r--  2.0 unx     1467 b- defN 24-Apr-02 16:03 etiket_client/remote/endpoints/dataset.py
--rw-r--r--  2.0 unx     2069 b- defN 24-May-15 07:27 etiket_client/remote/endpoints/file.py
+-rw-r--r--  2.0 unx     1745 b- defN 24-May-24 09:45 etiket_client/remote/endpoints/dataset.py
+-rw-r--r--  2.0 unx     2069 b- defN 24-May-28 07:56 etiket_client/remote/endpoints/file.py
 -rw-r--r--  2.0 unx      664 b- defN 24-May-08 12:39 etiket_client/remote/endpoints/schema.py
 -rw-r--r--  2.0 unx      813 b- defN 23-Dec-13 10:03 etiket_client/remote/endpoints/scope.py
 -rw-r--r--  2.0 unx      257 b- defN 23-Dec-13 10:03 etiket_client/remote/endpoints/user.py
--rw-r--r--  2.0 unx      206 b- defN 23-Dec-13 10:03 etiket_client/remote/endpoints/version.py
+-rw-r--r--  2.0 unx      846 b- defN 24-May-29 14:00 etiket_client/remote/endpoints/user_logs.py
+-rw-r--r--  2.0 unx     2078 b- defN 24-May-30 07:56 etiket_client/remote/endpoints/version.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/remote/endpoints/models/__init__.py
 -rw-r--r--  2.0 unx     3035 b- defN 24-Apr-04 14:51 etiket_client/remote/endpoints/models/dataset.py
 -rw-r--r--  2.0 unx     2203 b- defN 24-May-15 11:48 etiket_client/remote/endpoints/models/file.py
 -rw-r--r--  2.0 unx      708 b- defN 23-Dec-13 10:03 etiket_client/remote/endpoints/models/schema.py
 -rw-r--r--  2.0 unx     1722 b- defN 24-Apr-04 14:45 etiket_client/remote/endpoints/models/schema_base.py
 -rw-r--r--  2.0 unx     1490 b- defN 24-Apr-04 14:42 etiket_client/remote/endpoints/models/scope.py
--rw-r--r--  2.0 unx     1375 b- defN 24-Apr-16 14:48 etiket_client/remote/endpoints/models/types.py
+-rw-r--r--  2.0 unx     1572 b- defN 24-May-30 07:34 etiket_client/remote/endpoints/models/types.py
 -rw-r--r--  2.0 unx     1399 b- defN 24-Apr-04 14:54 etiket_client/remote/endpoints/models/user.py
 -rw-r--r--  2.0 unx     1270 b- defN 24-Apr-09 10:36 etiket_client/remote/endpoints/models/user_base.py
+-rw-r--r--  2.0 unx      589 b- defN 24-May-29 13:36 etiket_client/remote/endpoints/models/user_logs.py
 -rw-r--r--  2.0 unx      463 b- defN 24-May-16 12:41 etiket_client/remote/endpoints/models/utility.py
+-rw-r--r--  2.0 unx     1835 b- defN 24-May-30 07:35 etiket_client/remote/endpoints/models/version.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/remote/tools/__init__.py
 -rw-r--r--  2.0 unx     2560 b- defN 24-May-09 09:02 etiket_client/remote/tools/file_download.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/settings/__init__.py
 -rw-r--r--  2.0 unx     1289 b- defN 24-May-13 15:06 etiket_client/settings/folders.py
--rw-r--r--  2.0 unx     1639 b- defN 24-Jan-11 16:31 etiket_client/settings/logging.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-29 14:25 etiket_client/settings/logging.py
 -rw-r--r--  2.0 unx     1647 b- defN 24-May-09 09:41 etiket_client/settings/saver.py
 -rw-r--r--  2.0 unx      758 b- defN 23-Dec-13 10:03 etiket_client/settings/schema_settings.py
 -rw-r--r--  2.0 unx      691 b- defN 24-May-09 08:51 etiket_client/settings/user_settings.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/sync/__init__.py
 -rw-r--r--  2.0 unx     3067 b- defN 24-May-16 14:39 etiket_client/sync/proc.py
--rw-r--r--  2.0 unx     7890 b- defN 24-May-16 14:31 etiket_client/sync/run.py
+-rw-r--r--  2.0 unx     7988 b- defN 24-May-29 10:42 etiket_client/sync/run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/backends/__init__.py
 -rw-r--r--  2.0 unx     1633 b- defN 24-Mar-13 11:27 etiket_client/sync/backends/sources.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/backends/core_tools/__init__.py
 -rw-r--r--  2.0 unx      171 b- defN 24-Mar-13 15:06 etiket_client/sync/backends/core_tools/core_tools_config_class.py
--rw-r--r--  2.0 unx     6899 b- defN 24-May-17 12:41 etiket_client/sync/backends/core_tools/core_tools_sync_class.py
+-rw-r--r--  2.0 unx     6983 b- defN 24-May-27 12:12 etiket_client/sync/backends/core_tools/core_tools_sync_class.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-21 15:02 etiket_client/sync/backends/core_tools/data_getters/__init__.py
 -rw-r--r--  2.0 unx      570 b- defN 24-Apr-29 09:29 etiket_client/sync/backends/core_tools/data_getters/get_gates.py
 -rw-r--r--  2.0 unx     6693 b- defN 24-Apr-21 15:43 etiket_client/sync/backends/core_tools/data_getters/get_pulses.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 10:03 etiket_client/sync/backends/core_tools/real_time_sync/__init__.py
 -rw-r--r--  2.0 unx      485 b- defN 24-Apr-03 09:02 etiket_client/sync/backends/core_tools/real_time_sync/core_tools_m_param.py
--rw-r--r--  2.0 unx     4730 b- defN 24-Apr-17 07:27 etiket_client/sync/backends/core_tools/real_time_sync/measurement_sync.py
+-rw-r--r--  2.0 unx     4939 b- defN 24-May-30 09:12 etiket_client/sync/backends/core_tools/real_time_sync/measurement_sync.py
 -rw-r--r--  2.0 unx     8112 b- defN 24-Apr-17 08:21 etiket_client/sync/backends/core_tools/real_time_sync/qcodes_parameters.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/backends/native/__init__.py
--rw-r--r--  2.0 unx     6474 b- defN 24-May-16 12:12 etiket_client/sync/backends/native/sync_agent.py
+-rw-r--r--  2.0 unx     6551 b- defN 24-May-24 15:49 etiket_client/sync/backends/native/sync_agent.py
 -rw-r--r--  2.0 unx     2945 b- defN 24-May-17 07:53 etiket_client/sync/backends/native/sync_scopes.py
 -rw-r--r--  2.0 unx      971 b- defN 24-Apr-16 14:34 etiket_client/sync/backends/native/sync_user.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/backends/qcodes/__init__.py
 -rw-r--r--  2.0 unx      129 b- defN 24-Apr-02 10:03 etiket_client/sync/backends/qcodes/qcodes_config_class.py
--rw-r--r--  2.0 unx     5590 b- defN 24-May-17 07:49 etiket_client/sync/backends/qcodes/qcodes_sync_class.py
--rw-r--r--  2.0 unx     4230 b- defN 24-Apr-17 08:43 etiket_client/sync/backends/qcodes/real_time_sync.py
+-rw-r--r--  2.0 unx     5755 b- defN 24-May-30 08:29 etiket_client/sync/backends/qcodes/qcodes_sync_class.py
+-rw-r--r--  2.0 unx     4310 b- defN 24-May-30 08:42 etiket_client/sync/backends/qcodes/real_time_sync.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/backends/quantify/__init__.py
 -rw-r--r--  2.0 unx     5617 b- defN 24-May-03 12:37 etiket_client/sync/backends/quantify/quantify_sync_class.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/base/__init__.py
 -rw-r--r--  2.0 unx     1268 b- defN 24-May-16 09:55 etiket_client/sync/base/sync_source_abstract.py
--rw-r--r--  2.0 unx     8848 b- defN 24-May-14 14:47 etiket_client/sync/base/sync_utilities.py
+-rw-r--r--  2.0 unx     9774 b- defN 24-May-30 08:52 etiket_client/sync/base/sync_utilities.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/base/checksums/__init__.py
 -rw-r--r--  2.0 unx      259 b- defN 24-May-17 12:42 etiket_client/sync/base/checksums/any.py
--rw-r--r--  2.0 unx     1379 b- defN 24-Mar-14 09:58 etiket_client/sync/base/checksums/hdf5.py
+-rw-r--r--  2.0 unx     1502 b- defN 24-May-27 12:05 etiket_client/sync/base/checksums/hdf5.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 09:03 etiket_client/sync/database/__init__.py
 -rw-r--r--  2.0 unx     1998 b- defN 24-Mar-13 08:30 etiket_client/sync/database/dao_scope_mappings.py
 -rw-r--r--  2.0 unx     8349 b- defN 24-Mar-24 09:35 etiket_client/sync/database/dao_sync_items.py
 -rw-r--r--  2.0 unx     1690 b- defN 24-Mar-13 11:36 etiket_client/sync/database/dao_sync_sources.py
--rw-r--r--  2.0 unx     2486 b- defN 24-May-16 13:12 etiket_client/sync/database/models_db.py
+-rw-r--r--  2.0 unx     2485 b- defN 24-May-27 08:20 etiket_client/sync/database/models_db.py
 -rw-r--r--  2.0 unx     2416 b- defN 24-May-13 07:55 etiket_client/sync/database/models_pydantic.py
 -rw-r--r--  2.0 unx      563 b- defN 24-Mar-13 08:29 etiket_client/sync/database/start_up.py
 -rw-r--r--  2.0 unx      299 b- defN 24-Mar-08 14:37 etiket_client/sync/database/types.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Dec-13 10:03 etiket_client/sync/uploader/__init__.py
 -rw-r--r--  2.0 unx     3297 b- defN 24-May-15 12:49 etiket_client/sync/uploader/file_uploader.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-05 10:59 etiket_client/testing/__init__.py
 -rw-r--r--  2.0 unx       60 b- defN 24-Mar-14 15:05 etiket_client/testing/test_gui.py
 -rw-r--r--  2.0 unx     1174 b- defN 24-Mar-13 14:01 etiket_client/testing/test_live_sync.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-05 11:00 etiket_client/testing/live_data_generation/__init__.py
 -rw-r--r--  2.0 unx     4907 b- defN 24-Apr-16 18:39 etiket_client/testing/live_data_generation/core_tools_LD.py
 -rw-r--r--  2.0 unx    12577 b- defN 24-Apr-09 08:03 etiket_client/testing/live_data_generation/parameters.py
 -rw-r--r--  2.0 unx     4766 b- defN 24-Apr-16 18:40 etiket_client/testing/live_data_generation/qcodes_LD.py
 -rw-r--r--  2.0 unx     6594 b- defN 24-May-15 07:27 etiket_client/testing/live_data_generation/qdrive_LD.py
--rw-r--r--  2.0 unx    16695 b- defN 24-May-23 13:14 etiket_client-0.2.14.dist-info/LICENCE
--rw-r--r--  2.0 unx     1101 b- defN 24-May-23 13:14 etiket_client-0.2.14.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 13:14 etiket_client-0.2.14.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-May-23 13:14 etiket_client-0.2.14.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-25 08:37 etiket_client-0.2.14.dist-info/zip-safe
--rw-rw-r--  2.0 unx    14848 b- defN 24-May-23 13:14 etiket_client-0.2.14.dist-info/RECORD
-149 files, 352549 bytes uncompressed, 93082 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx    16695 b- defN 24-May-30 16:10 etiket_client-0.2.15.dist-info/LICENCE
+-rw-r--r--  2.0 unx     1101 b- defN 24-May-30 16:10 etiket_client-0.2.15.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 16:10 etiket_client-0.2.15.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-30 16:10 etiket_client-0.2.15.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Mar-25 08:37 etiket_client-0.2.15.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    17805 b- defN 24-May-30 16:10 etiket_client-0.2.15.dist-info/RECORD
+178 files, 426601 bytes uncompressed, 110685 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -66,14 +66,80 @@
 
 Filename: etiket_client/GUI/resources/__init__.py
 Comment: 
 
 Filename: etiket_client/GUI/resources/resource_rc.py
 Comment: 
 
+Filename: etiket_client/GUI/sync/__init__.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/app.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/models/__init__.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/models/login_mgmt.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/models/schema_mgmt.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/models/scope_mgmt.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/models/sync_def_scope.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/models/sync_mgmt.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/models/sync_proc_mgmt.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/__init__.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/login.qml
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/main.qml
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/settings_index.qml
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/icons/__init__.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/icons/delete.svg
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/icons/logout.svg
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/settings_pages/__init__.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/settings_pages/scope_settings.qml
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/settings_pages/sync_add_new_source.qml
+Comment: 
+
+Filename: etiket_client/GUI/sync/qml/settings_pages/sync_settings.qml
+Comment: 
+
+Filename: etiket_client/GUI/sync/resources/__init__.py
+Comment: 
+
+Filename: etiket_client/GUI/sync/resources/resource_rc.py
+Comment: 
+
 Filename: etiket_client/local/__init__.py
 Comment: 
 
 Filename: etiket_client/local/database.py
 Comment: 
 
 Filename: etiket_client/local/exceptions.py
@@ -93,14 +159,17 @@
 
 Filename: etiket_client/local/alembic/versions/24b0115d4cc7_adding_delete_cache_table.py
 Comment: 
 
 Filename: etiket_client/local/alembic/versions/4000a8b9703a_qdrive_v_0_1_0.py
 Comment: 
 
+Filename: etiket_client/local/alembic/versions/4b200763b2ff_fix_datatype.py
+Comment: 
+
 Filename: etiket_client/local/alembic/versions/6e8777d1c9f3_etiket_client_v_0_1_1.py
 Comment: 
 
 Filename: etiket_client/local/alembic/versions/716ce37a1bc1_etiket_client_v_0_1_3.py
 Comment: 
 
 Filename: etiket_client/local/alembic/versions/__init__.py
@@ -114,20 +183,26 @@
 
 Filename: etiket_client/local/alembic/versions/c5d93c68feda_etiket_client_v0_1_5.py
 Comment: 
 
 Filename: etiket_client/local/alembic/versions/c867b432fc6a_convert_time_to_utc.py
 Comment: 
 
+Filename: etiket_client/local/alembic/versions/f8337520d10d_add_app_register_table.py
+Comment: 
+
 Filename: etiket_client/local/alembic/versions/fe8c0d015ba2_update_sync_tables.py
 Comment: 
 
 Filename: etiket_client/local/dao/__init__.py
 Comment: 
 
+Filename: etiket_client/local/dao/app.py
+Comment: 
+
 Filename: etiket_client/local/dao/base.py
 Comment: 
 
 Filename: etiket_client/local/dao/dataset.py
 Comment: 
 
 Filename: etiket_client/local/dao/file.py
@@ -141,14 +216,17 @@
 
 Filename: etiket_client/local/dao/user.py
 Comment: 
 
 Filename: etiket_client/local/models/__init__.py
 Comment: 
 
+Filename: etiket_client/local/models/app.py
+Comment: 
+
 Filename: etiket_client/local/models/dataset.py
 Comment: 
 
 Filename: etiket_client/local/models/file.py
 Comment: 
 
 Filename: etiket_client/local/models/schema.py
@@ -219,14 +297,17 @@
 
 Filename: etiket_client/remote/endpoints/scope.py
 Comment: 
 
 Filename: etiket_client/remote/endpoints/user.py
 Comment: 
 
+Filename: etiket_client/remote/endpoints/user_logs.py
+Comment: 
+
 Filename: etiket_client/remote/endpoints/version.py
 Comment: 
 
 Filename: etiket_client/remote/endpoints/models/__init__.py
 Comment: 
 
 Filename: etiket_client/remote/endpoints/models/dataset.py
@@ -249,17 +330,23 @@
 
 Filename: etiket_client/remote/endpoints/models/user.py
 Comment: 
 
 Filename: etiket_client/remote/endpoints/models/user_base.py
 Comment: 
 
+Filename: etiket_client/remote/endpoints/models/user_logs.py
+Comment: 
+
 Filename: etiket_client/remote/endpoints/models/utility.py
 Comment: 
 
+Filename: etiket_client/remote/endpoints/models/version.py
+Comment: 
+
 Filename: etiket_client/remote/tools/__init__.py
 Comment: 
 
 Filename: etiket_client/remote/tools/file_download.py
 Comment: 
 
 Filename: etiket_client/settings/__init__.py
@@ -423,26 +510,26 @@
 
 Filename: etiket_client/testing/live_data_generation/qcodes_LD.py
 Comment: 
 
 Filename: etiket_client/testing/live_data_generation/qdrive_LD.py
 Comment: 
 
-Filename: etiket_client-0.2.14.dist-info/LICENCE
+Filename: etiket_client-0.2.15.dist-info/LICENCE
 Comment: 
 
-Filename: etiket_client-0.2.14.dist-info/METADATA
+Filename: etiket_client-0.2.15.dist-info/METADATA
 Comment: 
 
-Filename: etiket_client-0.2.14.dist-info/WHEEL
+Filename: etiket_client-0.2.15.dist-info/WHEEL
 Comment: 
 
-Filename: etiket_client-0.2.14.dist-info/top_level.txt
+Filename: etiket_client-0.2.15.dist-info/top_level.txt
 Comment: 
 
-Filename: etiket_client-0.2.14.dist-info/zip-safe
+Filename: etiket_client-0.2.15.dist-info/zip-safe
 Comment: 
 
-Filename: etiket_client-0.2.14.dist-info/RECORD
+Filename: etiket_client-0.2.15.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## etiket_client/__init__.py

```diff
@@ -1,8 +1,16 @@
-__version__  = '0.2.14'
+__version__  = '0.2.15'
+
+try:
+    from etiket_client.local.dao.app import dao_app_registerer
+    from etiket_client.local.types import ProcTypes
+
+    dao_app_registerer.register(__version__, ProcTypes.etiket_client, __file__)
+except Exception as e:
+    print("Failed to update version information about the current session (etiket_client). \nError: ", e)
 
 from etiket_client.settings.logging import set_up_logging
 set_up_logging(__name__)
 
 from etiket_client.sync.proc import start_sync_agent
 from etiket_client.remote.authenticate import login, logout
```

## etiket_client/local/model.py

```diff
@@ -1,13 +1,14 @@
 from typing import List, Optional
 
 from sqlalchemy import ForeignKey, UniqueConstraint, func, TIMESTAMP, types
 from sqlalchemy.orm import Mapped, mapped_column,\
                             DeclarativeBase, relationship
 
+from etiket_client.local.types import ProcTypes
 from etiket_client.remote.endpoints.models.types import FileStatusLocal, FileType, UserType
 from uuid import UUID
 from datetime import datetime
 
 class Base(DeclarativeBase):
     pass
 
@@ -135,8 +136,19 @@
     synchronized : Mapped[bool] = mapped_column(index=True)
     
 class FileDeleteQueue(Base):
     __tablename__ = "file_delete_queue"
     
     id: Mapped[int] = mapped_column(primary_key=True)
     local_path : Mapped[str]
-    delete_after : Mapped[datetime] = mapped_column(types.DateTime(timezone=True))
+    delete_after : Mapped[datetime] = mapped_column(types.DateTime(timezone=True))
+    
+class QHarborAppRegister(Base):
+    __tablename__ = "qharbor_app_register"
+    
+    id: Mapped[int] = mapped_column(primary_key=True)
+    
+    type : Mapped[ProcTypes]
+    version : Mapped[int]
+    
+    location : Mapped[str]
+    last_session : Mapped[datetime] = mapped_column(types.DateTime(timezone=True), default=func.now())
```

## etiket_client/local/types.py

```diff
@@ -0,0 +1,9 @@
+00000000: 696d 706f 7274 2065 6e75 6d0a 636c 6173  import enum.clas
+00000010: 7320 5072 6f63 5479 7065 7328 7374 722c  s ProcTypes(str,
+00000020: 2065 6e75 6d2e 456e 756d 293a 0a20 2020   enum.Enum):.   
+00000030: 2071 4472 6976 6520 3d20 2271 4472 6976   qDrive = "qDriv
+00000040: 6522 0a20 2020 2065 7469 6b65 745f 636c  e".    etiket_cl
+00000050: 6965 6e74 203d 2022 6574 696b 6574 5f63  ient = "etiket_c
+00000060: 6c69 656e 7422 0a20 2020 2064 6174 6151  lient".    dataQ
+00000070: 7275 6973 6572 203d 2022 6461 7461 5172  ruiser = "dataQr
+00000080: 7569 7365 7222                           uiser"
```

## etiket_client/local/dao/dataset.py

```diff
@@ -121,15 +121,15 @@
     def get_unsynced_datasets(session : Session):
         scopes_ids = _get_user_scope_ids(user_settings.user_name , session=session)
 
         stmt = select(Files.dataset_id).where(and_(Files.synchronized == False, Files.status == FileStatusLocal.complete, Files.type != FileType.HDF5_CACHE))
         stmt = stmt.group_by(Files.dataset_id)
         ds_ids = session.execute(stmt).scalars().all()
         
-        stmt = select(Datasets.uuid).where(or_(Datasets.synchronized is False, Datasets.id.in_(ds_ids)))
+        stmt = select(Datasets.uuid).where(or_(Datasets.synchronized == False, Datasets.id.in_(ds_ids)))
         stmt = stmt.where(Datasets.scope_id.in_(scopes_ids))
         stmt = stmt.order_by(Datasets.collected)
         return session.execute(stmt).scalars().all()
         
     @staticmethod
     def get_number_of_datasets(session : Session):
         stmt = select(func.count(Datasets.id))
```

## etiket_client/remote/endpoints/dataset.py

```diff
@@ -4,20 +4,25 @@
     DatasetSearch, DatasetSelection
 
 import uuid, typing
 
 def dataset_create(datasetCreate : DatasetCreate) -> None:
     client.post("/dataset/", json_data=datasetCreate.model_dump(mode="json"))
 
-def dataset_read(dataset_uuid :'uuid.UUID | str', scope_uuid : 'uuid.UUID | None' = None) -> DatasetRead:
+def dataset_read(dataset_uuid : uuid.UUID, scope_uuid : 'uuid.UUID | None' = None) -> DatasetRead:
     params = {"dataset_uuid" : str(dataset_uuid)}
     if scope_uuid is not None:
         params["scope_uuid"] = str(scope_uuid)
     data = client.get("/dataset/", params=params)
     return DatasetRead.model_validate(data)
+
+def dataset_read_by_alt_uid(dataset_alt_uid : str, scope_uuid : uuid.UUID) -> DatasetRead:
+    params = {"dataset_alt_uid" : str(dataset_alt_uid), "scope_uuid" : str(scope_uuid)}
+    data = client.get("/dataset/by_alt_uid/", params=params)
+    return DatasetRead.model_validate(data)
     
 def dataset_update(dataset_uuid :uuid.UUID, datasetUpdate : DatasetUpdate) ->  None :
     params = {"dataset_uuid" : str(dataset_uuid)}
     client.patch("/dataset/", json_data=datasetUpdate.model_dump(mode="json"), params=params)
 
 def dataset_search(datasetSearch : DatasetSearch, offset = 0, limit = 100) -> typing.List[DatasetRead]:
     params = {"offset" : offset, "limit" : limit}
```

## etiket_client/remote/endpoints/version.py

```diff
@@ -1,6 +1,39 @@
+from typing import List, Optional
+
 from etiket_client.remote.client import client
-from etiket_client.remote.endpoints.models.user import UserReadWithScopes
+from etiket_client.remote.endpoints.models.types import SoftwareType
+from etiket_client.remote.endpoints.models.version import VersionCreate, VersionRead, VersionUpdate, ReleaseCreate, ReleaseRead
+
+def get_web_api_version() -> str:
+    response = client.get("/version/API/")
+    return response
+
+def get_latest_version(software_type : SoftwareType, allow_beta : bool = None) -> VersionRead:
+    params = {"software_type": software_type, "allow_beta": allow_beta}
+    response = client.get("/version/latest/", params=params)
+    return VersionRead.model_validate(response)
+
+def get_versions(software_type : SoftwareType, min_version : Optional[str] = None,  allow_beta : bool = False) -> List[VersionRead]:
+    params = {"software_type": software_type, "min_version": min_version, "allow_beta": allow_beta}
+    response = client.get("/version/", params=params)
+    return [VersionRead.model_validate(version) for version in response]
+
+def get_latest_release(allow_beta : bool = False) -> ReleaseRead:
+    params = {"allow_beta": allow_beta}
+    response = client.get("/release/latest/", params=params)
+    return ReleaseRead.model_validate(response)
+
+def get_release_from_version(software_type : SoftwareType, version: str, allow_beta : bool = False) -> ReleaseRead:
+    params = {"version": version, "software_type": software_type, "allow_beta": allow_beta}
+    response = client.get("/release/get_release_from_version/", params=params)
+    return ReleaseRead.model_validate(response)
+
+def create_version(version_create: VersionCreate) -> None:
+    client.post("/version/create/", json_data=version_create.model_dump(mode="json"))
+
+def update_version(version_id: int, version_update: VersionUpdate) -> None:
+    params = {"version_id": version_id}
+    client.patch("/version/update/", json_data=version_update.model_dump(mode="json"), params=params)
 
-def api_version() -> str:
-    response = client.get("/version/")
-    return response
+def create_release(release_create: ReleaseCreate) -> None:
+    client.post("/release/create/", json_data=release_create.model_dump(mode="json"))
```

## etiket_client/remote/endpoints/models/types.py

```diff
@@ -28,14 +28,23 @@
     complete = "complete" # file is written and ready for upload.
     unavailable = "unavailable" # File is not created or deleted.
 
 class UploadConcat(str, enum.Enum):
     partial = "partial"
     final = "final"
 
+class UserLogStatus(str, enum.Enum):
+    pending = "pending"
+    secured = "secured"
+
+class SoftwareType(enum.StrEnum):
+    etiket = "etiket"
+    dataQruiser = "dataQruiser"
+    qdrive = "qdrive"
+
 namestr     = constr(min_length=1, max_length=100)
 usernamestr = constr(min_length=4, max_length=20, pattern=r"^[a-zA-Z0-9_]+$")
 metastr     = constr(min_length=1, max_length=255)
 filestr     = constr(min_length=2, max_length=255)
 datasetstr  = constr(min_length=2, max_length=255)
 collectionstr = constr(min_length=2, max_length=255)
 uidstr      = constr(min_length=5, max_length=80)
```

## etiket_client/settings/logging.py

```diff
@@ -1,23 +1,24 @@
 from etiket_client.settings.folders import get_log_dir
 import logging, logging.handlers, os
-import datetime
+import datetime, sys
 
 def set_up_logging(name):
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
     logger.propagate = True
 
     log_file = os.path.join(get_log_dir(), f'{datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")}_etiket_client.{os.getpid()}.log')
     handler = logging.handlers.TimedRotatingFileHandler(log_file, when="midnight", backupCount=10)
     handler.suffix = "%Y%m%d"
     handler.setLevel(logging.INFO)
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
     handler.setFormatter(formatter)
     logger.addHandler(handler)
+    logger.info("Logging started, using python version: %s", sys.version)
 
 def set_up_sync_logger(name):
     log_file = os.path.join(get_log_dir(), f'{datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")}_etiket_sync.{os.getpid()}.log')
     
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
     logger.propagate = True
@@ -35,9 +36,9 @@
     
     handler = logging.handlers.TimedRotatingFileHandler(log_file, when="midnight", backupCount=10)
     handler.suffix = "%Y%m%d"
     handler.setLevel(logging.INFO)
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
     handler.setFormatter(formatter)
     logger.addHandler(handler)
-
+    
     return logger
```

## etiket_client/sync/run.py

```diff
@@ -47,67 +47,67 @@
             n_syncs += items_synced
             continue
         else:
             try:
                 logger.info("Syncing %s, of type %s", sync_source.name, sync_source.sync_class.SyncAgentName)
                 get_new_sync_items(sync_source, session)
                 
-                sync_item = dao_sync_items.read_sync_item(sync_source.id, offset = 0, session=session)
+                s_item = dao_sync_items.read_sync_item(sync_source.id, offset = 0, session=session)
                 
-                if sync_item is not None:
-                    liveDS = sync_source.sync_class.checkLiveDataset(sync_source.sync_config, sync_item)
+                if s_item is not None:
+                    liveDS = sync_source.sync_class.checkLiveDataset(sync_source.sync_config, s_item)
                     # this is needed to not get stuck in a loop of live datasets (though not the cleanest way)
-                    liveDS_already_tried = check_live_DS_already_tried(sync_item, session)
+                    liveDS_already_tried = check_live_DS_already_tried(s_item, session)
                     if (liveDS and sync_source.sync_class.LiveSyncImplemented is False) or liveDS_already_tried:
                         # assume only one live dataset at a time.
-                        sync_item = dao_sync_items.read_sync_item(sync_source.id, offset = 1, session=session)
+                        s_item = dao_sync_items.read_sync_item(sync_source.id, offset = 1, session=session)
                         liveDS = False
                 
-                if sync_item is None:
+                if s_item is None:
                     ssu = sync_source_update(status=SyncSourceStatus.synchronized)
                     dao_sync_sources.update_status(sync_source.id, ssu, session)
                     logger.info("No new items to sync from %s.", sync_source.name)
                     continue
 
 
                 liveSync_successful = False
                 if liveDS is True:
                     try:
-                        logger.info("Syncing live dataset, %s from %s.", sync_item.dataIdentifier, sync_source.name)
-                        sync_source.sync_class.syncDatasetLive(sync_source.sync_config, sync_item)
+                        logger.info("Syncing live dataset, %s from %s.", s_item.dataIdentifier, sync_source.name)
+                        sync_source.sync_class.syncDatasetLive(sync_source.sync_config, s_item)
                         liveSync_successful = True
-                        logger.info("Synced live dataset, %s from %s.", sync_item.dataIdentifier, sync_source.name)
+                        logger.info("Synced live dataset, %s from %s.", s_item.dataIdentifier, sync_source.name)
                         # do not mark as successfull -- upload the final version of the files using the normal sync.
                     except Exception:
-                        logger.exception("Failed to synchronize %s from %s.", sync_item.dataIdentifier, sync_source.name)
-                        dao_sync_items.mark_failed_attempt(sync_source.id, sync_item.dataIdentifier,session)
+                        logger.exception("Failed to synchronize %s from %s.", s_item.dataIdentifier, sync_source.name)
+                        dao_sync_items.mark_failed_attempt(sync_source.id, s_item.dataIdentifier,session)
                                             
                 if liveDS is False or liveSync_successful is True:
                     try:
-                        logger.info("Syncing %s from %s.", sync_item.dataIdentifier, sync_source.name)
-                        sync_source.sync_class.syncDatasetNormal(sync_source.sync_config, sync_item)
+                        logger.info("Syncing %s from %s.", s_item.dataIdentifier, sync_source.name)
+                        sync_source.sync_class.syncDatasetNormal(sync_source.sync_config, s_item)
                         
                         try: # remove any dataset caches:
-                            dataset_local = dao_dataset.read(sync_item.datasetUUID, session)
+                            dataset_local = dao_dataset.read(s_item.datasetUUID, session)
                             for file in dataset_local.files:
                                 if file.type == FileType.HDF5_CACHE:
                                     fs = FileSelect(uuid=file.uuid, version_id=file.version_id)
                                     dao_file.delete(fs, session)
                         except DatasetNotFoundException:
                             pass
                         except Exception as e:
                             raise e                            
                         
                         n_syncs += 1
-                        logger.info("Synced %s from %s.", sync_item.dataIdentifier, sync_source.name)
+                        logger.info("Synced %s from %s.", s_item.dataIdentifier, sync_source.name)
 
-                        dao_sync_items.mark_successful_sync(sync_source.id, sync_item.dataIdentifier ,session)
+                        dao_sync_items.mark_successful_sync(sync_source.id, s_item.dataIdentifier ,session)
                     except Exception:
-                        logger.exception("Failed to synchronize %s from %s.", sync_item.dataIdentifier, sync_source.name)
-                        dao_sync_items.mark_failed_attempt(sync_source.id, sync_item.dataIdentifier,session)   
+                        logger.exception("Failed to synchronize %s from %s.", s_item.dataIdentifier, sync_source.name)
+                        dao_sync_items.mark_failed_attempt(sync_source.id, s_item.dataIdentifier,session)   
                 
                 # update statistics and state of the sync source.
                 n_items = dao_sync_items.count_items(sync_source.id, session)
                 n_items_failed = dao_sync_items.count_items_failed(sync_source.id, session)
                 n_items_synced = dao_sync_items.count_items_synchronized(sync_source.id, session)
                 n_items_skipped = dao_sync_items.count_items_not_in_scope(sync_source.id, session)
                 
@@ -125,28 +125,32 @@
                 logger.exception("Failed to sync %s", sync_source.name)
     if n_syncs == 0:
         time.sleep(1)
 
 def get_new_sync_items(sync_source : SyncSource, session):
     last_identifier = dao_sync_items.get_last_identifier(sync_source.id, session)
     new_items = sync_source.sync_class.getNewDatasets(sync_source.sync_config, last_identifier)
-    logger.info("Found %s new items to sync.", len(new_items))
+    logger.info("Found %s new items in remote location, to add to the list of things to synchronize.", len(new_items))
     dao_sync_items.write_sync_items(sync_source.id, new_items, session)
 
-def check_live_DS_already_tried(sync_item : sync_item, session):
+def check_live_DS_already_tried(s_item : sync_item, session):
     try:
-        dataset = dao_dataset.read(sync_item.datasetUUID, session)
+        dataset = dao_dataset.read(s_item.datasetUUID, session)
         for file in dataset.files:
             if file.type == FileType.HDF5_CACHE:
                 return True
     except DatasetNotFoundException:
         return False
     return False
 
 if __name__ == '__main__':
     import etiket_client
     from etiket_client.settings.logging import set_up_sync_logger
-
-    setproctitle('Python qdrive sync')
     
     logger = set_up_sync_logger(etiket_client.__name__)
+    
+    try: 
+        setproctitle('Python qdrive sync')
+    except Exception:
+        logger.exception("Failed to set process title.")
+    
     sync_loop()
```

## etiket_client/sync/backends/core_tools/core_tools_sync_class.py

```diff
@@ -94,40 +94,40 @@
 def upload_meta_data(ds_ct : 'data_set', syncIdentifier: sync_item):
     if ds_ct.snapshot:
         f_info = file_info(name = 'snapshot', created = ds_ct.run_timestamp,
                             fileName = 'snapshot.json',
                             fileType= FileType.JSON,
                             file_generator = "core-tools")
         sync_utilities.upload_JSON(ds_ct.snapshot, syncIdentifier, f_info)
-        logger.info(f"Uploaded snapshot for dataset with id : {ds_ct.id}")
+        logger.info(f"Uploaded snapshot for dataset with id : {syncIdentifier.dataIdentifier}")
         
         pulses = get_AWG_pulses(ds_ct.snapshot)
         if pulses:
             f_info = file_info(name = 'AWG pulses', created = ds_ct.run_timestamp,
                                 fileName = 'pulses.hdf5',
                                 fileType= FileType.HDF5_NETCDF,
                                 file_generator = "core-tools")
             sync_utilities.upload_xarray(pulses, syncIdentifier, f_info)
-        logger.info(f"Uploaded pulses for dataset with id : {ds_ct.id}")
+        logger.info(f"Uploaded pulses for dataset with id : {syncIdentifier.dataIdentifier}")
         gates = get_gates_formatted(ds_ct.snapshot)
         if gates:
             f_info = file_info(name = 'gates', created = ds_ct.run_timestamp,
                                 fileName = 'gates.json',
                                 fileType= FileType.JSON,
                                 file_generator = "core-tools")
             sync_utilities.upload_JSON(gates, syncIdentifier, f_info)
-        logger.info(f"Uploaded gates for dataset with id : {ds_ct.id}")
+        logger.info(f"Uploaded gates for dataset with id : {syncIdentifier.dataIdentifier}")
     
     if ds_ct.metadata:
         f_info = file_info(name = 'metadata', 
                             fileName = 'metadata.json',
                             fileType= FileType.JSON,
                             created = ds_ct.run_timestamp, file_generator = "core-tools")
         sync_utilities.upload_JSON(ds_ct.metadata, syncIdentifier, f_info)
-        logger.info(f"Uploaded metadata for dataset with id : {ds_ct.id}")
+        logger.info(f"Uploaded metadata for dataset with id : {syncIdentifier.dataIdentifier}")
 
 def create_ds_from_core_tools(configData: CoreToolsConfigData, syncIdentifier: sync_item, live : bool):
     ds_ct = load_by_id(int(syncIdentifier.dataIdentifier))
     
     description = f'database : {configData.dbname} | id : {ds_ct.id} | ct_uuid : {ds_ct.exp_uuid}'
     
     ds_info = dataset_info(name = ds_ct.name, datasetUUID = syncIdentifier.datasetUUID,
```

## etiket_client/sync/backends/core_tools/real_time_sync/measurement_sync.py

```diff
@@ -1,22 +1,23 @@
 from etiket_client.remote.endpoints.models.types import FileType
 from etiket_client.sync.backends.core_tools.real_time_sync.core_tools_m_param import core_tools_m_param
 from etiket_client.sync.backends.core_tools.real_time_sync.qcodes_parameters import qcodes_m_param_emulator
 
 from qdrive.measurement.data_collector import data_collector, from_QCoDeS_parameter
 from qdrive.dataset.dataset import dataset
 
+from qcodes.utils.helpers import NumpyJSONEncoder
 
 try:
     from core_tools.data.SQL.SQL_connection_mgr import SQL_database_manager
     from core_tools.data.ds.data_set import load_by_id
 except ImportError:
     pass
 
-import logging, time
+import logging, time, json
 logger = logging.getLogger(__name__)
 
 class live_measurement_synchronizer:
     def __init__(self, core_tools_id, datasetUUID) -> None:
         self.core_tools_ds = load_by_id(core_tools_id)
         self.native_ds = dataset(datasetUUID)
         
@@ -46,14 +47,17 @@
                 it = m_object_iterator(param, generated_qcodes_parameters)
                 self.sync_objects.append(it)
         
         if not self.__ready():
             raise ValueError("Not all parameters are ready")
         
         self.dc = data_collector(self.native_ds, dtype=FileType.HDF5_CACHE)
+        if self.core_tools_ds.snapshot:
+            self.dc.set_attr('snapshot', json.dumps(self.core_tools_ds.snapshot, cls=NumpyJSONEncoder))
+        
         for sync_obj in self.sync_objects:
             dep = [i.param for i in sync_obj.dependencies]
             self.dc += from_QCoDeS_parameter(sync_obj.m_param.param, dep[::-1] , self.dc)
         self.dc._enable_swmr()
 
         self._last_write = time.time()
         self.__marked_complete = False
```

## etiket_client/sync/backends/native/sync_agent.py

```diff
@@ -4,14 +4,15 @@
 
 from etiket_client.remote.endpoints.dataset import dataset_read, dataset_create, dataset_update
 from etiket_client.remote.endpoints.file import file_create, file_generate_presigned_upload_link_single
 
 from etiket_client.remote.endpoints.models.dataset import DatasetCreate, DatasetUpdate
 from etiket_client.remote.endpoints.models.file import FileCreate, FileRead
 
+from etiket_client.remote.endpoints.models.types import FileStatusRem
 from etiket_client.sync.database.types import SyncSourceStatus
 from etiket_client.sync.database.dao_sync_sources import dao_sync_sources
 from etiket_client.sync.database.models_pydantic import sync_source_update
 from etiket_client.sync.base.sync_utilities import md5
 from etiket_client.sync.uploader.file_uploader import upload_new_file_single
 from etiket_client.sync.backends.native.sync_scopes import sync_scopes
 from etiket_client.sync.backends.sources import SyncSource
@@ -75,15 +76,15 @@
                     logger.info("Synchronizing file with name %s, uuid %s and version_id %s", file.name, file.uuid, file.version_id)
                     fs = FileSelect(uuid=file.uuid, version_id=file.version_id)
 
                     file_remote = get_remote_file(dataset_remote.files, file.uuid, file.version_id)
                     if file_remote:
                         logger.info("File record already present on the remote server, updating details.")
                         # TODO update details.
-                        if file_remote.md5_checksum is not None:
+                        if file_remote.status == FileStatusRem.secured:
                             fu = FileUpdateLocal(synchronized=True)
                             dao_file.update(fs, fu, session)
                             continue
                     else:
                         logger.info("Creating file record on the remote server.")
                         fc = FileCreate(**file.model_dump(), ds_uuid=dataset_local.uuid)
                         file_create(fc)
```

## etiket_client/sync/backends/qcodes/qcodes_sync_class.py

```diff
@@ -1,17 +1,19 @@
+import typing, sqlite3, qcodes as qc, os, json
+from datetime import datetime
+
 from etiket_client.sync.base.sync_source_abstract import SyncSourceAbstract
 from etiket_client.sync.base.sync_utilities import file_info, sync_utilities,\
     dataset_info, sync_item, new_sync_item, FileType
 from etiket_client.sync.backends.qcodes.real_time_sync import QCoDeS_live_sync
 from etiket_client.sync.backends.qcodes.qcodes_config_class import QCoDeSConfigData
 
 from qcodes.dataset import initialise_database, load_by_id
-from datetime import datetime
+from qcodes.utils.helpers import NumpyJSONEncoder
 
-import typing, sqlite3, qcodes as qc, os
 
 class QCoDeSSync(SyncSourceAbstract):
     SyncAgentName = "QCoDeS"
     ConfigDataClass = QCoDeSConfigData
     MapToASingleScope = True
     LiveSyncImplemented = True
 
@@ -47,23 +49,25 @@
             
         ds_qc = load_by_id(int(syncIdentifier.dataIdentifier))
         return not ds_qc.completed
     
     @staticmethod
     def syncDatasetNormal(configData: QCoDeSConfigData, syncIdentifier: sync_item):
         ds_qc = create_ds_from_qcodes(configData, syncIdentifier, False)
-
+        ds_xr = ds_qc.to_xarray_dataset()
+        
         created_time = datetime.fromtimestamp(ds_qc.run_timestamp_raw)
         if ds_qc.snapshot:
+            ds_xr.attrs['snapshot'] = json.dumps(ds_qc.snapshot, cls=NumpyJSONEncoder)
+            
             f_info = file_info(name = 'Snapshot', fileName = 'snapshot.json',
                                fileType= FileType.JSON,
                                created = created_time, file_generator = "QCoDeS")
             sync_utilities.upload_JSON(ds_qc.snapshot, syncIdentifier, f_info)
         
-        ds_xr = ds_qc.to_xarray_dataset()
         f_info = file_info(name = 'measurement', fileName = 'measured_data.hdf5',
                            fileType= FileType.HDF5_NETCDF,
                            created = created_time, file_generator = "QCoDeS")
         sync_utilities.upload_xarray(ds_xr, syncIdentifier, f_info)
 
     @staticmethod
     def syncDatasetLive(configData: QCoDeSConfigData, syncIdentifier: sync_item):
```

## etiket_client/sync/backends/qcodes/real_time_sync.py

```diff
@@ -38,20 +38,22 @@
     native_ds = dataset(datasetUUID)
     dc = data_collector(native_ds, FileType.HDF5_CACHE)
     
     for k, v in relationships.items():
         dep = [parameters[i] for i in v]
         dc += from_QCoDeS_parameter(parameters[k], dep, dc)
 
-    dc._enable_swmr() # manually set this, sometimes it takes long for qCoDeS to start writing data ... .
-
     sync_idx = 0
-    res = c.execute("Select result_table_name from runs where run_id = ?", (run_id,))
-    table_name = res.fetchone()[0]
+    res = c.execute("Select result_table_name, snapshot from runs where run_id = ?", (run_id,)).fetchone()
+    table_name = res[0]
+    snapshot_json = res[1]
     
+    dc.set_attr('snapshot', snapshot_json)
+    dc._enable_swmr() # manually set this, sometimes it takes long for qCoDeS to start writing data ... .
+
     t_last_fetch = time.time()
     
     try: 
         while not (check_complete(c, run_id) and sync_idx == getMaxId(c, table_name)):            
             c.execute(f"SELECT * FROM '{table_name}' WHERE id > ?", (sync_idx,))
             c_names = [description[0] for description in c.description]
```

## etiket_client/sync/base/sync_utilities.py

```diff
@@ -1,8 +1,8 @@
-from etiket_client.remote.endpoints.dataset import dataset_create, dataset_read
+from etiket_client.remote.endpoints.dataset import dataset_create, dataset_read, dataset_read_by_alt_uid
 from etiket_client.remote.endpoints.file import file_create, file_generate_presigned_upload_link_single, file_read_by_name
 from etiket_client.remote.endpoints.models.dataset import DatasetCreate
 from etiket_client.remote.endpoints.models.types import FileStatusRem, FileType
 from etiket_client.remote.endpoints.models.file import FileCreate
 
 from etiket_client.local.database import Session
 from etiket_client.local.dao.dataset import dao_dataset
@@ -56,15 +56,15 @@
 class sync_utilities:
     @staticmethod
     def create_ds(live_mode : bool, s_item : sync_item, ds_info : dataset_info):
         try : 
             dataset_read(ds_info.datasetUUID)
         except Exception:
             try:
-                ds = dataset_read(ds_info.alt_uid, ds_info.scopeUUID)
+                ds = dataset_read_by_alt_uid(ds_info.alt_uid, ds_info.scopeUUID)
                 with Session() as session:
                     dao_sync_items.update_uuid(ds_info.datasetUUID, ds.uuid, session)
                 s_item.datasetUUID = ds.uuid
                 logger.info("Dataset record found on remote server, updated local record.")   
             except Exception:
                 dc = DatasetCreate(uuid = ds_info.datasetUUID, alt_uid= ds_info.alt_uid,
                         collected=ds_info.created,  name = ds_info.name, creator = ds_info.creator,
@@ -140,48 +140,58 @@
         # TODO fix definition of collected and created on the server
         # create the file entry (if needed)        
         version_id = generate_version_id(f_info.created)
         fc = FileCreate(name = f_info.name, filename=f_info.fileName,
                         creator=f_info.creator, uuid =uuid.uuid4(), collected = f_info.created,
                         size = os.stat(file_path).st_size, type = f_info.fileType,
                         file_generator = f_info.file_generator, version_id = version_id,
-                        ds_uuid = s_item.datasetUUID)
+                        ds_uuid = s_item.datasetUUID, immutable=f_info.immutable_on_completion)
         
         if len(r_files) == 0:
             try :
                 with Session() as session :
                     l_files = dao_file.get_file_by_name(s_item.datasetUUID, f_info.name, session)
                     if len(l_files) > 0:
                         fc.uuid = l_files[0].uuid
             except Exception:
                 pass
+            
+            logger.info("File %s not found on remote server, creating new file.", f_info.name)
             file_create(fc)
         else:
             fc.uuid = r_files[0].uuid
             
             f_dict = {file.version_id : file for file in r_files}
-
+            
             if version_id in f_dict.keys():
                 if f_dict[version_id].md5_checksum == md5_checksum:
+                    logger.info("File %s already uploaded to remote server (identical checksum), skipping.", f_info.name)
                     return
+                elif f_dict[version_id].md5_checksum is None and  f_dict[version_id].status is FileStatusRem.secured:
+                    logger.info("File %s already uploaded to remote server (no checksum present), skipping.", f_info.name)
+                    return # this means it is a very old upload, and we should not overwrite it
                 elif f_dict[version_id].status is FileStatusRem.pending:
                     # TODO : remove upload_id of the current upload and recheck status?
+                    logger.info("File %s is pending, reuploading file.", f_info.name)
                     pass
                 elif not f_dict[version_id].immutable:
                     logger.info("File %s is mutable, overwriting file.", f_info.name)
+                    # it is likely that this is an old upload, reupload the file 
                 else : #create a new version (if needed)
                     # if last file has the same checksum, skip
                     if f_dict[max(f_dict.keys())].md5_checksum == md5_checksum:
                         logger.info("File %s already uploaded to remote server, skipping.", f_info.name)
                         return
-                    logger.info("Creating new version for file %s.", f_info.name)
+                    logger.info("Creating new version for file '%s'.", f_info.name)
                     last_mod_time = datetime.datetime.fromtimestamp(os.path.getmtime(file_path))
+                    
                     fc.version_id = generate_version_id(last_mod_time)
                     file_create(fc)
             else:
+                logger.info("Creating new version for file %s.", f_info.name)
                 file_create(fc)
 
         # upload the file
         upload_info = file_generate_presigned_upload_link_single(fc.uuid, version_id)                
         # upload_new_file_multi(file_path, upload_info, md5_checksum)
         upload_new_file_single(file_path, upload_info, md5_checksum)
```

## etiket_client/sync/base/checksums/hdf5.py

```diff
@@ -1,26 +1,32 @@
 # adapted from https://github.com/willirath/netcdf-hash/blob/master/demo_001.ipynb
 from netCDF4 import Dataset
+import numpy as np
 
 import hashlib
 
 def attribute_filter(attributes):
     "Filter for elements which do not start with '__NCH'."
     return filter(lambda a: not a.startswith("__NCH"), attributes)
 
 def update_hash_attr(name, value, hash_obj : 'hashlib._Hash'):
     """Update `hash_obj` with the UTF8 encoded string version of first `name` and then `value`."""
     hash_obj.update(str(name).encode('utf8'))
-    hash_obj.update(str(value).encode('utf8'))
+    
+    if isinstance(value, np.ndarray):
+        hash_obj.update(value.tobytes())
+    else:
+        hash_obj.update(str(value).encode('utf8'))
     return hash_obj
 
 def update_hash_var(var_obj, hash_obj : 'hashlib._Hash'):
     """Update `hash_obj` from a variable."""
     hash_obj.update(str(var_obj.name).encode('utf8'))
-    hash_obj.update(var_obj[:].data)
+    hash_obj.update(var_obj[:].tobytes())
+
     for attr in attribute_filter(sorted(var_obj.ncattrs())):
         update_hash_attr(attr, var_obj.getncattr(attr), hash_obj)
     return hash_obj
 
 def md5_netcdf4(file_name):
     """Calculate hash for a given netCDF file."""
     with Dataset(str(file_name)) as data_set:
```

## etiket_client/sync/database/models_db.py

```diff
@@ -43,16 +43,16 @@
     
     __table_args__ = (UniqueConstraint('sync_source_id', 'dataIdentifier', name='sync_source_did_constraint_sync_items'),
                       Index('read_item_index', 'sync_source_id', 'scopeIdentifier', 'synchronized', 'dataIdentifier'),
                       Index('failed_upload_index', 'sync_source_id', 'attempts'),
                       Index('sync_upload_index', 'sync_source_id', 'attempts', 'synchronized'))
 
     id: Mapped[int] = mapped_column(primary_key=True)
-    sync_source_id : Mapped[str] = mapped_column(ForeignKey("sync_sources.id"))
+    sync_source_id : Mapped[int] = mapped_column(ForeignKey("sync_sources.id"))
     dataIdentifier: Mapped[int] = mapped_column(index = True)
     scopeIdentifier : Mapped[typing.Optional[str]]
     datasetUUID  : Mapped[uuid.UUID] = mapped_column(unique=True)
     
     synchronized : Mapped[bool] = mapped_column(default = False)
-    attempts : Mapped[bool] = mapped_column(default = 0)
+    attempts : Mapped[int] = mapped_column(default = 0)
     
     last_update : Mapped[datetime] = mapped_column(types.DateTime(timezone=True), server_default=func.now(), onupdate=func.now())
```

## Comparing `etiket_client-0.2.14.dist-info/LICENCE` & `etiket_client-0.2.15.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `etiket_client-0.2.14.dist-info/METADATA` & `etiket_client-0.2.15.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etiket_client
-Version: 0.2.14
+Version: 0.2.15
 Summary: A client to interact with the etiket web framework.
 Author: QDrive team
 Requires-Python: >=3.7
 License-File: LICENCE
 Requires-Dist: PyQt5 >=5.15.0
 Requires-Dist: SQLAlchemy >=2.0.0
 Requires-Dist: alembic >=1.6.0
```

## Comparing `etiket_client-0.2.14.dist-info/RECORD` & `etiket_client-0.2.15.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-etiket_client/__init__.py,sha256=-pqYNk1-63qcvHisZ6eqoEAVE_7Kc0o4tuvfHlwpGcw,241
+etiket_client/__init__.py,sha256=-MJGjVf4fXZXEPV5BgoLiCfyf8gNAeVz9uSvwKRSnxc,572
 etiket_client/exceptions.py,sha256=sCjzyCWAWClHGS4YPie6xJrwjVwr3Te6Avv35krYyW4,256
 etiket_client/GUI/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/GUI/app.py,sha256=A5gGtXvZ1M5ms5MB6l0RiOtPPCgm6S1Sz5WKWl5NtRk,1845
 etiket_client/GUI/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/GUI/models/login_mgmt.py,sha256=BLde15chZThFv0gCcstFg7kkijNn5SCvreC7Ri3pU_k,1362
 etiket_client/GUI/models/schema_mgmt.py,sha256=Obag2eR1agR9fUCjBBVKsQtVNlV3ZTbZhkL2VYUjzYs,1399
 etiket_client/GUI/models/scope_mgmt.py,sha256=kdB_vzFD7DlKJvlBqqB_gkmPVquzCThK3O1654f9U2A,2112
@@ -18,39 +18,65 @@
 etiket_client/GUI/qml/icons/logout.svg,sha256=63Lfu3L-5pQkM0lXKICAYxAQ6P1rJhM6AkRU8iSafCM,577
 etiket_client/GUI/qml/settings_pages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/GUI/qml/settings_pages/scope_settings.qml,sha256=7yY5nmBdYm9PcnYkgzeUaTj7aqnbws58KJEzFT3Jyoo,7366
 etiket_client/GUI/qml/settings_pages/sync_add_new_source.qml,sha256=Yp4udI--QTNbB9ciO6c1KEg3_MIDKAYeiKhlTm6uQvI,18481
 etiket_client/GUI/qml/settings_pages/sync_settings.qml,sha256=HnhSyl5qkGlmad0Z2JskXAcMporXB3wQxdNw2ls_MTY,7175
 etiket_client/GUI/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/GUI/resources/resource_rc.py,sha256=mX5GMKlYtRO4evpeswFokedjeh6VGfHm5qNgiW3BuV4,1434
+etiket_client/GUI/sync/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/GUI/sync/app.py,sha256=YMnfd8Ag8UeblxJOCA5O_IC-XOVxk1pSH-2WkVZOdEc,1880
+etiket_client/GUI/sync/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/GUI/sync/models/login_mgmt.py,sha256=BLde15chZThFv0gCcstFg7kkijNn5SCvreC7Ri3pU_k,1362
+etiket_client/GUI/sync/models/schema_mgmt.py,sha256=Obag2eR1agR9fUCjBBVKsQtVNlV3ZTbZhkL2VYUjzYs,1399
+etiket_client/GUI/sync/models/scope_mgmt.py,sha256=dWR_-fFOBp3zFVGpGa0iIJ2irgDLfr2eGySDi_bROM0,2102
+etiket_client/GUI/sync/models/sync_def_scope.py,sha256=B-pAtJzRoYgxPuvWPbRSHJwGheft0QXVjbP-mZII5Aw,1314
+etiket_client/GUI/sync/models/sync_mgmt.py,sha256=powx6Bn5FBPbYvlvU1OwNYxxZsIlEo68JxHAtWSQjCE,8340
+etiket_client/GUI/sync/models/sync_proc_mgmt.py,sha256=Eex-vihsmwqqryIn1KYOcDqB74w0RkN-kCbB7TZucgo,1195
+etiket_client/GUI/sync/qml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/GUI/sync/qml/login.qml,sha256=vrfPQ8NOeZp0eCnsHkdFPS3F2CJbPANZ-pei45-01tg,2748
+etiket_client/GUI/sync/qml/main.qml,sha256=pgT-xZnhiItFe457-wSW92Y3u_wpeUJMv88hPPyfpUk,921
+etiket_client/GUI/sync/qml/settings_index.qml,sha256=F6r73KG81iaYTWfjfAWwd5SxjYizHUw5Nfqio51siLY,970
+etiket_client/GUI/sync/qml/icons/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/GUI/sync/qml/icons/delete.svg,sha256=7HXnVq9ON6kmovZO-PWerIUnamWPyKeu8MwSxehx6XE,300
+etiket_client/GUI/sync/qml/icons/logout.svg,sha256=63Lfu3L-5pQkM0lXKICAYxAQ6P1rJhM6AkRU8iSafCM,577
+etiket_client/GUI/sync/qml/settings_pages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/GUI/sync/qml/settings_pages/scope_settings.qml,sha256=7yY5nmBdYm9PcnYkgzeUaTj7aqnbws58KJEzFT3Jyoo,7366
+etiket_client/GUI/sync/qml/settings_pages/sync_add_new_source.qml,sha256=Yp4udI--QTNbB9ciO6c1KEg3_MIDKAYeiKhlTm6uQvI,18481
+etiket_client/GUI/sync/qml/settings_pages/sync_settings.qml,sha256=SlByhqZnCJOQ411d7cTp8SU1YYdSpzuF2oIs0OrEj78,7382
+etiket_client/GUI/sync/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/GUI/sync/resources/resource_rc.py,sha256=mX5GMKlYtRO4evpeswFokedjeh6VGfHm5qNgiW3BuV4,1434
 etiket_client/local/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/local/database.py,sha256=T6RA5ygauKG82FW8EheiT9dqqCqv2251KjTVTG66xnk,1213
 etiket_client/local/exceptions.py,sha256=D5yaTw0ndwFYDmDl-8ngKIB33E4Yoc_kZFNmfBy-SKY,1144
-etiket_client/local/model.py,sha256=HQFf4EgyJzeP0CktEYMBn29HXYN7PjPhTDgqtcrhc34,6109
-etiket_client/local/types.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/local/model.py,sha256=Ax3Y-R3Mb4UABYrulgR69Q-DJb1TPPZM9SqquYy1kSg,6491
+etiket_client/local/types.py,sha256=n22DPWZx5N1B8U0TW65GNxSXYi3DYx21VB8pe5rnbVA,134
 etiket_client/local/alembic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/local/alembic/env.py,sha256=T4wmyp6pfdNn8qfY6YQpZXLXmXKNz-2TTNmZTNd82xE,2239
 etiket_client/local/alembic/versions/24b0115d4cc7_adding_delete_cache_table.py,sha256=k4hrypvmyJmJhlP5IxgAPoA8yOlGXUZUv7nRdakB6L8,850
 etiket_client/local/alembic/versions/4000a8b9703a_qdrive_v_0_1_0.py,sha256=TTdvTObM3aZO4D7pj2vbuZQZEjrCCAtu-jt90z7MvzU,8187
+etiket_client/local/alembic/versions/4b200763b2ff_fix_datatype.py,sha256=6_PVY1wY0EOOjuvWn9N_sO9v0Ji4S3qxGobnb1i6-oM,2433
 etiket_client/local/alembic/versions/6e8777d1c9f3_etiket_client_v_0_1_1.py,sha256=XJFQrTmJU1ENc7HqBiObuxCF2hxd7tjcI19d15b3RPs,802
 etiket_client/local/alembic/versions/716ce37a1bc1_etiket_client_v_0_1_3.py,sha256=V7RgRWlwb1qeFrSmUAlWUZm7oTA7tD4C7QtVwAlfGAI,3913
 etiket_client/local/alembic/versions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/local/alembic/versions/bec34208dd87_update_uniqueness_of_alt_uuid.py,sha256=Euh5hZw9TfYMG-WlgnLPllKO2PrTx-BYtpLd581MLeo,4611
 etiket_client/local/alembic/versions/c077798e06b9_adding_sync_attr_to_files.py,sha256=ZpyzhYAatiX-IHtoLBIjA1p5C_SVdFZUuPCWcTTiq-Q,1272
 etiket_client/local/alembic/versions/c5d93c68feda_etiket_client_v0_1_5.py,sha256=68MfKSfgLZmKvUWTr3A6xu3Cl8kTYZeaM4sb8SFZ3bE,1289
 etiket_client/local/alembic/versions/c867b432fc6a_convert_time_to_utc.py,sha256=7TDMzA3ToPhpFFFAEgFPvq9D0VFKQygmoSN4NcdmpmI,1812
+etiket_client/local/alembic/versions/f8337520d10d_add_app_register_table.py,sha256=5xeSKapzycd1rJFFzo7eKmFHIbwJ4zBRmjLb39y11pA,1157
 etiket_client/local/alembic/versions/fe8c0d015ba2_update_sync_tables.py,sha256=Dtx0GEgJ0Wrm6r1u_DEXs3HPzdzhLGc7IAeKrv8MMO8,4790
 etiket_client/local/dao/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/local/dao/app.py,sha256=xCmmLhsW2X4DchPldZdjzUcYXnUddOKtZBprWiHVhoU,940
 etiket_client/local/dao/base.py,sha256=UDa-pio52orIrbqkCMBdreAHUjHO5kAofWPKnSRjPuo,2060
-etiket_client/local/dao/dataset.py,sha256=gmOuhjulb_2yan2iT5Wxt-PxCuzFv2chMdDpMrqjM68,10377
+etiket_client/local/dao/dataset.py,sha256=KVkBDjuoBhoPwkqYfoMjU1j8kilRp1n9eoH0KVSA3Rk,10377
 etiket_client/local/dao/file.py,sha256=kuk0N10f8AE5jgpf3Az4L4bbeKQRL21scsrFx4XP8Js,3790
 etiket_client/local/dao/schema.py,sha256=NTqNru47Gjj---3gfNiUs44OB_4b3ACwkG4d_fgFsCo,2153
 etiket_client/local/dao/scope.py,sha256=P_GAplsCy09pfcjxoCLjH54VZPKDZz2O9s3yU7HlD4c,6113
 etiket_client/local/dao/user.py,sha256=PfPROEIc0RQgKGOc4cHQyskA0V2Q0WYxEBqgqjyK-JI,2397
 etiket_client/local/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+etiket_client/local/models/app.py,sha256=s2BlCz3hblRudXPk0SzHq6CxSEt4pPcBNY3p8VO_gbI,486
 etiket_client/local/models/dataset.py,sha256=1mfgBdMWa5dQnKuOKnCQAbBHKiQGeIN-dZUgVCGa-7k,3441
 etiket_client/local/models/file.py,sha256=DtVdRM3AP5ad13AtCmONGnIpSqbgbaDPUPivPa1kycI,2904
 etiket_client/local/models/schema.py,sha256=avkIZgHtuO-N7nkK6RIMvFjmEu7RNiAbfYIbblJeKfM,1427
 etiket_client/local/models/scope.py,sha256=lJPvQlCFjEDz3GQVLAYHFvf0290pb6KqmzyX0iroM2A,1342
 etiket_client/local/models/user.py,sha256=VeFzx4igCtI4r4J2qJFT8aEkz8zFUrlxvp0xXYXQ5P8,900
 etiket_client/local/models/user_base.py,sha256=B8ww8deiv6LKmIwG9MuMLy3AzUq8uO_IkDNw9Vwk57k,1292
 etiket_client/local/models/utility.py,sha256=HAAzudb8weTRswYmaOC7IhwM5pgFXs1noxIVdPit1GU,453
@@ -64,86 +90,89 @@
 etiket_client/python_api/dataset_model/dataset.py,sha256=2I70i8ZvQjoP9aHQ9EfFcAcDllZTQE5HVd188jOv8zc,3280
 etiket_client/python_api/dataset_model/files.py,sha256=UuU64d4S3oe-QS0FqUTlSDtqf_TXiApzwiEpK9PJD2I,11710
 etiket_client/python_api/dataset_model/utility.py,sha256=EvJ5lragZ9EL6BIZPpIsHj2svdXwQ7v-YPZzIIMV0IY,2060
 etiket_client/remote/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/remote/authenticate.py,sha256=zrnxKQCVJk0Pm4TFjsQuH2Os9G8GXkiBqTc5Ma_t6pw,1943
 etiket_client/remote/client.py,sha256=lLILVswIbO1erx5O4G-CXEaLw2ryKUEVcL6Z6DVqMKQ,6517
 etiket_client/remote/endpoints/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-etiket_client/remote/endpoints/dataset.py,sha256=Xak5XhveTVNr_P6O07SAaTggR-tZL2TlxlG-EGavJmI,1467
+etiket_client/remote/endpoints/dataset.py,sha256=nGK3u-mOg_jJhPsOAMKTKs-2iKuWOlAQuzP-6vaVyqA,1745
 etiket_client/remote/endpoints/file.py,sha256=oFmwiHr2vSqJZhyCXBh5_Csi0WHqw2v2AFPhAryI_RQ,2069
 etiket_client/remote/endpoints/schema.py,sha256=FmSaWAi2qPAVGPjhI5Mc3UiLcCiXbe_uiTo-6-X7ECU,664
 etiket_client/remote/endpoints/scope.py,sha256=by_jnt2erITX93LS7mJVeICa8tRw6GNOzDebLjYxkv4,813
 etiket_client/remote/endpoints/user.py,sha256=e6y1-Rirt7EJwdiKb23qCTlgcWaN7YkRn0JWswo7arg,257
-etiket_client/remote/endpoints/version.py,sha256=8p2TL7m5Q21BmATc8Gam-O2D6GVHRjHREQk0XypnSL4,206
+etiket_client/remote/endpoints/user_logs.py,sha256=qNPGkKziPRaosHER3XlXx5FVZGO8cRDDNIfdC9BdXxE,846
+etiket_client/remote/endpoints/version.py,sha256=jd3Rhpds7eyRJutN9nU78t-StT6Y2IudFfU3V7PUTTI,2078
 etiket_client/remote/endpoints/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/remote/endpoints/models/dataset.py,sha256=iFZ1nxeu2xIufhN5dHvkWqRJ7HIWj0eiwMwmbqAZlfI,3035
 etiket_client/remote/endpoints/models/file.py,sha256=AvdDlvDID-_uZpPiM-eqQ2jayNyeebtRYhwFHTUfmPI,2203
 etiket_client/remote/endpoints/models/schema.py,sha256=vGQv3whPmZAhLr8XsTN8GJmXqXQxFrPLeID21lCNAdM,708
 etiket_client/remote/endpoints/models/schema_base.py,sha256=_DTaNc7UVTMjZR5pJyGmX38b50-kYLBT6VZm03NuwQg,1722
 etiket_client/remote/endpoints/models/scope.py,sha256=_xhjEMhaCkNpFi7yQIED8IoCpT79X3ee4SS53p8-cy4,1490
-etiket_client/remote/endpoints/models/types.py,sha256=oWr5XFxLy1h3Wy5CQGV6dXM5m0AXqSis4o201r9H9T4,1375
+etiket_client/remote/endpoints/models/types.py,sha256=aHFf_udPQf6s34rsDZE-oMMAi6JNElkFILvsytmB9P8,1572
 etiket_client/remote/endpoints/models/user.py,sha256=B08By0kNwJcAeFfYVJhevFN46-psZzQM7rNFJ1yx7FQ,1399
 etiket_client/remote/endpoints/models/user_base.py,sha256=RUcNX6F1mfgwiYU6Uqn_-mK2Yo6eWV0WASGtD3Wg96k,1270
+etiket_client/remote/endpoints/models/user_logs.py,sha256=ipAFHyJ3LNv8D2nd09z3tmWUXzPn2DPrPIEPeiOfjJ4,589
 etiket_client/remote/endpoints/models/utility.py,sha256=brmqZipSmFLZXYuwGd1azIeYTVgx-8xNnY6uGPFC0l8,463
+etiket_client/remote/endpoints/models/version.py,sha256=t9nFdmmrnRNjPkp9ZNBQPArqOrXvgaeLZ4DPcLSft8E,1835
 etiket_client/remote/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/remote/tools/file_download.py,sha256=0hVxWsEeW279qJyOwHzn5T8fq8LXcAW2sPxxS1zUb64,2560
 etiket_client/settings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/settings/folders.py,sha256=VbAOmki1agxvoQPS8cjgtBH-RNqFX0lQUTx0g0LAd-A,1289
-etiket_client/settings/logging.py,sha256=JE3fDaRPz6LbeUEpDYvVuAeEmZKtBC0z0dvFrtL4IDA,1639
+etiket_client/settings/logging.py,sha256=yM770yO9v3sI5B2CW6XkNAu-VpdBzT1SuzFcFs7HywY,1722
 etiket_client/settings/saver.py,sha256=5UFg95XEC4UDi8DZJmp_KnizP9VlYBnA3Qaf968RiaE,1647
 etiket_client/settings/schema_settings.py,sha256=jzB6VYV7fJYHYlVKMx_QpObxAZ10x6BPxVrk6x0LOxg,758
 etiket_client/settings/user_settings.py,sha256=Ud_XIJeBT0FLFxY6RMUwLI29HemZOvNcuD0EZVgil6E,691
 etiket_client/sync/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/proc.py,sha256=DwmGblv4thtxLFLgiVSHnw7ywYHHOiMkpGnDW1Nb8_A,3067
-etiket_client/sync/run.py,sha256=uItKplcyT0hTeLk48M5tBnreNgWcn1e3E6-Au4BSpLA,7890
+etiket_client/sync/run.py,sha256=DdR3SVfnuwJ5NEwqLkEl-2Bnh842P59DQc-EH3O3oKo,7988
 etiket_client/sync/backends/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/backends/sources.py,sha256=R-se09PUBJ2BV2OyjrsQkEjFSHgNFxGrYFhxYyCCkoE,1633
 etiket_client/sync/backends/core_tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/backends/core_tools/core_tools_config_class.py,sha256=XN_yCG-K2AKGY1DvdsfqKvwPFJUqmLq4uDLII9Gz5gE,171
-etiket_client/sync/backends/core_tools/core_tools_sync_class.py,sha256=paCl-yEK4u-HyBkYqyB1MCXwk-kQgPGNOo8poo05S14,6899
+etiket_client/sync/backends/core_tools/core_tools_sync_class.py,sha256=veP1GbuGOENDn4p_85sNFFNOngwCeSUfQ4JImC7AHzI,6983
 etiket_client/sync/backends/core_tools/data_getters/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/backends/core_tools/data_getters/get_gates.py,sha256=QXNBAa9KaE4g4WTh5FC65BqXXEdvqYE5EIqhiHozI3o,570
 etiket_client/sync/backends/core_tools/data_getters/get_pulses.py,sha256=Hi7RfH2k7MamJOrVJCPXkq07FBP44suT7sek6ERR5-Q,6693
 etiket_client/sync/backends/core_tools/real_time_sync/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/backends/core_tools/real_time_sync/core_tools_m_param.py,sha256=XGh95z5Og5dj677SAMVlB6ttTm4pfHYyQBtVH1YKJy0,485
-etiket_client/sync/backends/core_tools/real_time_sync/measurement_sync.py,sha256=M020UrZ_313OssF6Soq_NfEe7jPPCN7a94nXUS0YMl0,4730
+etiket_client/sync/backends/core_tools/real_time_sync/measurement_sync.py,sha256=J0bRXyndAjjPl0Z35WhNqrnOIMyEPdNm6ypzVEqIIOk,4939
 etiket_client/sync/backends/core_tools/real_time_sync/qcodes_parameters.py,sha256=9Tpof8jdl49HqCsTAaUCD6mpS2QA2zbsayXpAaXHzsA,8112
 etiket_client/sync/backends/native/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-etiket_client/sync/backends/native/sync_agent.py,sha256=dADgDyjrpsU1DlbbeGScmVZD4vx-cUkc6w8wGnWHkJA,6474
+etiket_client/sync/backends/native/sync_agent.py,sha256=gc6TUYmLvWm0U2UeO3Bze0sYSCeRdr-OUS22cL80hvE,6551
 etiket_client/sync/backends/native/sync_scopes.py,sha256=u1bw8Jk2xYbNBt1zpUi1tPk9mzwlmvQtWkdG1wPem8c,2945
 etiket_client/sync/backends/native/sync_user.py,sha256=9AEcG9SEK--A_bGgEnMuNWLO_Dagjofe7gDU5dBEayw,971
 etiket_client/sync/backends/qcodes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/backends/qcodes/qcodes_config_class.py,sha256=0w7sNNW-TBib8-drNP464smaSUMbLQVhg6IfpkznTXI,129
-etiket_client/sync/backends/qcodes/qcodes_sync_class.py,sha256=ZsCnRxgilmA2u7qn3m4fxoVRa8FBo23QzCr8XD1ov20,5590
-etiket_client/sync/backends/qcodes/real_time_sync.py,sha256=i5Im84Rr3vnktOEYkhRaCyjSJj9usrvhOgXFy4xWd6U,4230
+etiket_client/sync/backends/qcodes/qcodes_sync_class.py,sha256=zLvF0RJkKVcTnJft08j4yVEofpsLTM69Gx1wsI4RfiY,5755
+etiket_client/sync/backends/qcodes/real_time_sync.py,sha256=u2xfMQcQ98NUUy67UMod4OxocUbHuvrlEnc9N-LyNcw,4310
 etiket_client/sync/backends/quantify/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/backends/quantify/quantify_sync_class.py,sha256=5ChlrGB1h80TypRV7cwWojWUjh1fWTpg5n2rbKT5r-A,5617
 etiket_client/sync/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/base/sync_source_abstract.py,sha256=7M9vO5iCOQKyKjNDCozied1It6-DkPE54aE13WKLOPg,1268
-etiket_client/sync/base/sync_utilities.py,sha256=8lpB6Za1VL80aOXI0CtHmoSPcZs6ylYaoyEKc5ExvUk,8848
+etiket_client/sync/base/sync_utilities.py,sha256=jwreoaee7yX4eWdSSX86jcMfH-MsawIHvsAKbxDKHto,9774
 etiket_client/sync/base/checksums/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/base/checksums/any.py,sha256=-usrF4FQr6t_XObFUHzSiyfGaZIB3nr4N51eOEZ1mhM,259
-etiket_client/sync/base/checksums/hdf5.py,sha256=nB0R-7ILqFpOkMNjqONsdaCizlQzHooUxb7Wv6GdvMI,1379
+etiket_client/sync/base/checksums/hdf5.py,sha256=pxK34UrMPdf_l9Kmv02doI3LENAqObeZdr_1u7ivBeM,1502
 etiket_client/sync/database/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/sync/database/dao_scope_mappings.py,sha256=pht7g_I8MufVgdBZydA2eDhqtnhan87dJqvBXXHqqbY,1998
 etiket_client/sync/database/dao_sync_items.py,sha256=MfzB_rPwNqIfocBoewd8R9szObciXkuc6NuzIB0ltyc,8349
 etiket_client/sync/database/dao_sync_sources.py,sha256=fmxa2_bZNwh8ivoEluiRSLO5zBEEuuqrnuGDtkifRIw,1690
-etiket_client/sync/database/models_db.py,sha256=hEQxhi8L1wQVqxNIU9Vp7EorYQHXG9UE7yH6Ff3Wugg,2486
+etiket_client/sync/database/models_db.py,sha256=VSK-r8x2gVMrpcsbrt1qOqZndhqlabBynf8b1sM5DbQ,2485
 etiket_client/sync/database/models_pydantic.py,sha256=8ze8LGqTBeN3GANdChm2mOqmtlzZfUifzVjz323Byg8,2416
 etiket_client/sync/database/start_up.py,sha256=D4OEGlf7yINGIyfiGKyJveBoicudVG6NpO7stFXlniw,563
 etiket_client/sync/database/types.py,sha256=-B1bm4xzPd0Gn2cRV9yNus4FxZQQYNk4VPLvdGkisMw,299
 etiket_client/sync/uploader/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 etiket_client/sync/uploader/file_uploader.py,sha256=55tx1uoRjNCShuwaAHTm4riAfueYGYc-lRUwGm-jQHA,3297
 etiket_client/testing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/testing/test_gui.py,sha256=jcfXkukTqeiPFZ1KeZIwXENNyMkrHOGXTo7oznthNuA,60
 etiket_client/testing/test_live_sync.py,sha256=kCL1O7Qs_gevWZOQyzpXhKGLIOxJEp21WeZ9NGX8Mh0,1174
 etiket_client/testing/live_data_generation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 etiket_client/testing/live_data_generation/core_tools_LD.py,sha256=RnL5ggi0a03AkHRhsUGLigyumWQBP_R-bv9pHOf4358,4907
 etiket_client/testing/live_data_generation/parameters.py,sha256=LPntIRK9Z2CqWmbcGdb-4AbQxhov8driBEOwBqky1uc,12577
 etiket_client/testing/live_data_generation/qcodes_LD.py,sha256=xaQlgRmKX4Ouf8pZxkRLpXecoccKzGLMTCb9DIRY8J0,4766
 etiket_client/testing/live_data_generation/qdrive_LD.py,sha256=OM3txBYXllVFGjeSnqb0yp17lmy0T_2RsbncUyVayKY,6594
-etiket_client-0.2.14.dist-info/LICENCE,sha256=BNXChWe7aLPGR3QkVckAkeLqK2cI2idnmInh-A3YOO0,16695
-etiket_client-0.2.14.dist-info/METADATA,sha256=2nw7wIUVPwGdNtQu_l21w_IMEFzPfkpuD9HEwaVFPzc,1101
-etiket_client-0.2.14.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-etiket_client-0.2.14.dist-info/top_level.txt,sha256=sQ0oXCO6SoO7HAFfJLohl1RDPxH9VbkQaa1Rwnd0kIc,14
-etiket_client-0.2.14.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-etiket_client-0.2.14.dist-info/RECORD,,
+etiket_client-0.2.15.dist-info/LICENCE,sha256=BNXChWe7aLPGR3QkVckAkeLqK2cI2idnmInh-A3YOO0,16695
+etiket_client-0.2.15.dist-info/METADATA,sha256=WmVpfNXX5rs-xbMYR0bHAtIyv5y5iDuZ-gCwppR11Z4,1101
+etiket_client-0.2.15.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+etiket_client-0.2.15.dist-info/top_level.txt,sha256=sQ0oXCO6SoO7HAFfJLohl1RDPxH9VbkQaa1Rwnd0kIc,14
+etiket_client-0.2.15.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+etiket_client-0.2.15.dist-info/RECORD,,
```

