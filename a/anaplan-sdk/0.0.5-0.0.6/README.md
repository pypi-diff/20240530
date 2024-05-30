# Comparing `tmp/anaplan_sdk-0.0.5.tar.gz` & `tmp/anaplan_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaplan_sdk-0.0.5.tar", max compression
+gzip compressed data, was "anaplan_sdk-0.0.6.tar", max compression
```

## Comparing `anaplan_sdk-0.0.5.tar` & `anaplan_sdk-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-05-29 17:35:40.232889 anaplan_sdk-0.0.5/LICENSE
--rw-r--r--   0        0        0      792 2024-05-29 17:35:40.232889 anaplan_sdk-0.0.5/README.md
--rw-r--r--   0        0        0      374 2024-05-29 17:35:40.236889 anaplan_sdk-0.0.5/anaplan_sdk/__init__.py
--rw-r--r--   0        0        0    13685 2024-05-29 17:35:40.236889 anaplan_sdk-0.0.5/anaplan_sdk/_async_client.py
--rw-r--r--   0        0        0     4855 2024-05-29 17:35:40.236889 anaplan_sdk-0.0.5/anaplan_sdk/_auth.py
--rw-r--r--   0        0        0    13920 2024-05-29 17:35:40.236889 anaplan_sdk-0.0.5/anaplan_sdk/_client.py
--rw-r--r--   0        0        0     1554 2024-05-29 17:35:40.236889 anaplan_sdk-0.0.5/anaplan_sdk/_exceptions.py
--rw-r--r--   0        0        0     5156 2024-05-29 17:35:40.236889 anaplan_sdk-0.0.5/anaplan_sdk/_models.py
--rw-r--r--   0        0        0     1429 2024-05-29 17:35:40.248889 anaplan_sdk-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 anaplan_sdk-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      391 2024-05-27 09:58:55.018964 anaplan_sdk-0.0.6/anaplan_sdk/__init__.py
+-rw-r--r--   0        0        0    14018 2024-05-29 17:33:09.626616 anaplan_sdk-0.0.6/anaplan_sdk/_async_client.py
+-rw-r--r--   0        0        0     4991 2024-05-29 16:38:22.487967 anaplan_sdk-0.0.6/anaplan_sdk/_auth.py
+-rw-r--r--   0        0        0    14257 2024-05-29 16:27:51.758229 anaplan_sdk-0.0.6/anaplan_sdk/_client.py
+-rw-r--r--   0        0        0     1612 2024-05-29 16:27:14.773666 anaplan_sdk-0.0.6/anaplan_sdk/_exceptions.py
+-rw-r--r--   0        0        0     5369 2024-05-29 14:54:16.478337 anaplan_sdk-0.0.6/anaplan_sdk/_models.py
+-rw-r--r--   0        0        0    11558 2024-05-27 16:31:14.513449 anaplan_sdk-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1503 2024-05-30 06:27:22.853966 anaplan_sdk-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2445 2024-05-30 06:26:29.522998 anaplan_sdk-0.0.6/README.md
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 anaplan_sdk-0.0.6/PKG-INFO
```

### Comparing `anaplan_sdk-0.0.5/LICENSE` & `anaplan_sdk-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `anaplan_sdk-0.0.5/anaplan_sdk/_async_client.py` & `anaplan_sdk-0.0.6/anaplan_sdk/_async_client.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,333 +1,333 @@
-"""
-Asynchronous Client.
-"""
-
-import gzip
-import logging
-import time
-from asyncio import gather
-
-import httpx
-from httpx import HTTPError
-
-from ._auth import AnaplanCertAuth, get_certificate, get_private_key, AnaplanBasicAuth
-from ._exceptions import (
-    AnaplanActionError,
-    raise_appropriate_error,
-)
-from ._models import (
-    Import,
-    Export,
-    Process,
-    File,
-    Action,
-    List,
-    Workspace,
-    Model,
-    to_workspaces,
-    to_models,
-    to_actions,
-    to_imports,
-    to_exports,
-    to_processes,
-    to_files,
-    to_lists,
-    determine_action_type,
-)
-
-logger = logging.getLogger("anaplan_sdk")
-
-
-class AsyncClient:
-    """
-    An asynchronous Client for pythonic access to the Anaplan Integration API v2:
-    https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API, so
-    you can deal with python objects and simple functions rather than implementation details like
-    http, json, compression, chunking etc.
-
-
-    For more information, quick start guides and detailed instructions refer to:
-    https://vinzenzklass.github.io/anaplan-sdk.
-    """
-
-    def __init__(
-        self,
-        workspace_id: str | None = None,
-        model_id: str | None = None,
-        user_email: str | None = None,
-        password: str | None = None,
-        certificate: str | bytes | None = None,
-        private_key: str | bytes | None = None,
-        private_key_password: str | bytes | None = None,
-        timeout: int = 30,
-        status_poll_delay: int = 1,
-        upload_chunk_size: int = 25_000_000,
-    ) -> None:
-        """
-        An asynchronous Client for pythonic access to the Anaplan Integration API v2:
-        https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API,
-        so you can deal with python objects and simple functions rather than implementation details
-        like http, json, compression, chunking etc.
-
-
-        For more information, quick start guides and detailed instructions refer to:
-        https://vinzenzklass.github.io/anaplan-sdk.
-
-        :param workspace_id: The Anaplan workspace Id. You can copy this from the browser URL or
-                             find them using an HTTP Client like Postman, Paw, Insomnia etc.
-        :param model_id: The identifier of the model.
-        :param user_email: A valid email registered with the Anaplan Workspace you are attempting
-                           to access. **The associated user must have Workspace Admin privileges**
-        :param password: Password for the given `user_email`. This is not suitable for production
-                         setups. If you intend to use this in production, acquire a client
-                         certificate as described under: https://help.anaplan.com/procure-ca-certificates-47842267-2cb3-4e38-90bf-13b1632bcd44
-        :param certificate: The absolute path to the client certificate file or the certificate
-                            itself.
-        :param private_key: The absolute path to the private key file or the private key itself.
-        :param private_key_password: The password to access the private key if there is one.
-        :param timeout: The timeout for the HTTP requests.
-        :param status_poll_delay: The delay between polling the status of a task.
-        :param upload_chunk_size: The size of the chunks to upload. This is the maximum size of
-                                  each chunk. Defaults to 25MB.
-        """
-        if not ((user_email and password) or (certificate and private_key)):
-            raise ValueError(
-                "Either `certificate` and `private_key` or `user_email` and `password` must be "
-                "provided."
-            )
-        auth = (
-            AnaplanCertAuth(
-                get_certificate(certificate), get_private_key(private_key, private_key_password)
-            )
-            if certificate
-            else AnaplanBasicAuth(user_email=user_email, password=password)
-        )
-        self._client = httpx.AsyncClient(auth=auth)
-        self._base_url = "https://api.anaplan.com/2/0/workspaces"
-        self.workspace_id = workspace_id
-        self.model_id = model_id
-        self.timeout = timeout
-        self.status_poll_delay = status_poll_delay
-        self.upload_chunk_size = upload_chunk_size
-
-    async def list_workspaces(self) -> list[Workspace]:
-        """
-        Lists all the Workspaces the authenticated user has access to.
-        :return: All Workspaces as a list of :py:class:`Workspace`.
-        """
-        return to_workspaces(await self._get(f"{self._base_url}?tenantDetails=true"))
-
-    async def list_models(self) -> list[Model]:
-        """
-        Lists all the Models the authenticated user has access to.
-        :return: All Models in the Workspace as a list of :py:class:`Model`.
-        """
-        return to_models(
-            await self._get(f"{self._base_url.replace('/workspaces', '/models')}?modelDetails=true")
-        )
-
-    async def list_actions(self) -> list[Action]:
-        """
-        Lists all the Actions in the Model. This will only return the Actions listed under
-        `Other Actions` in Anaplan. For Imports, exports, and processes, see their respective
-        methods instead.
-
-        :return: All Actions on this model as a list of :py:class:`Action`.
-        """
-        return to_actions(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/actions")
-        )
-
-    async def list_imports(self) -> list[Import]:
-        """
-        Lists all the Imports in the Model.
-        :return: All Imports on this model as a list of :py:class:`Import`.
-        """
-        return to_imports(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/imports")
-        )
-
-    async def list_exports(self) -> list[Export]:
-        """
-        Lists all the Exports in the Model.
-        :return: All Exports on this model as a list of :py:class:`Export`.
-        """
-        return to_exports(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/exports")
-        )
-
-    async def list_processes(self) -> list[Process]:
-        """
-        Lists all the Processes in the Model.
-        :return: All Processes on this model as a list of :py:class:`Process`.
-        """
-        return to_processes(
-            await self._get(
-                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/processes"
-            )
-        )
-
-    async def list_files(self) -> list[File]:
-        """
-        Lists all the Files in the Model.
-        :return: All Files on this model as a list of :py:class:`File`.
-        """
-        return to_files(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files")
-        )
-
-    async def list_lists(self) -> list[List]:
-        """
-        Lists all the Lists in the Model.
-        :return: All Lists on this model as a list of :py:class:`List`.
-        """
-        return to_lists(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/lists")
-        )
-
-    async def run_action(self, action_id: int) -> None:
-        """
-        Runs the specified Anaplan Action and validates the spawned task. If the Action fails or
-        completes with errors, will raise an :py:class:`AnaplanActionError`. Failed Tasks are
-        usually not something you can recover from at runtime and often require manual changes in
-        Anaplan, i.e. updating the mapping of an Import or similar. So, for convenience, this will
-        raise an Exception to handle - if you for e.g. think that one of the uploaded chunks may
-        have been dropped and simply retrying with new data may help - and not return the task
-        status information that needs to be handled by the caller.
-
-        If you need more information or control, you can use `invoke_action()` and
-        `get_task_status()`.
-        :param action_id: The identifier of the Action to run. Can be any Anaplan Invokable;
-                          Processes, Imports, Exports, Other Actions.
-        """
-        task_id = await self.invoke_action(action_id)
-        task_status = await self.get_task_status(action_id, task_id)
-
-        while "COMPLETE" not in task_status.get("taskState"):
-            time.sleep(self.status_poll_delay)
-            task_status = await self.get_task_status(action_id, task_id)
-
-        if task_status.get("taskState") == "COMPLETE" and not task_status.get("result").get(
-            "successful"
-        ):
-            raise AnaplanActionError(f"Task '{task_id}' completed with errors.")
-
-    async def get_file(self, file_id: int) -> bytes:
-        """
-        Retrieves the content of the specified file.
-        :param file_id: The identifier of the file to retrieve.
-        :return: The content of the file.
-        """
-        return await self._get_binary(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}"
-        )
-
-    async def upload_file(self, file_id: int, content: str | bytes) -> None:
-        """
-        Uploads the content to the specified file. If `upload_parallel` is set to True on the
-        instance you are invoking this from, will attempt to upload the chunks in parallel for
-        better performance. If you are network bound or are experiencing rate limiting issues, set
-        `upload_parallel` to False.
-
-        :param file_id: The identifier of the file to upload to.
-        :param content: The content to upload. **This Content will be compressed before uploading.
-                        If you are passing the Input as bytes, pass it uncompressed to avoid
-                        redundant work.**
-        """
-        if isinstance(content, str):
-            content = content.encode()
-        chunks = [
-            content[i : i + self.upload_chunk_size]
-            for i in range(0, len(content), self.upload_chunk_size)
-        ]
-        await self._set_chunk_count(file_id, len(chunks))
-        await gather(
-            *[self._upload_chunk(file_id, index, chunk) for index, chunk in enumerate(chunks)]
-        )
-        logger.info(f"Content loaded to  File '{file_id}'.")
-
-    async def get_task_status(
-        self, action_id: int, task_id: str
-    ) -> dict[str, float | int | str | list | dict | bool]:
-        """
-        Retrieves the status of the specified task.
-        :param action_id: The identifier of the action that was invoked.
-        :param task_id: The identifier of the spawned task.
-        :return: The status of the task as returned by the API. For more information
-                 see: https://anaplan.docs.apiary.io.
-        """
-        return (
-            await self._get(
-                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-                f"{determine_action_type(action_id)}/{action_id}/tasks/{task_id}"
-            )
-        ).get("task")
-
-    async def invoke_action(self, action_id: int) -> str:
-        """
-        You may want to consider using `run_action()` instead.
-
-        Invokes the specified Anaplan Action and returns the spawned Task identifier. This is
-        useful if you want to handle the Task status yourself or if you want to run multiple
-        Actions in parallel.
-        :param action_id:
-        :return:
-        """
-        response = await self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-            f"{determine_action_type(action_id)}/{action_id}/tasks",
-            json={"localeName": "en_US"},
-        )
-        task_id = response.get("task").get("taskId")
-        logger.info(f"Invoked Action '{action_id}', spawned Task: '{task_id}'.")
-        return task_id
-
-    async def _upload_chunk(self, file_id: int, index: int, chunk: bytes) -> None:
-        try:
-            response = await self._client.put(
-                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}/"
-                f"chunks/{index}",
-                headers={"Content-Type": "application/x-gzip"},
-                content=gzip.compress(chunk),
-                timeout=self.timeout,
-            )
-            response.raise_for_status()
-        except HTTPError as error:
-            raise_appropriate_error(error)
-
-    async def _set_chunk_count(self, file_id: int, num_chunks: int) -> None:
-        await self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}",
-            json={"chunkCount": num_chunks},
-        )
-
-    async def _get(self, url: str) -> dict[str, float | int | str | list | dict | bool]:
-        try:
-            response = await self._client.get(url, timeout=self.timeout)
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as error:
-            raise_appropriate_error(error)
-
-    async def _get_binary(self, url: str) -> bytes:
-        try:
-            response = await self._client.get(url, timeout=self.timeout)
-            response.raise_for_status()
-            return response.content
-        except HTTPError as error:
-            raise_appropriate_error(error)
-
-    async def _post(
-        self, url: str, json: dict | None = None
-    ) -> dict[str, float | int | str | list | dict | bool]:
-        try:
-            return (
-                await self._client.post(
-                    url,
-                    headers={"Content-Type": "application/json"},
-                    json=json,
-                    timeout=self.timeout,
-                )
-            ).json()
-        except HTTPError as error:
-            raise_appropriate_error(error)
+"""
+Asynchronous Client.
+"""
+
+import gzip
+import logging
+import time
+from asyncio import gather
+
+import httpx
+from httpx import HTTPError
+
+from ._auth import AnaplanCertAuth, get_certificate, get_private_key, AnaplanBasicAuth
+from ._exceptions import (
+    AnaplanActionError,
+    raise_appropriate_error,
+)
+from ._models import (
+    Import,
+    Export,
+    Process,
+    File,
+    Action,
+    List,
+    Workspace,
+    Model,
+    to_workspaces,
+    to_models,
+    to_actions,
+    to_imports,
+    to_exports,
+    to_processes,
+    to_files,
+    to_lists,
+    determine_action_type,
+)
+
+logger = logging.getLogger("anaplan_sdk")
+
+
+class AsyncClient:
+    """
+    An asynchronous Client for pythonic access to the Anaplan Integration API v2:
+    https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API, so
+    you can deal with python objects and simple functions rather than implementation details like
+    http, json, compression, chunking etc.
+
+
+    For more information, quick start guides and detailed instructions refer to:
+    https://vinzenzklass.github.io/anaplan-sdk.
+    """
+
+    def __init__(
+        self,
+        workspace_id: str | None = None,
+        model_id: str | None = None,
+        user_email: str | None = None,
+        password: str | None = None,
+        certificate: str | bytes | None = None,
+        private_key: str | bytes | None = None,
+        private_key_password: str | bytes | None = None,
+        timeout: int = 30,
+        status_poll_delay: int = 1,
+        upload_chunk_size: int = 25_000_000,
+    ) -> None:
+        """
+        An asynchronous Client for pythonic access to the Anaplan Integration API v2:
+        https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API,
+        so you can deal with python objects and simple functions rather than implementation details
+        like http, json, compression, chunking etc.
+
+
+        For more information, quick start guides and detailed instructions refer to:
+        https://vinzenzklass.github.io/anaplan-sdk.
+
+        :param workspace_id: The Anaplan workspace Id. You can copy this from the browser URL or
+                             find them using an HTTP Client like Postman, Paw, Insomnia etc.
+        :param model_id: The identifier of the model.
+        :param user_email: A valid email registered with the Anaplan Workspace you are attempting
+                           to access. **The associated user must have Workspace Admin privileges**
+        :param password: Password for the given `user_email`. This is not suitable for production
+                         setups. If you intend to use this in production, acquire a client
+                         certificate as described under: https://help.anaplan.com/procure-ca-certificates-47842267-2cb3-4e38-90bf-13b1632bcd44
+        :param certificate: The absolute path to the client certificate file or the certificate
+                            itself.
+        :param private_key: The absolute path to the private key file or the private key itself.
+        :param private_key_password: The password to access the private key if there is one.
+        :param timeout: The timeout for the HTTP requests.
+        :param status_poll_delay: The delay between polling the status of a task.
+        :param upload_chunk_size: The size of the chunks to upload. This is the maximum size of
+                                  each chunk. Defaults to 25MB.
+        """
+        if not ((user_email and password) or (certificate and private_key)):
+            raise ValueError(
+                "Either `certificate` and `private_key` or `user_email` and `password` must be "
+                "provided."
+            )
+        auth = (
+            AnaplanCertAuth(
+                get_certificate(certificate), get_private_key(private_key, private_key_password)
+            )
+            if certificate
+            else AnaplanBasicAuth(user_email=user_email, password=password)
+        )
+        self._client = httpx.AsyncClient(auth=auth)
+        self._base_url = "https://api.anaplan.com/2/0/workspaces"
+        self.workspace_id = workspace_id
+        self.model_id = model_id
+        self.timeout = timeout
+        self.status_poll_delay = status_poll_delay
+        self.upload_chunk_size = upload_chunk_size
+
+    async def list_workspaces(self) -> list[Workspace]:
+        """
+        Lists all the Workspaces the authenticated user has access to.
+        :return: All Workspaces as a list of :py:class:`Workspace`.
+        """
+        return to_workspaces(await self._get(f"{self._base_url}?tenantDetails=true"))
+
+    async def list_models(self) -> list[Model]:
+        """
+        Lists all the Models the authenticated user has access to.
+        :return: All Models in the Workspace as a list of :py:class:`Model`.
+        """
+        return to_models(
+            await self._get(f"{self._base_url.replace('/workspaces', '/models')}?modelDetails=true")
+        )
+
+    async def list_actions(self) -> list[Action]:
+        """
+        Lists all the Actions in the Model. This will only return the Actions listed under
+        `Other Actions` in Anaplan. For Imports, exports, and processes, see their respective
+        methods instead.
+
+        :return: All Actions on this model as a list of :py:class:`Action`.
+        """
+        return to_actions(
+            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/actions")
+        )
+
+    async def list_imports(self) -> list[Import]:
+        """
+        Lists all the Imports in the Model.
+        :return: All Imports on this model as a list of :py:class:`Import`.
+        """
+        return to_imports(
+            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/imports")
+        )
+
+    async def list_exports(self) -> list[Export]:
+        """
+        Lists all the Exports in the Model.
+        :return: All Exports on this model as a list of :py:class:`Export`.
+        """
+        return to_exports(
+            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/exports")
+        )
+
+    async def list_processes(self) -> list[Process]:
+        """
+        Lists all the Processes in the Model.
+        :return: All Processes on this model as a list of :py:class:`Process`.
+        """
+        return to_processes(
+            await self._get(
+                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/processes"
+            )
+        )
+
+    async def list_files(self) -> list[File]:
+        """
+        Lists all the Files in the Model.
+        :return: All Files on this model as a list of :py:class:`File`.
+        """
+        return to_files(
+            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files")
+        )
+
+    async def list_lists(self) -> list[List]:
+        """
+        Lists all the Lists in the Model.
+        :return: All Lists on this model as a list of :py:class:`List`.
+        """
+        return to_lists(
+            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/lists")
+        )
+
+    async def run_action(self, action_id: int) -> None:
+        """
+        Runs the specified Anaplan Action and validates the spawned task. If the Action fails or
+        completes with errors, will raise an :py:class:`AnaplanActionError`. Failed Tasks are
+        usually not something you can recover from at runtime and often require manual changes in
+        Anaplan, i.e. updating the mapping of an Import or similar. So, for convenience, this will
+        raise an Exception to handle - if you for e.g. think that one of the uploaded chunks may
+        have been dropped and simply retrying with new data may help - and not return the task
+        status information that needs to be handled by the caller.
+
+        If you need more information or control, you can use `invoke_action()` and
+        `get_task_status()`.
+        :param action_id: The identifier of the Action to run. Can be any Anaplan Invokable;
+                          Processes, Imports, Exports, Other Actions.
+        """
+        task_id = await self.invoke_action(action_id)
+        task_status = await self.get_task_status(action_id, task_id)
+
+        while "COMPLETE" not in task_status.get("taskState"):
+            time.sleep(self.status_poll_delay)
+            task_status = await self.get_task_status(action_id, task_id)
+
+        if task_status.get("taskState") == "COMPLETE" and not task_status.get("result").get(
+            "successful"
+        ):
+            raise AnaplanActionError(f"Task '{task_id}' completed with errors.")
+
+    async def get_file(self, file_id: int) -> bytes:
+        """
+        Retrieves the content of the specified file.
+        :param file_id: The identifier of the file to retrieve.
+        :return: The content of the file.
+        """
+        return await self._get_binary(
+            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}"
+        )
+
+    async def upload_file(self, file_id: int, content: str | bytes) -> None:
+        """
+        Uploads the content to the specified file. If `upload_parallel` is set to True on the
+        instance you are invoking this from, will attempt to upload the chunks in parallel for
+        better performance. If you are network bound or are experiencing rate limiting issues, set
+        `upload_parallel` to False.
+
+        :param file_id: The identifier of the file to upload to.
+        :param content: The content to upload. **This Content will be compressed before uploading.
+                        If you are passing the Input as bytes, pass it uncompressed to avoid
+                        redundant work.**
+        """
+        if isinstance(content, str):
+            content = content.encode()
+        chunks = [
+            content[i : i + self.upload_chunk_size]
+            for i in range(0, len(content), self.upload_chunk_size)
+        ]
+        await self._set_chunk_count(file_id, len(chunks))
+        await gather(
+            *[self._upload_chunk(file_id, index, chunk) for index, chunk in enumerate(chunks)]
+        )
+        logger.info(f"Content loaded to  File '{file_id}'.")
+
+    async def get_task_status(
+        self, action_id: int, task_id: str
+    ) -> dict[str, float | int | str | list | dict | bool]:
+        """
+        Retrieves the status of the specified task.
+        :param action_id: The identifier of the action that was invoked.
+        :param task_id: The identifier of the spawned task.
+        :return: The status of the task as returned by the API. For more information
+                 see: https://anaplan.docs.apiary.io.
+        """
+        return (
+            await self._get(
+                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
+                f"{determine_action_type(action_id)}/{action_id}/tasks/{task_id}"
+            )
+        ).get("task")
+
+    async def invoke_action(self, action_id: int) -> str:
+        """
+        You may want to consider using `run_action()` instead.
+
+        Invokes the specified Anaplan Action and returns the spawned Task identifier. This is
+        useful if you want to handle the Task status yourself or if you want to run multiple
+        Actions in parallel.
+        :param action_id:
+        :return:
+        """
+        response = await self._post(
+            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
+            f"{determine_action_type(action_id)}/{action_id}/tasks",
+            json={"localeName": "en_US"},
+        )
+        task_id = response.get("task").get("taskId")
+        logger.info(f"Invoked Action '{action_id}', spawned Task: '{task_id}'.")
+        return task_id
+
+    async def _upload_chunk(self, file_id: int, index: int, chunk: bytes) -> None:
+        try:
+            response = await self._client.put(
+                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}/"
+                f"chunks/{index}",
+                headers={"Content-Type": "application/x-gzip"},
+                content=gzip.compress(chunk),
+                timeout=self.timeout,
+            )
+            response.raise_for_status()
+        except HTTPError as error:
+            raise_appropriate_error(error)
+
+    async def _set_chunk_count(self, file_id: int, num_chunks: int) -> None:
+        await self._post(
+            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}",
+            json={"chunkCount": num_chunks},
+        )
+
+    async def _get(self, url: str) -> dict[str, float | int | str | list | dict | bool]:
+        try:
+            response = await self._client.get(url, timeout=self.timeout)
+            response.raise_for_status()
+            return response.json()
+        except HTTPError as error:
+            raise_appropriate_error(error)
+
+    async def _get_binary(self, url: str) -> bytes:
+        try:
+            response = await self._client.get(url, timeout=self.timeout)
+            response.raise_for_status()
+            return response.content
+        except HTTPError as error:
+            raise_appropriate_error(error)
+
+    async def _post(
+        self, url: str, json: dict | None = None
+    ) -> dict[str, float | int | str | list | dict | bool]:
+        try:
+            return (
+                await self._client.post(
+                    url,
+                    headers={"Content-Type": "application/json"},
+                    json=json,
+                    timeout=self.timeout,
+                )
+            ).json()
+        except HTTPError as error:
+            raise_appropriate_error(error)
```

### Comparing `anaplan_sdk-0.0.5/anaplan_sdk/_auth.py` & `anaplan_sdk-0.0.6/anaplan_sdk/_auth.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-"""
-Custom Authentication class to pass to httpx alongside some helper functions.
-"""
-
-import base64
-import logging
-import os
-
-import httpx
-from cryptography.exceptions import InvalidKey, UnsupportedAlgorithm
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding
-from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
-
-from ._exceptions import InvalidPrivateKeyException, InvalidCredentialsException
-
-logger = logging.getLogger("anaplan_sdk")
-
-
-class AnaplanBasicAuth(httpx.Auth):
-    requires_response_body = True
-
-    def __init__(
-        self,
-        user_email: str,
-        password: str,
-    ):
-        self.token = "none"
-        self.user_email = user_email
-        self.password = password
-
-    def auth_flow(self, request):
-        request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
-        response = yield request
-        if response.status_code == 401:
-            logger.info("Token expired, refreshing.")
-            response = yield self._basic_auth_request()
-            if "tokenInfo" not in response.json():
-                raise InvalidCredentialsException
-            self.token = response.json().get("tokenInfo").get("tokenValue")
-            request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
-            yield request
-
-    def _basic_auth_request(self):
-        credentials = base64.b64encode(f"{self.user_email}:{self.password}".encode()).decode()
-        return httpx.Request(
-            method="post",
-            url="https://auth.anaplan.com/token/authenticate",
-            headers={"Authorization": f"Basic {credentials}"},
-        )
-
-
-class AnaplanCertAuth(httpx.Auth):
-    requires_response_body = True
-    requires_request_body = True
-
-    def __init__(
-        self,
-        certificate: bytes,
-        private_key: RSAPrivateKey,
-    ):
-        self.token = "none"
-        self.certificate = certificate
-        self.private_key = private_key
-
-    def auth_flow(self, request):
-        request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
-        response = yield request
-        if response.status_code == 401:
-            logger.info("Token expired, refreshing.")
-            response = yield self._cert_auth_request()
-            if "tokenInfo" not in response.json():
-                raise InvalidCredentialsException
-            self.token = response.json().get("tokenInfo").get("tokenValue")
-            request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
-            yield request
-
-    def _cert_auth_request(self):
-        message = os.urandom(150)
-        encoded_cert = base64.b64encode(self.certificate).decode()
-        encoded_string = base64.b64encode(message).decode()
-        encoded_signed_string = base64.b64encode(
-            self.private_key.sign(message, padding.PKCS1v15(), hashes.SHA512())
-        ).decode()
-        return httpx.Request(
-            method="post",
-            url="https://auth.anaplan.com/token/authenticate",
-            headers={
-                "Authorization": f"CACertificate {encoded_cert}",
-                "Content-Type": "application/json",
-            },
-            json={"encodedData": encoded_string, "encodedSignedData": encoded_signed_string},
-        )
-
-
-def get_certificate(certificate: str | bytes) -> bytes:
-    """
-    Get the certificate from a file or string.
-    :param certificate: The certificate to use.
-    :return: The certificate as bytes.
-    """
-    if isinstance(certificate, str):
-        if os.path.isfile(certificate):
-            with open(certificate, "rb") as f:
-                return f.read()
-        return certificate.encode()
-    return certificate
-
-
-def get_private_key(private_key: str | bytes, private_key_password: str | bytes) -> RSAPrivateKey:
-    """
-    Get the private key from a file or string.
-    :param private_key: The private key to use.
-    :param private_key_password: The password for the private key.
-    :return: The private key as an RSAPrivateKey object.
-    """
-    try:
-        if isinstance(private_key, str):
-            if os.path.isfile(private_key):
-                with open(private_key, "rb") as f:
-                    data = f.read()
-            else:
-                data = private_key.encode()
-        else:
-            data = private_key
-
-        password = None
-        if private_key_password:
-            if isinstance(private_key_password, str):
-                password = private_key_password.encode()
-            else:
-                password = private_key_password
-        return serialization.load_pem_private_key(data, password, backend=default_backend())
-    except (IOError, InvalidKey, UnsupportedAlgorithm) as error:
-        raise InvalidPrivateKeyException from error
+"""
+Custom Authentication class to pass to httpx alongside some helper functions.
+"""
+
+import base64
+import logging
+import os
+
+import httpx
+from cryptography.exceptions import InvalidKey, UnsupportedAlgorithm
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
+
+from ._exceptions import InvalidPrivateKeyException, InvalidCredentialsException
+
+logger = logging.getLogger("anaplan_sdk")
+
+
+class AnaplanBasicAuth(httpx.Auth):
+    requires_response_body = True
+
+    def __init__(
+        self,
+        user_email: str,
+        password: str,
+    ):
+        self.token = "none"
+        self.user_email = user_email
+        self.password = password
+
+    def auth_flow(self, request):
+        request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
+        response = yield request
+        if response.status_code == 401:
+            logger.info("Token expired, refreshing.")
+            response = yield self._basic_auth_request()
+            if "tokenInfo" not in response.json():
+                raise InvalidCredentialsException
+            self.token = response.json().get("tokenInfo").get("tokenValue")
+            request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
+            yield request
+
+    def _basic_auth_request(self):
+        credentials = base64.b64encode(f"{self.user_email}:{self.password}".encode()).decode()
+        return httpx.Request(
+            method="post",
+            url="https://auth.anaplan.com/token/authenticate",
+            headers={"Authorization": f"Basic {credentials}"},
+        )
+
+
+class AnaplanCertAuth(httpx.Auth):
+    requires_response_body = True
+    requires_request_body = True
+
+    def __init__(
+        self,
+        certificate: bytes,
+        private_key: RSAPrivateKey,
+    ):
+        self.token = "none"
+        self.certificate = certificate
+        self.private_key = private_key
+
+    def auth_flow(self, request):
+        request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
+        response = yield request
+        if response.status_code == 401:
+            logger.info("Token expired, refreshing.")
+            response = yield self._cert_auth_request()
+            if "tokenInfo" not in response.json():
+                raise InvalidCredentialsException
+            self.token = response.json().get("tokenInfo").get("tokenValue")
+            request.headers["Authorization"] = f"AnaplanAuthToken {self.token}"
+            yield request
+
+    def _cert_auth_request(self):
+        message = os.urandom(150)
+        encoded_cert = base64.b64encode(self.certificate).decode()
+        encoded_string = base64.b64encode(message).decode()
+        encoded_signed_string = base64.b64encode(
+            self.private_key.sign(message, padding.PKCS1v15(), hashes.SHA512())
+        ).decode()
+        return httpx.Request(
+            method="post",
+            url="https://auth.anaplan.com/token/authenticate",
+            headers={
+                "Authorization": f"CACertificate {encoded_cert}",
+                "Content-Type": "application/json",
+            },
+            json={"encodedData": encoded_string, "encodedSignedData": encoded_signed_string},
+        )
+
+
+def get_certificate(certificate: str | bytes) -> bytes:
+    """
+    Get the certificate from a file or string.
+    :param certificate: The certificate to use.
+    :return: The certificate as bytes.
+    """
+    if isinstance(certificate, str):
+        if os.path.isfile(certificate):
+            with open(certificate, "rb") as f:
+                return f.read()
+        return certificate.encode()
+    return certificate
+
+
+def get_private_key(private_key: str | bytes, private_key_password: str | bytes) -> RSAPrivateKey:
+    """
+    Get the private key from a file or string.
+    :param private_key: The private key to use.
+    :param private_key_password: The password for the private key.
+    :return: The private key as an RSAPrivateKey object.
+    """
+    try:
+        if isinstance(private_key, str):
+            if os.path.isfile(private_key):
+                with open(private_key, "rb") as f:
+                    data = f.read()
+            else:
+                data = private_key.encode()
+        else:
+            data = private_key
+
+        password = None
+        if private_key_password:
+            if isinstance(private_key_password, str):
+                password = private_key_password.encode()
+            else:
+                password = private_key_password
+        return serialization.load_pem_private_key(data, password, backend=default_backend())
+    except (IOError, InvalidKey, UnsupportedAlgorithm) as error:
+        raise InvalidPrivateKeyException from error
```

### Comparing `anaplan_sdk-0.0.5/anaplan_sdk/_client.py` & `anaplan_sdk-0.0.6/anaplan_sdk/_client.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,337 +1,337 @@
-"""
-Synchronous Client.
-"""
-
-import gzip
-import logging
-import time
-from concurrent.futures import ThreadPoolExecutor
-
-import httpx
-from httpx import HTTPError
-
-from ._auth import AnaplanBasicAuth, AnaplanCertAuth, get_certificate, get_private_key
-from ._exceptions import (
-    AnaplanActionError,
-    raise_appropriate_error,
-)
-from ._models import (
-    Import,
-    Export,
-    Process,
-    File,
-    Action,
-    List,
-    Workspace,
-    Model,
-    to_workspaces,
-    to_models,
-    to_actions,
-    to_imports,
-    to_exports,
-    to_processes,
-    to_files,
-    to_lists,
-    determine_action_type,
-)
-
-logger = logging.getLogger("anaplan_sdk")
-
-
-class Client:
-    """
-    A synchronous Client for pythonic access to the Anaplan Integration API v2:
-    https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API, so
-    you can deal with python objects and simple functions rather than implementation details like
-    http, json, compression, chunking etc.
-
-
-    For more information, quick start guides and detailed instructions refer to:
-    https://vinzenzklass.github.io/anaplan-sdk.
-    """
-
-    def __init__(
-        self,
-        workspace_id: str | None = None,
-        model_id: str | None = None,
-        user_email: str | None = None,
-        password: str | None = None,
-        certificate: str | bytes | None = None,
-        private_key: str | bytes | None = None,
-        private_key_password: str | bytes | None = None,
-        timeout: int = 30,
-        status_poll_delay: int = 1,
-        upload_parallel: bool = True,
-        upload_chunk_size: int = 25_000_000,
-    ) -> None:
-        """
-        A synchronous Client for pythonic access to the Anaplan Integration API v2:
-        https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API,
-        so you can deal with python objects and simple functions rather than implementation details
-        like http, json, compression, chunking etc.
-
-
-        For more information, quick start guides and detailed instructions refer to:
-        https://vinzenzklass.github.io/anaplan-sdk.
-
-        :param workspace_id: The Anaplan workspace Id. You can copy this from the browser URL or
-                             find them using an HTTP Client like Postman, Paw, Insomnia etc.
-        :param model_id: The identifier of the model.
-        :param user_email: A valid email registered with the Anaplan Workspace you are attempting
-                           to access. **The associated user must have Workspace Admin privileges**
-        :param password: Password for the given `user_email`. This is not suitable for production
-                         setups. If you intend to use this in production, acquire a client
-                         certificate as described under: https://help.anaplan.com/procure-ca-certificates-47842267-2cb3-4e38-90bf-13b1632bcd44
-        :param certificate: The absolute path to the client certificate file or the certificate
-                            itself.
-        :param private_key: The absolute path to the private key file or the private key itself.
-        :param private_key_password: The password to access the private key if there is one.
-        :param timeout: The timeout for the HTTP requests.
-        :param status_poll_delay: The delay between polling the status of a task.
-        :param upload_parallel: Whether to upload the chunks in parallel. Defaults to True. **If
-                                you are heavily network bound or are experiencing rate limiting
-                                issues, set this to False.**
-        :param upload_chunk_size: The size of the chunks to upload. This is the maximum size of
-                                  each chunk. Defaults to 25MB.
-        """
-        if not ((user_email and password) or (certificate and private_key)):
-            raise ValueError(
-                "Either `certificate` and `private_key` or `user_email` and `password` must be "
-                "provided."
-            )
-        auth = (
-            AnaplanCertAuth(
-                get_certificate(certificate), get_private_key(private_key, private_key_password)
-            )
-            if certificate
-            else AnaplanBasicAuth(user_email=user_email, password=password)
-        )
-        self._client = httpx.Client(auth=auth)
-        self._base_url = "https://api.anaplan.com/2/0/workspaces"
-        self.workspace_id = workspace_id
-        self.model_id = model_id
-        self.timeout = timeout
-        self.status_poll_delay = status_poll_delay
-        self.upload_parallel = upload_parallel
-        self.upload_chunk_size = upload_chunk_size
-
-    def list_workspaces(self) -> list[Workspace]:
-        """
-        Lists all the Workspaces the authenticated user has access to.
-        :return: All Workspaces as a list of :py:class:`Workspace`.
-        """
-        return to_workspaces(self._get(f"{self._base_url}?tenantDetails=true"))
-
-    def list_models(self) -> list[Model]:
-        """
-        Lists all the Models the authenticated user has access to.
-        :return: All Models in the Workspace as a list of :py:class:`Model`.
-        """
-        return to_models(
-            self._get(f"{self._base_url.replace('/workspaces', '/models')}?modelDetails=true")
-        )
-
-    def list_actions(self) -> list[Action]:
-        """
-        Lists all the Actions in the Model. This will only return the Actions listed under
-        `Other Actions` in Anaplan. For Imports, exports, and processes, see their respective
-        methods instead.
-
-        :return: All Actions on this model as a list of :py:class:`Action`.
-        """
-        return to_actions(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/actions")
-        )
-
-    def list_imports(self) -> list[Import]:
-        """
-        Lists all the Imports in the Model.
-        :return: All Imports on this model as a list of :py:class:`Import`.
-        """
-        return to_imports(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/imports")
-        )
-
-    def list_exports(self) -> list[Export]:
-        """
-        Lists all the Exports in the Model.
-        :return: All Exports on this model as a list of :py:class:`Export`.
-        """
-        return to_exports(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/exports")
-        )
-
-    def list_processes(self) -> list[Process]:
-        """
-        Lists all the Processes in the Model.
-        :return: All Processes on this model as a list of :py:class:`Process`.
-        """
-        return to_processes(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/processes")
-        )
-
-    def list_files(self) -> list[File]:
-        """
-        Lists all the Files in the Model.
-        :return: All Files on this model as a list of :py:class:`File`.
-        """
-        return to_files(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files")
-        )
-
-    def list_lists(self) -> list[List]:
-        """
-        Lists all the Lists in the Model.
-        :return: All Lists on this model as a list of :py:class:`List`.
-        """
-        return to_lists(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/lists")
-        )
-
-    def run_action(self, action_id: int) -> None:
-        """
-        Runs the specified Anaplan Action and validates the spawned task. If the Action fails or
-        completes with errors, will raise an :py:class:`AnaplanActionError`. Failed Tasks are
-        usually not something you can recover from at runtime and often require manual changes in
-        Anaplan, i.e. updating the mapping of an Import or similar. So, for convenience, this will
-        raise an Exception to handle - if you for e.g. think that one of the uploaded chunks may
-        have been dropped and simply retrying with new data may help - and not return the task
-        status information that needs to be handled by the caller.
-
-        If you need more information or control, you can use `invoke_action()` and
-        `get_task_status()`.
-        :param action_id: The identifier of the Action to run. Can be any Anaplan Invokable;
-                          Processes, Imports, Exports, Other Actions.
-        """
-        task_id = self.invoke_action(action_id)
-        task_status = self.get_task_status(action_id, task_id)
-
-        while "COMPLETE" not in task_status.get("taskState"):
-            time.sleep(self.status_poll_delay)
-            task_status = self.get_task_status(action_id, task_id)
-
-        if task_status.get("taskState") == "COMPLETE" and not task_status.get("result").get(
-            "successful"
-        ):
-            raise AnaplanActionError(f"Task '{task_id}' completed with errors.")
-
-    def get_file(self, file_id: int) -> bytes:
-        """
-        Retrieves the content of the specified file.
-        :param file_id: The identifier of the file to retrieve.
-        :return: The content of the file.
-        """
-        return self._get_binary(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}"
-        )
-
-    def upload_file(self, file_id: int, content: str | bytes) -> None:
-        """
-        Uploads the content to the specified file. If `upload_parallel` is set to True on the
-        instance you are invoking this from, will attempt to upload the chunks in parallel for
-        better performance. If you are network bound or are experiencing rate limiting issues, set
-        `upload_parallel` to False.
-
-        :param file_id: The identifier of the file to upload to.
-        :param content: The content to upload. **This Content will be compressed before uploading.
-                        If you are passing the Input as bytes, pass it uncompressed to avoid
-                        redundant work.**
-        """
-        if isinstance(content, str):
-            content = content.encode()
-        chunks = [
-            content[i : i + self.upload_chunk_size]
-            for i in range(0, len(content), self.upload_chunk_size)
-        ]
-        self._set_chunk_count(file_id, len(chunks))
-        if self.upload_parallel:
-            with ThreadPoolExecutor(max_workers=4) as executor:
-                executor.map(
-                    self._upload_chunk, (file_id,) * len(chunks), range(len(chunks)), chunks
-                )
-        else:
-            for index, chunk in enumerate(chunks):
-                self._upload_chunk(file_id, index, chunk)
-        logger.info(f"Content loaded to  File '{file_id}'.")
-
-    def get_task_status(
-        self, action_id: int, task_id: str
-    ) -> dict[str, float | int | str | list | dict | bool]:
-        """
-        Retrieves the status of the specified task.
-        :param action_id: The identifier of the action that was invoked.
-        :param task_id: The identifier of the spawned task.
-        :return: The status of the task as returned by the API. For more information
-                 see: https://anaplan.docs.apiary.io.
-        """
-        return self._get(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-            f"{determine_action_type(action_id)}/{action_id}/tasks/{task_id}"
-        ).get("task")
-
-    def invoke_action(self, action_id: int) -> str:
-        """
-        You may want to consider using `run_action()` instead.
-
-        Invokes the specified Anaplan Action and returns the spawned Task identifier. This is
-        useful if you want to handle the Task status yourself or if you want to run multiple
-        Actions in parallel.
-        :param action_id:
-        :return:
-        """
-        response = self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-            f"{determine_action_type(action_id)}/{action_id}/tasks",
-            json={"localeName": "en_US"},
-        )
-        task_id = response.get("task").get("taskId")
-        logger.info(f"Invoked Action '{action_id}', spawned Task: '{task_id}'.")
-        return task_id
-
-    def _upload_chunk(self, file_id: int, index: int, chunk: bytes) -> None:
-        try:
-            response = self._client.put(
-                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}/"
-                f"chunks/{index}",
-                headers={"Content-Type": "application/x-gzip"},
-                content=gzip.compress(chunk),
-                timeout=self.timeout,
-            )
-            response.raise_for_status()
-        except HTTPError as error:
-            raise_appropriate_error(error)
-
-    def _set_chunk_count(self, file_id: int, num_chunks: int) -> None:
-        self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}",
-            json={"chunkCount": num_chunks},
-        )
-
-    def _get(self, url: str) -> dict[str, float | int | str | list | dict | bool]:
-        try:
-            response = self._client.get(url, timeout=self.timeout)
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as error:
-            raise_appropriate_error(error)
-
-    def _get_binary(self, url: str) -> bytes:
-        try:
-            response = self._client.get(url, timeout=self.timeout)
-            response.raise_for_status()
-            return response.content
-        except HTTPError as error:
-            raise_appropriate_error(error)
-
-    def _post(
-        self, url: str, json: dict | None = None
-    ) -> dict[str, float | int | str | list | dict | bool]:
-        try:
-            return self._client.post(
-                url,
-                headers={"Content-Type": "application/json"},
-                json=json,
-                timeout=self.timeout,
-            ).json()
-        except HTTPError as error:
-            raise_appropriate_error(error)
+"""
+Synchronous Client.
+"""
+
+import gzip
+import logging
+import time
+from concurrent.futures import ThreadPoolExecutor
+
+import httpx
+from httpx import HTTPError
+
+from ._auth import AnaplanBasicAuth, AnaplanCertAuth, get_certificate, get_private_key
+from ._exceptions import (
+    AnaplanActionError,
+    raise_appropriate_error,
+)
+from ._models import (
+    Import,
+    Export,
+    Process,
+    File,
+    Action,
+    List,
+    Workspace,
+    Model,
+    to_workspaces,
+    to_models,
+    to_actions,
+    to_imports,
+    to_exports,
+    to_processes,
+    to_files,
+    to_lists,
+    determine_action_type,
+)
+
+logger = logging.getLogger("anaplan_sdk")
+
+
+class Client:
+    """
+    A synchronous Client for pythonic access to the Anaplan Integration API v2:
+    https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API, so
+    you can deal with python objects and simple functions rather than implementation details like
+    http, json, compression, chunking etc.
+
+
+    For more information, quick start guides and detailed instructions refer to:
+    https://vinzenzklass.github.io/anaplan-sdk.
+    """
+
+    def __init__(
+        self,
+        workspace_id: str | None = None,
+        model_id: str | None = None,
+        user_email: str | None = None,
+        password: str | None = None,
+        certificate: str | bytes | None = None,
+        private_key: str | bytes | None = None,
+        private_key_password: str | bytes | None = None,
+        timeout: int = 30,
+        status_poll_delay: int = 1,
+        upload_parallel: bool = True,
+        upload_chunk_size: int = 25_000_000,
+    ) -> None:
+        """
+        A synchronous Client for pythonic access to the Anaplan Integration API v2:
+        https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API,
+        so you can deal with python objects and simple functions rather than implementation details
+        like http, json, compression, chunking etc.
+
+
+        For more information, quick start guides and detailed instructions refer to:
+        https://vinzenzklass.github.io/anaplan-sdk.
+
+        :param workspace_id: The Anaplan workspace Id. You can copy this from the browser URL or
+                             find them using an HTTP Client like Postman, Paw, Insomnia etc.
+        :param model_id: The identifier of the model.
+        :param user_email: A valid email registered with the Anaplan Workspace you are attempting
+                           to access. **The associated user must have Workspace Admin privileges**
+        :param password: Password for the given `user_email`. This is not suitable for production
+                         setups. If you intend to use this in production, acquire a client
+                         certificate as described under: https://help.anaplan.com/procure-ca-certificates-47842267-2cb3-4e38-90bf-13b1632bcd44
+        :param certificate: The absolute path to the client certificate file or the certificate
+                            itself.
+        :param private_key: The absolute path to the private key file or the private key itself.
+        :param private_key_password: The password to access the private key if there is one.
+        :param timeout: The timeout for the HTTP requests.
+        :param status_poll_delay: The delay between polling the status of a task.
+        :param upload_parallel: Whether to upload the chunks in parallel. Defaults to True. **If
+                                you are heavily network bound or are experiencing rate limiting
+                                issues, set this to False.**
+        :param upload_chunk_size: The size of the chunks to upload. This is the maximum size of
+                                  each chunk. Defaults to 25MB.
+        """
+        if not ((user_email and password) or (certificate and private_key)):
+            raise ValueError(
+                "Either `certificate` and `private_key` or `user_email` and `password` must be "
+                "provided."
+            )
+        auth = (
+            AnaplanCertAuth(
+                get_certificate(certificate), get_private_key(private_key, private_key_password)
+            )
+            if certificate
+            else AnaplanBasicAuth(user_email=user_email, password=password)
+        )
+        self._client = httpx.Client(auth=auth)
+        self._base_url = "https://api.anaplan.com/2/0/workspaces"
+        self.workspace_id = workspace_id
+        self.model_id = model_id
+        self.timeout = timeout
+        self.status_poll_delay = status_poll_delay
+        self.upload_parallel = upload_parallel
+        self.upload_chunk_size = upload_chunk_size
+
+    def list_workspaces(self) -> list[Workspace]:
+        """
+        Lists all the Workspaces the authenticated user has access to.
+        :return: All Workspaces as a list of :py:class:`Workspace`.
+        """
+        return to_workspaces(self._get(f"{self._base_url}?tenantDetails=true"))
+
+    def list_models(self) -> list[Model]:
+        """
+        Lists all the Models the authenticated user has access to.
+        :return: All Models in the Workspace as a list of :py:class:`Model`.
+        """
+        return to_models(
+            self._get(f"{self._base_url.replace('/workspaces', '/models')}?modelDetails=true")
+        )
+
+    def list_actions(self) -> list[Action]:
+        """
+        Lists all the Actions in the Model. This will only return the Actions listed under
+        `Other Actions` in Anaplan. For Imports, exports, and processes, see their respective
+        methods instead.
+
+        :return: All Actions on this model as a list of :py:class:`Action`.
+        """
+        return to_actions(
+            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/actions")
+        )
+
+    def list_imports(self) -> list[Import]:
+        """
+        Lists all the Imports in the Model.
+        :return: All Imports on this model as a list of :py:class:`Import`.
+        """
+        return to_imports(
+            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/imports")
+        )
+
+    def list_exports(self) -> list[Export]:
+        """
+        Lists all the Exports in the Model.
+        :return: All Exports on this model as a list of :py:class:`Export`.
+        """
+        return to_exports(
+            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/exports")
+        )
+
+    def list_processes(self) -> list[Process]:
+        """
+        Lists all the Processes in the Model.
+        :return: All Processes on this model as a list of :py:class:`Process`.
+        """
+        return to_processes(
+            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/processes")
+        )
+
+    def list_files(self) -> list[File]:
+        """
+        Lists all the Files in the Model.
+        :return: All Files on this model as a list of :py:class:`File`.
+        """
+        return to_files(
+            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files")
+        )
+
+    def list_lists(self) -> list[List]:
+        """
+        Lists all the Lists in the Model.
+        :return: All Lists on this model as a list of :py:class:`List`.
+        """
+        return to_lists(
+            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/lists")
+        )
+
+    def run_action(self, action_id: int) -> None:
+        """
+        Runs the specified Anaplan Action and validates the spawned task. If the Action fails or
+        completes with errors, will raise an :py:class:`AnaplanActionError`. Failed Tasks are
+        usually not something you can recover from at runtime and often require manual changes in
+        Anaplan, i.e. updating the mapping of an Import or similar. So, for convenience, this will
+        raise an Exception to handle - if you for e.g. think that one of the uploaded chunks may
+        have been dropped and simply retrying with new data may help - and not return the task
+        status information that needs to be handled by the caller.
+
+        If you need more information or control, you can use `invoke_action()` and
+        `get_task_status()`.
+        :param action_id: The identifier of the Action to run. Can be any Anaplan Invokable;
+                          Processes, Imports, Exports, Other Actions.
+        """
+        task_id = self.invoke_action(action_id)
+        task_status = self.get_task_status(action_id, task_id)
+
+        while "COMPLETE" not in task_status.get("taskState"):
+            time.sleep(self.status_poll_delay)
+            task_status = self.get_task_status(action_id, task_id)
+
+        if task_status.get("taskState") == "COMPLETE" and not task_status.get("result").get(
+            "successful"
+        ):
+            raise AnaplanActionError(f"Task '{task_id}' completed with errors.")
+
+    def get_file(self, file_id: int) -> bytes:
+        """
+        Retrieves the content of the specified file.
+        :param file_id: The identifier of the file to retrieve.
+        :return: The content of the file.
+        """
+        return self._get_binary(
+            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}"
+        )
+
+    def upload_file(self, file_id: int, content: str | bytes) -> None:
+        """
+        Uploads the content to the specified file. If `upload_parallel` is set to True on the
+        instance you are invoking this from, will attempt to upload the chunks in parallel for
+        better performance. If you are network bound or are experiencing rate limiting issues, set
+        `upload_parallel` to False.
+
+        :param file_id: The identifier of the file to upload to.
+        :param content: The content to upload. **This Content will be compressed before uploading.
+                        If you are passing the Input as bytes, pass it uncompressed to avoid
+                        redundant work.**
+        """
+        if isinstance(content, str):
+            content = content.encode()
+        chunks = [
+            content[i : i + self.upload_chunk_size]
+            for i in range(0, len(content), self.upload_chunk_size)
+        ]
+        self._set_chunk_count(file_id, len(chunks))
+        if self.upload_parallel:
+            with ThreadPoolExecutor(max_workers=4) as executor:
+                executor.map(
+                    self._upload_chunk, (file_id,) * len(chunks), range(len(chunks)), chunks
+                )
+        else:
+            for index, chunk in enumerate(chunks):
+                self._upload_chunk(file_id, index, chunk)
+        logger.info(f"Content loaded to  File '{file_id}'.")
+
+    def get_task_status(
+        self, action_id: int, task_id: str
+    ) -> dict[str, float | int | str | list | dict | bool]:
+        """
+        Retrieves the status of the specified task.
+        :param action_id: The identifier of the action that was invoked.
+        :param task_id: The identifier of the spawned task.
+        :return: The status of the task as returned by the API. For more information
+                 see: https://anaplan.docs.apiary.io.
+        """
+        return self._get(
+            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
+            f"{determine_action_type(action_id)}/{action_id}/tasks/{task_id}"
+        ).get("task")
+
+    def invoke_action(self, action_id: int) -> str:
+        """
+        You may want to consider using `run_action()` instead.
+
+        Invokes the specified Anaplan Action and returns the spawned Task identifier. This is
+        useful if you want to handle the Task status yourself or if you want to run multiple
+        Actions in parallel.
+        :param action_id:
+        :return:
+        """
+        response = self._post(
+            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
+            f"{determine_action_type(action_id)}/{action_id}/tasks",
+            json={"localeName": "en_US"},
+        )
+        task_id = response.get("task").get("taskId")
+        logger.info(f"Invoked Action '{action_id}', spawned Task: '{task_id}'.")
+        return task_id
+
+    def _upload_chunk(self, file_id: int, index: int, chunk: bytes) -> None:
+        try:
+            response = self._client.put(
+                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}/"
+                f"chunks/{index}",
+                headers={"Content-Type": "application/x-gzip"},
+                content=gzip.compress(chunk),
+                timeout=self.timeout,
+            )
+            response.raise_for_status()
+        except HTTPError as error:
+            raise_appropriate_error(error)
+
+    def _set_chunk_count(self, file_id: int, num_chunks: int) -> None:
+        self._post(
+            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}",
+            json={"chunkCount": num_chunks},
+        )
+
+    def _get(self, url: str) -> dict[str, float | int | str | list | dict | bool]:
+        try:
+            response = self._client.get(url, timeout=self.timeout)
+            response.raise_for_status()
+            return response.json()
+        except HTTPError as error:
+            raise_appropriate_error(error)
+
+    def _get_binary(self, url: str) -> bytes:
+        try:
+            response = self._client.get(url, timeout=self.timeout)
+            response.raise_for_status()
+            return response.content
+        except HTTPError as error:
+            raise_appropriate_error(error)
+
+    def _post(
+        self, url: str, json: dict | None = None
+    ) -> dict[str, float | int | str | list | dict | bool]:
+        try:
+            return self._client.post(
+                url,
+                headers={"Content-Type": "application/json"},
+                json=json,
+                timeout=self.timeout,
+            ).json()
+        except HTTPError as error:
+            raise_appropriate_error(error)
```

### Comparing `anaplan_sdk-0.0.5/anaplan_sdk/_exceptions.py` & `anaplan_sdk-0.0.6/anaplan_sdk/_exceptions.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from httpx import HTTPError, HTTPStatusError
-
-
-class AnaplanException(Exception):
-    """
-    Base class for all Anaplan SDK Exceptions.
-    """
-
-    def __init__(self, message: str):
-        self.message = f"\n\n\n{message}\n"
-        super().__init__(self.message)
-
-
-class InvalidCredentialsException(AnaplanException):
-    """
-    Exception raised when the provided credentials are invalid.
-    """
-
-    def __init__(self, message: str = "Invalid credentials."):
-        self.message = message
-        super().__init__(self.message)
-
-
-class InvalidPrivateKeyException(InvalidCredentialsException):
-    """
-    Exception raised when the provided private key is invalid.
-    """
-
-    def __init__(self, message: str = "Invalid private key."):
-        self.message = message
-        super().__init__(self.message)
-
-
-class InvalidIdentifierException(AnaplanException):
-    """
-    Exception raised when the provided identifier is invalid.
-    """
-
-    def __init__(self, message: str = "Invalid identifier."):
-        self.message = message
-        super().__init__(self.message)
-
-
-class AnaplanActionError(AnaplanException):
-    """
-    Exception raised when an Anaplan Action fails.
-    """
-
-    def __init__(self, message: str = "Anaplan completed with errors."):
-        self.message = message
-        super().__init__(self.message)
-
-
-def raise_appropriate_error(error: HTTPError) -> None:
-    if isinstance(error, HTTPStatusError):
-        if error.response.status_code == 404:
-            raise InvalidIdentifierException from error
-    raise error
+from httpx import HTTPError, HTTPStatusError
+
+
+class AnaplanException(Exception):
+    """
+    Base class for all Anaplan SDK Exceptions.
+    """
+
+    def __init__(self, message: str):
+        self.message = f"\n\n\n{message}\n"
+        super().__init__(self.message)
+
+
+class InvalidCredentialsException(AnaplanException):
+    """
+    Exception raised when the provided credentials are invalid.
+    """
+
+    def __init__(self, message: str = "Invalid credentials."):
+        self.message = message
+        super().__init__(self.message)
+
+
+class InvalidPrivateKeyException(InvalidCredentialsException):
+    """
+    Exception raised when the provided private key is invalid.
+    """
+
+    def __init__(self, message: str = "Invalid private key."):
+        self.message = message
+        super().__init__(self.message)
+
+
+class InvalidIdentifierException(AnaplanException):
+    """
+    Exception raised when the provided identifier is invalid.
+    """
+
+    def __init__(self, message: str = "Invalid identifier."):
+        self.message = message
+        super().__init__(self.message)
+
+
+class AnaplanActionError(AnaplanException):
+    """
+    Exception raised when an Anaplan Action fails.
+    """
+
+    def __init__(self, message: str = "Anaplan completed with errors."):
+        self.message = message
+        super().__init__(self.message)
+
+
+def raise_appropriate_error(error: HTTPError) -> None:
+    if isinstance(error, HTTPStatusError):
+        if error.response.status_code == 404:
+            raise InvalidIdentifierException from error
+    raise error
```

### Comparing `anaplan_sdk-0.0.5/pyproject.toml` & `anaplan_sdk-0.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-[tool.poetry]
-name = "anaplan-sdk"
-version = "0.0.5"
-description = "Provides pythonic access to the Anaplan API"
-license = "Apache-2.0"
-authors = ["Vinzenz Klass <vinzenz.klass@ba.valantic.com>"]
-readme = "README.md"
-homepage = "https://vinzenzklass.github.io/anaplan-sdk/"
-repository = "https://github.com/VinzenzKlass/anaplan-sdk"
-documentation = "https://vinzenzklass.github.io/anaplan-sdk/"
-keywords = ["anaplan"]
-
-[tool.poetry.dependencies]
-python = ">=3.10.4"
-httpx = "^0.27.0"
-cryptography = "^42.0.7"
-tenacity = "^8.3.0"
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.4.5"
-pre-commit = "^3.6.1"
-mkdocs-material = "^9.5.25"
-pytest = "^8.2.1"
-pytest-asyncio = "^0.16.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.ruff]
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".git-rewrite",
-    ".hg",
-    ".ipynb_checkpoints",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pyenv",
-    ".pytest_cache",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    ".vscode",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "site-packages",
-    "venv",
-]
-
-line-length = 100
-fix = true
-target-version = "py312"
-
-[tool.ruff.format]
-skip-magic-trailing-comma = false
-
-
-[tool.pytest.ini_options]
-minversion = "8.0"
-addopts = "-ra -q"
-pythonpath = "anaplan_sdk/"
-testpaths = [
-    "tests",
-]
+[tool.poetry]
+name = "anaplan-sdk"
+version = "0.0.6"
+description = "Provides pythonic access to the Anaplan API"
+license = "Apache-2.0"
+authors = ["Vinzenz Klass <vinzenz.klass@ba.valantic.com>"]
+readme = "README.md"
+homepage = "https://vinzenzklass.github.io/anaplan-sdk/"
+repository = "https://github.com/VinzenzKlass/anaplan-sdk"
+documentation = "https://vinzenzklass.github.io/anaplan-sdk/"
+keywords = ["anaplan"]
+
+[tool.poetry.dependencies]
+python = ">=3.10.4"
+httpx = "^0.27.0"
+cryptography = "^42.0.7"
+tenacity = "^8.3.0"
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.4.5"
+pre-commit = "^3.6.1"
+mkdocs-material = "^9.5.25"
+pytest = "^8.2.1"
+pytest-asyncio = "^0.16.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".git-rewrite",
+    ".hg",
+    ".ipynb_checkpoints",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pyenv",
+    ".pytest_cache",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    ".vscode",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "site-packages",
+    "venv",
+]
+
+line-length = 100
+fix = true
+target-version = "py312"
+
+[tool.ruff.format]
+skip-magic-trailing-comma = false
+
+
+[tool.pytest.ini_options]
+minversion = "8.0"
+addopts = "-ra -q"
+pythonpath = "anaplan_sdk/"
+testpaths = [
+    "tests",
+]
```

