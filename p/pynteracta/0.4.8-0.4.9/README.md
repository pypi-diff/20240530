# Comparing `tmp/pynteracta-0.4.8.tar.gz` & `tmp/pynteracta-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynteracta-0.4.8.tar", max compression
+gzip compressed data, was "pynteracta-0.4.9.tar", max compression
```

## Comparing `pynteracta-0.4.8.tar` & `pynteracta-0.4.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1477 2022-10-14 12:01:15.549467 pynteracta-0.4.8/LICENSE
--rw-r--r--   0        0        0     1080 2023-09-15 07:52:49.852438 pynteracta-0.4.8/README.md
--rw-r--r--   0        0        0     4096 2023-11-03 10:25:21.682189 pynteracta-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       54 2023-11-03 10:25:21.682680 pynteracta-0.4.8/src/pynteracta/__init__.py
--rw-r--r--   0        0        0      318 2023-11-03 10:25:21.683143 pynteracta-0.4.8/src/pynteracta/__main__.py
--rw-r--r--   0        0        0    17507 2023-11-03 10:13:58.018306 pynteracta-0.4.8/src/pynteracta/api.py
--rw-r--r--   0        0        0        0 2023-09-14 10:26:43.090117 pynteracta-0.4.8/src/pynteracta/cli/__init__.py
--rw-r--r--   0        0        0     5789 2023-11-02 14:24:22.762513 pynteracta-0.4.8/src/pynteracta/cli/commands.py
--rw-r--r--   0        0        0     3826 2023-10-16 16:35:29.071727 pynteracta-0.4.8/src/pynteracta/cli/users.py
--rw-r--r--   0        0        0     1991 2023-10-16 15:14:26.081986 pynteracta-0.4.8/src/pynteracta/cli/utils.py
--rw-r--r--   0        0        0     1104 2023-09-25 14:54:29.630871 pynteracta-0.4.8/src/pynteracta/core.py
--rw-r--r--   0        0        0      582 2023-10-16 14:54:09.999959 pynteracta-0.4.8/src/pynteracta/enums.py
--rw-r--r--   0        0        0      503 2023-06-23 11:46:47.344379 pynteracta-0.4.8/src/pynteracta/exceptions.py
--rw-r--r--   0        0        0     1656 2023-09-25 14:51:29.228386 pynteracta-0.4.8/src/pynteracta/models.py
--rw-r--r--   0        0        0        0 2023-02-08 13:17:38.339337 pynteracta-0.4.8/src/pynteracta/schemas/__init__.py
--rw-r--r--   0        0        0     1084 2023-09-22 20:20:30.272856 pynteracta-0.4.8/src/pynteracta/schemas/core.py
--rw-r--r--   0        0        0    20170 2023-10-16 16:00:24.181663 pynteracta-0.4.8/src/pynteracta/schemas/models.py
--rw-r--r--   0        0        0     7420 2023-09-22 20:57:59.204074 pynteracta-0.4.8/src/pynteracta/schemas/requests.py
--rw-r--r--   0        0        0     4002 2023-09-22 20:36:16.351176 pynteracta-0.4.8/src/pynteracta/schemas/responses.py
--rw-r--r--   0        0        0     2749 2023-10-16 14:54:05.835078 pynteracta-0.4.8/src/pynteracta/settings.py
--rw-r--r--   0        0        0      213 2023-06-22 09:19:49.998454 pynteracta-0.4.8/src/pynteracta/urls.py
--rw-r--r--   0        0        0        0 2023-09-25 14:49:45.776334 pynteracta-0.4.8/src/pynteracta/utils/__init__.py
--rw-r--r--   0        0        0     1089 2023-09-25 14:54:02.784377 pynteracta-0.4.8/src/pynteracta/utils/consts.py
--rw-r--r--   0        0        0     3013 2023-10-16 10:01:37.000317 pynteracta-0.4.8/src/pynteracta/utils/models.py
--rw-r--r--   0        0        0        0 2023-10-14 08:19:11.994294 pynteracta-0.4.8/src/pynteracta/utils/stats.py
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 pynteracta-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1477 2023-11-22 11:26:57.649791 pynteracta-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1080 2023-09-15 07:52:49.852438 pynteracta-0.4.9/README.md
+-rw-r--r--   0        0        0     4096 2023-11-23 11:51:10.572906 pynteracta-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-11-23 11:51:10.573330 pynteracta-0.4.9/src/pynteracta/__init__.py
+-rw-r--r--   0        0        0      318 2023-11-23 11:51:10.573707 pynteracta-0.4.9/src/pynteracta/__main__.py
+-rw-r--r--   0        0        0    18457 2023-11-23 11:48:49.729964 pynteracta-0.4.9/src/pynteracta/api.py
+-rw-r--r--   0        0        0        0 2023-09-14 10:26:43.090117 pynteracta-0.4.9/src/pynteracta/cli/__init__.py
+-rw-r--r--   0        0        0     5789 2023-11-02 14:24:22.762513 pynteracta-0.4.9/src/pynteracta/cli/commands.py
+-rw-r--r--   0        0        0     3826 2023-10-16 16:35:29.071727 pynteracta-0.4.9/src/pynteracta/cli/users.py
+-rw-r--r--   0        0        0     1991 2023-10-16 15:14:26.081986 pynteracta-0.4.9/src/pynteracta/cli/utils.py
+-rw-r--r--   0        0        0     1104 2023-09-25 14:54:29.630871 pynteracta-0.4.9/src/pynteracta/core.py
+-rw-r--r--   0        0        0      582 2023-10-16 14:54:09.999959 pynteracta-0.4.9/src/pynteracta/enums.py
+-rw-r--r--   0        0        0      503 2023-06-23 11:46:47.344379 pynteracta-0.4.9/src/pynteracta/exceptions.py
+-rw-r--r--   0        0        0     1656 2023-09-25 14:51:29.228386 pynteracta-0.4.9/src/pynteracta/models.py
+-rw-r--r--   0        0        0        0 2023-02-08 13:17:38.339337 pynteracta-0.4.9/src/pynteracta/schemas/__init__.py
+-rw-r--r--   0        0        0     1084 2023-09-22 20:20:30.272856 pynteracta-0.4.9/src/pynteracta/schemas/core.py
+-rw-r--r--   0        0        0    21065 2023-11-23 10:46:06.476791 pynteracta-0.4.9/src/pynteracta/schemas/models.py
+-rw-r--r--   0        0        0     7544 2023-11-23 08:44:17.160652 pynteracta-0.4.9/src/pynteracta/schemas/requests.py
+-rw-r--r--   0        0        0     4322 2023-11-23 08:48:04.818735 pynteracta-0.4.9/src/pynteracta/schemas/responses.py
+-rw-r--r--   0        0        0     2749 2023-10-16 14:54:05.835078 pynteracta-0.4.9/src/pynteracta/settings.py
+-rw-r--r--   0        0        0      213 2023-06-22 09:19:49.998454 pynteracta-0.4.9/src/pynteracta/urls.py
+-rw-r--r--   0        0        0        0 2023-09-25 14:49:45.776334 pynteracta-0.4.9/src/pynteracta/utils/__init__.py
+-rw-r--r--   0        0        0     1089 2023-09-25 14:54:02.784377 pynteracta-0.4.9/src/pynteracta/utils/consts.py
+-rw-r--r--   0        0        0     3013 2023-10-16 10:01:37.000317 pynteracta-0.4.9/src/pynteracta/utils/models.py
+-rw-r--r--   0        0        0        0 2023-10-14 08:19:11.994294 pynteracta-0.4.9/src/pynteracta/utils/stats.py
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 pynteracta-0.4.9/PKG-INFO
```

### Comparing `pynteracta-0.4.8/LICENSE` & `pynteracta-0.4.9/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022, Simone Dalla
+Copyright (c) 2023, Simone Dalla
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `pynteracta-0.4.8/README.md` & `pynteracta-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/pyproject.toml` & `pynteracta-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynteracta"
-version = "0.4.8"
+version = "0.4.9"
 description = "A wrapper for Interacta API"
 authors = ["Simone Dalla <simodalla@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{ include = "pynteracta", from = "src" }]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -67,15 +67,15 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.4.8"
+current_version = "0.4.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version v{old_version} -> v{new_version}"
 tag_message = "v{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `pynteracta-0.4.8/src/pynteracta/api.py` & `pynteracta-0.4.9/src/pynteracta/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,30 +30,33 @@
 )
 from .schemas.requests import (
     CreateGroupIn,
     CreateUserIn,
     EditGroupIn,
     EditUserIn,
     ExecutePostWorkflowOperationIn,
+    GetPostDefinitionCatalogsIn,
     ListCommunityPostsIn,
     ListGroupMembersIn,
     ListSystemGroupsIn,
     ListSystemUsersIn,
 )
 from .schemas.responses import (
     CreateGroupOut,
     CreateUserOut,
     EditGroupOut,
     EditUserOut,
     ExecutePostWorkflowOperationResponse,
     GetGroupForEditOut,
+    GetPostDefinitionCatalogsOut,
     GetPostDefinitionOut,
     GetUserForEditOut,
     HashtagsOut,
     ListGroupMembersOut,
+    ListPostDefinitionCatalogEntriesOut,
     ListSystemGroupsOut,
     ListSystemUsersElement,
     ListSystemUsersOut,
     PostCreatedOut,
     PostDetailOut,
     PostsOut,
 )
@@ -344,14 +347,33 @@
         return self.call_get(path=path, headers=headers)
 
     @interactapi()
     def list_business_units(self, headers: dict = None) -> Response:
         path = "/admin/data/business-units"
         return self.call_get(path=path, headers=headers)
 
+    @interactapi(schema_out=GetPostDefinitionCatalogsOut)
+    def list_catalogs(
+        self,
+        catalog_ids: set[int],
+        load_entries: bool = False,
+        headers: dict = None,
+    ) -> GetPostDefinitionCatalogsOut | Response:
+        path = "/communication/settings/post-definition/catalogs"
+        params = {"loadEntries": load_entries}
+        data = GetPostDefinitionCatalogsIn(catalog_ids=list(catalog_ids))
+        return self.call_post(path=path, headers=headers, data=data, params=params)
+
+    @interactapi(schema_out=ListPostDefinitionCatalogEntriesOut)
+    def list_catalog_entries(
+        self, catalog_id: int | str, headers: dict = None, data: dict = None
+    ) -> ListPostDefinitionCatalogEntriesOut | Response:
+        path = f"/communication/settings/post-definition/catalogs/{catalog_id}/entries"
+        return self.call_post(path=path, headers=headers, data=data)
+
     ### worflow operations
 
     @interactapi(schema_out=GetPostWorkflowScreenDataForEditResponse)
     def get_post_workflow_screen_data_for_edit(
         self, post_id: int, workflow_operation_id: int | None = None, headers: dict = None
     ) -> GetPostWorkflowScreenDataForEditResponse | Response:
         path = f"/communication/posts/manage/post-workflow-screen-data-for-edit/{post_id}"
@@ -399,16 +421,14 @@
                 f"Multiple post with title '{title}' founded in interacta"
             )
         return posts[0]
 
     def list_all_posts(
         self,
         community_id: str | int,
-        params: dict = None,
-        headers: dict = None,
         data: ListCommunityPostsIn = None,
     ) -> list[BaseListPostsElement]:
         all_posts = []
         page_token = None
         data = data if data else ListCommunityPostsIn()
         while True:
             data.page_token = page_token
@@ -466,15 +486,15 @@
             data = ListSystemUsersIn()
             data.calculate_total_items_count = True
         if email_external_auth_service:
             data.external_auth_service_email_full_text_filter = email_external_auth_service
 
         result = self.list_users(data=data)
 
-        json_data = data.model_dump_json(exclude_unset=True, exclude=["page_size"])
+        json_data = data.model_dump_json(exclude_unset=True, exclude={"page_size"})
         if len(result.items) == 0:
             raise ObjectDoesNotFound(f"User with data '{json_data}' non found in interacta")
         elif len(result.items) > 1:
             raise MultipleObjectsReturned(
                 f"Multiple users with data '{json_data}' founded in interacta"
             )
         return result.items[0]
```

### Comparing `pynteracta-0.4.8/src/pynteracta/cli/commands.py` & `pynteracta-0.4.9/src/pynteracta/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/cli/users.py` & `pynteracta-0.4.9/src/pynteracta/cli/users.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/cli/utils.py` & `pynteracta-0.4.9/src/pynteracta/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/core.py` & `pynteracta-0.4.9/src/pynteracta/core.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/enums.py` & `pynteracta-0.4.9/src/pynteracta/enums.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/models.py` & `pynteracta-0.4.9/src/pynteracta/models.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/schemas/core.py` & `pynteracta-0.4.9/src/pynteracta/schemas/core.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/schemas/models.py` & `pynteracta-0.4.9/src/pynteracta/schemas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from datetime import datetime as type_datetime
 from typing import Any
 
-from pydantic import BaseModel, EmailStr
+from pydantic import BaseModel, ConfigDict, EmailStr
 
 from ..enums import FieldFilterTypeEnum, FieldTypeEnum
 from ..exceptions import ObjectDoesNotFound
 from .core import InteractaModel, InteractaOut
 
 
 class Link(BaseModel):
@@ -357,24 +357,37 @@
     id: int
     label: str | None = None
     external_id: str | None = None
     parent_ids: list[int] | None = None
     deleted: bool | None = None
 
 
+class FieldMetadata(InteractaModel):
+    model_config = ConfigDict(extra="allow")
+
+    catalog_id: int | None = None
+    hierarchical: bool | None = None
+    generic_entity_list_config_id: str | None = None
+    community_id: int | None = None
+
+
 class FieldBase(InteractaModel):
     id: int
     name: str | None = None
     label: str | None = None
     type: FieldTypeEnum | None = None
     required: bool | None = None
     searchable: bool | None = None
     sortable: bool | None = None
     enum_values: list[EnumValue] | None = None
-    metadata: dict | None = None
+    metadata: FieldMetadata | None = None
+
+    @property
+    def catalog_id(self):
+        return self.metadata.catalog_id
 
 
 class FieldDefinition(FieldBase):
     description: str | None = None
     parent_id: int | None = None
     readonly: bool | None = None
     visible_in_preview: bool | None = None
@@ -481,14 +494,18 @@
                 return option.id
         return None
 
     @property
     def custom_fields_ids(self) -> list[int]:
         return [int(field.id) for field in self.field_definitions]
 
+    @property
+    def catalog_ids(self) -> list[int]:
+        return [field.catalog_id for field in self.field_definitions if field.catalog_id]
+
 
 class PostEditableContentData(InteractaModel):
     title: str = ""
     description: str | None = ""
     description_delta: str | None = None
     visibility: int | None = None
     custom_data: dict | None = None
@@ -526,23 +543,42 @@
 class CustomFieldFilter(InteractaModel):
     # CustomFieldFilterDTO
     # Identificativo univoco del campo del post.
     column_id: int | None = None
     # ipo di ricerca [1=EQUAL, 2=INTERVAL, 3=LIKE, 4=IN, 5=CONTAINS, 6=IS_NULL_OR_IN, 7=IS_EMPTY].
     type_id: FieldFilterTypeEnum | None = None
     # Parametri del filtro, ove necessari.
-    parameters: list[Any] = None
+    parameters: list[Any] | None = None
 
 
 class AcknowledgeTaskFilter(InteractaModel):
     # AcknowledgeTaskFilterDTO
     confirmed: bool | None = None
     assigned_to_me: bool | None = None
 
 
+class CatalogEntry(InteractaModel):
+    # CatalogEntryDTO
+    id: int
+    catalog_id: int
+    label: str | None = None
+    external_id: str | None = None
+    parent_ids: list[int] | None = None
+    deleted: bool = False
+
+
+class Catalog(InteractaModel):
+    # CatalogDTO
+    id: int
+    name: str
+    etag: int | None = None
+    paged: bool = False
+    entries: list[CatalogEntry] | None = None
+
+
 # Out Models #######################################################################################
 
 
 class GetCustomPostForEditResponse(InteractaOut):
     # -- GetCustomPostForEditResponseDTO
     content_data: PostEditableContentData | None = None
     occ_token: int
```

### Comparing `pynteracta-0.4.8/src/pynteracta/schemas/requests.py` & `pynteracta-0.4.9/src/pynteracta/schemas/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,7 +210,12 @@
     add_user_ids: list[int] | None = None
     delete_user_ids: list[int] | None = None
 
 
 class EditGroupMembersIn(InteractaModel):
     # creato da rreverse engineering, non supportato da api a settembre 2023
     group_members: list[EditGroupMember] | None = None
+
+
+class GetPostDefinitionCatalogsIn(InteractaModel):
+    # GetPostDefinitionCatalogsRequest
+    catalog_ids: list[int] = []
```

### Comparing `pynteracta-0.4.8/src/pynteracta/schemas/responses.py` & `pynteracta-0.4.9/src/pynteracta/schemas/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pydantic import HttpUrl
 
 from .core import InteractaOut, ItemCreatedEditedOut, PagedItemsOut
 from .models import (
     BaseListPostsElement,
+    Catalog,
+    CatalogEntry,
     Group,
     Hashtag,
     ListSystemGroupsElement,
     ListSystemUsersElement,
     Post,
     PostDefinition,
     PostDetail,
@@ -35,14 +37,19 @@
 
 
 class ListGroupMembersOut(PagedItemsOut):
     # ListGroupMembersResponseDTO
     items: list[User] | None = []
 
 
+class ListPostDefinitionCatalogEntriesOut(PagedItemsOut):
+    # ListPostDefinitionCatalogEntriesResponseDTO
+    items: list[CatalogEntry] | None = []
+
+
 class PostDetailOut(InteractaOut, Post):
     # GetPostDetailResponseDTO
     current_workflow_state: PostWorkflowDefinitionState | None = None
     current_workflow_screen_data: dict | None = None
     mentions: list[User] | None = None
     comment_mentions: ListUsersOut | None = None
     watchers: list[User] | None = None
@@ -131,7 +138,12 @@
     pass
 
 
 class GetGroupForEditOut(InteractaOut, Group):
     # GetGroupForEditResponseDTO
     members: list[User] | None = None
     tags: list[Tag] | None = None
+
+
+class GetPostDefinitionCatalogsOut(InteractaOut):
+    # GetPostDefinitionCatalogsResponseDTO
+    catalogs: list[Catalog] | None = None
```

### Comparing `pynteracta-0.4.8/src/pynteracta/settings.py` & `pynteracta-0.4.9/src/pynteracta/settings.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/utils/consts.py` & `pynteracta-0.4.9/src/pynteracta/utils/consts.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/src/pynteracta/utils/models.py` & `pynteracta-0.4.9/src/pynteracta/utils/models.py`

 * *Files identical despite different names*

### Comparing `pynteracta-0.4.8/PKG-INFO` & `pynteracta-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynteracta
-Version: 0.4.8
+Version: 0.4.9
 Summary: A wrapper for Interacta API
 Home-page: https://github.com/simodalla/pynteracta
 License: BSD-3-Clause
 Author: Simone Dalla
 Author-email: simodalla@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 5 - Production/Stable
```

