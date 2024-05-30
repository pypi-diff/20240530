# Comparing `tmp/privacera_shield-1.1.5-py3-none-any.whl.zip` & `tmp/privacera_shield-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 37234 bytes, number of entries: 20
+Zip file size: 37247 bytes, number of entries: 20
 -rw-r--r--  2.0 unx     1682 b- defN 20-Feb-02 00:00 privacera_shield/PluginAccessRequestEncryptor.py
 -rw-r--r--  2.0 unx       10 b- defN 20-Feb-02 00:00 privacera_shield/__init__.py
--rw-r--r--  2.0 unx    28741 b- defN 20-Feb-02 00:00 privacera_shield/backend.py
+-rw-r--r--  2.0 unx    28813 b- defN 20-Feb-02 00:00 privacera_shield/backend.py
 -rw-r--r--  2.0 unx     5605 b- defN 20-Feb-02 00:00 privacera_shield/client.py
--rw-r--r--  2.0 unx    39974 b- defN 20-Feb-02 00:00 privacera_shield/core.py
+-rw-r--r--  2.0 unx    39994 b- defN 20-Feb-02 00:00 privacera_shield/core.py
 -rw-r--r--  2.0 unx     6927 b- defN 20-Feb-02 00:00 privacera_shield/encryption.py
 -rw-r--r--  2.0 unx      642 b- defN 20-Feb-02 00:00 privacera_shield/exception.py
 -rw-r--r--  2.0 unx     4407 b- defN 20-Feb-02 00:00 privacera_shield/interceptor.py
 -rw-r--r--  2.0 unx      963 b- defN 20-Feb-02 00:00 privacera_shield/interceptor_setup.py
 -rw-r--r--  2.0 unx    14330 b- defN 20-Feb-02 00:00 privacera_shield/langchain_callback.py
 -rw-r--r--  2.0 unx    16229 b- defN 20-Feb-02 00:00 privacera_shield/langchain_method_interceptor.py
 -rw-r--r--  2.0 unx     7277 b- defN 20-Feb-02 00:00 privacera_shield/langchain_streaming_interceptor.py
 -rw-r--r--  2.0 unx     5734 b- defN 20-Feb-02 00:00 privacera_shield/message.py
 -rw-r--r--  2.0 unx     7575 b- defN 20-Feb-02 00:00 privacera_shield/milvus_method_interceptor.py
 -rw-r--r--  2.0 unx      600 b- defN 20-Feb-02 00:00 privacera_shield/model.py
 -rw-r--r--  2.0 unx     2616 b- defN 20-Feb-02 00:00 privacera_shield/util.py
-?rw-r--r--  2.0 unx      888 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx       17 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1785 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/RECORD
-20 files, 146089 bytes uncompressed, 34282 bytes compressed:  76.5%
+?rw-r--r--  2.0 unx      888 b- defN 20-Feb-02 00:00 privacera_shield-1.1.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 privacera_shield-1.1.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx       17 b- defN 20-Feb-02 00:00 privacera_shield-1.1.6.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1785 b- defN 20-Feb-02 00:00 privacera_shield-1.1.6.dist-info/RECORD
+20 files, 146181 bytes uncompressed, 34295 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: privacera_shield/model.py
 Comment: 
 
 Filename: privacera_shield/util.py
 Comment: 
 
-Filename: privacera_shield-1.1.5.dist-info/METADATA
+Filename: privacera_shield-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: privacera_shield-1.1.5.dist-info/WHEEL
+Filename: privacera_shield-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: privacera_shield-1.1.5.dist-info/licenses/LICENSE
+Filename: privacera_shield-1.1.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: privacera_shield-1.1.5.dist-info/RECORD
+Filename: privacera_shield-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## privacera_shield/backend.py

```diff
@@ -540,23 +540,25 @@
                         f"Access response status: {response.status}, access_result: {json.dumps(access_result.__dict__)}")
             return access_result
         else:
             error_message = f"Request failed with status code {response.status}: {response.data}"
             _logger.error(error_message)
             raise Exception(error_message)
 
-    def init_shield_server(self) -> None:
+    def init_shield_server(self, application_key) -> None:
         """
         Initialize shield server for the tenant id.
         """
+
         if _logger.isEnabledFor(logging.DEBUG):
             _logger.debug(f"Initializing shield server for tenant: tenant_id={self.tenant_id}")
 
         request = {"shieldServerKeyId": self.plugin_access_request_encryptor.shield_server_key_id,
-                   "shieldPluginKeyId": self.plugin_access_request_encryptor.shield_plugin_key_id}
+                   "shieldPluginKeyId": self.plugin_access_request_encryptor.shield_plugin_key_id,
+                   "applicationKey": application_key}
 
         error_message = ""
         init_success = False
         response_status = 0
 
         try:
             response = HttpTransport.get_http().request(method="POST",
```

## privacera_shield/core.py

```diff
@@ -488,15 +488,15 @@
             "shield_plugin_private_key": self.shield_plugin_private_key
         }
 
         self.shield_client = ShieldRestHttpClient(base_url=self.shield_base_url, tenant_id=self.tenant_id,
                                                   api_key=self.api_key, encryption_keys_info=encryption_keys_info,
                                                   request_kwargs=kwargs.get("request_kwargs", {}))
 
-        self.shield_client.init_shield_server()
+        self.shield_client.init_shield_server(self.application_key)
 
         self.llm_stream_audit_logger = None
 
         if _logger.isEnabledFor(logging.DEBUG):
             _logger.debug(f"PAIGPlugin initialized with {self.__dict__}")
 
     def get_plugin_app_config(self, kwargs):
```

## Comparing `privacera_shield-1.1.5.dist-info/METADATA` & `privacera_shield-1.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: privacera_shield
-Version: 1.1.5
+Version: 1.1.6
 Summary: Privacera AI Governance (PAIG) Shield Plugin Library
 Project-URL: Homepage, https://github.com/pypa/privacera_shield
 Project-URL: Bug Tracker, https://github.com/pypa/privacera_shield/issues
 Author-email: PAIG Shield <paig@privacera.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.1
 Requires-Dist: cryptography>=41.0.4
-Requires-Dist: privacera-shield-common==1.0.0
+Requires-Dist: privacera-shield-common==1.1.0
 Requires-Dist: urllib3>=2.0.6
 Description-Content-Type: text/markdown
 
 # Privacera AI Goverance Shield Library
 
 The `privacera_shield` library allows you to seamlessly integrate Privacera AI Governance into your Langchain projects.
```

## Comparing `privacera_shield-1.1.5.dist-info/RECORD` & `privacera_shield-1.1.6.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 privacera_shield/PluginAccessRequestEncryptor.py,sha256=vPuctK9G-eulvFLqEK5_-2wE16Y9OXd0iedOiUQyz-w,1682
 privacera_shield/__init__.py,sha256=UnxmjVrk-eNORsitiM48W0pB6yfsaErOak8RYh_ELt8,10
-privacera_shield/backend.py,sha256=FSln0S47zeenigv75-O8xp5uHFVdoGFF1MRnvMpTPo0,28741
+privacera_shield/backend.py,sha256=qgyHHdzxifeQN9tbFXKkwILqK8TB6DPEuJSBHhH6wIA,28813
 privacera_shield/client.py,sha256=7MNwv7xullB9fXV4KV13Vc_hJmJk2EAVpTS94emWzzw,5605
-privacera_shield/core.py,sha256=Aur3FuRlhB7bsUX647rj9sRZlbMBagJHtUETAMRnQyc,39974
+privacera_shield/core.py,sha256=_v-NaCKIUJRkFIYemjT4z0y0I_aRUyAoLcPywLjk8hs,39994
 privacera_shield/encryption.py,sha256=pOW5gLrho9oAqK2Z9Pm6tw59fUDL61e4v_TcSjr2dKE,6927
 privacera_shield/exception.py,sha256=__5EU2XWjig09R3wg8eAde6mFFLex0Zthk_CpKIeq6s,642
 privacera_shield/interceptor.py,sha256=MKYECHkYiyuf8eRbtdJi8NBmR09i-UPFQuVwOoOQVZQ,4407
 privacera_shield/interceptor_setup.py,sha256=hcx7jiNk4wT0c3LngkhVOJtJRRkyXVtdLkeSWDeJMzE,963
 privacera_shield/langchain_callback.py,sha256=7uXyZmyBpS9ifG0pYbRVFW3pMRpD3ZOiWbE9lMtXNTg,14330
 privacera_shield/langchain_method_interceptor.py,sha256=Crohb-qjmKglU4xClWaj3o-mTM5By4THQ2JJRFvbJWU,16229
 privacera_shield/langchain_streaming_interceptor.py,sha256=-YVe8J11X6gopGsnEjN9P-vBBG0AEU5N98fBO2QLvws,7277
 privacera_shield/message.py,sha256=ymFaVHs28MZuHs50AkunbU43PVhV5R2UxwPMiJb4U_s,5734
 privacera_shield/milvus_method_interceptor.py,sha256=E-HoAd_1OwYtfhibqpjet1ZIIakX8kJssPbUaqgXpao,7575
 privacera_shield/model.py,sha256=DYivnpTvFCrTyotnUThN-_VyJwiKleoN6D3_Cddt5ZE,600
 privacera_shield/util.py,sha256=WLsdCnAAQLasvVvXebWoyHDbfgk6fNlTE8ho-NJhTpY,2616
-privacera_shield-1.1.5.dist-info/METADATA,sha256=iTzLKYXgp8cJNtp0QeW8kmV1GrHz9YWRz6XkfQ9e06Q,888
-privacera_shield-1.1.5.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-privacera_shield-1.1.5.dist-info/licenses/LICENSE,sha256=141Y00luDiocNKqpg-owxKfwapO9XSfng11NjgHWAmQ,17
-privacera_shield-1.1.5.dist-info/RECORD,,
+privacera_shield-1.1.6.dist-info/METADATA,sha256=auVSgYKfhivgaBxrLnjKZVKV_q7Ko-rq21viioJb8PI,888
+privacera_shield-1.1.6.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+privacera_shield-1.1.6.dist-info/licenses/LICENSE,sha256=141Y00luDiocNKqpg-owxKfwapO9XSfng11NjgHWAmQ,17
+privacera_shield-1.1.6.dist-info/RECORD,,
```

