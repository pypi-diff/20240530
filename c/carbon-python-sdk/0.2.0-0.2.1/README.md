# Comparing `tmp/carbon_python_sdk-0.2.0.tar.gz` & `tmp/carbon_python_sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon_python_sdk-0.2.0.tar", max compression
+gzip compressed data, was "carbon_python_sdk-0.2.1.tar", max compression
```

## Comparing `carbon_python_sdk-0.2.0.tar` & `carbon_python_sdk-0.2.1.tar`

### file list

```diff
@@ -1,977 +1,981 @@
--rw-r--r--   0        0        0     1081 2024-05-29 00:18:21.457892 carbon_python_sdk-0.2.0/LICENSE
--rw-r--r--   0        0        0   112746 2024-05-29 00:21:37.940324 carbon_python_sdk-0.2.0/README.md
--rw-r--r--   0        0        0      675 2024-05-29 00:21:37.940990 carbon_python_sdk-0.2.0/carbon/__init__.py
--rw-r--r--   0        0        0    76940 2024-05-29 00:21:37.941796 carbon_python_sdk-0.2.0/carbon/api_client.py
--rw-r--r--   0        0        0      663 2024-05-29 00:18:21.317261 carbon_python_sdk-0.2.0/carbon/api_response.py
--rw-r--r--   0        0        0      214 2024-05-29 00:18:21.317350 carbon_python_sdk-0.2.0/carbon/apis/__init__.py
--rw-r--r--   0        0        0    11104 2024-05-29 00:21:37.942975 carbon_python_sdk-0.2.0/carbon/apis/path_to_api.py
--rw-r--r--   0        0        0      233 2024-05-29 00:18:21.318223 carbon_python_sdk-0.2.0/carbon/apis/paths/__init__.py
--rw-r--r--   0        0        0      101 2024-05-29 00:18:21.318317 carbon_python_sdk-0.2.0/carbon/apis/paths/add_webhook.py
--rw-r--r--   0        0        0      114 2024-05-29 00:18:21.318410 carbon_python_sdk-0.2.0/carbon/apis/paths/auth_v1_access_token.py
--rw-r--r--   0        0        0      118 2024-05-29 00:18:21.318496 carbon_python_sdk-0.2.0/carbon/apis/paths/auth_v1_white_labeling.py
--rw-r--r--   0        0        0      119 2024-05-29 00:18:21.318577 carbon_python_sdk-0.2.0/carbon/apis/paths/create_user_file_tags.py
--rw-r--r--   0        0        0      103 2024-05-29 00:18:21.318662 carbon_python_sdk-0.2.0/carbon/apis/paths/delete_files.py
--rw-r--r--   0        0        0      108 2024-05-29 00:18:21.318743 carbon_python_sdk-0.2.0/carbon/apis/paths/delete_files_v2.py
--rw-r--r--   0        0        0      119 2024-05-29 00:18:21.318825 carbon_python_sdk-0.2.0/carbon/apis/paths/delete_user_file_tags.py
--rw-r--r--   0        0        0      103 2024-05-29 00:18:21.318910 carbon_python_sdk-0.2.0/carbon/apis/paths/delete_users.py
--rw-r--r--   0        0        0      133 2024-05-29 00:18:21.319018 carbon_python_sdk-0.2.0/carbon/apis/paths/delete_webhook_webhook_id.py
--rw-r--r--   0        0        0      120 2024-05-29 00:18:21.319125 carbon_python_sdk-0.2.0/carbon/apis/paths/deletefile_file_id.py
--rw-r--r--   0        0        0      100 2024-05-29 00:18:21.319209 carbon_python_sdk-0.2.0/carbon/apis/paths/embeddings.py
--rw-r--r--   0        0        0       96 2024-05-29 00:18:21.319300 carbon_python_sdk-0.2.0/carbon/apis/paths/fetch_urls.py
--rw-r--r--   0        0        0      123 2024-05-29 00:18:21.319386 carbon_python_sdk-0.2.0/carbon/apis/paths/fetch_youtube_transcript.py
--rw-r--r--   0        0        0       89 2024-05-29 00:18:21.319472 carbon_python_sdk-0.2.0/carbon/apis/paths/health.py
--rw-r--r--   0        0        0      134 2024-05-29 00:18:21.319564 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_confluence_list.py
--rw-r--r--   0        0        0      134 2024-05-29 00:18:21.319655 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_confluence_sync.py
--rw-r--r--   0        0        0      119 2024-05-29 00:18:21.319739 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_connect.py
--rw-r--r--   0        0        0      124 2024-05-29 00:18:21.319825 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_files_sync.py
--rw-r--r--   0        0        0      123 2024-05-29 00:18:21.319911 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_freshdesk.py
--rw-r--r--   0        0        0      119 2024-05-29 00:18:21.319998 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_gitbook.py
--rw-r--r--   0        0        0      129 2024-05-29 00:18:21.320094 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_gitbook_spaces.py
--rw-r--r--   0        0        0      128 2024-05-29 00:18:21.320187 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_gitbook_sync.py
--rw-r--r--   0        0        0      117 2024-05-29 00:18:21.320286 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_github.py
--rw-r--r--   0        0        0      125 2024-05-29 00:18:21.320376 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_github_repos.py
--rw-r--r--   0        0        0      137 2024-05-29 00:18:21.320463 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_github_sync_repos.py
--rw-r--r--   0        0        0      124 2024-05-29 00:18:21.320545 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_gmail_sync.py
--rw-r--r--   0        0        0      134 2024-05-29 00:18:21.320633 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_gmail_user_labels.py
--rw-r--r--   0        0        0      124 2024-05-29 00:18:21.320720 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_items_list.py
--rw-r--r--   0        0        0      124 2024-05-29 00:18:21.320808 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_items_sync.py
--rw-r--r--   0        0        0      122 2024-05-29 00:18:21.320895 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_oauth_url.py
--rw-r--r--   0        0        0      128 2024-05-29 00:18:21.320981 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_outlook_sync.py
--rw-r--r--   0        0        0      146 2024-05-29 00:18:21.321071 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_outlook_user_categories.py
--rw-r--r--   0        0        0      140 2024-05-29 00:18:21.321158 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_outlook_user_folders.py
--rw-r--r--   0        0        0      120 2024-05-29 00:18:21.321255 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_rss_feed.py
--rw-r--r--   0        0        0      109 2024-05-29 00:18:21.321341 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_s3.py
--rw-r--r--   0        0        0      120 2024-05-29 00:18:21.321426 carbon_python_sdk-0.2.0/carbon/apis/paths/integrations_s3_files.py
--rw-r--r--   0        0        0      128 2024-05-29 00:18:21.321510 carbon_python_sdk-0.2.0/carbon/apis/paths/modify_user_configuration.py
--rw-r--r--   0        0        0      101 2024-05-29 00:18:21.321592 carbon_python_sdk-0.2.0/carbon/apis/paths/organization.py
--rw-r--r--   0        0        0      125 2024-05-29 00:21:37.943184 carbon_python_sdk-0.2.0/carbon/apis/paths/organization_statistics.py
--rw-r--r--   0        0        0      117 2024-05-29 00:18:21.321761 carbon_python_sdk-0.2.0/carbon/apis/paths/organization_update.py
--rw-r--r--   0        0        0      112 2024-05-29 00:18:21.321851 carbon_python_sdk-0.2.0/carbon/apis/paths/parsed_file_file_id.py
--rw-r--r--   0        0        0      106 2024-05-29 00:18:21.321935 carbon_python_sdk-0.2.0/carbon/apis/paths/process_sitemap.py
--rw-r--r--   0        0        0      106 2024-05-29 00:18:21.322014 carbon_python_sdk-0.2.0/carbon/apis/paths/raw_file_file_id.py
--rw-r--r--   0        0        0      101 2024-05-29 00:18:21.322230 carbon_python_sdk-0.2.0/carbon/apis/paths/resync_file.py
--rw-r--r--   0        0        0      116 2024-05-29 00:18:21.322325 carbon_python_sdk-0.2.0/carbon/apis/paths/revoke_access_token.py
--rw-r--r--   0        0        0      107 2024-05-29 00:18:21.322419 carbon_python_sdk-0.2.0/carbon/apis/paths/scrape_sitemap.py
--rw-r--r--   0        0        0       98 2024-05-29 00:18:21.322502 carbon_python_sdk-0.2.0/carbon/apis/paths/search_urls.py
--rw-r--r--   0        0        0      101 2024-05-29 00:18:21.322582 carbon_python_sdk-0.2.0/carbon/apis/paths/text_chunks.py
--rw-r--r--   0        0        0      103 2024-05-29 00:18:21.322659 carbon_python_sdk-0.2.0/carbon/apis/paths/update_users.py
--rw-r--r--   0        0        0      133 2024-05-29 00:18:21.322746 carbon_python_sdk-0.2.0/carbon/apis/paths/upload_chunks_and_embeddings.py
--rw-r--r--   0        0        0      117 2024-05-29 00:18:21.322833 carbon_python_sdk-0.2.0/carbon/apis/paths/upload_file_from_url.py
--rw-r--r--   0        0        0      101 2024-05-29 00:18:21.322921 carbon_python_sdk-0.2.0/carbon/apis/paths/upload_text.py
--rw-r--r--   0        0        0      100 2024-05-29 00:18:21.323012 carbon_python_sdk-0.2.0/carbon/apis/paths/uploadfile.py
--rw-r--r--   0        0        0       88 2024-05-29 00:18:21.323096 carbon_python_sdk-0.2.0/carbon/apis/paths/user.py
--rw-r--r--   0        0        0      112 2024-05-29 00:18:21.323324 carbon_python_sdk-0.2.0/carbon/apis/paths/user_data_sources.py
--rw-r--r--   0        0        0       99 2024-05-29 00:18:21.323458 carbon_python_sdk-0.2.0/carbon/apis/paths/user_files.py
--rw-r--r--   0        0        0      104 2024-05-29 00:18:21.323556 carbon_python_sdk-0.2.0/carbon/apis/paths/user_files_v2.py
--rw-r--r--   0        0        0       99 2024-05-29 00:18:21.323645 carbon_python_sdk-0.2.0/carbon/apis/paths/web_scrape.py
--rw-r--r--   0        0        0       96 2024-05-29 00:18:21.323738 carbon_python_sdk-0.2.0/carbon/apis/paths/webhooks.py
--rw-r--r--   0        0        0     2044 2024-05-29 00:21:37.943424 carbon_python_sdk-0.2.0/carbon/apis/tag_to_api.py
--rw-r--r--   0        0        0      655 2024-05-29 00:21:37.943742 carbon_python_sdk-0.2.0/carbon/apis/tags/__init__.py
--rw-r--r--   0        0        0      125 2024-05-29 00:18:21.324039 carbon_python_sdk-0.2.0/carbon/apis/tags/auth_api.py
--rw-r--r--   0        0        0      671 2024-05-29 00:18:21.324125 carbon_python_sdk-0.2.0/carbon/apis/tags/auth_api_generated.py
--rw-r--r--   0        0        0      493 2024-05-29 00:18:21.324213 carbon_python_sdk-0.2.0/carbon/apis/tags/auth_api_raw.py
--rw-r--r--   0        0        0      154 2024-05-29 00:18:21.324311 carbon_python_sdk-0.2.0/carbon/apis/tags/data_sources_api.py
--rw-r--r--   0        0        0      717 2024-05-29 00:18:21.324431 carbon_python_sdk-0.2.0/carbon/apis/tags/data_sources_api_generated.py
--rw-r--r--   0        0        0      510 2024-05-29 00:18:21.324544 carbon_python_sdk-0.2.0/carbon/apis/tags/data_sources_api_raw.py
--rw-r--r--   0        0        0      149 2024-05-29 00:18:21.324645 carbon_python_sdk-0.2.0/carbon/apis/tags/embeddings_api.py
--rw-r--r--   0        0        0      806 2024-05-29 00:18:21.324741 carbon_python_sdk-0.2.0/carbon/apis/tags/embeddings_api_generated.py
--rw-r--r--   0        0        0      610 2024-05-29 00:18:21.324827 carbon_python_sdk-0.2.0/carbon/apis/tags/embeddings_api_raw.py
--rw-r--r--   0        0        0      129 2024-05-29 00:18:21.324912 carbon_python_sdk-0.2.0/carbon/apis/tags/files_api.py
--rw-r--r--   0        0        0     1495 2024-05-29 00:18:21.325001 carbon_python_sdk-0.2.0/carbon/apis/tags/files_api_generated.py
--rw-r--r--   0        0        0     1379 2024-05-29 00:18:21.325091 carbon_python_sdk-0.2.0/carbon/apis/tags/files_api_raw.py
--rw-r--r--   0        0        0      133 2024-05-29 00:18:21.325174 carbon_python_sdk-0.2.0/carbon/apis/tags/health_api.py
--rw-r--r--   0        0        0      558 2024-05-29 00:18:21.325260 carbon_python_sdk-0.2.0/carbon/apis/tags/health_api_generated.py
--rw-r--r--   0        0        0      366 2024-05-29 00:18:21.325341 carbon_python_sdk-0.2.0/carbon/apis/tags/health_api_raw.py
--rw-r--r--   0        0        0      157 2024-05-29 00:18:21.325572 carbon_python_sdk-0.2.0/carbon/apis/tags/integrations_api.py
--rw-r--r--   0        0        0     2493 2024-05-29 00:18:21.325667 carbon_python_sdk-0.2.0/carbon/apis/tags/integrations_api_generated.py
--rw-r--r--   0        0        0     2403 2024-05-29 00:18:21.325749 carbon_python_sdk-0.2.0/carbon/apis/tags/integrations_api_raw.py
--rw-r--r--   0        0        0      161 2024-05-29 00:18:21.325832 carbon_python_sdk-0.2.0/carbon/apis/tags/organizations_api.py
--rw-r--r--   0        0        0      747 2024-05-29 00:21:37.943986 carbon_python_sdk-0.2.0/carbon/apis/tags/organizations_api_generated.py
--rw-r--r--   0        0        0      539 2024-05-29 00:21:37.944469 carbon_python_sdk-0.2.0/carbon/apis/tags/organizations_api_raw.py
--rw-r--r--   0        0        0      129 2024-05-29 00:18:21.326637 carbon_python_sdk-0.2.0/carbon/apis/tags/users_api.py
--rw-r--r--   0        0        0      781 2024-05-29 00:18:21.326717 carbon_python_sdk-0.2.0/carbon/apis/tags/users_api_generated.py
--rw-r--r--   0        0        0      611 2024-05-29 00:18:21.326799 carbon_python_sdk-0.2.0/carbon/apis/tags/users_api_raw.py
--rw-r--r--   0        0        0      145 2024-05-29 00:18:21.326883 carbon_python_sdk-0.2.0/carbon/apis/tags/utilities_api.py
--rw-r--r--   0        0        0      984 2024-05-29 00:18:21.326973 carbon_python_sdk-0.2.0/carbon/apis/tags/utilities_api_generated.py
--rw-r--r--   0        0        0      810 2024-05-29 00:18:21.327056 carbon_python_sdk-0.2.0/carbon/apis/tags/utilities_api_raw.py
--rw-r--r--   0        0        0      141 2024-05-29 00:18:21.327139 carbon_python_sdk-0.2.0/carbon/apis/tags/webhooks_api.py
--rw-r--r--   0        0        0      713 2024-05-29 00:18:21.327230 carbon_python_sdk-0.2.0/carbon/apis/tags/webhooks_api_generated.py
--rw-r--r--   0        0        0      525 2024-05-29 00:18:21.327321 carbon_python_sdk-0.2.0/carbon/apis/tags/webhooks_api_raw.py
--rw-r--r--   0        0        0     1986 2024-05-29 00:18:21.327410 carbon_python_sdk-0.2.0/carbon/client.py
--rw-r--r--   0        0        0     1986 2024-05-29 00:18:21.327496 carbon_python_sdk-0.2.0/carbon/client.pyi
--rw-r--r--   0        0        0      676 2024-05-29 00:18:21.327576 carbon_python_sdk-0.2.0/carbon/client_custom.py
--rw-r--r--   0        0        0    17804 2024-05-29 00:21:37.944855 carbon_python_sdk-0.2.0/carbon/configuration.py
--rw-r--r--   0        0        0     7679 2024-05-29 00:18:21.327814 carbon_python_sdk-0.2.0/carbon/exceptions.py
--rw-r--r--   0        0        0     2274 2024-05-29 00:18:21.327900 carbon_python_sdk-0.2.0/carbon/exceptions_base.py
--rw-r--r--   0        0        0      340 2024-05-29 00:18:21.328126 carbon_python_sdk-0.2.0/carbon/model/__init__.py
--rw-r--r--   0        0        0     2282 2024-05-29 00:18:21.328208 carbon_python_sdk-0.2.0/carbon/model/add_webhook_props.py
--rw-r--r--   0        0        0     2282 2024-05-29 00:18:21.328294 carbon_python_sdk-0.2.0/carbon/model/add_webhook_props.pyi
--rw-r--r--   0        0        0     2371 2024-05-29 00:18:21.328389 carbon_python_sdk-0.2.0/carbon/model/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0     2371 2024-05-29 00:18:21.328484 carbon_python_sdk-0.2.0/carbon/model/body_create_upload_file_uploadfile_post.pyi
--rw-r--r--   0        0        0     4752 2024-05-29 00:18:21.328597 carbon_python_sdk-0.2.0/carbon/model/chunk_properties.py
--rw-r--r--   0        0        0     4752 2024-05-29 00:18:21.328736 carbon_python_sdk-0.2.0/carbon/model/chunk_properties.pyi
--rw-r--r--   0        0        0     4359 2024-05-29 00:18:21.328830 carbon_python_sdk-0.2.0/carbon/model/chunk_properties_nullable.py
--rw-r--r--   0        0        0     4359 2024-05-29 00:18:21.328924 carbon_python_sdk-0.2.0/carbon/model/chunk_properties_nullable.pyi
--rw-r--r--   0        0        0     4319 2024-05-29 00:18:21.329043 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings.py
--rw-r--r--   0        0        0     4319 2024-05-29 00:18:21.329158 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings.pyi
--rw-r--r--   0        0        0     1100 2024-05-29 00:18:21.329253 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1100 2024-05-29 00:18:21.329343 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_embedding.pyi
--rw-r--r--   0        0        0     6672 2024-05-29 00:18:21.329445 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     6672 2024-05-29 00:18:21.329542 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input.pyi
--rw-r--r--   0        0        0     1521 2024-05-29 00:18:21.329665 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py
--rw-r--r--   0        0        0     1521 2024-05-29 00:18:21.329770 carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi
--rw-r--r--   0        0        0      548 2024-05-29 00:18:21.329880 carbon_python_sdk-0.2.0/carbon/model/configuration_keys.py
--rw-r--r--   0        0        0      548 2024-05-29 00:18:21.329982 carbon_python_sdk-0.2.0/carbon/model/configuration_keys.pyi
--rw-r--r--   0        0        0     4861 2024-05-29 00:18:21.330077 carbon_python_sdk-0.2.0/carbon/model/confluence_authentication.py
--rw-r--r--   0        0        0     4861 2024-05-29 00:18:21.330294 carbon_python_sdk-0.2.0/carbon/model/confluence_authentication.pyi
--rw-r--r--   0        0        0     6269 2024-05-29 00:18:21.330424 carbon_python_sdk-0.2.0/carbon/model/connect_data_source_input.py
--rw-r--r--   0        0        0     6269 2024-05-29 00:18:21.330530 carbon_python_sdk-0.2.0/carbon/model/connect_data_source_input.pyi
--rw-r--r--   0        0        0     3763 2024-05-29 00:18:21.330633 carbon_python_sdk-0.2.0/carbon/model/connect_data_source_response.py
--rw-r--r--   0        0        0     3763 2024-05-29 00:18:21.330758 carbon_python_sdk-0.2.0/carbon/model/connect_data_source_response.pyi
--rw-r--r--   0        0        0     1369 2024-05-29 00:18:21.330868 carbon_python_sdk-0.2.0/carbon/model/custom_credentials_type.py
--rw-r--r--   0        0        0     1114 2024-05-29 00:18:21.330967 carbon_python_sdk-0.2.0/carbon/model/custom_credentials_type.pyi
--rw-r--r--   0        0        0      554 2024-05-29 00:18:21.331065 carbon_python_sdk-0.2.0/carbon/model/data_source_extended_input.py
--rw-r--r--   0        0        0      554 2024-05-29 00:18:21.331157 carbon_python_sdk-0.2.0/carbon/model/data_source_extended_input.pyi
--rw-r--r--   0        0        0     1183 2024-05-29 00:18:21.331266 carbon_python_sdk-0.2.0/carbon/model/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      998 2024-05-29 00:18:21.331362 carbon_python_sdk-0.2.0/carbon/model/data_source_last_sync_actions.pyi
--rw-r--r--   0        0        0     1256 2024-05-29 00:18:21.331454 carbon_python_sdk-0.2.0/carbon/model/data_source_sync_statuses.py
--rw-r--r--   0        0        0     1033 2024-05-29 00:18:21.331553 carbon_python_sdk-0.2.0/carbon/model/data_source_sync_statuses.pyi
--rw-r--r--   0        0        0     6578 2024-05-29 00:21:37.945354 carbon_python_sdk-0.2.0/carbon/model/data_source_type.py
--rw-r--r--   0        0        0     4915 2024-05-29 00:21:37.946477 carbon_python_sdk-0.2.0/carbon/model/data_source_type.pyi
--rw-r--r--   0        0        0     6953 2024-05-29 00:21:37.946898 carbon_python_sdk-0.2.0/carbon/model/data_source_type_nullable.py
--rw-r--r--   0        0        0     6953 2024-05-29 00:21:37.947214 carbon_python_sdk-0.2.0/carbon/model/data_source_type_nullable.pyi
--rw-r--r--   0        0        0     6047 2024-05-29 00:18:21.332134 carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input.py
--rw-r--r--   0        0        0     6047 2024-05-29 00:18:21.332237 carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input.pyi
--rw-r--r--   0        0        0     1097 2024-05-29 00:18:21.332547 carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0     1097 2024-05-29 00:18:21.332662 carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input_file_ids.pyi
--rw-r--r--   0        0        0     3161 2024-05-29 00:18:21.332760 carbon_python_sdk-0.2.0/carbon/model/delete_files_v2_query_input.py
--rw-r--r--   0        0        0     3161 2024-05-29 00:18:21.332857 carbon_python_sdk-0.2.0/carbon/model/delete_files_v2_query_input.pyi
--rw-r--r--   0        0        0     2600 2024-05-29 00:18:21.332954 carbon_python_sdk-0.2.0/carbon/model/delete_users_input.py
--rw-r--r--   0        0        0     2600 2024-05-29 00:18:21.333051 carbon_python_sdk-0.2.0/carbon/model/delete_users_input.pyi
--rw-r--r--   0        0        0     1199 2024-05-29 00:18:21.333149 carbon_python_sdk-0.2.0/carbon/model/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0     1199 2024-05-29 00:18:21.333241 carbon_python_sdk-0.2.0/carbon/model/delete_users_input_customer_ids.pyi
--rw-r--r--   0        0        0     3902 2024-05-29 00:18:21.333334 carbon_python_sdk-0.2.0/carbon/model/directory_item.py
--rw-r--r--   0        0        0     3902 2024-05-29 00:18:21.333428 carbon_python_sdk-0.2.0/carbon/model/directory_item.pyi
--rw-r--r--   0        0        0    16065 2024-05-29 00:18:21.333528 carbon_python_sdk-0.2.0/carbon/model/document_response.py
--rw-r--r--   0        0        0    16065 2024-05-29 00:18:21.333704 carbon_python_sdk-0.2.0/carbon/model/document_response.pyi
--rw-r--r--   0        0        0     3350 2024-05-29 00:18:21.333859 carbon_python_sdk-0.2.0/carbon/model/document_response_list.py
--rw-r--r--   0        0        0     3350 2024-05-29 00:18:21.333950 carbon_python_sdk-0.2.0/carbon/model/document_response_list.pyi
--rw-r--r--   0        0        0     7489 2024-05-29 00:18:21.334055 carbon_python_sdk-0.2.0/carbon/model/document_response_tags.py
--rw-r--r--   0        0        0     7489 2024-05-29 00:18:21.334154 carbon_python_sdk-0.2.0/carbon/model/document_response_tags.pyi
--rw-r--r--   0        0        0     1088 2024-05-29 00:18:21.334255 carbon_python_sdk-0.2.0/carbon/model/document_response_vector.py
--rw-r--r--   0        0        0     1088 2024-05-29 00:18:21.334355 carbon_python_sdk-0.2.0/carbon/model/document_response_vector.pyi
--rw-r--r--   0        0        0     6594 2024-05-29 00:18:21.334458 carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk.py
--rw-r--r--   0        0        0     6594 2024-05-29 00:18:21.334558 carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk.pyi
--rw-r--r--   0        0        0     1096 2024-05-29 00:18:21.334654 carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0     1096 2024-05-29 00:18:21.334747 carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk_embedding.pyi
--rw-r--r--   0        0        0     3163 2024-05-29 00:18:21.334845 carbon_python_sdk-0.2.0/carbon/model/embedding_generators.py
--rw-r--r--   0        0        0     2260 2024-05-29 00:18:21.334941 carbon_python_sdk-0.2.0/carbon/model/embedding_generators.pyi
--rw-r--r--   0        0        0     3543 2024-05-29 00:18:21.335041 carbon_python_sdk-0.2.0/carbon/model/embedding_generators_nullable.py
--rw-r--r--   0        0        0     3543 2024-05-29 00:18:21.335135 carbon_python_sdk-0.2.0/carbon/model/embedding_generators_nullable.pyi
--rw-r--r--   0        0        0     4307 2024-05-29 00:18:21.335240 carbon_python_sdk-0.2.0/carbon/model/embedding_properties.py
--rw-r--r--   0        0        0     4307 2024-05-29 00:18:21.335341 carbon_python_sdk-0.2.0/carbon/model/embedding_properties.pyi
--rw-r--r--   0        0        0     3267 2024-05-29 00:18:21.335440 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0     3267 2024-05-29 00:18:21.335541 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_filters.pyi
--rw-r--r--   0        0        0     1141 2024-05-29 00:18:21.335637 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0      956 2024-05-29 00:18:21.335739 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_order_by_columns.pyi
--rw-r--r--   0        0        0     5194 2024-05-29 00:18:21.335845 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0     5194 2024-05-29 00:18:21.335950 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_query_input.pyi
--rw-r--r--   0        0        0     3847 2024-05-29 00:18:21.336050 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0     3847 2024-05-29 00:18:21.336449 carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_response.pyi
--rw-r--r--   0        0        0     1944 2024-05-29 00:18:21.336549 carbon_python_sdk-0.2.0/carbon/model/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1503 2024-05-29 00:18:21.336648 carbon_python_sdk-0.2.0/carbon/model/external_file_sync_statuses.pyi
--rw-r--r--   0        0        0    17950 2024-05-29 00:18:21.336763 carbon_python_sdk-0.2.0/carbon/model/external_source_item.py
--rw-r--r--   0        0        0    17950 2024-05-29 00:18:21.336923 carbon_python_sdk-0.2.0/carbon/model/external_source_item.pyi
--rw-r--r--   0        0        0     1102 2024-05-29 00:18:21.337056 carbon_python_sdk-0.2.0/carbon/model/external_source_items_order_by.py
--rw-r--r--   0        0        0      933 2024-05-29 00:18:21.337156 carbon_python_sdk-0.2.0/carbon/model/external_source_items_order_by.pyi
--rw-r--r--   0        0        0     4287 2024-05-29 00:18:21.337259 carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response.py
--rw-r--r--   0        0        0     4287 2024-05-29 00:18:21.337360 carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response.pyi
--rw-r--r--   0        0        0     1187 2024-05-29 00:18:21.337457 carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response_urls.py
--rw-r--r--   0        0        0     1187 2024-05-29 00:18:21.337560 carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response_urls.pyi
--rw-r--r--   0        0        0     1166 2024-05-29 00:21:37.947432 carbon_python_sdk-0.2.0/carbon/model/file_content_types.py
--rw-r--r--   0        0        0      985 2024-05-29 00:21:37.947606 carbon_python_sdk-0.2.0/carbon/model/file_content_types.pyi
--rw-r--r--   0        0        0     1926 2024-05-29 00:21:37.947785 carbon_python_sdk-0.2.0/carbon/model/file_content_types_nullable.py
--rw-r--r--   0        0        0     1926 2024-05-29 00:21:37.947929 carbon_python_sdk-0.2.0/carbon/model/file_content_types_nullable.pyi
--rw-r--r--   0        0        0     5789 2024-05-29 00:21:37.948170 carbon_python_sdk-0.2.0/carbon/model/file_formats.py
--rw-r--r--   0        0        0     4344 2024-05-29 00:21:37.948468 carbon_python_sdk-0.2.0/carbon/model/file_formats.pyi
--rw-r--r--   0        0        0     6161 2024-05-29 00:21:37.948727 carbon_python_sdk-0.2.0/carbon/model/file_formats_nullable.py
--rw-r--r--   0        0        0     6161 2024-05-29 00:21:37.948868 carbon_python_sdk-0.2.0/carbon/model/file_formats_nullable.pyi
--rw-r--r--   0        0        0     8647 2024-05-29 00:18:21.338420 carbon_python_sdk-0.2.0/carbon/model/file_statistics.py
--rw-r--r--   0        0        0     8647 2024-05-29 00:18:21.338683 carbon_python_sdk-0.2.0/carbon/model/file_statistics.pyi
--rw-r--r--   0        0        0     8000 2024-05-29 00:18:21.339016 carbon_python_sdk-0.2.0/carbon/model/file_statistics_nullable.py
--rw-r--r--   0        0        0     8000 2024-05-29 00:18:21.339117 carbon_python_sdk-0.2.0/carbon/model/file_statistics_nullable.pyi
--rw-r--r--   0        0        0     4847 2024-05-29 00:18:21.339213 carbon_python_sdk-0.2.0/carbon/model/file_sync_config.py
--rw-r--r--   0        0        0     4847 2024-05-29 00:18:21.339306 carbon_python_sdk-0.2.0/carbon/model/file_sync_config.pyi
--rw-r--r--   0        0        0     5047 2024-05-29 00:18:21.339408 carbon_python_sdk-0.2.0/carbon/model/file_sync_config_nullable.py
--rw-r--r--   0        0        0     5047 2024-05-29 00:18:21.339505 carbon_python_sdk-0.2.0/carbon/model/file_sync_config_nullable.pyi
--rw-r--r--   0        0        0     1283 2024-05-29 00:18:21.339620 carbon_python_sdk-0.2.0/carbon/model/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     1283 2024-05-29 00:18:21.339724 carbon_python_sdk-0.2.0/carbon/model/files_query_user_files_deprecated_response.pyi
--rw-r--r--   0        0        0    15514 2024-05-29 00:18:21.339823 carbon_python_sdk-0.2.0/carbon/model/fresh_desk_connect_request.py
--rw-r--r--   0        0        0    15514 2024-05-29 00:18:21.339975 carbon_python_sdk-0.2.0/carbon/model/fresh_desk_connect_request.pyi
--rw-r--r--   0        0        0     3529 2024-05-29 00:18:21.340114 carbon_python_sdk-0.2.0/carbon/model/freskdesk_authentication.py
--rw-r--r--   0        0        0     3529 2024-05-29 00:18:21.340207 carbon_python_sdk-0.2.0/carbon/model/freskdesk_authentication.pyi
--rw-r--r--   0        0        0     2362 2024-05-29 00:18:21.340302 carbon_python_sdk-0.2.0/carbon/model/generic_success_response.py
--rw-r--r--   0        0        0     2362 2024-05-29 00:18:21.340405 carbon_python_sdk-0.2.0/carbon/model/generic_success_response.pyi
--rw-r--r--   0        0        0    15782 2024-05-29 00:18:21.340505 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body.py
--rw-r--r--   0        0        0    15631 2024-05-29 00:18:21.340652 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body.pyi
--rw-r--r--   0        0        0     1159 2024-05-29 00:18:21.340796 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0     1159 2024-05-29 00:18:21.340889 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_file_ids.pyi
--rw-r--r--   0        0        0     1264 2024-05-29 00:18:21.340976 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0     1264 2024-05-29 00:18:21.341067 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_parent_file_ids.pyi
--rw-r--r--   0        0        0     1377 2024-05-29 00:18:21.341161 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0     1377 2024-05-29 00:18:21.341251 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_query_vector.pyi
--rw-r--r--   0        0        0     6490 2024-05-29 00:18:21.341349 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0     6490 2024-05-29 00:18:21.341443 carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_tags.pyi
--rw-r--r--   0        0        0     3779 2024-05-29 00:18:21.341534 carbon_python_sdk-0.2.0/carbon/model/gitbook_authetication.py
--rw-r--r--   0        0        0     3779 2024-05-29 00:18:21.341623 carbon_python_sdk-0.2.0/carbon/model/gitbook_authetication.pyi
--rw-r--r--   0        0        0    14852 2024-05-29 00:18:21.341716 carbon_python_sdk-0.2.0/carbon/model/gitbook_connect_request.py
--rw-r--r--   0        0        0    14852 2024-05-29 00:18:21.341868 carbon_python_sdk-0.2.0/carbon/model/gitbook_connect_request.pyi
--rw-r--r--   0        0        0    13012 2024-05-29 00:18:21.342015 carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request.py
--rw-r--r--   0        0        0    13012 2024-05-29 00:18:21.342172 carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request.pyi
--rw-r--r--   0        0        0     1220 2024-05-29 00:18:21.342324 carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0     1197 2024-05-29 00:18:21.342421 carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request_space_ids.pyi
--rw-r--r--   0        0        0     3635 2024-05-29 00:18:21.342510 carbon_python_sdk-0.2.0/carbon/model/github_authentication.py
--rw-r--r--   0        0        0     3635 2024-05-29 00:18:21.342610 carbon_python_sdk-0.2.0/carbon/model/github_authentication.pyi
--rw-r--r--   0        0        0     3626 2024-05-29 00:18:21.342709 carbon_python_sdk-0.2.0/carbon/model/github_connect_request.py
--rw-r--r--   0        0        0     3626 2024-05-29 00:18:21.342808 carbon_python_sdk-0.2.0/carbon/model/github_connect_request.pyi
--rw-r--r--   0        0        0     3792 2024-05-29 00:18:21.342912 carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request.py
--rw-r--r--   0        0        0     3792 2024-05-29 00:18:21.343021 carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request.pyi
--rw-r--r--   0        0        0     1246 2024-05-29 00:18:21.343127 carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request_repos.py
--rw-r--r--   0        0        0     1201 2024-05-29 00:18:21.343229 carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request_repos.pyi
--rw-r--r--   0        0        0    16085 2024-05-29 00:18:21.343336 carbon_python_sdk-0.2.0/carbon/model/gmail_sync_input.py
--rw-r--r--   0        0        0    16085 2024-05-29 00:18:21.343494 carbon_python_sdk-0.2.0/carbon/model/gmail_sync_input.pyi
--rw-r--r--   0        0        0      963 2024-05-29 00:18:21.343655 carbon_python_sdk-0.2.0/carbon/model/helpdesk_file_types.py
--rw-r--r--   0        0        0      834 2024-05-29 00:18:21.343762 carbon_python_sdk-0.2.0/carbon/model/helpdesk_file_types.pyi
--rw-r--r--   0        0        0     3251 2024-05-29 00:18:21.343863 carbon_python_sdk-0.2.0/carbon/model/http_validation_error.py
--rw-r--r--   0        0        0     3251 2024-05-29 00:18:21.344078 carbon_python_sdk-0.2.0/carbon/model/http_validation_error.pyi
--rw-r--r--   0        0        0     2974 2024-05-29 00:18:21.344186 carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0     2974 2024-05-29 00:18:21.344283 carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params.pyi
--rw-r--r--   0        0        0     2907 2024-05-29 00:18:21.344395 carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0     2907 2024-05-29 00:18:21.344500 carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params_nullable.pyi
--rw-r--r--   0        0        0     6323 2024-05-29 00:18:21.344610 carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_request.py
--rw-r--r--   0        0        0     6323 2024-05-29 00:18:21.344715 carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_request.pyi
--rw-r--r--   0        0        0     3820 2024-05-29 00:18:21.344819 carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_response.py
--rw-r--r--   0        0        0     3820 2024-05-29 00:18:21.344923 carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_response.pyi
--rw-r--r--   0        0        0     5498 2024-05-29 00:18:21.345021 carbon_python_sdk-0.2.0/carbon/model/list_items_filters.py
--rw-r--r--   0        0        0     5498 2024-05-29 00:18:21.345126 carbon_python_sdk-0.2.0/carbon/model/list_items_filters.pyi
--rw-r--r--   0        0        0     1095 2024-05-29 00:18:21.345228 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_external_ids.py
--rw-r--r--   0        0        0     1095 2024-05-29 00:18:21.345326 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_external_ids.pyi
--rw-r--r--   0        0        0     1079 2024-05-29 00:18:21.345422 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_ids.py
--rw-r--r--   0        0        0     1079 2024-05-29 00:18:21.345518 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_ids.pyi
--rw-r--r--   0        0        0     5708 2024-05-29 00:18:21.345626 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable.py
--rw-r--r--   0        0        0     5708 2024-05-29 00:18:21.345739 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable.pyi
--rw-r--r--   0        0        0     1111 2024-05-29 00:18:21.345834 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_external_ids.py
--rw-r--r--   0        0        0     1111 2024-05-29 00:18:21.345941 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_external_ids.pyi
--rw-r--r--   0        0        0     1095 2024-05-29 00:18:21.346041 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_ids.py
--rw-r--r--   0        0        0     1095 2024-05-29 00:18:21.346142 carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_ids.pyi
--rw-r--r--   0        0        0     3613 2024-05-29 00:18:21.346355 carbon_python_sdk-0.2.0/carbon/model/list_request.py
--rw-r--r--   0        0        0     3613 2024-05-29 00:18:21.346448 carbon_python_sdk-0.2.0/carbon/model/list_request.pyi
--rw-r--r--   0        0        0     3228 2024-05-29 00:18:21.346544 carbon_python_sdk-0.2.0/carbon/model/list_response.py
--rw-r--r--   0        0        0     3228 2024-05-29 00:18:21.346636 carbon_python_sdk-0.2.0/carbon/model/list_response.pyi
--rw-r--r--   0        0        0     3129 2024-05-29 00:18:21.346732 carbon_python_sdk-0.2.0/carbon/model/modify_user_configuration_input.py
--rw-r--r--   0        0        0     3129 2024-05-29 00:18:21.346833 carbon_python_sdk-0.2.0/carbon/model/modify_user_configuration_input.pyi
--rw-r--r--   0        0        0     3699 2024-05-29 00:18:21.346931 carbon_python_sdk-0.2.0/carbon/model/notion_authentication.py
--rw-r--r--   0        0        0     3699 2024-05-29 00:18:21.347030 carbon_python_sdk-0.2.0/carbon/model/notion_authentication.pyi
--rw-r--r--   0        0        0     4300 2024-05-29 00:18:21.347127 carbon_python_sdk-0.2.0/carbon/model/o_auth_authentication.py
--rw-r--r--   0        0        0     4300 2024-05-29 00:18:21.347222 carbon_python_sdk-0.2.0/carbon/model/o_auth_authentication.pyi
--rw-r--r--   0        0        0    29598 2024-05-29 00:18:21.347339 carbon_python_sdk-0.2.0/carbon/model/o_auth_url_request.py
--rw-r--r--   0        0        0    29598 2024-05-29 00:18:21.347501 carbon_python_sdk-0.2.0/carbon/model/o_auth_url_request.pyi
--rw-r--r--   0        0        0      930 2024-05-29 00:18:21.347626 carbon_python_sdk-0.2.0/carbon/model/order_dir.py
--rw-r--r--   0        0        0      813 2024-05-29 00:18:21.347720 carbon_python_sdk-0.2.0/carbon/model/order_dir.pyi
--rw-r--r--   0        0        0      932 2024-05-29 00:18:21.347847 carbon_python_sdk-0.2.0/carbon/model/order_dir_v2.py
--rw-r--r--   0        0        0      815 2024-05-29 00:18:21.347967 carbon_python_sdk-0.2.0/carbon/model/order_dir_v2.pyi
--rw-r--r--   0        0        0    18921 2024-05-29 00:21:37.949670 carbon_python_sdk-0.2.0/carbon/model/organization_response.py
--rw-r--r--   0        0        0    18921 2024-05-29 00:21:37.949975 carbon_python_sdk-0.2.0/carbon/model/organization_response.pyi
--rw-r--r--   0        0        0    17065 2024-05-29 00:18:21.348378 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_api.py
--rw-r--r--   0        0        0    17065 2024-05-29 00:18:21.348523 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_api.pyi
--rw-r--r--   0        0        0     4467 2024-05-29 00:18:21.348663 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters.py
--rw-r--r--   0        0        0     4467 2024-05-29 00:18:21.348770 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters.pyi
--rw-r--r--   0        0        0     1113 2024-05-29 00:18:21.348875 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0     1113 2024-05-29 00:18:21.348976 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters_ids.pyi
--rw-r--r--   0        0        0     1014 2024-05-29 00:18:21.349084 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0      871 2024-05-29 00:18:21.349185 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_order_by_columns.pyi
--rw-r--r--   0        0        0     4657 2024-05-29 00:18:21.349293 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0     4657 2024-05-29 00:18:21.349400 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_query_input.pyi
--rw-r--r--   0        0        0     3947 2024-05-29 00:18:21.349506 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_response.py
--rw-r--r--   0        0        0     3947 2024-05-29 00:18:21.349613 carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_response.pyi
--rw-r--r--   0        0        0     3408 2024-05-29 00:18:21.349715 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create.py
--rw-r--r--   0        0        0     3408 2024-05-29 00:18:21.349814 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create.pyi
--rw-r--r--   0        0        0     6330 2024-05-29 00:18:21.349914 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0     6330 2024-05-29 00:18:21.350020 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create_tags.pyi
--rw-r--r--   0        0        0     3418 2024-05-29 00:18:21.350120 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0     3418 2024-05-29 00:18:21.350220 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove.pyi
--rw-r--r--   0        0        0     1213 2024-05-29 00:18:21.350313 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     1213 2024-05-29 00:18:21.350416 carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove_tags.pyi
--rw-r--r--   0        0        0    21692 2024-05-29 00:18:21.350526 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0    21692 2024-05-29 00:18:21.350665 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters.pyi
--rw-r--r--   0        0        0     1238 2024-05-29 00:18:21.350948 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0     1238 2024-05-29 00:18:21.351067 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi
--rw-r--r--   0        0        0     1186 2024-05-29 00:18:21.351189 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0     1186 2024-05-29 00:18:21.351298 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_ids.pyi
--rw-r--r--   0        0        0     1296 2024-05-29 00:18:21.351406 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0     1296 2024-05-29 00:18:21.351510 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi
--rw-r--r--   0        0        0     1135 2024-05-29 00:18:21.351739 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0     1135 2024-05-29 00:18:21.351829 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi
--rw-r--r--   0        0        0     1216 2024-05-29 00:18:21.351925 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_request_ids.py
--rw-r--r--   0        0        0     1192 2024-05-29 00:18:21.352019 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi
--rw-r--r--   0        0        0     6420 2024-05-29 00:18:21.352128 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0     6420 2024-05-29 00:18:21.352227 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_tags.pyi
--rw-r--r--   0        0        0     1469 2024-05-29 00:18:21.352322 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1198 2024-05-29 00:18:21.352544 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_order_by_types.pyi
--rw-r--r--   0        0        0     8629 2024-05-29 00:18:21.352675 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0     8629 2024-05-29 00:18:21.353113 carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_query_input.pyi
--rw-r--r--   0        0        0     2378 2024-05-29 00:18:21.353805 carbon_python_sdk-0.2.0/carbon/model/outh_url_response.py
--rw-r--r--   0        0        0     2378 2024-05-29 00:18:21.353895 carbon_python_sdk-0.2.0/carbon/model/outh_url_response.pyi
--rw-r--r--   0        0        0    17193 2024-05-29 00:18:21.353993 carbon_python_sdk-0.2.0/carbon/model/outlook_sync_input.py
--rw-r--r--   0        0        0    17193 2024-05-29 00:18:21.354111 carbon_python_sdk-0.2.0/carbon/model/outlook_sync_input.pyi
--rw-r--r--   0        0        0     2807 2024-05-29 00:18:21.354229 carbon_python_sdk-0.2.0/carbon/model/pagination.py
--rw-r--r--   0        0        0     2807 2024-05-29 00:18:21.354326 carbon_python_sdk-0.2.0/carbon/model/pagination.pyi
--rw-r--r--   0        0        0     2452 2024-05-29 00:18:21.354426 carbon_python_sdk-0.2.0/carbon/model/presigned_url_response.py
--rw-r--r--   0        0        0     2452 2024-05-29 00:18:21.354629 carbon_python_sdk-0.2.0/carbon/model/presigned_url_response.pyi
--rw-r--r--   0        0        0    10223 2024-05-29 00:18:21.354738 carbon_python_sdk-0.2.0/carbon/model/raw_text_input.py
--rw-r--r--   0        0        0    10151 2024-05-29 00:18:21.354863 carbon_python_sdk-0.2.0/carbon/model/raw_text_input.pyi
--rw-r--r--   0        0        0     5578 2024-05-29 00:18:21.354994 carbon_python_sdk-0.2.0/carbon/model/resync_file_query_input.py
--rw-r--r--   0        0        0     5578 2024-05-29 00:18:21.355093 carbon_python_sdk-0.2.0/carbon/model/resync_file_query_input.pyi
--rw-r--r--   0        0        0     2489 2024-05-29 00:18:21.355178 carbon_python_sdk-0.2.0/carbon/model/revoke_access_token_input.py
--rw-r--r--   0        0        0     2489 2024-05-29 00:18:21.355260 carbon_python_sdk-0.2.0/carbon/model/revoke_access_token_input.pyi
--rw-r--r--   0        0        0    12076 2024-05-29 00:18:21.355341 carbon_python_sdk-0.2.0/carbon/model/rss_feed_input.py
--rw-r--r--   0        0        0    12076 2024-05-29 00:18:21.355458 carbon_python_sdk-0.2.0/carbon/model/rss_feed_input.pyi
--rw-r--r--   0        0        0     3724 2024-05-29 00:18:21.355589 carbon_python_sdk-0.2.0/carbon/model/s3_auth_request.py
--rw-r--r--   0        0        0     3724 2024-05-29 00:18:21.355690 carbon_python_sdk-0.2.0/carbon/model/s3_auth_request.pyi
--rw-r--r--   0        0        0     3739 2024-05-29 00:18:21.355784 carbon_python_sdk-0.2.0/carbon/model/s3_authentication.py
--rw-r--r--   0        0        0     3739 2024-05-29 00:18:21.355885 carbon_python_sdk-0.2.0/carbon/model/s3_authentication.pyi
--rw-r--r--   0        0        0    19565 2024-05-29 00:18:21.355990 carbon_python_sdk-0.2.0/carbon/model/s3_file_sync_input.py
--rw-r--r--   0        0        0    19565 2024-05-29 00:18:21.356115 carbon_python_sdk-0.2.0/carbon/model/s3_file_sync_input.pyi
--rw-r--r--   0        0        0     3936 2024-05-29 00:18:21.356346 carbon_python_sdk-0.2.0/carbon/model/s3_get_file_input.py
--rw-r--r--   0        0        0     3936 2024-05-29 00:18:21.356446 carbon_python_sdk-0.2.0/carbon/model/s3_get_file_input.pyi
--rw-r--r--   0        0        0     4813 2024-05-29 00:18:21.356546 carbon_python_sdk-0.2.0/carbon/model/salesforce_authentication.py
--rw-r--r--   0        0        0     4813 2024-05-29 00:18:21.356644 carbon_python_sdk-0.2.0/carbon/model/salesforce_authentication.pyi
--rw-r--r--   0        0        0     5449 2024-05-29 00:18:21.356745 carbon_python_sdk-0.2.0/carbon/model/sharepoint_authentication.py
--rw-r--r--   0        0        0     5449 2024-05-29 00:18:21.356845 carbon_python_sdk-0.2.0/carbon/model/sharepoint_authentication.pyi
--rw-r--r--   0        0        0     1566 2024-05-29 00:18:21.356945 carbon_python_sdk-0.2.0/carbon/model/simple_o_auth_data_sources.py
--rw-r--r--   0        0        0     1263 2024-05-29 00:18:21.357040 carbon_python_sdk-0.2.0/carbon/model/simple_o_auth_data_sources.pyi
--rw-r--r--   0        0        0     6587 2024-05-29 00:18:21.357143 carbon_python_sdk-0.2.0/carbon/model/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     6587 2024-05-29 00:18:21.357245 carbon_python_sdk-0.2.0/carbon/model/single_chunks_and_embeddings_upload_input.pyi
--rw-r--r--   0        0        0    15650 2024-05-29 00:18:21.357336 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request.py
--rw-r--r--   0        0        0    15608 2024-05-29 00:18:21.357490 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request.pyi
--rw-r--r--   0        0        0     1113 2024-05-29 00:18:21.357648 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0     1113 2024-05-29 00:18:21.357751 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi
--rw-r--r--   0        0        0     1117 2024-05-29 00:18:21.357848 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0     1117 2024-05-29 00:18:21.357937 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi
--rw-r--r--   0        0        0     1109 2024-05-29 00:18:21.358027 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0     1109 2024-05-29 00:18:21.358119 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi
--rw-r--r--   0        0        0     6392 2024-05-29 00:18:21.358212 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0     6392 2024-05-29 00:18:21.358312 carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_tags.pyi
--rw-r--r--   0        0        0     2485 2024-05-29 00:18:21.358401 carbon_python_sdk-0.2.0/carbon/model/sync_directory_request.py
--rw-r--r--   0        0        0     2485 2024-05-29 00:18:21.358489 carbon_python_sdk-0.2.0/carbon/model/sync_directory_request.pyi
--rw-r--r--   0        0        0     2784 2024-05-29 00:18:21.358571 carbon_python_sdk-0.2.0/carbon/model/sync_files_ids.py
--rw-r--r--   0        0        0     2784 2024-05-29 00:18:21.358651 carbon_python_sdk-0.2.0/carbon/model/sync_files_ids.pyi
--rw-r--r--   0        0        0    22189 2024-05-29 00:18:21.358746 carbon_python_sdk-0.2.0/carbon/model/sync_files_request.py
--rw-r--r--   0        0        0    22189 2024-05-29 00:18:21.358853 carbon_python_sdk-0.2.0/carbon/model/sync_files_request.pyi
--rw-r--r--   0        0        0    16413 2024-05-29 00:18:21.358952 carbon_python_sdk-0.2.0/carbon/model/sync_options.py
--rw-r--r--   0        0        0    16413 2024-05-29 00:18:21.359050 carbon_python_sdk-0.2.0/carbon/model/sync_options.pyi
--rw-r--r--   0        0        0     3009 2024-05-29 00:18:21.359146 carbon_python_sdk-0.2.0/carbon/model/text_embedding_generators.py
--rw-r--r--   0        0        0     2160 2024-05-29 00:18:21.359231 carbon_python_sdk-0.2.0/carbon/model/text_embedding_generators.pyi
--rw-r--r--   0        0        0     3042 2024-05-29 00:18:21.359313 carbon_python_sdk-0.2.0/carbon/model/token_response.py
--rw-r--r--   0        0        0     3042 2024-05-29 00:18:21.359482 carbon_python_sdk-0.2.0/carbon/model/token_response.pyi
--rw-r--r--   0        0        0     2620 2024-05-29 00:18:21.359567 carbon_python_sdk-0.2.0/carbon/model/update_organization_input.py
--rw-r--r--   0        0        0     2620 2024-05-29 00:18:21.359648 carbon_python_sdk-0.2.0/carbon/model/update_organization_input.pyi
--rw-r--r--   0        0        0     9214 2024-05-29 00:18:21.359735 carbon_python_sdk-0.2.0/carbon/model/update_users_input.py
--rw-r--r--   0        0        0     9128 2024-05-29 00:18:21.359848 carbon_python_sdk-0.2.0/carbon/model/update_users_input.pyi
--rw-r--r--   0        0        0     1267 2024-05-29 00:18:21.360281 carbon_python_sdk-0.2.0/carbon/model/update_users_input_customer_ids.py
--rw-r--r--   0        0        0     1243 2024-05-29 00:18:21.360376 carbon_python_sdk-0.2.0/carbon/model/update_users_input_customer_ids.pyi
--rw-r--r--   0        0        0    12928 2024-05-29 00:18:21.360470 carbon_python_sdk-0.2.0/carbon/model/upload_file_from_url_input.py
--rw-r--r--   0        0        0    12928 2024-05-29 00:18:21.360635 carbon_python_sdk-0.2.0/carbon/model/upload_file_from_url_input.pyi
--rw-r--r--   0        0        0     8405 2024-05-29 00:18:21.360799 carbon_python_sdk-0.2.0/carbon/model/user_configuration.py
--rw-r--r--   0        0        0     8319 2024-05-29 00:18:21.360941 carbon_python_sdk-0.2.0/carbon/model/user_configuration.pyi
--rw-r--r--   0        0        0     8665 2024-05-29 00:18:21.361069 carbon_python_sdk-0.2.0/carbon/model/user_configuration_nullable.py
--rw-r--r--   0        0        0     8579 2024-05-29 00:18:21.361199 carbon_python_sdk-0.2.0/carbon/model/user_configuration_nullable.pyi
--rw-r--r--   0        0        0    35549 2024-05-29 00:18:21.361342 carbon_python_sdk-0.2.0/carbon/model/user_file.py
--rw-r--r--   0        0        0    35549 2024-05-29 00:18:21.361474 carbon_python_sdk-0.2.0/carbon/model/user_file.pyi
--rw-r--r--   0        0        0     1650 2024-05-29 00:18:21.361607 carbon_python_sdk-0.2.0/carbon/model/user_file_embedding_properties.py
--rw-r--r--   0        0        0     1650 2024-05-29 00:18:21.361813 carbon_python_sdk-0.2.0/carbon/model/user_file_embedding_properties.pyi
--rw-r--r--   0        0        0     3751 2024-05-29 00:18:21.361905 carbon_python_sdk-0.2.0/carbon/model/user_files_v2.py
--rw-r--r--   0        0        0     3751 2024-05-29 00:18:21.362000 carbon_python_sdk-0.2.0/carbon/model/user_files_v2.pyi
--rw-r--r--   0        0        0     2416 2024-05-29 00:18:21.362095 carbon_python_sdk-0.2.0/carbon/model/user_request_content.py
--rw-r--r--   0        0        0     2416 2024-05-29 00:18:21.362188 carbon_python_sdk-0.2.0/carbon/model/user_request_content.pyi
--rw-r--r--   0        0        0    17500 2024-05-29 00:21:37.950501 carbon_python_sdk-0.2.0/carbon/model/user_response.py
--rw-r--r--   0        0        0    17500 2024-05-29 00:21:37.951062 carbon_python_sdk-0.2.0/carbon/model/user_response.pyi
--rw-r--r--   0        0        0     1511 2024-05-29 00:18:21.362514 carbon_python_sdk-0.2.0/carbon/model/user_response_auto_sync_enabled_sources.py
--rw-r--r--   0        0        0     1511 2024-05-29 00:18:21.362609 carbon_python_sdk-0.2.0/carbon/model/user_response_auto_sync_enabled_sources.pyi
--rw-r--r--   0        0        0     1246 2024-05-29 00:18:21.362710 carbon_python_sdk-0.2.0/carbon/model/user_response_unique_file_tags.py
--rw-r--r--   0        0        0     1246 2024-05-29 00:18:21.362811 carbon_python_sdk-0.2.0/carbon/model/user_response_unique_file_tags.pyi
--rw-r--r--   0        0        0     1315 2024-05-29 00:18:21.363332 carbon_python_sdk-0.2.0/carbon/model/utilities_scrape_web_request.py
--rw-r--r--   0        0        0     1315 2024-05-29 00:18:21.363428 carbon_python_sdk-0.2.0/carbon/model/utilities_scrape_web_request.pyi
--rw-r--r--   0        0        0     3352 2024-05-29 00:18:21.363515 carbon_python_sdk-0.2.0/carbon/model/validation_error.py
--rw-r--r--   0        0        0     3352 2024-05-29 00:18:21.363603 carbon_python_sdk-0.2.0/carbon/model/validation_error.pyi
--rw-r--r--   0        0        0     3149 2024-05-29 00:18:21.363721 carbon_python_sdk-0.2.0/carbon/model/validation_error_loc.py
--rw-r--r--   0        0        0     3149 2024-05-29 00:18:21.363815 carbon_python_sdk-0.2.0/carbon/model/validation_error_loc.pyi
--rw-r--r--   0        0        0     6973 2024-05-29 00:21:37.952667 carbon_python_sdk-0.2.0/carbon/model/webhook.py
--rw-r--r--   0        0        0     6973 2024-05-29 00:21:37.952854 carbon_python_sdk-0.2.0/carbon/model/webhook.pyi
--rw-r--r--   0        0        0     2396 2024-05-29 00:18:21.364110 carbon_python_sdk-0.2.0/carbon/model/webhook_filters.py
--rw-r--r--   0        0        0     2396 2024-05-29 00:18:21.364202 carbon_python_sdk-0.2.0/carbon/model/webhook_filters.pyi
--rw-r--r--   0        0        0     1075 2024-05-29 00:18:21.364294 carbon_python_sdk-0.2.0/carbon/model/webhook_filters_ids.py
--rw-r--r--   0        0        0     1075 2024-05-29 00:18:21.364388 carbon_python_sdk-0.2.0/carbon/model/webhook_filters_ids.pyi
--rw-r--r--   0        0        0     6395 2024-05-29 00:21:37.953037 carbon_python_sdk-0.2.0/carbon/model/webhook_no_key.py
--rw-r--r--   0        0        0     6395 2024-05-29 00:21:37.953179 carbon_python_sdk-0.2.0/carbon/model/webhook_no_key.pyi
--rw-r--r--   0        0        0      995 2024-05-29 00:18:21.364686 carbon_python_sdk-0.2.0/carbon/model/webhook_order_by_columns.py
--rw-r--r--   0        0        0      852 2024-05-29 00:18:21.364778 carbon_python_sdk-0.2.0/carbon/model/webhook_order_by_columns.pyi
--rw-r--r--   0        0        0     4347 2024-05-29 00:18:21.364878 carbon_python_sdk-0.2.0/carbon/model/webhook_query_input.py
--rw-r--r--   0        0        0     4347 2024-05-29 00:18:21.365005 carbon_python_sdk-0.2.0/carbon/model/webhook_query_input.pyi
--rw-r--r--   0        0        0     3798 2024-05-29 00:18:21.365097 carbon_python_sdk-0.2.0/carbon/model/webhook_query_response.py
--rw-r--r--   0        0        0     3798 2024-05-29 00:18:21.365192 carbon_python_sdk-0.2.0/carbon/model/webhook_query_response.pyi
--rw-r--r--   0        0        0      959 2024-05-29 00:21:37.953416 carbon_python_sdk-0.2.0/carbon/model/webhook_status.py
--rw-r--r--   0        0        0      830 2024-05-29 00:21:37.953690 carbon_python_sdk-0.2.0/carbon/model/webhook_status.pyi
--rw-r--r--   0        0        0    16894 2024-05-29 00:18:21.365762 carbon_python_sdk-0.2.0/carbon/model/webscrape_request.py
--rw-r--r--   0        0        0    16810 2024-05-29 00:18:21.365890 carbon_python_sdk-0.2.0/carbon/model/webscrape_request.pyi
--rw-r--r--   0        0        0     1105 2024-05-29 00:18:21.366006 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0     1105 2024-05-29 00:18:21.366106 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_classes_to_skip.pyi
--rw-r--r--   0        0        0     1109 2024-05-29 00:18:21.366607 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0     1109 2024-05-29 00:18:21.366858 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_selectors_to_skip.pyi
--rw-r--r--   0        0        0     1101 2024-05-29 00:18:21.366963 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0     1101 2024-05-29 00:18:21.367070 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_html_tags_to_skip.pyi
--rw-r--r--   0        0        0     6384 2024-05-29 00:18:21.367175 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_tags.py
--rw-r--r--   0        0        0     6384 2024-05-29 00:18:21.367272 carbon_python_sdk-0.2.0/carbon/model/webscrape_request_tags.pyi
--rw-r--r--   0        0        0     3117 2024-05-29 00:18:21.367360 carbon_python_sdk-0.2.0/carbon/model/white_labeling_response.py
--rw-r--r--   0        0        0     3117 2024-05-29 00:18:21.367456 carbon_python_sdk-0.2.0/carbon/model/white_labeling_response.pyi
--rw-r--r--   0        0        0     5401 2024-05-29 00:18:21.367558 carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response.py
--rw-r--r--   0        0        0     5401 2024-05-29 00:18:21.367659 carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response.pyi
--rw-r--r--   0        0        0     1375 2024-05-29 00:18:21.367756 carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0     1375 2024-05-29 00:18:21.367962 carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript.pyi
--rw-r--r--   0        0        0     3326 2024-05-29 00:18:21.368202 carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0     3326 2024-05-29 00:18:21.368299 carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript_item.pyi
--rw-r--r--   0        0        0     3653 2024-05-29 00:18:21.368531 carbon_python_sdk-0.2.0/carbon/model/zendesk_authentication.py
--rw-r--r--   0        0        0     3653 2024-05-29 00:18:21.368625 carbon_python_sdk-0.2.0/carbon/model/zendesk_authentication.pyi
--rw-r--r--   0        0        0     4907 2024-05-29 00:18:21.368724 carbon_python_sdk-0.2.0/carbon/model/zotero_authentication.py
--rw-r--r--   0        0        0     4907 2024-05-29 00:18:21.368824 carbon_python_sdk-0.2.0/carbon/model/zotero_authentication.pyi
--rw-r--r--   0        0        0    13472 2024-05-29 00:21:37.954593 carbon_python_sdk-0.2.0/carbon/models/__init__.py
--rw-r--r--   0        0        0    25498 2024-05-29 00:21:37.954946 carbon_python_sdk-0.2.0/carbon/operation_parameter_map.py
--rw-r--r--   0        0        0     3147 2024-05-29 00:21:37.955661 carbon_python_sdk-0.2.0/carbon/paths/__init__.py
--rw-r--r--   0        0        0      293 2024-05-29 00:18:21.369333 carbon_python_sdk-0.2.0/carbon/paths/add_webhook/__init__.py
--rw-r--r--   0        0        0    13948 2024-05-29 00:18:21.369424 carbon_python_sdk-0.2.0/carbon/paths/add_webhook/post.py
--rw-r--r--   0        0        0    13811 2024-05-29 00:18:21.369589 carbon_python_sdk-0.2.0/carbon/paths/add_webhook/post.pyi
--rw-r--r--   0        0        0      311 2024-05-29 00:18:21.369757 carbon_python_sdk-0.2.0/carbon/paths/auth_v1_access_token/__init__.py
--rw-r--r--   0        0        0    11830 2024-05-29 00:18:21.369858 carbon_python_sdk-0.2.0/carbon/paths/auth_v1_access_token/get.py
--rw-r--r--   0        0        0    11656 2024-05-29 00:18:21.369987 carbon_python_sdk-0.2.0/carbon/paths/auth_v1_access_token/get.pyi
--rw-r--r--   0        0        0      315 2024-05-29 00:18:21.370226 carbon_python_sdk-0.2.0/carbon/paths/auth_v1_white_labeling/__init__.py
--rw-r--r--   0        0        0    11193 2024-05-29 00:18:21.370323 carbon_python_sdk-0.2.0/carbon/paths/auth_v1_white_labeling/get.py
--rw-r--r--   0        0        0    11049 2024-05-29 00:18:21.370447 carbon_python_sdk-0.2.0/carbon/paths/auth_v1_white_labeling/get.pyi
--rw-r--r--   0        0        0      313 2024-05-29 00:18:21.370571 carbon_python_sdk-0.2.0/carbon/paths/create_user_file_tags/__init__.py
--rw-r--r--   0        0        0    15880 2024-05-29 00:18:21.370664 carbon_python_sdk-0.2.0/carbon/paths/create_user_file_tags/post.py
--rw-r--r--   0        0        0    15706 2024-05-29 00:18:21.370835 carbon_python_sdk-0.2.0/carbon/paths/create_user_file_tags/post.pyi
--rw-r--r--   0        0        0      295 2024-05-29 00:18:21.370998 carbon_python_sdk-0.2.0/carbon/paths/delete_files/__init__.py
--rw-r--r--   0        0        0    19307 2024-05-29 00:18:21.371099 carbon_python_sdk-0.2.0/carbon/paths/delete_files/post.py
--rw-r--r--   0        0        0    19133 2024-05-29 00:18:21.371205 carbon_python_sdk-0.2.0/carbon/paths/delete_files/post.pyi
--rw-r--r--   0        0        0      301 2024-05-29 00:18:21.371302 carbon_python_sdk-0.2.0/carbon/paths/delete_files_v2/__init__.py
--rw-r--r--   0        0        0    15967 2024-05-29 00:18:21.371382 carbon_python_sdk-0.2.0/carbon/paths/delete_files_v2/post.py
--rw-r--r--   0        0        0    15793 2024-05-29 00:18:21.371539 carbon_python_sdk-0.2.0/carbon/paths/delete_files_v2/post.pyi
--rw-r--r--   0        0        0      313 2024-05-29 00:18:21.371712 carbon_python_sdk-0.2.0/carbon/paths/delete_user_file_tags/__init__.py
--rw-r--r--   0        0        0    15814 2024-05-29 00:18:21.371795 carbon_python_sdk-0.2.0/carbon/paths/delete_user_file_tags/post.py
--rw-r--r--   0        0        0    15640 2024-05-29 00:18:21.371957 carbon_python_sdk-0.2.0/carbon/paths/delete_user_file_tags/post.pyi
--rw-r--r--   0        0        0      295 2024-05-29 00:18:21.372318 carbon_python_sdk-0.2.0/carbon/paths/delete_users/__init__.py
--rw-r--r--   0        0        0    14899 2024-05-29 00:18:21.372420 carbon_python_sdk-0.2.0/carbon/paths/delete_users/post.py
--rw-r--r--   0        0        0    14762 2024-05-29 00:18:21.372606 carbon_python_sdk-0.2.0/carbon/paths/delete_users/post.pyi
--rw-r--r--   0        0        0      321 2024-05-29 00:18:21.372791 carbon_python_sdk-0.2.0/carbon/paths/delete_webhook_webhook_id/__init__.py
--rw-r--r--   0        0        0    14359 2024-05-29 00:18:21.372872 carbon_python_sdk-0.2.0/carbon/paths/delete_webhook_webhook_id/delete.py
--rw-r--r--   0        0        0    14222 2024-05-29 00:18:21.373059 carbon_python_sdk-0.2.0/carbon/paths/delete_webhook_webhook_id/delete.pyi
--rw-r--r--   0        0        0      307 2024-05-29 00:18:21.373249 carbon_python_sdk-0.2.0/carbon/paths/deletefile_file_id/__init__.py
--rw-r--r--   0        0        0    14552 2024-05-29 00:18:21.373333 carbon_python_sdk-0.2.0/carbon/paths/deletefile_file_id/delete.py
--rw-r--r--   0        0        0    14378 2024-05-29 00:18:21.373528 carbon_python_sdk-0.2.0/carbon/paths/deletefile_file_id/delete.pyi
--rw-r--r--   0        0        0      291 2024-05-29 00:18:21.373867 carbon_python_sdk-0.2.0/carbon/paths/embeddings/__init__.py
--rw-r--r--   0        0        0    29199 2024-05-29 00:18:21.374023 carbon_python_sdk-0.2.0/carbon/paths/embeddings/post.py
--rw-r--r--   0        0        0    29025 2024-05-29 00:18:21.374167 carbon_python_sdk-0.2.0/carbon/paths/embeddings/post.pyi
--rw-r--r--   0        0        0      291 2024-05-29 00:18:21.374295 carbon_python_sdk-0.2.0/carbon/paths/fetch_urls/__init__.py
--rw-r--r--   0        0        0    14466 2024-05-29 00:18:21.374397 carbon_python_sdk-0.2.0/carbon/paths/fetch_urls/get.py
--rw-r--r--   0        0        0    14292 2024-05-29 00:18:21.374619 carbon_python_sdk-0.2.0/carbon/paths/fetch_urls/get.pyi
--rw-r--r--   0        0        0      319 2024-05-29 00:18:21.374843 carbon_python_sdk-0.2.0/carbon/paths/fetch_youtube_transcript/__init__.py
--rw-r--r--   0        0        0    15695 2024-05-29 00:18:21.374951 carbon_python_sdk-0.2.0/carbon/paths/fetch_youtube_transcript/get.py
--rw-r--r--   0        0        0    15521 2024-05-29 00:18:21.375307 carbon_python_sdk-0.2.0/carbon/paths/fetch_youtube_transcript/get.pyi
--rw-r--r--   0        0        0      283 2024-05-29 00:18:21.375518 carbon_python_sdk-0.2.0/carbon/paths/health/__init__.py
--rw-r--r--   0        0        0    10429 2024-05-29 00:18:21.375609 carbon_python_sdk-0.2.0/carbon/paths/health/get.py
--rw-r--r--   0        0        0    10348 2024-05-29 00:18:21.376041 carbon_python_sdk-0.2.0/carbon/paths/health/get.pyi
--rw-r--r--   0        0        0      327 2024-05-29 00:18:21.376163 carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_list/__init__.py
--rw-r--r--   0        0        0    15289 2024-05-29 00:18:21.376250 carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_list/post.py
--rw-r--r--   0        0        0    15115 2024-05-29 00:18:21.376445 carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_list/post.pyi
--rw-r--r--   0        0        0      327 2024-05-29 00:18:21.376645 carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_sync/__init__.py
--rw-r--r--   0        0        0    29028 2024-05-29 00:18:21.376740 carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_sync/post.py
--rw-r--r--   0        0        0    28854 2024-05-29 00:18:21.376849 carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_sync/post.pyi
--rw-r--r--   0        0        0      311 2024-05-29 00:18:21.376949 carbon_python_sdk-0.2.0/carbon/paths/integrations_connect/__init__.py
--rw-r--r--   0        0        0    20686 2024-05-29 00:18:21.377041 carbon_python_sdk-0.2.0/carbon/paths/integrations_connect/post.py
--rw-r--r--   0        0        0    20512 2024-05-29 00:18:21.377156 carbon_python_sdk-0.2.0/carbon/paths/integrations_connect/post.pyi
--rw-r--r--   0        0        0      317 2024-05-29 00:18:21.377254 carbon_python_sdk-0.2.0/carbon/paths/integrations_files_sync/__init__.py
--rw-r--r--   0        0        0    28913 2024-05-29 00:18:21.377349 carbon_python_sdk-0.2.0/carbon/paths/integrations_files_sync/post.py
--rw-r--r--   0        0        0    28739 2024-05-29 00:18:21.377462 carbon_python_sdk-0.2.0/carbon/paths/integrations_files_sync/post.pyi
--rw-r--r--   0        0        0      315 2024-05-29 00:18:21.377560 carbon_python_sdk-0.2.0/carbon/paths/integrations_freshdesk/__init__.py
--rw-r--r--   0        0        0    26091 2024-05-29 00:18:21.377661 carbon_python_sdk-0.2.0/carbon/paths/integrations_freshdesk/post.py
--rw-r--r--   0        0        0    25917 2024-05-29 00:18:21.377769 carbon_python_sdk-0.2.0/carbon/paths/integrations_freshdesk/post.pyi
--rw-r--r--   0        0        0      311 2024-05-29 00:18:21.377867 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook/__init__.py
--rw-r--r--   0        0        0    24946 2024-05-29 00:18:21.377971 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook/post.py
--rw-r--r--   0        0        0    24772 2024-05-29 00:18:21.378078 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook/post.pyi
--rw-r--r--   0        0        0      325 2024-05-29 00:18:21.378180 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_spaces/__init__.py
--rw-r--r--   0        0        0    14816 2024-05-29 00:18:21.378267 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_spaces/get.py
--rw-r--r--   0        0        0    14642 2024-05-29 00:18:21.378461 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_spaces/get.pyi
--rw-r--r--   0        0        0      321 2024-05-29 00:18:21.378653 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_sync/__init__.py
--rw-r--r--   0        0        0    23173 2024-05-29 00:18:21.378746 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_sync/post.py
--rw-r--r--   0        0        0    22999 2024-05-29 00:18:21.378873 carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_sync/post.pyi
--rw-r--r--   0        0        0      309 2024-05-29 00:18:21.378988 carbon_python_sdk-0.2.0/carbon/paths/integrations_github/__init__.py
--rw-r--r--   0        0        0    15826 2024-05-29 00:18:21.379087 carbon_python_sdk-0.2.0/carbon/paths/integrations_github/post.py
--rw-r--r--   0        0        0    15652 2024-05-29 00:18:21.379292 carbon_python_sdk-0.2.0/carbon/paths/integrations_github/post.pyi
--rw-r--r--   0        0        0      321 2024-05-29 00:18:21.379497 carbon_python_sdk-0.2.0/carbon/paths/integrations_github_repos/__init__.py
--rw-r--r--   0        0        0    17078 2024-05-29 00:18:21.379601 carbon_python_sdk-0.2.0/carbon/paths/integrations_github_repos/get.py
--rw-r--r--   0        0        0    16904 2024-05-29 00:18:21.379721 carbon_python_sdk-0.2.0/carbon/paths/integrations_github_repos/get.pyi
--rw-r--r--   0        0        0      331 2024-05-29 00:18:21.379856 carbon_python_sdk-0.2.0/carbon/paths/integrations_github_sync_repos/__init__.py
--rw-r--r--   0        0        0    15560 2024-05-29 00:18:21.379954 carbon_python_sdk-0.2.0/carbon/paths/integrations_github_sync_repos/post.py
--rw-r--r--   0        0        0    15386 2024-05-29 00:18:21.380169 carbon_python_sdk-0.2.0/carbon/paths/integrations_github_sync_repos/post.pyi
--rw-r--r--   0        0        0      317 2024-05-29 00:18:21.380378 carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_sync/__init__.py
--rw-r--r--   0        0        0    26562 2024-05-29 00:18:21.380495 carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_sync/post.py
--rw-r--r--   0        0        0    26388 2024-05-29 00:18:21.380625 carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_sync/post.pyi
--rw-r--r--   0        0        0      331 2024-05-29 00:18:21.380734 carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_user_labels/__init__.py
--rw-r--r--   0        0        0    15340 2024-05-29 00:18:21.380836 carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_user_labels/get.py
--rw-r--r--   0        0        0    15166 2024-05-29 00:18:21.381043 carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_user_labels/get.pyi
--rw-r--r--   0        0        0      317 2024-05-29 00:18:21.381247 carbon_python_sdk-0.2.0/carbon/paths/integrations_items_list/__init__.py
--rw-r--r--   0        0        0    19585 2024-05-29 00:18:21.381357 carbon_python_sdk-0.2.0/carbon/paths/integrations_items_list/post.py
--rw-r--r--   0        0        0    19411 2024-05-29 00:18:21.381475 carbon_python_sdk-0.2.0/carbon/paths/integrations_items_list/post.pyi
--rw-r--r--   0        0        0      317 2024-05-29 00:18:21.381597 carbon_python_sdk-0.2.0/carbon/paths/integrations_items_sync/__init__.py
--rw-r--r--   0        0        0    14992 2024-05-29 00:18:21.381702 carbon_python_sdk-0.2.0/carbon/paths/integrations_items_sync/post.py
--rw-r--r--   0        0        0    14818 2024-05-29 00:18:21.381908 carbon_python_sdk-0.2.0/carbon/paths/integrations_items_sync/post.pyi
--rw-r--r--   0        0        0      315 2024-05-29 00:18:21.382118 carbon_python_sdk-0.2.0/carbon/paths/integrations_oauth_url/__init__.py
--rw-r--r--   0        0        0    37674 2024-05-29 00:18:21.382238 carbon_python_sdk-0.2.0/carbon/paths/integrations_oauth_url/post.py
--rw-r--r--   0        0        0    37500 2024-05-29 00:18:21.382391 carbon_python_sdk-0.2.0/carbon/paths/integrations_oauth_url/post.pyi
--rw-r--r--   0        0        0      321 2024-05-29 00:18:21.382505 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_sync/__init__.py
--rw-r--r--   0        0        0    27296 2024-05-29 00:18:21.382618 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_sync/post.py
--rw-r--r--   0        0        0    27122 2024-05-29 00:18:21.382742 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_sync/post.pyi
--rw-r--r--   0        0        0      343 2024-05-29 00:18:21.382867 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_categories/__init__.py
--rw-r--r--   0        0        0    15590 2024-05-29 00:18:21.382985 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_categories/get.py
--rw-r--r--   0        0        0    15416 2024-05-29 00:18:21.383211 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_categories/get.pyi
--rw-r--r--   0        0        0      337 2024-05-29 00:18:21.383418 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_folders/__init__.py
--rw-r--r--   0        0        0    15371 2024-05-29 00:18:21.383520 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_folders/get.py
--rw-r--r--   0        0        0    15197 2024-05-29 00:18:21.383727 carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_folders/get.pyi
--rw-r--r--   0        0        0      313 2024-05-29 00:18:21.384146 carbon_python_sdk-0.2.0/carbon/paths/integrations_rss_feed/__init__.py
--rw-r--r--   0        0        0    22218 2024-05-29 00:18:21.384257 carbon_python_sdk-0.2.0/carbon/paths/integrations_rss_feed/post.py
--rw-r--r--   0        0        0    22044 2024-05-29 00:18:21.384385 carbon_python_sdk-0.2.0/carbon/paths/integrations_rss_feed/post.pyi
--rw-r--r--   0        0        0      301 2024-05-29 00:18:21.384507 carbon_python_sdk-0.2.0/carbon/paths/integrations_s3/__init__.py
--rw-r--r--   0        0        0    16130 2024-05-29 00:18:21.384610 carbon_python_sdk-0.2.0/carbon/paths/integrations_s3/post.py
--rw-r--r--   0        0        0    15956 2024-05-29 00:18:21.384826 carbon_python_sdk-0.2.0/carbon/paths/integrations_s3/post.pyi
--rw-r--r--   0        0        0      313 2024-05-29 00:18:21.385034 carbon_python_sdk-0.2.0/carbon/paths/integrations_s3_files/__init__.py
--rw-r--r--   0        0        0    28274 2024-05-29 00:18:21.385148 carbon_python_sdk-0.2.0/carbon/paths/integrations_s3_files/post.py
--rw-r--r--   0        0        0    28100 2024-05-29 00:18:21.385286 carbon_python_sdk-0.2.0/carbon/paths/integrations_s3_files/post.pyi
--rw-r--r--   0        0        0      321 2024-05-29 00:18:21.385399 carbon_python_sdk-0.2.0/carbon/paths/modify_user_configuration/__init__.py
--rw-r--r--   0        0        0    16382 2024-05-29 00:18:21.385504 carbon_python_sdk-0.2.0/carbon/paths/modify_user_configuration/post.py
--rw-r--r--   0        0        0    16208 2024-05-29 00:18:21.385712 carbon_python_sdk-0.2.0/carbon/paths/modify_user_configuration/post.pyi
--rw-r--r--   0        0        0      295 2024-05-29 00:18:21.385920 carbon_python_sdk-0.2.0/carbon/paths/organization/__init__.py
--rw-r--r--   0        0        0    10831 2024-05-29 00:18:21.386021 carbon_python_sdk-0.2.0/carbon/paths/organization/get.py
--rw-r--r--   0        0        0    10724 2024-05-29 00:18:21.386150 carbon_python_sdk-0.2.0/carbon/paths/organization/get.pyi
--rw-r--r--   0        0        0      317 2024-05-29 00:21:37.955933 carbon_python_sdk-0.2.0/carbon/paths/organization_statistics/__init__.py
--rw-r--r--   0        0        0    11092 2024-05-29 00:21:37.956331 carbon_python_sdk-0.2.0/carbon/paths/organization_statistics/post.py
--rw-r--r--   0        0        0    10985 2024-05-29 00:21:37.957015 carbon_python_sdk-0.2.0/carbon/paths/organization_statistics/post.pyi
--rw-r--r--   0        0        0      309 2024-05-29 00:18:21.386615 carbon_python_sdk-0.2.0/carbon/paths/organization_update/__init__.py
--rw-r--r--   0        0        0    15275 2024-05-29 00:18:21.386712 carbon_python_sdk-0.2.0/carbon/paths/organization_update/post.py
--rw-r--r--   0        0        0    15138 2024-05-29 00:18:21.386926 carbon_python_sdk-0.2.0/carbon/paths/organization_update/post.pyi
--rw-r--r--   0        0        0      309 2024-05-29 00:18:21.387141 carbon_python_sdk-0.2.0/carbon/paths/parsed_file_file_id/__init__.py
--rw-r--r--   0        0        0    14654 2024-05-29 00:18:21.387241 carbon_python_sdk-0.2.0/carbon/paths/parsed_file_file_id/get.py
--rw-r--r--   0        0        0    14480 2024-05-29 00:18:21.387445 carbon_python_sdk-0.2.0/carbon/paths/parsed_file_file_id/get.pyi
--rw-r--r--   0        0        0      301 2024-05-29 00:18:21.387654 carbon_python_sdk-0.2.0/carbon/paths/process_sitemap/__init__.py
--rw-r--r--   0        0        0    14363 2024-05-29 00:18:21.387758 carbon_python_sdk-0.2.0/carbon/paths/process_sitemap/get.py
--rw-r--r--   0        0        0    14189 2024-05-29 00:18:21.387969 carbon_python_sdk-0.2.0/carbon/paths/process_sitemap/get.pyi
--rw-r--r--   0        0        0      303 2024-05-29 00:18:21.388167 carbon_python_sdk-0.2.0/carbon/paths/raw_file_file_id/__init__.py
--rw-r--r--   0        0        0    14585 2024-05-29 00:18:21.388264 carbon_python_sdk-0.2.0/carbon/paths/raw_file_file_id/get.py
--rw-r--r--   0        0        0    14411 2024-05-29 00:18:21.388462 carbon_python_sdk-0.2.0/carbon/paths/raw_file_file_id/get.pyi
--rw-r--r--   0        0        0      293 2024-05-29 00:18:21.388926 carbon_python_sdk-0.2.0/carbon/paths/resync_file/__init__.py
--rw-r--r--   0        0        0    16696 2024-05-29 00:18:21.389033 carbon_python_sdk-0.2.0/carbon/paths/resync_file/post.py
--rw-r--r--   0        0        0    16522 2024-05-29 00:18:21.389152 carbon_python_sdk-0.2.0/carbon/paths/resync_file/post.pyi
--rw-r--r--   0        0        0      309 2024-05-29 00:18:21.389265 carbon_python_sdk-0.2.0/carbon/paths/revoke_access_token/__init__.py
--rw-r--r--   0        0        0    14828 2024-05-29 00:18:21.389362 carbon_python_sdk-0.2.0/carbon/paths/revoke_access_token/post.py
--rw-r--r--   0        0        0    14654 2024-05-29 00:18:21.389563 carbon_python_sdk-0.2.0/carbon/paths/revoke_access_token/post.pyi
--rw-r--r--   0        0        0      299 2024-05-29 00:18:21.389890 carbon_python_sdk-0.2.0/carbon/paths/scrape_sitemap/__init__.py
--rw-r--r--   0        0        0    27300 2024-05-29 00:18:21.389993 carbon_python_sdk-0.2.0/carbon/paths/scrape_sitemap/post.py
--rw-r--r--   0        0        0    27126 2024-05-29 00:18:21.390109 carbon_python_sdk-0.2.0/carbon/paths/scrape_sitemap/post.pyi
--rw-r--r--   0        0        0      293 2024-05-29 00:18:21.390214 carbon_python_sdk-0.2.0/carbon/paths/search_urls/__init__.py
--rw-r--r--   0        0        0    14549 2024-05-29 00:18:21.390307 carbon_python_sdk-0.2.0/carbon/paths/search_urls/get.py
--rw-r--r--   0        0        0    14375 2024-05-29 00:18:21.390504 carbon_python_sdk-0.2.0/carbon/paths/search_urls/get.pyi
--rw-r--r--   0        0        0      293 2024-05-29 00:18:21.390707 carbon_python_sdk-0.2.0/carbon/paths/text_chunks/__init__.py
--rw-r--r--   0        0        0    19073 2024-05-29 00:18:21.390798 carbon_python_sdk-0.2.0/carbon/paths/text_chunks/post.py
--rw-r--r--   0        0        0    18899 2024-05-29 00:18:21.390904 carbon_python_sdk-0.2.0/carbon/paths/text_chunks/post.pyi
--rw-r--r--   0        0        0      295 2024-05-29 00:18:21.390998 carbon_python_sdk-0.2.0/carbon/paths/update_users/__init__.py
--rw-r--r--   0        0        0    18200 2024-05-29 00:18:21.391083 carbon_python_sdk-0.2.0/carbon/paths/update_users/post.py
--rw-r--r--   0        0        0    18063 2024-05-29 00:18:21.391180 carbon_python_sdk-0.2.0/carbon/paths/update_users/post.pyi
--rw-r--r--   0        0        0      327 2024-05-29 00:18:21.391290 carbon_python_sdk-0.2.0/carbon/paths/upload_chunks_and_embeddings/__init__.py
--rw-r--r--   0        0        0    20060 2024-05-29 00:18:21.391379 carbon_python_sdk-0.2.0/carbon/paths/upload_chunks_and_embeddings/post.py
--rw-r--r--   0        0        0    19886 2024-05-29 00:18:21.391487 carbon_python_sdk-0.2.0/carbon/paths/upload_chunks_and_embeddings/post.pyi
--rw-r--r--   0        0        0      311 2024-05-29 00:18:21.391608 carbon_python_sdk-0.2.0/carbon/paths/upload_file_from_url/__init__.py
--rw-r--r--   0        0        0    24942 2024-05-29 00:18:21.391709 carbon_python_sdk-0.2.0/carbon/paths/upload_file_from_url/post.py
--rw-r--r--   0        0        0    24768 2024-05-29 00:18:21.391820 carbon_python_sdk-0.2.0/carbon/paths/upload_file_from_url/post.pyi
--rw-r--r--   0        0        0      293 2024-05-29 00:18:21.391917 carbon_python_sdk-0.2.0/carbon/paths/upload_text/__init__.py
--rw-r--r--   0        0        0    20504 2024-05-29 00:18:21.392031 carbon_python_sdk-0.2.0/carbon/paths/upload_text/post.py
--rw-r--r--   0        0        0    20330 2024-05-29 00:18:21.392156 carbon_python_sdk-0.2.0/carbon/paths/upload_text/post.pyi
--rw-r--r--   0        0        0      291 2024-05-29 00:18:21.392303 carbon_python_sdk-0.2.0/carbon/paths/uploadfile/__init__.py
--rw-r--r--   0        0        0    33555 2024-05-29 00:21:37.957956 carbon_python_sdk-0.2.0/carbon/paths/uploadfile/post.py
--rw-r--r--   0        0        0    33381 2024-05-29 00:21:37.958951 carbon_python_sdk-0.2.0/carbon/paths/uploadfile/post.pyi
--rw-r--r--   0        0        0      279 2024-05-29 00:18:21.392768 carbon_python_sdk-0.2.0/carbon/paths/user/__init__.py
--rw-r--r--   0        0        0    14156 2024-05-29 00:18:21.392881 carbon_python_sdk-0.2.0/carbon/paths/user/post.py
--rw-r--r--   0        0        0    14019 2024-05-29 00:18:21.393098 carbon_python_sdk-0.2.0/carbon/paths/user/post.pyi
--rw-r--r--   0        0        0      305 2024-05-29 00:18:21.393323 carbon_python_sdk-0.2.0/carbon/paths/user_data_sources/__init__.py
--rw-r--r--   0        0        0    18865 2024-05-29 00:18:21.393439 carbon_python_sdk-0.2.0/carbon/paths/user_data_sources/post.py
--rw-r--r--   0        0        0    18691 2024-05-29 00:18:21.393573 carbon_python_sdk-0.2.0/carbon/paths/user_data_sources/post.pyi
--rw-r--r--   0        0        0      291 2024-05-29 00:18:21.393721 carbon_python_sdk-0.2.0/carbon/paths/user_files/__init__.py
--rw-r--r--   0        0        0    22374 2024-05-29 00:18:21.393852 carbon_python_sdk-0.2.0/carbon/paths/user_files/post.py
--rw-r--r--   0        0        0    22200 2024-05-29 00:18:21.394009 carbon_python_sdk-0.2.0/carbon/paths/user_files/post.pyi
--rw-r--r--   0        0        0      297 2024-05-29 00:18:21.394150 carbon_python_sdk-0.2.0/carbon/paths/user_files_v2/__init__.py
--rw-r--r--   0        0        0    21370 2024-05-29 00:18:21.394281 carbon_python_sdk-0.2.0/carbon/paths/user_files_v2/post.py
--rw-r--r--   0        0        0    21196 2024-05-29 00:18:21.394426 carbon_python_sdk-0.2.0/carbon/paths/user_files_v2/post.pyi
--rw-r--r--   0        0        0      291 2024-05-29 00:18:21.394565 carbon_python_sdk-0.2.0/carbon/paths/web_scrape/__init__.py
--rw-r--r--   0        0        0    14274 2024-05-29 00:18:21.394684 carbon_python_sdk-0.2.0/carbon/paths/web_scrape/post.py
--rw-r--r--   0        0        0    14100 2024-05-29 00:18:21.394923 carbon_python_sdk-0.2.0/carbon/paths/web_scrape/post.pyi
--rw-r--r--   0        0        0      287 2024-05-29 00:18:21.395156 carbon_python_sdk-0.2.0/carbon/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    17367 2024-05-29 00:18:21.395298 carbon_python_sdk-0.2.0/carbon/paths/webhooks/post.py
--rw-r--r--   0        0        0    17230 2024-05-29 00:18:21.395463 carbon_python_sdk-0.2.0/carbon/paths/webhooks/post.pyi
--rw-r--r--   0        0        0        0 2024-05-29 00:18:21.395636 carbon_python_sdk-0.2.0/carbon/pydantic/__init__.py
--rw-r--r--   0        0        0      559 2024-05-29 00:18:21.395761 carbon_python_sdk-0.2.0/carbon/pydantic/add_webhook_props.py
--rw-r--r--   0        0        0      586 2024-05-29 00:18:21.395872 carbon_python_sdk-0.2.0/carbon/pydantic/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0      760 2024-05-29 00:18:21.395987 carbon_python_sdk-0.2.0/carbon/pydantic/chunk_properties.py
--rw-r--r--   0        0        0      768 2024-05-29 00:18:21.396126 carbon_python_sdk-0.2.0/carbon/pydantic/chunk_properties_nullable.py
--rw-r--r--   0        0        0      821 2024-05-29 00:18:21.396264 carbon_python_sdk-0.2.0/carbon/pydantic/chunks_and_embeddings.py
--rw-r--r--   0        0        0      469 2024-05-29 00:18:21.396382 carbon_python_sdk-0.2.0/carbon/pydantic/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1333 2024-05-29 00:18:21.396489 carbon_python_sdk-0.2.0/carbon/pydantic/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0      438 2024-05-29 00:18:21.396607 carbon_python_sdk-0.2.0/carbon/pydantic/chunks_and_embeddings_upload_input_custom_credentials.py
--rw-r--r--   0        0        0      418 2024-05-29 00:18:21.396713 carbon_python_sdk-0.2.0/carbon/pydantic/configuration_keys.py
--rw-r--r--   0        0        0      835 2024-05-29 00:18:21.396828 carbon_python_sdk-0.2.0/carbon/pydantic/confluence_authentication.py
--rw-r--r--   0        0        0     1791 2024-05-29 00:18:21.396942 carbon_python_sdk-0.2.0/carbon/pydantic/connect_data_source_input.py
--rw-r--r--   0        0        0      765 2024-05-29 00:18:21.397054 carbon_python_sdk-0.2.0/carbon/pydantic/connect_data_source_response.py
--rw-r--r--   0        0        0      481 2024-05-29 00:18:21.397162 carbon_python_sdk-0.2.0/carbon/pydantic/custom_credentials_type.py
--rw-r--r--   0        0        0      424 2024-05-29 00:18:21.397271 carbon_python_sdk-0.2.0/carbon/pydantic/data_source_extended_input.py
--rw-r--r--   0        0        0      456 2024-05-29 00:18:21.397383 carbon_python_sdk-0.2.0/carbon/pydantic/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      472 2024-05-29 00:18:21.397492 carbon_python_sdk-0.2.0/carbon/pydantic/data_source_sync_statuses.py
--rw-r--r--   0        0        0      890 2024-05-29 00:21:37.960154 carbon_python_sdk-0.2.0/carbon/pydantic/data_source_type.py
--rw-r--r--   0        0        0      898 2024-05-29 00:21:37.960464 carbon_python_sdk-0.2.0/carbon/pydantic/data_source_type_nullable.py
--rw-r--r--   0        0        0     1187 2024-05-29 00:18:21.397813 carbon_python_sdk-0.2.0/carbon/pydantic/delete_files_query_input.py
--rw-r--r--   0        0        0      448 2024-05-29 00:18:21.397924 carbon_python_sdk-0.2.0/carbon/pydantic/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0      809 2024-05-29 00:18:21.398036 carbon_python_sdk-0.2.0/carbon/pydantic/delete_files_v2_query_input.py
--rw-r--r--   0        0        0      690 2024-05-29 00:18:21.398146 carbon_python_sdk-0.2.0/carbon/pydantic/delete_users_input.py
--rw-r--r--   0        0        0      430 2024-05-29 00:18:21.398275 carbon_python_sdk-0.2.0/carbon/pydantic/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0      694 2024-05-29 00:18:21.398383 carbon_python_sdk-0.2.0/carbon/pydantic/directory_item.py
--rw-r--r--   0        0        0     1674 2024-05-29 00:18:21.398497 carbon_python_sdk-0.2.0/carbon/pydantic/document_response.py
--rw-r--r--   0        0        0      665 2024-05-29 00:18:21.398744 carbon_python_sdk-0.2.0/carbon/pydantic/document_response_list.py
--rw-r--r--   0        0        0      411 2024-05-29 00:18:21.398844 carbon_python_sdk-0.2.0/carbon/pydantic/document_response_tags.py
--rw-r--r--   0        0        0      463 2024-05-29 00:18:21.398950 carbon_python_sdk-0.2.0/carbon/pydantic/document_response_vector.py
--rw-r--r--   0        0        0     1021 2024-05-29 00:18:21.399035 carbon_python_sdk-0.2.0/carbon/pydantic/embedding_and_chunk.py
--rw-r--r--   0        0        0      467 2024-05-29 00:18:21.399115 carbon_python_sdk-0.2.0/carbon/pydantic/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0      743 2024-05-29 00:18:21.399202 carbon_python_sdk-0.2.0/carbon/pydantic/embedding_generators.py
--rw-r--r--   0        0        0      751 2024-05-29 00:18:21.399299 carbon_python_sdk-0.2.0/carbon/pydantic/embedding_generators_nullable.py
--rw-r--r--   0        0        0      666 2024-05-29 00:18:21.399392 carbon_python_sdk-0.2.0/carbon/pydantic/embedding_properties.py
--rw-r--r--   0        0        0      780 2024-05-29 00:18:21.399480 carbon_python_sdk-0.2.0/carbon/pydantic/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0      470 2024-05-29 00:18:21.399573 carbon_python_sdk-0.2.0/carbon/pydantic/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0     1222 2024-05-29 00:18:21.399658 carbon_python_sdk-0.2.0/carbon/pydantic/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0      711 2024-05-29 00:18:21.399750 carbon_python_sdk-0.2.0/carbon/pydantic/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0      553 2024-05-29 00:18:21.399841 carbon_python_sdk-0.2.0/carbon/pydantic/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1780 2024-05-29 00:18:21.399935 carbon_python_sdk-0.2.0/carbon/pydantic/external_source_item.py
--rw-r--r--   0        0        0      455 2024-05-29 00:18:21.400029 carbon_python_sdk-0.2.0/carbon/pydantic/external_source_items_order_by.py
--rw-r--r--   0        0        0      781 2024-05-29 00:18:21.400123 carbon_python_sdk-0.2.0/carbon/pydantic/fetch_urls_response.py
--rw-r--r--   0        0        0      424 2024-05-29 00:18:21.400213 carbon_python_sdk-0.2.0/carbon/pydantic/fetch_urls_response_urls.py
--rw-r--r--   0        0        0      445 2024-05-29 00:21:37.960716 carbon_python_sdk-0.2.0/carbon/pydantic/file_content_types.py
--rw-r--r--   0        0        0      453 2024-05-29 00:21:37.961034 carbon_python_sdk-0.2.0/carbon/pydantic/file_content_types_nullable.py
--rw-r--r--   0        0        0      820 2024-05-29 00:21:37.961290 carbon_python_sdk-0.2.0/carbon/pydantic/file_formats.py
--rw-r--r--   0        0        0      828 2024-05-29 00:21:37.961543 carbon_python_sdk-0.2.0/carbon/pydantic/file_formats_nullable.py
--rw-r--r--   0        0        0     1002 2024-05-29 00:18:21.400670 carbon_python_sdk-0.2.0/carbon/pydantic/file_statistics.py
--rw-r--r--   0        0        0     1010 2024-05-29 00:18:21.400765 carbon_python_sdk-0.2.0/carbon/pydantic/file_statistics_nullable.py
--rw-r--r--   0        0        0     1240 2024-05-29 00:18:21.400857 carbon_python_sdk-0.2.0/carbon/pydantic/file_sync_config.py
--rw-r--r--   0        0        0     1248 2024-05-29 00:18:21.400946 carbon_python_sdk-0.2.0/carbon/pydantic/file_sync_config_nullable.py
--rw-r--r--   0        0        0      492 2024-05-29 00:18:21.401043 carbon_python_sdk-0.2.0/carbon/pydantic/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     2096 2024-05-29 00:18:21.401133 carbon_python_sdk-0.2.0/carbon/pydantic/fresh_desk_connect_request.py
--rw-r--r--   0        0        0      723 2024-05-29 00:18:21.401225 carbon_python_sdk-0.2.0/carbon/pydantic/freskdesk_authentication.py
--rw-r--r--   0        0        0      575 2024-05-29 00:18:21.401318 carbon_python_sdk-0.2.0/carbon/pydantic/generic_success_response.py
--rw-r--r--   0        0        0     3379 2024-05-29 00:18:21.401417 carbon_python_sdk-0.2.0/carbon/pydantic/get_embedding_documents_body.py
--rw-r--r--   0        0        0      452 2024-05-29 00:18:21.401516 carbon_python_sdk-0.2.0/carbon/pydantic/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0      458 2024-05-29 00:18:21.401613 carbon_python_sdk-0.2.0/carbon/pydantic/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0      477 2024-05-29 00:18:21.401706 carbon_python_sdk-0.2.0/carbon/pydantic/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0      420 2024-05-29 00:18:21.401797 carbon_python_sdk-0.2.0/carbon/pydantic/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0      752 2024-05-29 00:18:21.401888 carbon_python_sdk-0.2.0/carbon/pydantic/gitbook_authetication.py
--rw-r--r--   0        0        0     1911 2024-05-29 00:18:21.401977 carbon_python_sdk-0.2.0/carbon/pydantic/gitbook_connect_request.py
--rw-r--r--   0        0        0     1699 2024-05-29 00:18:21.402067 carbon_python_sdk-0.2.0/carbon/pydantic/gitbook_sync_request.py
--rw-r--r--   0        0        0      429 2024-05-29 00:18:21.402165 carbon_python_sdk-0.2.0/carbon/pydantic/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0      734 2024-05-29 00:18:21.402255 carbon_python_sdk-0.2.0/carbon/pydantic/github_authentication.py
--rw-r--r--   0        0        0      825 2024-05-29 00:18:21.402345 carbon_python_sdk-0.2.0/carbon/pydantic/github_connect_request.py
--rw-r--r--   0        0        0      783 2024-05-29 00:18:21.402439 carbon_python_sdk-0.2.0/carbon/pydantic/github_fetch_repos_request.py
--rw-r--r--   0        0        0      431 2024-05-29 00:18:21.402664 carbon_python_sdk-0.2.0/carbon/pydantic/github_fetch_repos_request_repos.py
--rw-r--r--   0        0        0     2073 2024-05-29 00:18:21.402759 carbon_python_sdk-0.2.0/carbon/pydantic/gmail_sync_input.py
--rw-r--r--   0        0        0      432 2024-05-29 00:18:21.402852 carbon_python_sdk-0.2.0/carbon/pydantic/helpdesk_file_types.py
--rw-r--r--   0        0        0      678 2024-05-29 00:18:21.402944 carbon_python_sdk-0.2.0/carbon/pydantic/http_validation_error.py
--rw-r--r--   0        0        0      665 2024-05-29 00:18:21.403039 carbon_python_sdk-0.2.0/carbon/pydantic/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0      673 2024-05-29 00:18:21.403133 carbon_python_sdk-0.2.0/carbon/pydantic/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0     1282 2024-05-29 00:18:21.403222 carbon_python_sdk-0.2.0/carbon/pydantic/list_data_source_items_request.py
--rw-r--r--   0        0        0      710 2024-05-29 00:18:21.403313 carbon_python_sdk-0.2.0/carbon/pydantic/list_data_source_items_response.py
--rw-r--r--   0        0        0     1035 2024-05-29 00:18:21.403403 carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters.py
--rw-r--r--   0        0        0      447 2024-05-29 00:18:21.403493 carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters_external_ids.py
--rw-r--r--   0        0        0      439 2024-05-29 00:18:21.403584 carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters_ids.py
--rw-r--r--   0        0        0     1093 2024-05-29 00:18:21.403667 carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters_nullable.py
--rw-r--r--   0        0        0      455 2024-05-29 00:18:21.403751 carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters_nullable_external_ids.py
--rw-r--r--   0        0        0      447 2024-05-29 00:18:21.403837 carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters_nullable_ids.py
--rw-r--r--   0        0        0      664 2024-05-29 00:18:21.403916 carbon_python_sdk-0.2.0/carbon/pydantic/list_request.py
--rw-r--r--   0        0        0      638 2024-05-29 00:18:21.404004 carbon_python_sdk-0.2.0/carbon/pydantic/list_response.py
--rw-r--r--   0        0        0      733 2024-05-29 00:18:21.404096 carbon_python_sdk-0.2.0/carbon/pydantic/modify_user_configuration_input.py
--rw-r--r--   0        0        0      742 2024-05-29 00:18:21.404186 carbon_python_sdk-0.2.0/carbon/pydantic/notion_authentication.py
--rw-r--r--   0        0        0      814 2024-05-29 00:18:21.404287 carbon_python_sdk-0.2.0/carbon/pydantic/o_auth_authentication.py
--rw-r--r--   0        0        0     4718 2024-05-29 00:21:37.961870 carbon_python_sdk-0.2.0/carbon/pydantic/o_auth_url_request.py
--rw-r--r--   0        0        0      417 2024-05-29 00:18:21.404494 carbon_python_sdk-0.2.0/carbon/pydantic/order_dir.py
--rw-r--r--   0        0        0      419 2024-05-29 00:18:21.404585 carbon_python_sdk-0.2.0/carbon/pydantic/order_dir_v2.py
--rw-r--r--   0        0        0     2547 2024-05-29 00:21:37.962310 carbon_python_sdk-0.2.0/carbon/pydantic/organization_response.py
--rw-r--r--   0        0        0     2100 2024-05-29 00:18:21.404778 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_api.py
--rw-r--r--   0        0        0      998 2024-05-29 00:18:21.404871 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_filters.py
--rw-r--r--   0        0        0      456 2024-05-29 00:18:21.404962 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0      462 2024-05-29 00:18:21.405055 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0     1213 2024-05-29 00:18:21.405155 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0      756 2024-05-29 00:18:21.405249 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_response.py
--rw-r--r--   0        0        0      785 2024-05-29 00:18:21.405346 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_file_tag_create.py
--rw-r--r--   0        0        0      424 2024-05-29 00:18:21.405432 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0      789 2024-05-29 00:18:21.405516 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0      437 2024-05-29 00:18:21.405601 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     5786 2024-05-29 00:18:21.405689 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0      469 2024-05-29 00:18:21.405776 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0      457 2024-05-29 00:18:21.405857 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0      482 2024-05-29 00:18:21.405947 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0      467 2024-05-29 00:18:21.406037 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0      464 2024-05-29 00:18:21.406121 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters_request_ids.py
--rw-r--r--   0        0        0      429 2024-05-29 00:18:21.406217 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0      501 2024-05-29 00:18:21.406301 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1554 2024-05-29 00:18:21.406384 carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0      571 2024-05-29 00:18:21.406461 carbon_python_sdk-0.2.0/carbon/pydantic/outh_url_response.py
--rw-r--r--   0        0        0     2156 2024-05-29 00:18:21.406540 carbon_python_sdk-0.2.0/carbon/pydantic/outlook_sync_input.py
--rw-r--r--   0        0        0      645 2024-05-29 00:18:21.406620 carbon_python_sdk-0.2.0/carbon/pydantic/pagination.py
--rw-r--r--   0        0        0      584 2024-05-29 00:18:21.406700 carbon_python_sdk-0.2.0/carbon/pydantic/presigned_url_response.py
--rw-r--r--   0        0        0     1341 2024-05-29 00:18:21.406781 carbon_python_sdk-0.2.0/carbon/pydantic/raw_text_input.py
--rw-r--r--   0        0        0      861 2024-05-29 00:18:21.406861 carbon_python_sdk-0.2.0/carbon/pydantic/resync_file_query_input.py
--rw-r--r--   0        0        0      588 2024-05-29 00:18:21.406947 carbon_python_sdk-0.2.0/carbon/pydantic/revoke_access_token_input.py
--rw-r--r--   0        0        0     1515 2024-05-29 00:18:21.407028 carbon_python_sdk-0.2.0/carbon/pydantic/rss_feed_input.py
--rw-r--r--   0        0        0      832 2024-05-29 00:18:21.407112 carbon_python_sdk-0.2.0/carbon/pydantic/s3_auth_request.py
--rw-r--r--   0        0        0      744 2024-05-29 00:18:21.407188 carbon_python_sdk-0.2.0/carbon/pydantic/s3_authentication.py
--rw-r--r--   0        0        0     2360 2024-05-29 00:18:21.407266 carbon_python_sdk-0.2.0/carbon/pydantic/s3_file_sync_input.py
--rw-r--r--   0        0        0      677 2024-05-29 00:18:21.407355 carbon_python_sdk-0.2.0/carbon/pydantic/s3_get_file_input.py
--rw-r--r--   0        0        0      829 2024-05-29 00:18:21.407442 carbon_python_sdk-0.2.0/carbon/pydantic/salesforce_authentication.py
--rw-r--r--   0        0        0      886 2024-05-29 00:18:21.407531 carbon_python_sdk-0.2.0/carbon/pydantic/sharepoint_authentication.py
--rw-r--r--   0        0        0      494 2024-05-29 00:18:21.407620 carbon_python_sdk-0.2.0/carbon/pydantic/simple_o_auth_data_sources.py
--rw-r--r--   0        0        0      942 2024-05-29 00:18:21.407702 carbon_python_sdk-0.2.0/carbon/pydantic/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     2337 2024-05-29 00:18:21.407789 carbon_python_sdk-0.2.0/carbon/pydantic/sitemap_scrape_request.py
--rw-r--r--   0        0        0      456 2024-05-29 00:18:21.407884 carbon_python_sdk-0.2.0/carbon/pydantic/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      458 2024-05-29 00:18:21.407978 carbon_python_sdk-0.2.0/carbon/pydantic/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      454 2024-05-29 00:18:21.408081 carbon_python_sdk-0.2.0/carbon/pydantic/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      415 2024-05-29 00:18:21.408174 carbon_python_sdk-0.2.0/carbon/pydantic/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0      586 2024-05-29 00:18:21.408265 carbon_python_sdk-0.2.0/carbon/pydantic/sync_directory_request.py
--rw-r--r--   0        0        0      597 2024-05-29 00:18:21.408358 carbon_python_sdk-0.2.0/carbon/pydantic/sync_files_ids.py
--rw-r--r--   0        0        0     2668 2024-05-29 00:18:21.408445 carbon_python_sdk-0.2.0/carbon/pydantic/sync_files_request.py
--rw-r--r--   0        0        0     2932 2024-05-29 00:18:21.408526 carbon_python_sdk-0.2.0/carbon/pydantic/sync_options.py
--rw-r--r--   0        0        0      726 2024-05-29 00:18:21.408608 carbon_python_sdk-0.2.0/carbon/pydantic/text_embedding_generators.py
--rw-r--r--   0        0        0      630 2024-05-29 00:18:21.408691 carbon_python_sdk-0.2.0/carbon/pydantic/token_response.py
--rw-r--r--   0        0        0      724 2024-05-29 00:18:21.408779 carbon_python_sdk-0.2.0/carbon/pydantic/update_organization_input.py
--rw-r--r--   0        0        0     1746 2024-05-29 00:18:21.408861 carbon_python_sdk-0.2.0/carbon/pydantic/update_users_input.py
--rw-r--r--   0        0        0      430 2024-05-29 00:18:21.408951 carbon_python_sdk-0.2.0/carbon/pydantic/update_users_input_customer_ids.py
--rw-r--r--   0        0        0     1862 2024-05-29 00:18:21.409070 carbon_python_sdk-0.2.0/carbon/pydantic/upload_file_from_url_input.py
--rw-r--r--   0        0        0     1582 2024-05-29 00:18:21.409155 carbon_python_sdk-0.2.0/carbon/pydantic/user_configuration.py
--rw-r--r--   0        0        0     1590 2024-05-29 00:18:21.409237 carbon_python_sdk-0.2.0/carbon/pydantic/user_configuration_nullable.py
--rw-r--r--   0        0        0     3606 2024-05-29 00:18:21.409328 carbon_python_sdk-0.2.0/carbon/pydantic/user_file.py
--rw-r--r--   0        0        0      487 2024-05-29 00:18:21.409415 carbon_python_sdk-0.2.0/carbon/pydantic/user_file_embedding_properties.py
--rw-r--r--   0        0        0      667 2024-05-29 00:18:21.409498 carbon_python_sdk-0.2.0/carbon/pydantic/user_files_v2.py
--rw-r--r--   0        0        0      578 2024-05-29 00:18:21.409646 carbon_python_sdk-0.2.0/carbon/pydantic/user_request_content.py
--rw-r--r--   0        0        0     2736 2024-05-29 00:21:37.962762 carbon_python_sdk-0.2.0/carbon/pydantic/user_response.py
--rw-r--r--   0        0        0      503 2024-05-29 00:18:21.409925 carbon_python_sdk-0.2.0/carbon/pydantic/user_response_auto_sync_enabled_sources.py
--rw-r--r--   0        0        0      432 2024-05-29 00:18:21.410011 carbon_python_sdk-0.2.0/carbon/pydantic/user_response_unique_file_tags.py
--rw-r--r--   0        0        0      504 2024-05-29 00:18:21.410115 carbon_python_sdk-0.2.0/carbon/pydantic/utilities_scrape_web_request.py
--rw-r--r--   0        0        0      714 2024-05-29 00:18:21.410225 carbon_python_sdk-0.2.0/carbon/pydantic/validation_error.py
--rw-r--r--   0        0        0      440 2024-05-29 00:18:21.410333 carbon_python_sdk-0.2.0/carbon/pydantic/validation_error_loc.py
--rw-r--r--   0        0        0      982 2024-05-29 00:21:37.963262 carbon_python_sdk-0.2.0/carbon/pydantic/webhook.py
--rw-r--r--   0        0        0      661 2024-05-29 00:18:21.410546 carbon_python_sdk-0.2.0/carbon/pydantic/webhook_filters.py
--rw-r--r--   0        0        0      437 2024-05-29 00:18:21.410658 carbon_python_sdk-0.2.0/carbon/pydantic/webhook_filters_ids.py
--rw-r--r--   0        0        0      936 2024-05-29 00:21:37.963773 carbon_python_sdk-0.2.0/carbon/pydantic/webhook_no_key.py
--rw-r--r--   0        0        0      443 2024-05-29 00:18:21.410886 carbon_python_sdk-0.2.0/carbon/pydantic/webhook_order_by_columns.py
--rw-r--r--   0        0        0     1074 2024-05-29 00:18:21.411009 carbon_python_sdk-0.2.0/carbon/pydantic/webhook_query_input.py
--rw-r--r--   0        0        0      689 2024-05-29 00:18:21.411122 carbon_python_sdk-0.2.0/carbon/pydantic/webhook_query_response.py
--rw-r--r--   0        0        0      428 2024-05-29 00:21:37.964658 carbon_python_sdk-0.2.0/carbon/pydantic/webhook_status.py
--rw-r--r--   0        0        0     2380 2024-05-29 00:18:21.411327 carbon_python_sdk-0.2.0/carbon/pydantic/webscrape_request.py
--rw-r--r--   0        0        0      452 2024-05-29 00:18:21.411590 carbon_python_sdk-0.2.0/carbon/pydantic/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      454 2024-05-29 00:18:21.411702 carbon_python_sdk-0.2.0/carbon/pydantic/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      450 2024-05-29 00:18:21.411792 carbon_python_sdk-0.2.0/carbon/pydantic/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      411 2024-05-29 00:18:21.411883 carbon_python_sdk-0.2.0/carbon/pydantic/webscrape_request_tags.py
--rw-r--r--   0        0        0      727 2024-05-29 00:18:21.411975 carbon_python_sdk-0.2.0/carbon/pydantic/white_labeling_response.py
--rw-r--r--   0        0        0      887 2024-05-29 00:18:21.412073 carbon_python_sdk-0.2.0/carbon/pydantic/youtube_transcript_response.py
--rw-r--r--   0        0        0      616 2024-05-29 00:18:21.412163 carbon_python_sdk-0.2.0/carbon/pydantic/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0      433 2024-05-29 00:18:21.412259 carbon_python_sdk-0.2.0/carbon/pydantic/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0      737 2024-05-29 00:18:21.412357 carbon_python_sdk-0.2.0/carbon/pydantic/zendesk_authentication.py
--rw-r--r--   0        0        0      848 2024-05-29 00:18:21.412456 carbon_python_sdk-0.2.0/carbon/pydantic/zotero_authentication.py
--rw-r--r--   0        0        0      654 2024-05-29 00:18:21.412623 carbon_python_sdk-0.2.0/carbon/request_after_hook.py
--rw-r--r--   0        0        0      712 2024-05-29 00:18:21.412746 carbon_python_sdk-0.2.0/carbon/request_before_hook.py
--rw-r--r--   0        0        0      677 2024-05-29 00:18:21.412865 carbon_python_sdk-0.2.0/carbon/request_before_url_hook.py
--rw-r--r--   0        0        0    10974 2024-05-29 00:18:21.412998 carbon_python_sdk-0.2.0/carbon/rest.py
--rw-r--r--   0        0        0    96042 2024-05-29 00:18:21.413237 carbon_python_sdk-0.2.0/carbon/schemas.py
--rw-r--r--   0        0        0        0 2024-05-29 00:18:21.413422 carbon_python_sdk-0.2.0/carbon/type/__init__.py
--rw-r--r--   0        0        0      525 2024-05-29 00:18:21.413557 carbon_python_sdk-0.2.0/carbon/type/add_webhook_props.py
--rw-r--r--   0        0        0      627 2024-05-29 00:18:21.413788 carbon_python_sdk-0.2.0/carbon/type/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0      628 2024-05-29 00:18:21.413902 carbon_python_sdk-0.2.0/carbon/type/chunk_properties.py
--rw-r--r--   0        0        0      668 2024-05-29 00:18:21.414026 carbon_python_sdk-0.2.0/carbon/type/chunk_properties_nullable.py
--rw-r--r--   0        0        0      725 2024-05-29 00:18:21.414147 carbon_python_sdk-0.2.0/carbon/type/chunks_and_embeddings.py
--rw-r--r--   0        0        0      408 2024-05-29 00:18:21.414286 carbon_python_sdk-0.2.0/carbon/type/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1117 2024-05-29 00:18:21.414412 carbon_python_sdk-0.2.0/carbon/type/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0      377 2024-05-29 00:18:21.414545 carbon_python_sdk-0.2.0/carbon/type/chunks_and_embeddings_upload_input_custom_credentials.py
--rw-r--r--   0        0        0      346 2024-05-29 00:18:21.414645 carbon_python_sdk-0.2.0/carbon/type/configuration_keys.py
--rw-r--r--   0        0        0      714 2024-05-29 00:18:21.414754 carbon_python_sdk-0.2.0/carbon/type/confluence_authentication.py
--rw-r--r--   0        0        0     1664 2024-05-29 00:18:21.414853 carbon_python_sdk-0.2.0/carbon/type/connect_data_source_input.py
--rw-r--r--   0        0        0      733 2024-05-29 00:18:21.414965 carbon_python_sdk-0.2.0/carbon/type/connect_data_source_response.py
--rw-r--r--   0        0        0      420 2024-05-29 00:18:21.415094 carbon_python_sdk-0.2.0/carbon/type/custom_credentials_type.py
--rw-r--r--   0        0        0      352 2024-05-29 00:18:21.415216 carbon_python_sdk-0.2.0/carbon/type/data_source_extended_input.py
--rw-r--r--   0        0        0      395 2024-05-29 00:18:21.415324 carbon_python_sdk-0.2.0/carbon/type/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      411 2024-05-29 00:18:21.415425 carbon_python_sdk-0.2.0/carbon/type/data_source_sync_statuses.py
--rw-r--r--   0        0        0      829 2024-05-29 00:21:37.965633 carbon_python_sdk-0.2.0/carbon/type/data_source_type.py
--rw-r--r--   0        0        0      837 2024-05-29 00:21:37.966879 carbon_python_sdk-0.2.0/carbon/type/data_source_type_nullable.py
--rw-r--r--   0        0        0      929 2024-05-29 00:18:21.415732 carbon_python_sdk-0.2.0/carbon/type/delete_files_query_input.py
--rw-r--r--   0        0        0      387 2024-05-29 00:18:21.415836 carbon_python_sdk-0.2.0/carbon/type/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0      723 2024-05-29 00:18:21.415931 carbon_python_sdk-0.2.0/carbon/type/delete_files_v2_query_input.py
--rw-r--r--   0        0        0      647 2024-05-29 00:18:21.416026 carbon_python_sdk-0.2.0/carbon/type/delete_users_input.py
--rw-r--r--   0        0        0      369 2024-05-29 00:18:21.416123 carbon_python_sdk-0.2.0/carbon/type/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0      574 2024-05-29 00:18:21.416235 carbon_python_sdk-0.2.0/carbon/type/directory_item.py
--rw-r--r--   0        0        0     1356 2024-05-29 00:18:21.416333 carbon_python_sdk-0.2.0/carbon/type/document_response.py
--rw-r--r--   0        0        0      641 2024-05-29 00:18:21.416426 carbon_python_sdk-0.2.0/carbon/type/document_response_list.py
--rw-r--r--   0        0        0      350 2024-05-29 00:18:21.416517 carbon_python_sdk-0.2.0/carbon/type/document_response_tags.py
--rw-r--r--   0        0        0      402 2024-05-29 00:18:21.416615 carbon_python_sdk-0.2.0/carbon/type/document_response_vector.py
--rw-r--r--   0        0        0      877 2024-05-29 00:18:21.416711 carbon_python_sdk-0.2.0/carbon/type/embedding_and_chunk.py
--rw-r--r--   0        0        0      406 2024-05-29 00:18:21.416816 carbon_python_sdk-0.2.0/carbon/type/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0      682 2024-05-29 00:18:21.416908 carbon_python_sdk-0.2.0/carbon/type/embedding_generators.py
--rw-r--r--   0        0        0      690 2024-05-29 00:18:21.417005 carbon_python_sdk-0.2.0/carbon/type/embedding_generators_nullable.py
--rw-r--r--   0        0        0      610 2024-05-29 00:18:21.417103 carbon_python_sdk-0.2.0/carbon/type/embedding_properties.py
--rw-r--r--   0        0        0      729 2024-05-29 00:18:21.417195 carbon_python_sdk-0.2.0/carbon/type/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0      409 2024-05-29 00:18:21.417295 carbon_python_sdk-0.2.0/carbon/type/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0     1009 2024-05-29 00:18:21.417389 carbon_python_sdk-0.2.0/carbon/type/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0      694 2024-05-29 00:18:21.417483 carbon_python_sdk-0.2.0/carbon/type/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0      492 2024-05-29 00:18:21.417572 carbon_python_sdk-0.2.0/carbon/type/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1189 2024-05-29 00:18:21.417664 carbon_python_sdk-0.2.0/carbon/type/external_source_item.py
--rw-r--r--   0        0        0      394 2024-05-29 00:18:21.417751 carbon_python_sdk-0.2.0/carbon/type/external_source_items_order_by.py
--rw-r--r--   0        0        0      689 2024-05-29 00:18:21.418101 carbon_python_sdk-0.2.0/carbon/type/fetch_urls_response.py
--rw-r--r--   0        0        0      363 2024-05-29 00:18:21.418216 carbon_python_sdk-0.2.0/carbon/type/fetch_urls_response_urls.py
--rw-r--r--   0        0        0      384 2024-05-29 00:21:37.967846 carbon_python_sdk-0.2.0/carbon/type/file_content_types.py
--rw-r--r--   0        0        0      392 2024-05-29 00:21:37.968732 carbon_python_sdk-0.2.0/carbon/type/file_content_types_nullable.py
--rw-r--r--   0        0        0      759 2024-05-29 00:21:37.969116 carbon_python_sdk-0.2.0/carbon/type/file_formats.py
--rw-r--r--   0        0        0      767 2024-05-29 00:21:37.969404 carbon_python_sdk-0.2.0/carbon/type/file_formats_nullable.py
--rw-r--r--   0        0        0      823 2024-05-29 00:18:21.418762 carbon_python_sdk-0.2.0/carbon/type/file_statistics.py
--rw-r--r--   0        0        0      863 2024-05-29 00:18:21.418858 carbon_python_sdk-0.2.0/carbon/type/file_statistics_nullable.py
--rw-r--r--   0        0        0     1035 2024-05-29 00:18:21.418943 carbon_python_sdk-0.2.0/carbon/type/file_sync_config.py
--rw-r--r--   0        0        0     1075 2024-05-29 00:18:21.419030 carbon_python_sdk-0.2.0/carbon/type/file_sync_config_nullable.py
--rw-r--r--   0        0        0      427 2024-05-29 00:18:21.419128 carbon_python_sdk-0.2.0/carbon/type/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     1449 2024-05-29 00:18:21.419211 carbon_python_sdk-0.2.0/carbon/type/fresh_desk_connect_request.py
--rw-r--r--   0        0        0      669 2024-05-29 00:18:21.419293 carbon_python_sdk-0.2.0/carbon/type/freskdesk_authentication.py
--rw-r--r--   0        0        0      565 2024-05-29 00:18:21.419380 carbon_python_sdk-0.2.0/carbon/type/generic_success_response.py
--rw-r--r--   0        0        0     2735 2024-05-29 00:18:21.419497 carbon_python_sdk-0.2.0/carbon/type/get_embedding_documents_body.py
--rw-r--r--   0        0        0      391 2024-05-29 00:18:21.419586 carbon_python_sdk-0.2.0/carbon/type/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0      397 2024-05-29 00:18:21.419671 carbon_python_sdk-0.2.0/carbon/type/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0      416 2024-05-29 00:18:21.419759 carbon_python_sdk-0.2.0/carbon/type/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0      359 2024-05-29 00:18:21.419857 carbon_python_sdk-0.2.0/carbon/type/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0      670 2024-05-29 00:18:21.419947 carbon_python_sdk-0.2.0/carbon/type/gitbook_authetication.py
--rw-r--r--   0        0        0     1272 2024-05-29 00:18:21.420031 carbon_python_sdk-0.2.0/carbon/type/gitbook_connect_request.py
--rw-r--r--   0        0        0     1168 2024-05-29 00:18:21.420114 carbon_python_sdk-0.2.0/carbon/type/gitbook_sync_request.py
--rw-r--r--   0        0        0      368 2024-05-29 00:18:21.420199 carbon_python_sdk-0.2.0/carbon/type/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0      661 2024-05-29 00:18:21.420296 carbon_python_sdk-0.2.0/carbon/type/github_authentication.py
--rw-r--r--   0        0        0      709 2024-05-29 00:18:21.420383 carbon_python_sdk-0.2.0/carbon/type/github_connect_request.py
--rw-r--r--   0        0        0      711 2024-05-29 00:18:21.420468 carbon_python_sdk-0.2.0/carbon/type/github_fetch_repos_request.py
--rw-r--r--   0        0        0      370 2024-05-29 00:18:21.420566 carbon_python_sdk-0.2.0/carbon/type/github_fetch_repos_request_repos.py
--rw-r--r--   0        0        0     1351 2024-05-29 00:18:21.420650 carbon_python_sdk-0.2.0/carbon/type/gmail_sync_input.py
--rw-r--r--   0        0        0      371 2024-05-29 00:18:21.420735 carbon_python_sdk-0.2.0/carbon/type/helpdesk_file_types.py
--rw-r--r--   0        0        0      630 2024-05-29 00:18:21.420936 carbon_python_sdk-0.2.0/carbon/type/http_validation_error.py
--rw-r--r--   0        0        0      636 2024-05-29 00:18:21.421025 carbon_python_sdk-0.2.0/carbon/type/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0      676 2024-05-29 00:18:21.421119 carbon_python_sdk-0.2.0/carbon/type/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0     1025 2024-05-29 00:18:21.421217 carbon_python_sdk-0.2.0/carbon/type/list_data_source_items_request.py
--rw-r--r--   0        0        0      695 2024-05-29 00:18:21.421312 carbon_python_sdk-0.2.0/carbon/type/list_data_source_items_response.py
--rw-r--r--   0        0        0      854 2024-05-29 00:18:21.421411 carbon_python_sdk-0.2.0/carbon/type/list_items_filters.py
--rw-r--r--   0        0        0      386 2024-05-29 00:18:21.421511 carbon_python_sdk-0.2.0/carbon/type/list_items_filters_external_ids.py
--rw-r--r--   0        0        0      378 2024-05-29 00:18:21.421605 carbon_python_sdk-0.2.0/carbon/type/list_items_filters_ids.py
--rw-r--r--   0        0        0      944 2024-05-29 00:18:21.421702 carbon_python_sdk-0.2.0/carbon/type/list_items_filters_nullable.py
--rw-r--r--   0        0        0      394 2024-05-29 00:18:21.421798 carbon_python_sdk-0.2.0/carbon/type/list_items_filters_nullable_external_ids.py
--rw-r--r--   0        0        0      386 2024-05-29 00:18:21.421893 carbon_python_sdk-0.2.0/carbon/type/list_items_filters_nullable_ids.py
--rw-r--r--   0        0        0      544 2024-05-29 00:18:21.421977 carbon_python_sdk-0.2.0/carbon/type/list_request.py
--rw-r--r--   0        0        0      587 2024-05-29 00:18:21.422062 carbon_python_sdk-0.2.0/carbon/type/list_response.py
--rw-r--r--   0        0        0      709 2024-05-29 00:18:21.422142 carbon_python_sdk-0.2.0/carbon/type/modify_user_configuration_input.py
--rw-r--r--   0        0        0      665 2024-05-29 00:18:21.422228 carbon_python_sdk-0.2.0/carbon/type/notion_authentication.py
--rw-r--r--   0        0        0      696 2024-05-29 00:18:21.422311 carbon_python_sdk-0.2.0/carbon/type/o_auth_authentication.py
--rw-r--r--   0        0        0     3249 2024-05-29 00:21:37.969823 carbon_python_sdk-0.2.0/carbon/type/o_auth_url_request.py
--rw-r--r--   0        0        0      356 2024-05-29 00:18:21.422482 carbon_python_sdk-0.2.0/carbon/type/order_dir.py
--rw-r--r--   0        0        0      358 2024-05-29 00:18:21.422567 carbon_python_sdk-0.2.0/carbon/type/order_dir_v2.py
--rw-r--r--   0        0        0     1922 2024-05-29 00:21:37.970197 carbon_python_sdk-0.2.0/carbon/type/organization_response.py
--rw-r--r--   0        0        0     1567 2024-05-29 00:18:21.422743 carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_api.py
--rw-r--r--   0        0        0      937 2024-05-29 00:18:21.422832 carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_filters.py
--rw-r--r--   0        0        0      395 2024-05-29 00:18:21.422918 carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0      401 2024-05-29 00:18:21.422999 carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0     1070 2024-05-29 00:18:21.423084 carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0      767 2024-05-29 00:18:21.423169 carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_response.py
--rw-r--r--   0        0        0      759 2024-05-29 00:18:21.423252 carbon_python_sdk-0.2.0/carbon/type/organization_user_file_tag_create.py
--rw-r--r--   0        0        0      363 2024-05-29 00:18:21.423332 carbon_python_sdk-0.2.0/carbon/type/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0      767 2024-05-29 00:18:21.423413 carbon_python_sdk-0.2.0/carbon/type/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0      376 2024-05-29 00:18:21.423495 carbon_python_sdk-0.2.0/carbon/type/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     5041 2024-05-29 00:18:21.423599 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0      408 2024-05-29 00:18:21.423692 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0      396 2024-05-29 00:18:21.423788 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0      421 2024-05-29 00:18:21.423905 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0      406 2024-05-29 00:18:21.424004 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0      403 2024-05-29 00:18:21.424103 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters_request_ids.py
--rw-r--r--   0        0        0      368 2024-05-29 00:18:21.424196 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0      440 2024-05-29 00:18:21.424295 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1228 2024-05-29 00:18:21.424518 carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0      531 2024-05-29 00:18:21.424614 carbon_python_sdk-0.2.0/carbon/type/outh_url_response.py
--rw-r--r--   0        0        0     1395 2024-05-29 00:18:21.424704 carbon_python_sdk-0.2.0/carbon/type/outlook_sync_input.py
--rw-r--r--   0        0        0      519 2024-05-29 00:18:21.424797 carbon_python_sdk-0.2.0/carbon/type/pagination.py
--rw-r--r--   0        0        0      560 2024-05-29 00:18:21.424891 carbon_python_sdk-0.2.0/carbon/type/presigned_url_response.py
--rw-r--r--   0        0        0      900 2024-05-29 00:18:21.424972 carbon_python_sdk-0.2.0/carbon/type/raw_text_input.py
--rw-r--r--   0        0        0      662 2024-05-29 00:18:21.425055 carbon_python_sdk-0.2.0/carbon/type/resync_file_query_input.py
--rw-r--r--   0        0        0      571 2024-05-29 00:18:21.425138 carbon_python_sdk-0.2.0/carbon/type/revoke_access_token_input.py
--rw-r--r--   0        0        0     1002 2024-05-29 00:18:21.425224 carbon_python_sdk-0.2.0/carbon/type/rss_feed_input.py
--rw-r--r--   0        0        0      681 2024-05-29 00:18:21.425305 carbon_python_sdk-0.2.0/carbon/type/s3_auth_request.py
--rw-r--r--   0        0        0      648 2024-05-29 00:18:21.425389 carbon_python_sdk-0.2.0/carbon/type/s3_authentication.py
--rw-r--r--   0        0        0     1521 2024-05-29 00:18:21.425478 carbon_python_sdk-0.2.0/carbon/type/s3_file_sync_input.py
--rw-r--r--   0        0        0      570 2024-05-29 00:18:21.425561 carbon_python_sdk-0.2.0/carbon/type/s3_get_file_input.py
--rw-r--r--   0        0        0      711 2024-05-29 00:18:21.425646 carbon_python_sdk-0.2.0/carbon/type/salesforce_authentication.py
--rw-r--r--   0        0        0      736 2024-05-29 00:18:21.425728 carbon_python_sdk-0.2.0/carbon/type/sharepoint_authentication.py
--rw-r--r--   0        0        0      433 2024-05-29 00:18:21.425836 carbon_python_sdk-0.2.0/carbon/type/simple_o_auth_data_sources.py
--rw-r--r--   0        0        0      831 2024-05-29 00:18:21.426051 carbon_python_sdk-0.2.0/carbon/type/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     1662 2024-05-29 00:18:21.426134 carbon_python_sdk-0.2.0/carbon/type/sitemap_scrape_request.py
--rw-r--r--   0        0        0      395 2024-05-29 00:18:21.426215 carbon_python_sdk-0.2.0/carbon/type/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      397 2024-05-29 00:18:21.426297 carbon_python_sdk-0.2.0/carbon/type/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      393 2024-05-29 00:18:21.426378 carbon_python_sdk-0.2.0/carbon/type/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      354 2024-05-29 00:18:21.426462 carbon_python_sdk-0.2.0/carbon/type/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0      561 2024-05-29 00:18:21.426550 carbon_python_sdk-0.2.0/carbon/type/sync_directory_request.py
--rw-r--r--   0        0        0      527 2024-05-29 00:18:21.426633 carbon_python_sdk-0.2.0/carbon/type/sync_files_ids.py
--rw-r--r--   0        0        0     1816 2024-05-29 00:18:21.426715 carbon_python_sdk-0.2.0/carbon/type/sync_files_request.py
--rw-r--r--   0        0        0     2058 2024-05-29 00:18:21.426794 carbon_python_sdk-0.2.0/carbon/type/sync_options.py
--rw-r--r--   0        0        0      665 2024-05-29 00:18:21.426877 carbon_python_sdk-0.2.0/carbon/type/text_embedding_generators.py
--rw-r--r--   0        0        0      548 2024-05-29 00:18:21.426967 carbon_python_sdk-0.2.0/carbon/type/token_response.py
--rw-r--r--   0        0        0      697 2024-05-29 00:18:21.427058 carbon_python_sdk-0.2.0/carbon/type/update_organization_input.py
--rw-r--r--   0        0        0     1513 2024-05-29 00:18:21.427145 carbon_python_sdk-0.2.0/carbon/type/update_users_input.py
--rw-r--r--   0        0        0      369 2024-05-29 00:18:21.427242 carbon_python_sdk-0.2.0/carbon/type/update_users_input_customer_ids.py
--rw-r--r--   0        0        0     1133 2024-05-29 00:18:21.427341 carbon_python_sdk-0.2.0/carbon/type/upload_file_from_url_input.py
--rw-r--r--   0        0        0     1396 2024-05-29 00:18:21.427438 carbon_python_sdk-0.2.0/carbon/type/user_configuration.py
--rw-r--r--   0        0        0     1436 2024-05-29 00:18:21.427534 carbon_python_sdk-0.2.0/carbon/type/user_configuration_nullable.py
--rw-r--r--   0        0        0     2555 2024-05-29 00:18:21.427618 carbon_python_sdk-0.2.0/carbon/type/user_file.py
--rw-r--r--   0        0        0      422 2024-05-29 00:18:21.427706 carbon_python_sdk-0.2.0/carbon/type/user_file_embedding_properties.py
--rw-r--r--   0        0        0      586 2024-05-29 00:18:21.427799 carbon_python_sdk-0.2.0/carbon/type/user_files_v2.py
--rw-r--r--   0        0        0      548 2024-05-29 00:18:21.428026 carbon_python_sdk-0.2.0/carbon/type/user_request_content.py
--rw-r--r--   0        0        0     2011 2024-05-29 00:21:37.970937 carbon_python_sdk-0.2.0/carbon/type/user_response.py
--rw-r--r--   0        0        0      442 2024-05-29 00:18:21.428196 carbon_python_sdk-0.2.0/carbon/type/user_response_auto_sync_enabled_sources.py
--rw-r--r--   0        0        0      371 2024-05-29 00:18:21.428281 carbon_python_sdk-0.2.0/carbon/type/user_response_unique_file_tags.py
--rw-r--r--   0        0        0      439 2024-05-29 00:18:21.428375 carbon_python_sdk-0.2.0/carbon/type/utilities_scrape_web_request.py
--rw-r--r--   0        0        0      633 2024-05-29 00:18:21.428454 carbon_python_sdk-0.2.0/carbon/type/validation_error.py
--rw-r--r--   0        0        0      379 2024-05-29 00:18:21.428532 carbon_python_sdk-0.2.0/carbon/type/validation_error_loc.py
--rw-r--r--   0        0        0      719 2024-05-29 00:21:37.972176 carbon_python_sdk-0.2.0/carbon/type/webhook.py
--rw-r--r--   0        0        0      613 2024-05-29 00:18:21.428687 carbon_python_sdk-0.2.0/carbon/type/webhook_filters.py
--rw-r--r--   0        0        0      376 2024-05-29 00:18:21.428764 carbon_python_sdk-0.2.0/carbon/type/webhook_filters_ids.py
--rw-r--r--   0        0        0      722 2024-05-29 00:21:37.973095 carbon_python_sdk-0.2.0/carbon/type/webhook_no_key.py
--rw-r--r--   0        0        0      382 2024-05-29 00:18:21.428923 carbon_python_sdk-0.2.0/carbon/type/webhook_order_by_columns.py
--rw-r--r--   0        0        0      855 2024-05-29 00:18:21.429003 carbon_python_sdk-0.2.0/carbon/type/webhook_query_input.py
--rw-r--r--   0        0        0      644 2024-05-29 00:18:21.429085 carbon_python_sdk-0.2.0/carbon/type/webhook_query_response.py
--rw-r--r--   0        0        0      367 2024-05-29 00:21:37.973298 carbon_python_sdk-0.2.0/carbon/type/webhook_status.py
--rw-r--r--   0        0        0     1633 2024-05-29 00:18:21.429243 carbon_python_sdk-0.2.0/carbon/type/webscrape_request.py
--rw-r--r--   0        0        0      391 2024-05-29 00:18:21.429327 carbon_python_sdk-0.2.0/carbon/type/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      393 2024-05-29 00:18:21.429413 carbon_python_sdk-0.2.0/carbon/type/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      389 2024-05-29 00:18:21.429496 carbon_python_sdk-0.2.0/carbon/type/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      350 2024-05-29 00:18:21.429578 carbon_python_sdk-0.2.0/carbon/type/webscrape_request_tags.py
--rw-r--r--   0        0        0      675 2024-05-29 00:18:21.429658 carbon_python_sdk-0.2.0/carbon/type/white_labeling_response.py
--rw-r--r--   0        0        0      826 2024-05-29 00:18:21.429742 carbon_python_sdk-0.2.0/carbon/type/youtube_transcript_response.py
--rw-r--r--   0        0        0      551 2024-05-29 00:18:21.429833 carbon_python_sdk-0.2.0/carbon/type/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0      372 2024-05-29 00:18:21.429926 carbon_python_sdk-0.2.0/carbon/type/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0      667 2024-05-29 00:18:21.430014 carbon_python_sdk-0.2.0/carbon/type/zendesk_authentication.py
--rw-r--r--   0        0        0      711 2024-05-29 00:18:21.430106 carbon_python_sdk-0.2.0/carbon/type/zotero_authentication.py
--rw-r--r--   0        0        0      514 2024-05-29 00:18:21.430201 carbon_python_sdk-0.2.0/carbon/type_util.py
--rw-r--r--   0        0        0     3162 2024-05-29 00:18:21.430296 carbon_python_sdk-0.2.0/carbon/validation_metadata.py
--rw-r--r--   0        0        0      746 2024-05-29 00:21:37.974084 carbon_python_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0   113673 1970-01-01 00:00:00.000000 carbon_python_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-30 19:55:10.782600 carbon_python_sdk-0.2.1/LICENSE
+-rw-r--r--   0        0        0   112828 2024-05-30 19:57:32.272363 carbon_python_sdk-0.2.1/README.md
+-rw-r--r--   0        0        0      675 2024-05-30 19:57:32.272988 carbon_python_sdk-0.2.1/carbon/__init__.py
+-rw-r--r--   0        0        0    76940 2024-05-30 19:57:32.274703 carbon_python_sdk-0.2.1/carbon/api_client.py
+-rw-r--r--   0        0        0      663 2024-05-30 19:55:10.639307 carbon_python_sdk-0.2.1/carbon/api_response.py
+-rw-r--r--   0        0        0      214 2024-05-30 19:55:10.639416 carbon_python_sdk-0.2.1/carbon/apis/__init__.py
+-rw-r--r--   0        0        0    11104 2024-05-30 19:55:10.639511 carbon_python_sdk-0.2.1/carbon/apis/path_to_api.py
+-rw-r--r--   0        0        0      233 2024-05-30 19:55:10.639705 carbon_python_sdk-0.2.1/carbon/apis/paths/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-30 19:55:10.639790 carbon_python_sdk-0.2.1/carbon/apis/paths/add_webhook.py
+-rw-r--r--   0        0        0      114 2024-05-30 19:55:10.639877 carbon_python_sdk-0.2.1/carbon/apis/paths/auth_v1_access_token.py
+-rw-r--r--   0        0        0      118 2024-05-30 19:55:10.639963 carbon_python_sdk-0.2.1/carbon/apis/paths/auth_v1_white_labeling.py
+-rw-r--r--   0        0        0      119 2024-05-30 19:55:10.640210 carbon_python_sdk-0.2.1/carbon/apis/paths/create_user_file_tags.py
+-rw-r--r--   0        0        0      103 2024-05-30 19:55:10.640347 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_files.py
+-rw-r--r--   0        0        0      108 2024-05-30 19:55:10.640448 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_files_v2.py
+-rw-r--r--   0        0        0      119 2024-05-30 19:55:10.640540 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_user_file_tags.py
+-rw-r--r--   0        0        0      103 2024-05-30 19:55:10.640627 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_users.py
+-rw-r--r--   0        0        0      133 2024-05-30 19:55:10.640715 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_webhook_webhook_id.py
+-rw-r--r--   0        0        0      120 2024-05-30 19:55:10.640803 carbon_python_sdk-0.2.1/carbon/apis/paths/deletefile_file_id.py
+-rw-r--r--   0        0        0      100 2024-05-30 19:55:10.640891 carbon_python_sdk-0.2.1/carbon/apis/paths/embeddings.py
+-rw-r--r--   0        0        0       96 2024-05-30 19:55:10.640978 carbon_python_sdk-0.2.1/carbon/apis/paths/fetch_urls.py
+-rw-r--r--   0        0        0      123 2024-05-30 19:55:10.641072 carbon_python_sdk-0.2.1/carbon/apis/paths/fetch_youtube_transcript.py
+-rw-r--r--   0        0        0       89 2024-05-30 19:55:10.641154 carbon_python_sdk-0.2.1/carbon/apis/paths/health.py
+-rw-r--r--   0        0        0      134 2024-05-30 19:55:10.641235 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_confluence_list.py
+-rw-r--r--   0        0        0      134 2024-05-30 19:55:10.641317 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_confluence_sync.py
+-rw-r--r--   0        0        0      119 2024-05-30 19:55:10.641399 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_connect.py
+-rw-r--r--   0        0        0      124 2024-05-30 19:55:10.641482 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_files_sync.py
+-rw-r--r--   0        0        0      123 2024-05-30 19:55:10.641564 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_freshdesk.py
+-rw-r--r--   0        0        0      119 2024-05-30 19:55:10.641644 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gitbook.py
+-rw-r--r--   0        0        0      129 2024-05-30 19:55:10.641725 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gitbook_spaces.py
+-rw-r--r--   0        0        0      128 2024-05-30 19:55:10.641811 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gitbook_sync.py
+-rw-r--r--   0        0        0      117 2024-05-30 19:55:10.641897 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_github.py
+-rw-r--r--   0        0        0      125 2024-05-30 19:55:10.641993 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_github_repos.py
+-rw-r--r--   0        0        0      137 2024-05-30 19:55:10.642079 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_github_sync_repos.py
+-rw-r--r--   0        0        0      124 2024-05-30 19:55:10.642164 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gmail_sync.py
+-rw-r--r--   0        0        0      134 2024-05-30 19:55:10.642252 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gmail_user_labels.py
+-rw-r--r--   0        0        0      124 2024-05-30 19:55:10.642339 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_items_list.py
+-rw-r--r--   0        0        0      124 2024-05-30 19:55:10.642419 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_items_sync.py
+-rw-r--r--   0        0        0      122 2024-05-30 19:55:10.642499 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_oauth_url.py
+-rw-r--r--   0        0        0      128 2024-05-30 19:55:10.642586 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_outlook_sync.py
+-rw-r--r--   0        0        0      146 2024-05-30 19:55:10.642674 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_outlook_user_categories.py
+-rw-r--r--   0        0        0      140 2024-05-30 19:55:10.642757 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_outlook_user_folders.py
+-rw-r--r--   0        0        0      120 2024-05-30 19:55:10.642840 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_rss_feed.py
+-rw-r--r--   0        0        0      109 2024-05-30 19:55:10.642921 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_s3.py
+-rw-r--r--   0        0        0      120 2024-05-30 19:55:10.643007 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_s3_files.py
+-rw-r--r--   0        0        0      128 2024-05-30 19:55:10.643095 carbon_python_sdk-0.2.1/carbon/apis/paths/modify_user_configuration.py
+-rw-r--r--   0        0        0      101 2024-05-30 19:55:10.643332 carbon_python_sdk-0.2.1/carbon/apis/paths/organization.py
+-rw-r--r--   0        0        0      125 2024-05-30 19:55:10.643422 carbon_python_sdk-0.2.1/carbon/apis/paths/organization_statistics.py
+-rw-r--r--   0        0        0      117 2024-05-30 19:55:10.643518 carbon_python_sdk-0.2.1/carbon/apis/paths/organization_update.py
+-rw-r--r--   0        0        0      112 2024-05-30 19:55:10.643604 carbon_python_sdk-0.2.1/carbon/apis/paths/parsed_file_file_id.py
+-rw-r--r--   0        0        0      106 2024-05-30 19:55:10.643687 carbon_python_sdk-0.2.1/carbon/apis/paths/process_sitemap.py
+-rw-r--r--   0        0        0      106 2024-05-30 19:55:10.643766 carbon_python_sdk-0.2.1/carbon/apis/paths/raw_file_file_id.py
+-rw-r--r--   0        0        0      101 2024-05-30 19:55:10.643852 carbon_python_sdk-0.2.1/carbon/apis/paths/resync_file.py
+-rw-r--r--   0        0        0      116 2024-05-30 19:55:10.643941 carbon_python_sdk-0.2.1/carbon/apis/paths/revoke_access_token.py
+-rw-r--r--   0        0        0      107 2024-05-30 19:55:10.644023 carbon_python_sdk-0.2.1/carbon/apis/paths/scrape_sitemap.py
+-rw-r--r--   0        0        0       98 2024-05-30 19:55:10.644104 carbon_python_sdk-0.2.1/carbon/apis/paths/search_urls.py
+-rw-r--r--   0        0        0      101 2024-05-30 19:55:10.644183 carbon_python_sdk-0.2.1/carbon/apis/paths/text_chunks.py
+-rw-r--r--   0        0        0      103 2024-05-30 19:55:10.644262 carbon_python_sdk-0.2.1/carbon/apis/paths/update_users.py
+-rw-r--r--   0        0        0      133 2024-05-30 19:55:10.644340 carbon_python_sdk-0.2.1/carbon/apis/paths/upload_chunks_and_embeddings.py
+-rw-r--r--   0        0        0      117 2024-05-30 19:55:10.644424 carbon_python_sdk-0.2.1/carbon/apis/paths/upload_file_from_url.py
+-rw-r--r--   0        0        0      101 2024-05-30 19:55:10.644500 carbon_python_sdk-0.2.1/carbon/apis/paths/upload_text.py
+-rw-r--r--   0        0        0      100 2024-05-30 19:55:10.644579 carbon_python_sdk-0.2.1/carbon/apis/paths/uploadfile.py
+-rw-r--r--   0        0        0       88 2024-05-30 19:55:10.644658 carbon_python_sdk-0.2.1/carbon/apis/paths/user.py
+-rw-r--r--   0        0        0      112 2024-05-30 19:55:10.644745 carbon_python_sdk-0.2.1/carbon/apis/paths/user_data_sources.py
+-rw-r--r--   0        0        0       99 2024-05-30 19:55:10.644831 carbon_python_sdk-0.2.1/carbon/apis/paths/user_files.py
+-rw-r--r--   0        0        0      104 2024-05-30 19:55:10.644916 carbon_python_sdk-0.2.1/carbon/apis/paths/user_files_v2.py
+-rw-r--r--   0        0        0       99 2024-05-30 19:55:10.644999 carbon_python_sdk-0.2.1/carbon/apis/paths/web_scrape.py
+-rw-r--r--   0        0        0       96 2024-05-30 19:55:10.645082 carbon_python_sdk-0.2.1/carbon/apis/paths/webhooks.py
+-rw-r--r--   0        0        0     2044 2024-05-30 19:55:10.645166 carbon_python_sdk-0.2.1/carbon/apis/tag_to_api.py
+-rw-r--r--   0        0        0      655 2024-05-30 19:55:10.645270 carbon_python_sdk-0.2.1/carbon/apis/tags/__init__.py
+-rw-r--r--   0        0        0      125 2024-05-30 19:55:10.645348 carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api.py
+-rw-r--r--   0        0        0      671 2024-05-30 19:55:10.645433 carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api_generated.py
+-rw-r--r--   0        0        0      493 2024-05-30 19:55:10.645515 carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api_raw.py
+-rw-r--r--   0        0        0      154 2024-05-30 19:55:10.645597 carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api.py
+-rw-r--r--   0        0        0      717 2024-05-30 19:55:10.645682 carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api_generated.py
+-rw-r--r--   0        0        0      510 2024-05-30 19:55:10.645763 carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api_raw.py
+-rw-r--r--   0        0        0      149 2024-05-30 19:55:10.645848 carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api.py
+-rw-r--r--   0        0        0      806 2024-05-30 19:55:10.645933 carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_generated.py
+-rw-r--r--   0        0        0      610 2024-05-30 19:55:10.646012 carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_raw.py
+-rw-r--r--   0        0        0      129 2024-05-30 19:55:10.646090 carbon_python_sdk-0.2.1/carbon/apis/tags/files_api.py
+-rw-r--r--   0        0        0     1495 2024-05-30 19:55:10.646295 carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_generated.py
+-rw-r--r--   0        0        0     1379 2024-05-30 19:55:10.646406 carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_raw.py
+-rw-r--r--   0        0        0      133 2024-05-30 19:55:10.646492 carbon_python_sdk-0.2.1/carbon/apis/tags/health_api.py
+-rw-r--r--   0        0        0      558 2024-05-30 19:55:10.646578 carbon_python_sdk-0.2.1/carbon/apis/tags/health_api_generated.py
+-rw-r--r--   0        0        0      366 2024-05-30 19:55:10.646666 carbon_python_sdk-0.2.1/carbon/apis/tags/health_api_raw.py
+-rw-r--r--   0        0        0      157 2024-05-30 19:55:10.646744 carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api.py
+-rw-r--r--   0        0        0     2493 2024-05-30 19:55:10.646827 carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_generated.py
+-rw-r--r--   0        0        0     2403 2024-05-30 19:55:10.646903 carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_raw.py
+-rw-r--r--   0        0        0      161 2024-05-30 19:55:10.646982 carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api.py
+-rw-r--r--   0        0        0      747 2024-05-30 19:55:10.647061 carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_generated.py
+-rw-r--r--   0        0        0      539 2024-05-30 19:55:10.647142 carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_raw.py
+-rw-r--r--   0        0        0      129 2024-05-30 19:55:10.647225 carbon_python_sdk-0.2.1/carbon/apis/tags/users_api.py
+-rw-r--r--   0        0        0      781 2024-05-30 19:55:10.647306 carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_generated.py
+-rw-r--r--   0        0        0      611 2024-05-30 19:55:10.647383 carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_raw.py
+-rw-r--r--   0        0        0      145 2024-05-30 19:55:10.647462 carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api.py
+-rw-r--r--   0        0        0      984 2024-05-30 19:55:10.647544 carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_generated.py
+-rw-r--r--   0        0        0      810 2024-05-30 19:55:10.647622 carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_raw.py
+-rw-r--r--   0        0        0      141 2024-05-30 19:55:10.647698 carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api.py
+-rw-r--r--   0        0        0      713 2024-05-30 19:55:10.647778 carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_generated.py
+-rw-r--r--   0        0        0      525 2024-05-30 19:55:10.647859 carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_raw.py
+-rw-r--r--   0        0        0     1986 2024-05-30 19:55:10.647939 carbon_python_sdk-0.2.1/carbon/client.py
+-rw-r--r--   0        0        0     1986 2024-05-30 19:55:10.648012 carbon_python_sdk-0.2.1/carbon/client.pyi
+-rw-r--r--   0        0        0      676 2024-05-30 19:55:10.648089 carbon_python_sdk-0.2.1/carbon/client_custom.py
+-rw-r--r--   0        0        0    17804 2024-05-30 19:57:32.275865 carbon_python_sdk-0.2.1/carbon/configuration.py
+-rw-r--r--   0        0        0     7679 2024-05-30 19:55:10.648289 carbon_python_sdk-0.2.1/carbon/exceptions.py
+-rw-r--r--   0        0        0     2274 2024-05-30 19:55:10.648364 carbon_python_sdk-0.2.1/carbon/exceptions_base.py
+-rw-r--r--   0        0        0      340 2024-05-30 19:55:10.648568 carbon_python_sdk-0.2.1/carbon/model/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-30 19:55:10.648646 carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.py
+-rw-r--r--   0        0        0     2282 2024-05-30 19:55:10.648722 carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.pyi
+-rw-r--r--   0        0        0     2371 2024-05-30 19:55:10.648802 carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0     2371 2024-05-30 19:55:10.648879 carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.pyi
+-rw-r--r--   0        0        0     4752 2024-05-30 19:55:10.648965 carbon_python_sdk-0.2.1/carbon/model/chunk_properties.py
+-rw-r--r--   0        0        0     4752 2024-05-30 19:55:10.649050 carbon_python_sdk-0.2.1/carbon/model/chunk_properties.pyi
+-rw-r--r--   0        0        0     4359 2024-05-30 19:55:10.649256 carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.py
+-rw-r--r--   0        0        0     4359 2024-05-30 19:55:10.649342 carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.pyi
+-rw-r--r--   0        0        0     4319 2024-05-30 19:55:10.649430 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.py
+-rw-r--r--   0        0        0     4319 2024-05-30 19:55:10.649513 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.pyi
+-rw-r--r--   0        0        0     1100 2024-05-30 19:55:10.649588 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1100 2024-05-30 19:55:10.649667 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.pyi
+-rw-r--r--   0        0        0     6672 2024-05-30 19:55:10.649750 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     6672 2024-05-30 19:55:10.649834 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.pyi
+-rw-r--r--   0        0        0     1521 2024-05-30 19:55:10.649914 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py
+-rw-r--r--   0        0        0     1521 2024-05-30 19:55:10.649997 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi
+-rw-r--r--   0        0        0      548 2024-05-30 19:55:10.650072 carbon_python_sdk-0.2.1/carbon/model/configuration_keys.py
+-rw-r--r--   0        0        0      548 2024-05-30 19:55:10.650148 carbon_python_sdk-0.2.1/carbon/model/configuration_keys.pyi
+-rw-r--r--   0        0        0     4861 2024-05-30 19:55:10.650237 carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.py
+-rw-r--r--   0        0        0     4861 2024-05-30 19:55:10.650322 carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.pyi
+-rw-r--r--   0        0        0     6269 2024-05-30 19:55:10.650409 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.py
+-rw-r--r--   0        0        0     6269 2024-05-30 19:55:10.650494 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.pyi
+-rw-r--r--   0        0        0     3763 2024-05-30 19:55:10.650570 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.py
+-rw-r--r--   0        0        0     3763 2024-05-30 19:55:10.650647 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.pyi
+-rw-r--r--   0        0        0     1369 2024-05-30 19:55:10.650722 carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.py
+-rw-r--r--   0        0        0     1114 2024-05-30 19:55:10.650799 carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.pyi
+-rw-r--r--   0        0        0      554 2024-05-30 19:55:10.650872 carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.py
+-rw-r--r--   0        0        0      554 2024-05-30 19:55:10.650947 carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.pyi
+-rw-r--r--   0        0        0     1183 2024-05-30 19:55:10.651021 carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      998 2024-05-30 19:55:10.651099 carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.pyi
+-rw-r--r--   0        0        0     1256 2024-05-30 19:55:10.651174 carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.py
+-rw-r--r--   0        0        0     1033 2024-05-30 19:55:10.651247 carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.pyi
+-rw-r--r--   0        0        0     6578 2024-05-30 19:55:10.651329 carbon_python_sdk-0.2.1/carbon/model/data_source_type.py
+-rw-r--r--   0        0        0     4915 2024-05-30 19:55:10.651414 carbon_python_sdk-0.2.1/carbon/model/data_source_type.pyi
+-rw-r--r--   0        0        0     6953 2024-05-30 19:55:10.651500 carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.py
+-rw-r--r--   0        0        0     6953 2024-05-30 19:55:10.651584 carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.pyi
+-rw-r--r--   0        0        0     6047 2024-05-30 19:55:10.651668 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.py
+-rw-r--r--   0        0        0     6047 2024-05-30 19:55:10.651756 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.pyi
+-rw-r--r--   0        0        0     1097 2024-05-30 19:55:10.651835 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0     1097 2024-05-30 19:55:10.651911 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.pyi
+-rw-r--r--   0        0        0     3161 2024-05-30 19:55:10.651985 carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.py
+-rw-r--r--   0        0        0     3161 2024-05-30 19:55:10.652059 carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.pyi
+-rw-r--r--   0        0        0     2600 2024-05-30 19:55:10.652134 carbon_python_sdk-0.2.1/carbon/model/delete_users_input.py
+-rw-r--r--   0        0        0     2600 2024-05-30 19:55:10.652211 carbon_python_sdk-0.2.1/carbon/model/delete_users_input.pyi
+-rw-r--r--   0        0        0     1199 2024-05-30 19:55:10.652286 carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1199 2024-05-30 19:55:10.652361 carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.pyi
+-rw-r--r--   0        0        0     3902 2024-05-30 19:55:10.652435 carbon_python_sdk-0.2.1/carbon/model/directory_item.py
+-rw-r--r--   0        0        0     3902 2024-05-30 19:55:10.652512 carbon_python_sdk-0.2.1/carbon/model/directory_item.pyi
+-rw-r--r--   0        0        0    16065 2024-05-30 19:55:10.652593 carbon_python_sdk-0.2.1/carbon/model/document_response.py
+-rw-r--r--   0        0        0    16065 2024-05-30 19:55:10.652824 carbon_python_sdk-0.2.1/carbon/model/document_response.pyi
+-rw-r--r--   0        0        0     3350 2024-05-30 19:55:10.653034 carbon_python_sdk-0.2.1/carbon/model/document_response_list.py
+-rw-r--r--   0        0        0     3350 2024-05-30 19:55:10.653118 carbon_python_sdk-0.2.1/carbon/model/document_response_list.pyi
+-rw-r--r--   0        0        0     7489 2024-05-30 19:55:10.653217 carbon_python_sdk-0.2.1/carbon/model/document_response_tags.py
+-rw-r--r--   0        0        0     7489 2024-05-30 19:55:10.653532 carbon_python_sdk-0.2.1/carbon/model/document_response_tags.pyi
+-rw-r--r--   0        0        0     1088 2024-05-30 19:55:10.653728 carbon_python_sdk-0.2.1/carbon/model/document_response_vector.py
+-rw-r--r--   0        0        0     1088 2024-05-30 19:55:10.653835 carbon_python_sdk-0.2.1/carbon/model/document_response_vector.pyi
+-rw-r--r--   0        0        0     6594 2024-05-30 19:55:10.653948 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.py
+-rw-r--r--   0        0        0     6594 2024-05-30 19:55:10.654057 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.pyi
+-rw-r--r--   0        0        0     1096 2024-05-30 19:55:10.654159 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0     1096 2024-05-30 19:55:10.654257 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.pyi
+-rw-r--r--   0        0        0     3163 2024-05-30 19:55:10.654362 carbon_python_sdk-0.2.1/carbon/model/embedding_generators.py
+-rw-r--r--   0        0        0     2260 2024-05-30 19:55:10.654460 carbon_python_sdk-0.2.1/carbon/model/embedding_generators.pyi
+-rw-r--r--   0        0        0     3543 2024-05-30 19:55:10.654564 carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.py
+-rw-r--r--   0        0        0     3543 2024-05-30 19:55:10.654659 carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.pyi
+-rw-r--r--   0        0        0     4307 2024-05-30 19:55:10.654765 carbon_python_sdk-0.2.1/carbon/model/embedding_properties.py
+-rw-r--r--   0        0        0     4307 2024-05-30 19:55:10.654878 carbon_python_sdk-0.2.1/carbon/model/embedding_properties.pyi
+-rw-r--r--   0        0        0     3267 2024-05-30 19:55:10.654977 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0     3267 2024-05-30 19:55:10.655079 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.pyi
+-rw-r--r--   0        0        0     1141 2024-05-30 19:55:10.655176 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0      956 2024-05-30 19:55:10.655294 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.pyi
+-rw-r--r--   0        0        0     5194 2024-05-30 19:55:10.655400 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0     5194 2024-05-30 19:55:10.655496 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.pyi
+-rw-r--r--   0        0        0     3847 2024-05-30 19:55:10.655592 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0     3847 2024-05-30 19:55:10.655697 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.pyi
+-rw-r--r--   0        0        0     1944 2024-05-30 19:55:10.655789 carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1503 2024-05-30 19:55:10.655883 carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.pyi
+-rw-r--r--   0        0        0    17950 2024-05-30 19:55:10.655984 carbon_python_sdk-0.2.1/carbon/model/external_source_item.py
+-rw-r--r--   0        0        0    17950 2024-05-30 19:55:10.656098 carbon_python_sdk-0.2.1/carbon/model/external_source_item.pyi
+-rw-r--r--   0        0        0     1102 2024-05-30 19:55:10.656204 carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.py
+-rw-r--r--   0        0        0      933 2024-05-30 19:55:10.656297 carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.pyi
+-rw-r--r--   0        0        0     4287 2024-05-30 19:55:10.656396 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.py
+-rw-r--r--   0        0        0     4287 2024-05-30 19:55:10.656485 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.pyi
+-rw-r--r--   0        0        0     1187 2024-05-30 19:55:10.656569 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0     1187 2024-05-30 19:55:10.656654 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.pyi
+-rw-r--r--   0        0        0     1166 2024-05-30 19:55:10.656733 carbon_python_sdk-0.2.1/carbon/model/file_content_types.py
+-rw-r--r--   0        0        0      985 2024-05-30 19:55:10.656808 carbon_python_sdk-0.2.1/carbon/model/file_content_types.pyi
+-rw-r--r--   0        0        0     1926 2024-05-30 19:55:10.656885 carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.py
+-rw-r--r--   0        0        0     1926 2024-05-30 19:55:10.656973 carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.pyi
+-rw-r--r--   0        0        0     5789 2024-05-30 19:55:10.657063 carbon_python_sdk-0.2.1/carbon/model/file_formats.py
+-rw-r--r--   0        0        0     4344 2024-05-30 19:55:10.657150 carbon_python_sdk-0.2.1/carbon/model/file_formats.pyi
+-rw-r--r--   0        0        0     6161 2024-05-30 19:55:10.657240 carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.py
+-rw-r--r--   0        0        0     6161 2024-05-30 19:55:10.657328 carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.pyi
+-rw-r--r--   0        0        0     8647 2024-05-30 19:55:10.657413 carbon_python_sdk-0.2.1/carbon/model/file_statistics.py
+-rw-r--r--   0        0        0     8647 2024-05-30 19:55:10.657559 carbon_python_sdk-0.2.1/carbon/model/file_statistics.pyi
+-rw-r--r--   0        0        0     8000 2024-05-30 19:55:10.657704 carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.py
+-rw-r--r--   0        0        0     8000 2024-05-30 19:55:10.657794 carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.pyi
+-rw-r--r--   0        0        0     4847 2024-05-30 19:55:10.657887 carbon_python_sdk-0.2.1/carbon/model/file_sync_config.py
+-rw-r--r--   0        0        0     4847 2024-05-30 19:55:10.657977 carbon_python_sdk-0.2.1/carbon/model/file_sync_config.pyi
+-rw-r--r--   0        0        0     5047 2024-05-30 19:55:10.658070 carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.py
+-rw-r--r--   0        0        0     5047 2024-05-30 19:55:10.658162 carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.pyi
+-rw-r--r--   0        0        0     1283 2024-05-30 19:55:10.658246 carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     1283 2024-05-30 19:55:10.658337 carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.pyi
+-rw-r--r--   0        0        0    15514 2024-05-30 19:55:10.658422 carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0    15514 2024-05-30 19:55:10.658648 carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.pyi
+-rw-r--r--   0        0        0     3529 2024-05-30 19:55:10.658860 carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.py
+-rw-r--r--   0        0        0     3529 2024-05-30 19:55:10.658949 carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.pyi
+-rw-r--r--   0        0        0     2362 2024-05-30 19:55:10.659032 carbon_python_sdk-0.2.1/carbon/model/generic_success_response.py
+-rw-r--r--   0        0        0     2362 2024-05-30 19:55:10.659109 carbon_python_sdk-0.2.1/carbon/model/generic_success_response.pyi
+-rw-r--r--   0        0        0    15782 2024-05-30 19:55:10.659195 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.py
+-rw-r--r--   0        0        0    15631 2024-05-30 19:55:10.659611 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.pyi
+-rw-r--r--   0        0        0     1159 2024-05-30 19:55:10.660004 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0     1159 2024-05-30 19:55:10.660104 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.pyi
+-rw-r--r--   0        0        0     1264 2024-05-30 19:55:10.660210 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0     1264 2024-05-30 19:55:10.660304 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.pyi
+-rw-r--r--   0        0        0     1377 2024-05-30 19:55:10.660400 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0     1377 2024-05-30 19:55:10.660498 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.pyi
+-rw-r--r--   0        0        0     6490 2024-05-30 19:55:10.660598 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0     6490 2024-05-30 19:55:10.660702 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.pyi
+-rw-r--r--   0        0        0     3779 2024-05-30 19:55:10.660795 carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.py
+-rw-r--r--   0        0        0     3779 2024-05-30 19:55:10.660885 carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.pyi
+-rw-r--r--   0        0        0    14852 2024-05-30 19:55:10.660977 carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.py
+-rw-r--r--   0        0        0    14852 2024-05-30 19:55:10.661208 carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.pyi
+-rw-r--r--   0        0        0    13012 2024-05-30 19:55:10.661449 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.py
+-rw-r--r--   0        0        0    13012 2024-05-30 19:55:10.661830 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.pyi
+-rw-r--r--   0        0        0     1220 2024-05-30 19:55:10.662054 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0     1197 2024-05-30 19:55:10.662150 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.pyi
+-rw-r--r--   0        0        0     3635 2024-05-30 19:55:10.662253 carbon_python_sdk-0.2.1/carbon/model/github_authentication.py
+-rw-r--r--   0        0        0     3635 2024-05-30 19:55:10.662355 carbon_python_sdk-0.2.1/carbon/model/github_authentication.pyi
+-rw-r--r--   0        0        0     3626 2024-05-30 19:55:10.662451 carbon_python_sdk-0.2.1/carbon/model/github_connect_request.py
+-rw-r--r--   0        0        0     3626 2024-05-30 19:55:10.662549 carbon_python_sdk-0.2.1/carbon/model/github_connect_request.pyi
+-rw-r--r--   0        0        0     3792 2024-05-30 19:55:10.662653 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.py
+-rw-r--r--   0        0        0     3792 2024-05-30 19:55:10.662756 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.pyi
+-rw-r--r--   0        0        0     1246 2024-05-30 19:55:10.662987 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.py
+-rw-r--r--   0        0        0     1201 2024-05-30 19:55:10.663108 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.pyi
+-rw-r--r--   0        0        0    16085 2024-05-30 19:55:10.663216 carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.py
+-rw-r--r--   0        0        0    16085 2024-05-30 19:55:10.663455 carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.pyi
+-rw-r--r--   0        0        0      963 2024-05-30 19:55:10.663691 carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.py
+-rw-r--r--   0        0        0      834 2024-05-30 19:55:10.663787 carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.pyi
+-rw-r--r--   0        0        0     3251 2024-05-30 19:55:10.663886 carbon_python_sdk-0.2.1/carbon/model/http_validation_error.py
+-rw-r--r--   0        0        0     3251 2024-05-30 19:55:10.663982 carbon_python_sdk-0.2.1/carbon/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     2974 2024-05-30 19:55:10.664086 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0     2974 2024-05-30 19:55:10.664184 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.pyi
+-rw-r--r--   0        0        0     2907 2024-05-30 19:55:10.664286 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0     2907 2024-05-30 19:55:10.664385 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.pyi
+-rw-r--r--   0        0        0     6323 2024-05-30 19:55:10.664491 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.py
+-rw-r--r--   0        0        0     6323 2024-05-30 19:55:10.664600 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.pyi
+-rw-r--r--   0        0        0     3820 2024-05-30 19:55:10.664697 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.py
+-rw-r--r--   0        0        0     3820 2024-05-30 19:55:10.664793 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.pyi
+-rw-r--r--   0        0        0     5498 2024-05-30 19:55:10.664900 carbon_python_sdk-0.2.1/carbon/model/list_items_filters.py
+-rw-r--r--   0        0        0     5498 2024-05-30 19:55:10.665003 carbon_python_sdk-0.2.1/carbon/model/list_items_filters.pyi
+-rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665102 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.py
+-rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665198 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.pyi
+-rw-r--r--   0        0        0     1079 2024-05-30 19:55:10.665291 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.py
+-rw-r--r--   0        0        0     1079 2024-05-30 19:55:10.665392 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.pyi
+-rw-r--r--   0        0        0     5708 2024-05-30 19:55:10.665498 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.py
+-rw-r--r--   0        0        0     5708 2024-05-30 19:55:10.665603 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.pyi
+-rw-r--r--   0        0        0     1111 2024-05-30 19:55:10.665690 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.py
+-rw-r--r--   0        0        0     1111 2024-05-30 19:55:10.665785 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.pyi
+-rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665876 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.py
+-rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665957 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.pyi
+-rw-r--r--   0        0        0     3613 2024-05-30 19:55:10.666037 carbon_python_sdk-0.2.1/carbon/model/list_request.py
+-rw-r--r--   0        0        0     3613 2024-05-30 19:55:10.666117 carbon_python_sdk-0.2.1/carbon/model/list_request.pyi
+-rw-r--r--   0        0        0     3228 2024-05-30 19:55:10.666200 carbon_python_sdk-0.2.1/carbon/model/list_response.py
+-rw-r--r--   0        0        0     3228 2024-05-30 19:55:10.666284 carbon_python_sdk-0.2.1/carbon/model/list_response.pyi
+-rw-r--r--   0        0        0     3129 2024-05-30 19:55:10.666466 carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.py
+-rw-r--r--   0        0        0     3129 2024-05-30 19:55:10.666580 carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.pyi
+-rw-r--r--   0        0        0      560 2024-05-30 19:57:32.276931 carbon_python_sdk-0.2.1/carbon/model/multi_modal_embedding_generators.py
+-rw-r--r--   0        0        0      560 2024-05-30 19:57:32.277033 carbon_python_sdk-0.2.1/carbon/model/multi_modal_embedding_generators.pyi
+-rw-r--r--   0        0        0     3699 2024-05-30 19:55:10.666853 carbon_python_sdk-0.2.1/carbon/model/notion_authentication.py
+-rw-r--r--   0        0        0     3699 2024-05-30 19:55:10.666933 carbon_python_sdk-0.2.1/carbon/model/notion_authentication.pyi
+-rw-r--r--   0        0        0     4300 2024-05-30 19:55:10.667026 carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.py
+-rw-r--r--   0        0        0     4300 2024-05-30 19:55:10.667119 carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.pyi
+-rw-r--r--   0        0        0    29598 2024-05-30 19:55:10.667218 carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.py
+-rw-r--r--   0        0        0    29598 2024-05-30 19:55:10.667346 carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.pyi
+-rw-r--r--   0        0        0      930 2024-05-30 19:55:10.667437 carbon_python_sdk-0.2.1/carbon/model/order_dir.py
+-rw-r--r--   0        0        0      813 2024-05-30 19:55:10.667515 carbon_python_sdk-0.2.1/carbon/model/order_dir.pyi
+-rw-r--r--   0        0        0      932 2024-05-30 19:55:10.667596 carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.py
+-rw-r--r--   0        0        0      815 2024-05-30 19:55:10.667673 carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.pyi
+-rw-r--r--   0        0        0    18921 2024-05-30 19:55:10.667758 carbon_python_sdk-0.2.1/carbon/model/organization_response.py
+-rw-r--r--   0        0        0    18921 2024-05-30 19:55:10.667858 carbon_python_sdk-0.2.1/carbon/model/organization_response.pyi
+-rw-r--r--   0        0        0    17065 2024-05-30 19:55:10.667967 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.py
+-rw-r--r--   0        0        0    17065 2024-05-30 19:55:10.668074 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.pyi
+-rw-r--r--   0        0        0     4467 2024-05-30 19:55:10.668181 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0     4467 2024-05-30 19:55:10.668283 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.pyi
+-rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.668373 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.668461 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.pyi
+-rw-r--r--   0        0        0     1014 2024-05-30 19:55:10.668550 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0      871 2024-05-30 19:55:10.668632 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.pyi
+-rw-r--r--   0        0        0     4657 2024-05-30 19:55:10.668724 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0     4657 2024-05-30 19:55:10.668816 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.pyi
+-rw-r--r--   0        0        0     3947 2024-05-30 19:55:10.668899 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.py
+-rw-r--r--   0        0        0     3947 2024-05-30 19:55:10.668980 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.pyi
+-rw-r--r--   0        0        0     3408 2024-05-30 19:55:10.669059 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0     3408 2024-05-30 19:55:10.669138 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.pyi
+-rw-r--r--   0        0        0     6330 2024-05-30 19:55:10.669244 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0     6330 2024-05-30 19:55:10.669340 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.pyi
+-rw-r--r--   0        0        0     3418 2024-05-30 19:55:10.669421 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0     3418 2024-05-30 19:55:10.669505 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.pyi
+-rw-r--r--   0        0        0     1213 2024-05-30 19:55:10.669589 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     1213 2024-05-30 19:55:10.669673 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.pyi
+-rw-r--r--   0        0        0    21692 2024-05-30 19:55:10.669764 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0    21692 2024-05-30 19:55:10.669866 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.pyi
+-rw-r--r--   0        0        0     1238 2024-05-30 19:55:10.669961 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0     1238 2024-05-30 19:55:10.670057 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi
+-rw-r--r--   0        0        0     1186 2024-05-30 19:55:10.670149 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0     1186 2024-05-30 19:55:10.670244 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.pyi
+-rw-r--r--   0        0        0     1296 2024-05-30 19:55:10.670497 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0     1296 2024-05-30 19:55:10.670608 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi
+-rw-r--r--   0        0        0     1135 2024-05-30 19:55:10.670705 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0     1135 2024-05-30 19:55:10.670798 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi
+-rw-r--r--   0        0        0     1216 2024-05-30 19:55:10.670893 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.py
+-rw-r--r--   0        0        0     1192 2024-05-30 19:55:10.670982 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi
+-rw-r--r--   0        0        0     6420 2024-05-30 19:55:10.671075 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0     6420 2024-05-30 19:55:10.671174 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.pyi
+-rw-r--r--   0        0        0     1469 2024-05-30 19:55:10.671390 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1198 2024-05-30 19:55:10.671492 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.pyi
+-rw-r--r--   0        0        0     8629 2024-05-30 19:55:10.671586 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0     8629 2024-05-30 19:55:10.671738 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.pyi
+-rw-r--r--   0        0        0     2378 2024-05-30 19:55:10.671879 carbon_python_sdk-0.2.1/carbon/model/outh_url_response.py
+-rw-r--r--   0        0        0     2378 2024-05-30 19:55:10.671973 carbon_python_sdk-0.2.1/carbon/model/outh_url_response.pyi
+-rw-r--r--   0        0        0    17193 2024-05-30 19:55:10.672075 carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.py
+-rw-r--r--   0        0        0    17193 2024-05-30 19:55:10.672467 carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.pyi
+-rw-r--r--   0        0        0     2807 2024-05-30 19:55:10.672569 carbon_python_sdk-0.2.1/carbon/model/pagination.py
+-rw-r--r--   0        0        0     2807 2024-05-30 19:55:10.672767 carbon_python_sdk-0.2.1/carbon/model/pagination.pyi
+-rw-r--r--   0        0        0     2452 2024-05-30 19:55:10.672853 carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.py
+-rw-r--r--   0        0        0     2452 2024-05-30 19:55:10.672932 carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.pyi
+-rw-r--r--   0        0        0    10223 2024-05-30 19:55:10.673010 carbon_python_sdk-0.2.1/carbon/model/raw_text_input.py
+-rw-r--r--   0        0        0    10151 2024-05-30 19:55:10.673141 carbon_python_sdk-0.2.1/carbon/model/raw_text_input.pyi
+-rw-r--r--   0        0        0     5578 2024-05-30 19:55:10.673283 carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.py
+-rw-r--r--   0        0        0     5578 2024-05-30 19:55:10.673376 carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.pyi
+-rw-r--r--   0        0        0     2489 2024-05-30 19:55:10.673455 carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.py
+-rw-r--r--   0        0        0     2489 2024-05-30 19:55:10.673537 carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.pyi
+-rw-r--r--   0        0        0    12076 2024-05-30 19:55:10.673614 carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.py
+-rw-r--r--   0        0        0    12076 2024-05-30 19:55:10.673746 carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.pyi
+-rw-r--r--   0        0        0     3724 2024-05-30 19:55:10.673876 carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.py
+-rw-r--r--   0        0        0     3724 2024-05-30 19:55:10.674059 carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.pyi
+-rw-r--r--   0        0        0     3739 2024-05-30 19:55:10.674136 carbon_python_sdk-0.2.1/carbon/model/s3_authentication.py
+-rw-r--r--   0        0        0     3739 2024-05-30 19:55:10.674222 carbon_python_sdk-0.2.1/carbon/model/s3_authentication.pyi
+-rw-r--r--   0        0        0    19565 2024-05-30 19:55:10.674310 carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.py
+-rw-r--r--   0        0        0    19565 2024-05-30 19:55:10.674406 carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.pyi
+-rw-r--r--   0        0        0     3936 2024-05-30 19:55:10.674492 carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.py
+-rw-r--r--   0        0        0     3936 2024-05-30 19:55:10.674568 carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.pyi
+-rw-r--r--   0        0        0     4813 2024-05-30 19:55:10.674656 carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.py
+-rw-r--r--   0        0        0     4813 2024-05-30 19:55:10.674744 carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.pyi
+-rw-r--r--   0        0        0     5449 2024-05-30 19:55:10.674829 carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.py
+-rw-r--r--   0        0        0     5449 2024-05-30 19:55:10.674916 carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.pyi
+-rw-r--r--   0        0        0     1566 2024-05-30 19:55:10.675002 carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0     1263 2024-05-30 19:55:10.675082 carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.pyi
+-rw-r--r--   0        0        0     6587 2024-05-30 19:55:10.675172 carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     6587 2024-05-30 19:55:10.675269 carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.pyi
+-rw-r--r--   0        0        0    15650 2024-05-30 19:55:10.675348 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.py
+-rw-r--r--   0        0        0    15608 2024-05-30 19:55:10.675568 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.pyi
+-rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.676392 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.676479 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi
+-rw-r--r--   0        0        0     1117 2024-05-30 19:55:10.676562 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0     1117 2024-05-30 19:55:10.676647 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi
+-rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.676727 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.676807 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi
+-rw-r--r--   0        0        0     6392 2024-05-30 19:55:10.676896 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0     6392 2024-05-30 19:55:10.676989 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.pyi
+-rw-r--r--   0        0        0     2485 2024-05-30 19:55:10.677069 carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.py
+-rw-r--r--   0        0        0     2485 2024-05-30 19:55:10.677155 carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.pyi
+-rw-r--r--   0        0        0     2784 2024-05-30 19:55:10.677232 carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.py
+-rw-r--r--   0        0        0     2784 2024-05-30 19:55:10.677309 carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.pyi
+-rw-r--r--   0        0        0    22189 2024-05-30 19:55:10.677396 carbon_python_sdk-0.2.1/carbon/model/sync_files_request.py
+-rw-r--r--   0        0        0    22189 2024-05-30 19:55:10.677492 carbon_python_sdk-0.2.1/carbon/model/sync_files_request.pyi
+-rw-r--r--   0        0        0    16413 2024-05-30 19:55:10.677586 carbon_python_sdk-0.2.1/carbon/model/sync_options.py
+-rw-r--r--   0        0        0    16413 2024-05-30 19:55:10.677679 carbon_python_sdk-0.2.1/carbon/model/sync_options.pyi
+-rw-r--r--   0        0        0     3009 2024-05-30 19:55:10.677765 carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.py
+-rw-r--r--   0        0        0     2160 2024-05-30 19:55:10.677846 carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.pyi
+-rw-r--r--   0        0        0     3042 2024-05-30 19:55:10.677926 carbon_python_sdk-0.2.1/carbon/model/token_response.py
+-rw-r--r--   0        0        0     3042 2024-05-30 19:55:10.678008 carbon_python_sdk-0.2.1/carbon/model/token_response.pyi
+-rw-r--r--   0        0        0     2620 2024-05-30 19:55:10.678085 carbon_python_sdk-0.2.1/carbon/model/update_organization_input.py
+-rw-r--r--   0        0        0     2620 2024-05-30 19:55:10.678165 carbon_python_sdk-0.2.1/carbon/model/update_organization_input.pyi
+-rw-r--r--   0        0        0     9214 2024-05-30 19:55:10.678249 carbon_python_sdk-0.2.1/carbon/model/update_users_input.py
+-rw-r--r--   0        0        0     9128 2024-05-30 19:55:10.678384 carbon_python_sdk-0.2.1/carbon/model/update_users_input.pyi
+-rw-r--r--   0        0        0     1267 2024-05-30 19:55:10.678526 carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1243 2024-05-30 19:55:10.678815 carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.pyi
+-rw-r--r--   0        0        0    12928 2024-05-30 19:55:10.678905 carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.py
+-rw-r--r--   0        0        0    12928 2024-05-30 19:55:10.679123 carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.pyi
+-rw-r--r--   0        0        0     8405 2024-05-30 19:55:10.679342 carbon_python_sdk-0.2.1/carbon/model/user_configuration.py
+-rw-r--r--   0        0        0     8319 2024-05-30 19:55:10.679633 carbon_python_sdk-0.2.1/carbon/model/user_configuration.pyi
+-rw-r--r--   0        0        0     8665 2024-05-30 19:55:10.679916 carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.py
+-rw-r--r--   0        0        0     8579 2024-05-30 19:55:10.680045 carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.pyi
+-rw-r--r--   0        0        0    35549 2024-05-30 19:55:10.680194 carbon_python_sdk-0.2.1/carbon/model/user_file.py
+-rw-r--r--   0        0        0    35549 2024-05-30 19:55:10.680300 carbon_python_sdk-0.2.1/carbon/model/user_file.pyi
+-rw-r--r--   0        0        0     1650 2024-05-30 19:55:10.680390 carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.py
+-rw-r--r--   0        0        0     1650 2024-05-30 19:55:10.680469 carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.pyi
+-rw-r--r--   0        0        0     3751 2024-05-30 19:55:10.680549 carbon_python_sdk-0.2.1/carbon/model/user_files_v2.py
+-rw-r--r--   0        0        0     3751 2024-05-30 19:55:10.680625 carbon_python_sdk-0.2.1/carbon/model/user_files_v2.pyi
+-rw-r--r--   0        0        0     2416 2024-05-30 19:55:10.680704 carbon_python_sdk-0.2.1/carbon/model/user_request_content.py
+-rw-r--r--   0        0        0     2416 2024-05-30 19:55:10.680934 carbon_python_sdk-0.2.1/carbon/model/user_request_content.pyi
+-rw-r--r--   0        0        0    17500 2024-05-30 19:55:10.681021 carbon_python_sdk-0.2.1/carbon/model/user_response.py
+-rw-r--r--   0        0        0    17500 2024-05-30 19:55:10.681140 carbon_python_sdk-0.2.1/carbon/model/user_response.pyi
+-rw-r--r--   0        0        0     1511 2024-05-30 19:55:10.681232 carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.py
+-rw-r--r--   0        0        0     1511 2024-05-30 19:55:10.681311 carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.pyi
+-rw-r--r--   0        0        0     1246 2024-05-30 19:55:10.681392 carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0     1246 2024-05-30 19:55:10.681475 carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.pyi
+-rw-r--r--   0        0        0     1315 2024-05-30 19:55:10.681559 carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0     1315 2024-05-30 19:55:10.681642 carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.pyi
+-rw-r--r--   0        0        0     3352 2024-05-30 19:55:10.681722 carbon_python_sdk-0.2.1/carbon/model/validation_error.py
+-rw-r--r--   0        0        0     3352 2024-05-30 19:55:10.681802 carbon_python_sdk-0.2.1/carbon/model/validation_error.pyi
+-rw-r--r--   0        0        0     3149 2024-05-30 19:55:10.681883 carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.py
+-rw-r--r--   0        0        0     3149 2024-05-30 19:55:10.681963 carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.pyi
+-rw-r--r--   0        0        0     6973 2024-05-30 19:55:10.682051 carbon_python_sdk-0.2.1/carbon/model/webhook.py
+-rw-r--r--   0        0        0     6973 2024-05-30 19:55:10.682143 carbon_python_sdk-0.2.1/carbon/model/webhook.pyi
+-rw-r--r--   0        0        0     2396 2024-05-30 19:55:10.682229 carbon_python_sdk-0.2.1/carbon/model/webhook_filters.py
+-rw-r--r--   0        0        0     2396 2024-05-30 19:55:10.682460 carbon_python_sdk-0.2.1/carbon/model/webhook_filters.pyi
+-rw-r--r--   0        0        0     1075 2024-05-30 19:55:10.682542 carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.py
+-rw-r--r--   0        0        0     1075 2024-05-30 19:55:10.682619 carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.pyi
+-rw-r--r--   0        0        0     6395 2024-05-30 19:55:10.682704 carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.py
+-rw-r--r--   0        0        0     6395 2024-05-30 19:55:10.682788 carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.pyi
+-rw-r--r--   0        0        0      995 2024-05-30 19:55:10.682868 carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.py
+-rw-r--r--   0        0        0      852 2024-05-30 19:55:10.682943 carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.pyi
+-rw-r--r--   0        0        0     4347 2024-05-30 19:55:10.683030 carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.py
+-rw-r--r--   0        0        0     4347 2024-05-30 19:55:10.683121 carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.pyi
+-rw-r--r--   0        0        0     3798 2024-05-30 19:55:10.683207 carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.py
+-rw-r--r--   0        0        0     3798 2024-05-30 19:55:10.683287 carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.pyi
+-rw-r--r--   0        0        0      959 2024-05-30 19:55:10.683367 carbon_python_sdk-0.2.1/carbon/model/webhook_status.py
+-rw-r--r--   0        0        0      830 2024-05-30 19:55:10.683445 carbon_python_sdk-0.2.1/carbon/model/webhook_status.pyi
+-rw-r--r--   0        0        0    16894 2024-05-30 19:55:10.683532 carbon_python_sdk-0.2.1/carbon/model/webscrape_request.py
+-rw-r--r--   0        0        0    16810 2024-05-30 19:55:10.683644 carbon_python_sdk-0.2.1/carbon/model/webscrape_request.pyi
+-rw-r--r--   0        0        0     1105 2024-05-30 19:55:10.683738 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0     1105 2024-05-30 19:55:10.683820 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.pyi
+-rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.683902 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.683983 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.pyi
+-rw-r--r--   0        0        0     1101 2024-05-30 19:55:10.684184 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0     1101 2024-05-30 19:55:10.684380 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.pyi
+-rw-r--r--   0        0        0     6384 2024-05-30 19:55:10.684576 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.py
+-rw-r--r--   0        0        0     6384 2024-05-30 19:55:10.684677 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.pyi
+-rw-r--r--   0        0        0     3117 2024-05-30 19:55:10.684770 carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.py
+-rw-r--r--   0        0        0     3117 2024-05-30 19:55:10.684866 carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.pyi
+-rw-r--r--   0        0        0     5401 2024-05-30 19:55:10.684969 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.py
+-rw-r--r--   0        0        0     5401 2024-05-30 19:55:10.685075 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.pyi
+-rw-r--r--   0        0        0     1375 2024-05-30 19:55:10.685172 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0     1375 2024-05-30 19:55:10.685274 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.pyi
+-rw-r--r--   0        0        0     3326 2024-05-30 19:55:10.685374 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0     3326 2024-05-30 19:55:10.685594 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.pyi
+-rw-r--r--   0        0        0     3653 2024-05-30 19:55:10.685809 carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.py
+-rw-r--r--   0        0        0     3653 2024-05-30 19:55:10.685905 carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.pyi
+-rw-r--r--   0        0        0     4907 2024-05-30 19:55:10.685999 carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.py
+-rw-r--r--   0        0        0     4907 2024-05-30 19:55:10.686097 carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.pyi
+-rw-r--r--   0        0        0    13560 2024-05-30 19:57:32.277856 carbon_python_sdk-0.2.1/carbon/models/__init__.py
+-rw-r--r--   0        0        0    25498 2024-05-30 19:55:10.686466 carbon_python_sdk-0.2.1/carbon/operation_parameter_map.py
+-rw-r--r--   0        0        0     3147 2024-05-30 19:55:10.686693 carbon_python_sdk-0.2.1/carbon/paths/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-30 19:55:10.686787 carbon_python_sdk-0.2.1/carbon/paths/add_webhook/__init__.py
+-rw-r--r--   0        0        0    13948 2024-05-30 19:55:10.686875 carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.py
+-rw-r--r--   0        0        0    13811 2024-05-30 19:55:10.687094 carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.pyi
+-rw-r--r--   0        0        0      311 2024-05-30 19:55:10.687312 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/__init__.py
+-rw-r--r--   0        0        0    11830 2024-05-30 19:55:10.687394 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.py
+-rw-r--r--   0        0        0    11656 2024-05-30 19:55:10.687528 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.pyi
+-rw-r--r--   0        0        0      315 2024-05-30 19:55:10.687669 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/__init__.py
+-rw-r--r--   0        0        0    11193 2024-05-30 19:55:10.687752 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.py
+-rw-r--r--   0        0        0    11049 2024-05-30 19:55:10.687884 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.pyi
+-rw-r--r--   0        0        0      313 2024-05-30 19:55:10.688134 carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/__init__.py
+-rw-r--r--   0        0        0    15880 2024-05-30 19:55:10.688212 carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.py
+-rw-r--r--   0        0        0    15706 2024-05-30 19:55:10.688423 carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.pyi
+-rw-r--r--   0        0        0      295 2024-05-30 19:55:10.688634 carbon_python_sdk-0.2.1/carbon/paths/delete_files/__init__.py
+-rw-r--r--   0        0        0    19307 2024-05-30 19:55:10.688719 carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.py
+-rw-r--r--   0        0        0    19133 2024-05-30 19:55:10.688810 carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.pyi
+-rw-r--r--   0        0        0      301 2024-05-30 19:55:10.688902 carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/__init__.py
+-rw-r--r--   0        0        0    15967 2024-05-30 19:55:10.688995 carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.py
+-rw-r--r--   0        0        0    15793 2024-05-30 19:55:10.689212 carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.pyi
+-rw-r--r--   0        0        0      313 2024-05-30 19:55:10.689786 carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/__init__.py
+-rw-r--r--   0        0        0    15814 2024-05-30 19:55:10.689864 carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.py
+-rw-r--r--   0        0        0    15640 2024-05-30 19:55:10.690460 carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.pyi
+-rw-r--r--   0        0        0      295 2024-05-30 19:55:10.690682 carbon_python_sdk-0.2.1/carbon/paths/delete_users/__init__.py
+-rw-r--r--   0        0        0    14899 2024-05-30 19:55:10.690762 carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.py
+-rw-r--r--   0        0        0    14762 2024-05-30 19:55:10.690974 carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.pyi
+-rw-r--r--   0        0        0      321 2024-05-30 19:55:10.691328 carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/__init__.py
+-rw-r--r--   0        0        0    14359 2024-05-30 19:55:10.691410 carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.py
+-rw-r--r--   0        0        0    14222 2024-05-30 19:55:10.691621 carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.pyi
+-rw-r--r--   0        0        0      307 2024-05-30 19:55:10.691832 carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/__init__.py
+-rw-r--r--   0        0        0    14552 2024-05-30 19:55:10.691908 carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.py
+-rw-r--r--   0        0        0    14378 2024-05-30 19:55:10.692117 carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.pyi
+-rw-r--r--   0        0        0      291 2024-05-30 19:55:10.692326 carbon_python_sdk-0.2.1/carbon/paths/embeddings/__init__.py
+-rw-r--r--   0        0        0    29199 2024-05-30 19:55:10.692420 carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.py
+-rw-r--r--   0        0        0    29025 2024-05-30 19:55:10.692517 carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.pyi
+-rw-r--r--   0        0        0      291 2024-05-30 19:55:10.692743 carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/__init__.py
+-rw-r--r--   0        0        0    14466 2024-05-30 19:55:10.692824 carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.py
+-rw-r--r--   0        0        0    14292 2024-05-30 19:55:10.693035 carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.pyi
+-rw-r--r--   0        0        0      319 2024-05-30 19:55:10.693244 carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/__init__.py
+-rw-r--r--   0        0        0    15695 2024-05-30 19:55:10.693320 carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.py
+-rw-r--r--   0        0        0    15521 2024-05-30 19:55:10.693529 carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.pyi
+-rw-r--r--   0        0        0      283 2024-05-30 19:55:10.693743 carbon_python_sdk-0.2.1/carbon/paths/health/__init__.py
+-rw-r--r--   0        0        0    10429 2024-05-30 19:55:10.693823 carbon_python_sdk-0.2.1/carbon/paths/health/get.py
+-rw-r--r--   0        0        0    10348 2024-05-30 19:55:10.693955 carbon_python_sdk-0.2.1/carbon/paths/health/get.pyi
+-rw-r--r--   0        0        0      327 2024-05-30 19:55:10.694094 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/__init__.py
+-rw-r--r--   0        0        0    15289 2024-05-30 19:55:10.694179 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.py
+-rw-r--r--   0        0        0    15115 2024-05-30 19:55:10.694402 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.pyi
+-rw-r--r--   0        0        0      327 2024-05-30 19:55:10.694621 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/__init__.py
+-rw-r--r--   0        0        0    29028 2024-05-30 19:55:10.694722 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.py
+-rw-r--r--   0        0        0    28854 2024-05-30 19:55:10.694836 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.pyi
+-rw-r--r--   0        0        0      311 2024-05-30 19:55:10.694941 carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/__init__.py
+-rw-r--r--   0        0        0    20686 2024-05-30 19:55:10.695038 carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.py
+-rw-r--r--   0        0        0    20512 2024-05-30 19:55:10.695143 carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.pyi
+-rw-r--r--   0        0        0      317 2024-05-30 19:55:10.695252 carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/__init__.py
+-rw-r--r--   0        0        0    28913 2024-05-30 19:55:10.695362 carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.py
+-rw-r--r--   0        0        0    28739 2024-05-30 19:55:10.695484 carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.pyi
+-rw-r--r--   0        0        0      315 2024-05-30 19:55:10.695590 carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/__init__.py
+-rw-r--r--   0        0        0    26091 2024-05-30 19:55:10.695698 carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.py
+-rw-r--r--   0        0        0    25917 2024-05-30 19:55:10.695819 carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.pyi
+-rw-r--r--   0        0        0      311 2024-05-30 19:55:10.695923 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/__init__.py
+-rw-r--r--   0        0        0    24946 2024-05-30 19:55:10.696027 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.py
+-rw-r--r--   0        0        0    24772 2024-05-30 19:55:10.696139 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.pyi
+-rw-r--r--   0        0        0      325 2024-05-30 19:55:10.696244 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/__init__.py
+-rw-r--r--   0        0        0    14816 2024-05-30 19:55:10.696340 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.py
+-rw-r--r--   0        0        0    14642 2024-05-30 19:55:10.696579 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.pyi
+-rw-r--r--   0        0        0      321 2024-05-30 19:55:10.696820 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/__init__.py
+-rw-r--r--   0        0        0    23173 2024-05-30 19:55:10.696919 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.py
+-rw-r--r--   0        0        0    22999 2024-05-30 19:55:10.697029 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.pyi
+-rw-r--r--   0        0        0      309 2024-05-30 19:55:10.697145 carbon_python_sdk-0.2.1/carbon/paths/integrations_github/__init__.py
+-rw-r--r--   0        0        0    15826 2024-05-30 19:55:10.697241 carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.py
+-rw-r--r--   0        0        0    15652 2024-05-30 19:55:10.697475 carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.pyi
+-rw-r--r--   0        0        0      321 2024-05-30 19:55:10.697881 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/__init__.py
+-rw-r--r--   0        0        0    17078 2024-05-30 19:55:10.697994 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.py
+-rw-r--r--   0        0        0    16904 2024-05-30 19:55:10.698115 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.pyi
+-rw-r--r--   0        0        0      331 2024-05-30 19:55:10.698223 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/__init__.py
+-rw-r--r--   0        0        0    15560 2024-05-30 19:55:10.698318 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.py
+-rw-r--r--   0        0        0    15386 2024-05-30 19:55:10.698559 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.pyi
+-rw-r--r--   0        0        0      317 2024-05-30 19:55:10.698801 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/__init__.py
+-rw-r--r--   0        0        0    26562 2024-05-30 19:55:10.698904 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.py
+-rw-r--r--   0        0        0    26388 2024-05-30 19:55:10.699022 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.pyi
+-rw-r--r--   0        0        0      331 2024-05-30 19:55:10.699127 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/__init__.py
+-rw-r--r--   0        0        0    15340 2024-05-30 19:55:10.699222 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.py
+-rw-r--r--   0        0        0    15166 2024-05-30 19:55:10.699620 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.pyi
+-rw-r--r--   0        0        0      317 2024-05-30 19:55:10.699867 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/__init__.py
+-rw-r--r--   0        0        0    19585 2024-05-30 19:55:10.699970 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.py
+-rw-r--r--   0        0        0    19411 2024-05-30 19:55:10.700072 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.pyi
+-rw-r--r--   0        0        0      317 2024-05-30 19:55:10.700169 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/__init__.py
+-rw-r--r--   0        0        0    14992 2024-05-30 19:55:10.700251 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.py
+-rw-r--r--   0        0        0    14818 2024-05-30 19:55:10.700481 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.pyi
+-rw-r--r--   0        0        0      315 2024-05-30 19:55:10.700707 carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/__init__.py
+-rw-r--r--   0        0        0    37674 2024-05-30 19:55:10.700815 carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.py
+-rw-r--r--   0        0        0    37500 2024-05-30 19:55:10.700929 carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.pyi
+-rw-r--r--   0        0        0      321 2024-05-30 19:55:10.701033 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/__init__.py
+-rw-r--r--   0        0        0    27296 2024-05-30 19:55:10.701125 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.py
+-rw-r--r--   0        0        0    27122 2024-05-30 19:55:10.701225 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.pyi
+-rw-r--r--   0        0        0      343 2024-05-30 19:55:10.701332 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/__init__.py
+-rw-r--r--   0        0        0    15590 2024-05-30 19:55:10.701413 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.py
+-rw-r--r--   0        0        0    15416 2024-05-30 19:55:10.701639 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.pyi
+-rw-r--r--   0        0        0      337 2024-05-30 19:55:10.701862 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/__init__.py
+-rw-r--r--   0        0        0    15371 2024-05-30 19:55:10.701947 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.py
+-rw-r--r--   0        0        0    15197 2024-05-30 19:55:10.702169 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.pyi
+-rw-r--r--   0        0        0      313 2024-05-30 19:55:10.702390 carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/__init__.py
+-rw-r--r--   0        0        0    22218 2024-05-30 19:55:10.702479 carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.py
+-rw-r--r--   0        0        0    22044 2024-05-30 19:55:10.702582 carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.pyi
+-rw-r--r--   0        0        0      301 2024-05-30 19:55:10.702690 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/__init__.py
+-rw-r--r--   0        0        0    16130 2024-05-30 19:55:10.702782 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.py
+-rw-r--r--   0        0        0    15956 2024-05-30 19:55:10.703019 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.pyi
+-rw-r--r--   0        0        0      313 2024-05-30 19:55:10.703413 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/__init__.py
+-rw-r--r--   0        0        0    28274 2024-05-30 19:55:10.703522 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.py
+-rw-r--r--   0        0        0    28100 2024-05-30 19:55:10.703649 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.pyi
+-rw-r--r--   0        0        0      321 2024-05-30 19:55:10.703759 carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/__init__.py
+-rw-r--r--   0        0        0    16382 2024-05-30 19:55:10.703851 carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.py
+-rw-r--r--   0        0        0    16208 2024-05-30 19:55:10.704087 carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.pyi
+-rw-r--r--   0        0        0      295 2024-05-30 19:55:10.704321 carbon_python_sdk-0.2.1/carbon/paths/organization/__init__.py
+-rw-r--r--   0        0        0    10831 2024-05-30 19:55:10.704415 carbon_python_sdk-0.2.1/carbon/paths/organization/get.py
+-rw-r--r--   0        0        0    10724 2024-05-30 19:55:10.704562 carbon_python_sdk-0.2.1/carbon/paths/organization/get.pyi
+-rw-r--r--   0        0        0      317 2024-05-30 19:55:10.704713 carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/__init__.py
+-rw-r--r--   0        0        0    11092 2024-05-30 19:55:10.704808 carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.py
+-rw-r--r--   0        0        0    10985 2024-05-30 19:55:10.704956 carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.pyi
+-rw-r--r--   0        0        0      309 2024-05-30 19:55:10.705105 carbon_python_sdk-0.2.1/carbon/paths/organization_update/__init__.py
+-rw-r--r--   0        0        0    15275 2024-05-30 19:55:10.705205 carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.py
+-rw-r--r--   0        0        0    15138 2024-05-30 19:55:10.705716 carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.pyi
+-rw-r--r--   0        0        0      309 2024-05-30 19:55:10.705947 carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/__init__.py
+-rw-r--r--   0        0        0    14654 2024-05-30 19:55:10.706027 carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.py
+-rw-r--r--   0        0        0    14480 2024-05-30 19:55:10.706247 carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.pyi
+-rw-r--r--   0        0        0      301 2024-05-30 19:55:10.706469 carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/__init__.py
+-rw-r--r--   0        0        0    14363 2024-05-30 19:55:10.706549 carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.py
+-rw-r--r--   0        0        0    14189 2024-05-30 19:55:10.706767 carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.pyi
+-rw-r--r--   0        0        0      303 2024-05-30 19:55:10.706992 carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/__init__.py
+-rw-r--r--   0        0        0    14585 2024-05-30 19:55:10.707083 carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.py
+-rw-r--r--   0        0        0    14411 2024-05-30 19:55:10.707302 carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.pyi
+-rw-r--r--   0        0        0      293 2024-05-30 19:55:10.707524 carbon_python_sdk-0.2.1/carbon/paths/resync_file/__init__.py
+-rw-r--r--   0        0        0    16696 2024-05-30 19:55:10.707611 carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.py
+-rw-r--r--   0        0        0    16522 2024-05-30 19:55:10.707723 carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.pyi
+-rw-r--r--   0        0        0      309 2024-05-30 19:55:10.707828 carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/__init__.py
+-rw-r--r--   0        0        0    14828 2024-05-30 19:55:10.707922 carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.py
+-rw-r--r--   0        0        0    14654 2024-05-30 19:55:10.708156 carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.pyi
+-rw-r--r--   0        0        0      299 2024-05-30 19:55:10.708377 carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/__init__.py
+-rw-r--r--   0        0        0    27300 2024-05-30 19:55:10.708481 carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.py
+-rw-r--r--   0        0        0    27126 2024-05-30 19:55:10.708583 carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.pyi
+-rw-r--r--   0        0        0      293 2024-05-30 19:55:10.709024 carbon_python_sdk-0.2.1/carbon/paths/search_urls/__init__.py
+-rw-r--r--   0        0        0    14549 2024-05-30 19:55:10.709104 carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.py
+-rw-r--r--   0        0        0    14375 2024-05-30 19:55:10.709321 carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.pyi
+-rw-r--r--   0        0        0      293 2024-05-30 19:55:10.709671 carbon_python_sdk-0.2.1/carbon/paths/text_chunks/__init__.py
+-rw-r--r--   0        0        0    19073 2024-05-30 19:55:10.709755 carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.py
+-rw-r--r--   0        0        0    18899 2024-05-30 19:55:10.709857 carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.pyi
+-rw-r--r--   0        0        0      295 2024-05-30 19:55:10.709953 carbon_python_sdk-0.2.1/carbon/paths/update_users/__init__.py
+-rw-r--r--   0        0        0    18200 2024-05-30 19:55:10.710044 carbon_python_sdk-0.2.1/carbon/paths/update_users/post.py
+-rw-r--r--   0        0        0    18063 2024-05-30 19:55:10.710142 carbon_python_sdk-0.2.1/carbon/paths/update_users/post.pyi
+-rw-r--r--   0        0        0      327 2024-05-30 19:55:10.710245 carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/__init__.py
+-rw-r--r--   0        0        0    20060 2024-05-30 19:55:10.710341 carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.py
+-rw-r--r--   0        0        0    19886 2024-05-30 19:55:10.710448 carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.pyi
+-rw-r--r--   0        0        0      311 2024-05-30 19:55:10.710552 carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/__init__.py
+-rw-r--r--   0        0        0    24942 2024-05-30 19:55:10.710654 carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.py
+-rw-r--r--   0        0        0    24768 2024-05-30 19:55:10.710769 carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.pyi
+-rw-r--r--   0        0        0      293 2024-05-30 19:55:10.710859 carbon_python_sdk-0.2.1/carbon/paths/upload_text/__init__.py
+-rw-r--r--   0        0        0    20504 2024-05-30 19:55:10.710946 carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.py
+-rw-r--r--   0        0        0    20330 2024-05-30 19:55:10.711042 carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.pyi
+-rw-r--r--   0        0        0      291 2024-05-30 19:55:10.711137 carbon_python_sdk-0.2.1/carbon/paths/uploadfile/__init__.py
+-rw-r--r--   0        0        0    35190 2024-05-30 19:57:32.278568 carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.py
+-rw-r--r--   0        0        0    35016 2024-05-30 19:57:32.279260 carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.pyi
+-rw-r--r--   0        0        0      279 2024-05-30 19:55:10.711454 carbon_python_sdk-0.2.1/carbon/paths/user/__init__.py
+-rw-r--r--   0        0        0    14156 2024-05-30 19:55:10.711532 carbon_python_sdk-0.2.1/carbon/paths/user/post.py
+-rw-r--r--   0        0        0    14019 2024-05-30 19:55:10.711762 carbon_python_sdk-0.2.1/carbon/paths/user/post.pyi
+-rw-r--r--   0        0        0      305 2024-05-30 19:55:10.711988 carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/__init__.py
+-rw-r--r--   0        0        0    18865 2024-05-30 19:55:10.712087 carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.py
+-rw-r--r--   0        0        0    18691 2024-05-30 19:55:10.712205 carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.pyi
+-rw-r--r--   0        0        0      291 2024-05-30 19:55:10.712297 carbon_python_sdk-0.2.1/carbon/paths/user_files/__init__.py
+-rw-r--r--   0        0        0    22374 2024-05-30 19:55:10.712384 carbon_python_sdk-0.2.1/carbon/paths/user_files/post.py
+-rw-r--r--   0        0        0    22200 2024-05-30 19:55:10.712486 carbon_python_sdk-0.2.1/carbon/paths/user_files/post.pyi
+-rw-r--r--   0        0        0      297 2024-05-30 19:55:10.712583 carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/__init__.py
+-rw-r--r--   0        0        0    21370 2024-05-30 19:55:10.712679 carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.py
+-rw-r--r--   0        0        0    21196 2024-05-30 19:55:10.712789 carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.pyi
+-rw-r--r--   0        0        0      291 2024-05-30 19:55:10.712890 carbon_python_sdk-0.2.1/carbon/paths/web_scrape/__init__.py
+-rw-r--r--   0        0        0    14274 2024-05-30 19:55:10.712979 carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.py
+-rw-r--r--   0        0        0    14100 2024-05-30 19:55:10.713204 carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.pyi
+-rw-r--r--   0        0        0      287 2024-05-30 19:55:10.713555 carbon_python_sdk-0.2.1/carbon/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    17367 2024-05-30 19:55:10.713641 carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.py
+-rw-r--r--   0        0        0    17230 2024-05-30 19:55:10.713734 carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0        0 2024-05-30 19:55:10.713869 carbon_python_sdk-0.2.1/carbon/pydantic/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-30 19:55:10.713949 carbon_python_sdk-0.2.1/carbon/pydantic/add_webhook_props.py
+-rw-r--r--   0        0        0      586 2024-05-30 19:55:10.714034 carbon_python_sdk-0.2.1/carbon/pydantic/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0      760 2024-05-30 19:55:10.714112 carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties.py
+-rw-r--r--   0        0        0      768 2024-05-30 19:55:10.714199 carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties_nullable.py
+-rw-r--r--   0        0        0      821 2024-05-30 19:55:10.714283 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings.py
+-rw-r--r--   0        0        0      469 2024-05-30 19:55:10.714367 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1333 2024-05-30 19:55:10.714451 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0      438 2024-05-30 19:55:10.714534 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_upload_input_custom_credentials.py
+-rw-r--r--   0        0        0      418 2024-05-30 19:55:10.714613 carbon_python_sdk-0.2.1/carbon/pydantic/configuration_keys.py
+-rw-r--r--   0        0        0      835 2024-05-30 19:55:10.714694 carbon_python_sdk-0.2.1/carbon/pydantic/confluence_authentication.py
+-rw-r--r--   0        0        0     1791 2024-05-30 19:55:10.714775 carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_input.py
+-rw-r--r--   0        0        0      765 2024-05-30 19:55:10.714864 carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_response.py
+-rw-r--r--   0        0        0      481 2024-05-30 19:55:10.714952 carbon_python_sdk-0.2.1/carbon/pydantic/custom_credentials_type.py
+-rw-r--r--   0        0        0      424 2024-05-30 19:55:10.715031 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_extended_input.py
+-rw-r--r--   0        0        0      456 2024-05-30 19:55:10.715111 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      472 2024-05-30 19:55:10.715191 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_sync_statuses.py
+-rw-r--r--   0        0        0      890 2024-05-30 19:55:10.715273 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type.py
+-rw-r--r--   0        0        0      898 2024-05-30 19:55:10.715357 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type_nullable.py
+-rw-r--r--   0        0        0     1187 2024-05-30 19:55:10.715436 carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_query_input.py
+-rw-r--r--   0        0        0      448 2024-05-30 19:55:10.715518 carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0      809 2024-05-30 19:55:10.715617 carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_v2_query_input.py
+-rw-r--r--   0        0        0      690 2024-05-30 19:55:10.715702 carbon_python_sdk-0.2.1/carbon/pydantic/delete_users_input.py
+-rw-r--r--   0        0        0      430 2024-05-30 19:55:10.715788 carbon_python_sdk-0.2.1/carbon/pydantic/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0      694 2024-05-30 19:55:10.715867 carbon_python_sdk-0.2.1/carbon/pydantic/directory_item.py
+-rw-r--r--   0        0        0     1674 2024-05-30 19:55:10.715952 carbon_python_sdk-0.2.1/carbon/pydantic/document_response.py
+-rw-r--r--   0        0        0      665 2024-05-30 19:55:10.716036 carbon_python_sdk-0.2.1/carbon/pydantic/document_response_list.py
+-rw-r--r--   0        0        0      411 2024-05-30 19:55:10.716320 carbon_python_sdk-0.2.1/carbon/pydantic/document_response_tags.py
+-rw-r--r--   0        0        0      463 2024-05-30 19:55:10.716421 carbon_python_sdk-0.2.1/carbon/pydantic/document_response_vector.py
+-rw-r--r--   0        0        0     1021 2024-05-30 19:55:10.716509 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_and_chunk.py
+-rw-r--r--   0        0        0      467 2024-05-30 19:55:10.716595 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0      743 2024-05-30 19:55:10.716682 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators.py
+-rw-r--r--   0        0        0      751 2024-05-30 19:55:10.716779 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators_nullable.py
+-rw-r--r--   0        0        0      666 2024-05-30 19:55:10.716860 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_properties.py
+-rw-r--r--   0        0        0      780 2024-05-30 19:55:10.716946 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0      470 2024-05-30 19:55:10.717037 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0     1222 2024-05-30 19:55:10.717128 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0      711 2024-05-30 19:55:10.717210 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0      553 2024-05-30 19:55:10.717289 carbon_python_sdk-0.2.1/carbon/pydantic/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1780 2024-05-30 19:55:10.717373 carbon_python_sdk-0.2.1/carbon/pydantic/external_source_item.py
+-rw-r--r--   0        0        0      455 2024-05-30 19:55:10.717457 carbon_python_sdk-0.2.1/carbon/pydantic/external_source_items_order_by.py
+-rw-r--r--   0        0        0      781 2024-05-30 19:55:10.717539 carbon_python_sdk-0.2.1/carbon/pydantic/fetch_urls_response.py
+-rw-r--r--   0        0        0      424 2024-05-30 19:55:10.717622 carbon_python_sdk-0.2.1/carbon/pydantic/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0      445 2024-05-30 19:55:10.717708 carbon_python_sdk-0.2.1/carbon/pydantic/file_content_types.py
+-rw-r--r--   0        0        0      453 2024-05-30 19:55:10.717791 carbon_python_sdk-0.2.1/carbon/pydantic/file_content_types_nullable.py
+-rw-r--r--   0        0        0      820 2024-05-30 19:55:10.717883 carbon_python_sdk-0.2.1/carbon/pydantic/file_formats.py
+-rw-r--r--   0        0        0      828 2024-05-30 19:55:10.717975 carbon_python_sdk-0.2.1/carbon/pydantic/file_formats_nullable.py
+-rw-r--r--   0        0        0     1002 2024-05-30 19:55:10.718056 carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics.py
+-rw-r--r--   0        0        0     1010 2024-05-30 19:55:10.718136 carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics_nullable.py
+-rw-r--r--   0        0        0     1240 2024-05-30 19:55:10.718314 carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config.py
+-rw-r--r--   0        0        0     1248 2024-05-30 19:55:10.718402 carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config_nullable.py
+-rw-r--r--   0        0        0      492 2024-05-30 19:55:10.718486 carbon_python_sdk-0.2.1/carbon/pydantic/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     2096 2024-05-30 19:55:10.718568 carbon_python_sdk-0.2.1/carbon/pydantic/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0      723 2024-05-30 19:55:10.718645 carbon_python_sdk-0.2.1/carbon/pydantic/freskdesk_authentication.py
+-rw-r--r--   0        0        0      575 2024-05-30 19:55:10.718724 carbon_python_sdk-0.2.1/carbon/pydantic/generic_success_response.py
+-rw-r--r--   0        0        0     3379 2024-05-30 19:55:10.718805 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body.py
+-rw-r--r--   0        0        0      452 2024-05-30 19:55:10.718883 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0      458 2024-05-30 19:55:10.718959 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0      477 2024-05-30 19:55:10.719044 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0      420 2024-05-30 19:55:10.719124 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0      752 2024-05-30 19:55:10.719205 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_authetication.py
+-rw-r--r--   0        0        0     1911 2024-05-30 19:55:10.719284 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_connect_request.py
+-rw-r--r--   0        0        0     1699 2024-05-30 19:55:10.719370 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_sync_request.py
+-rw-r--r--   0        0        0      429 2024-05-30 19:55:10.719464 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0      734 2024-05-30 19:55:10.719556 carbon_python_sdk-0.2.1/carbon/pydantic/github_authentication.py
+-rw-r--r--   0        0        0      825 2024-05-30 19:55:10.719644 carbon_python_sdk-0.2.1/carbon/pydantic/github_connect_request.py
+-rw-r--r--   0        0        0      783 2024-05-30 19:55:10.719735 carbon_python_sdk-0.2.1/carbon/pydantic/github_fetch_repos_request.py
+-rw-r--r--   0        0        0      431 2024-05-30 19:55:10.719830 carbon_python_sdk-0.2.1/carbon/pydantic/github_fetch_repos_request_repos.py
+-rw-r--r--   0        0        0     2073 2024-05-30 19:55:10.719918 carbon_python_sdk-0.2.1/carbon/pydantic/gmail_sync_input.py
+-rw-r--r--   0        0        0      432 2024-05-30 19:55:10.720008 carbon_python_sdk-0.2.1/carbon/pydantic/helpdesk_file_types.py
+-rw-r--r--   0        0        0      678 2024-05-30 19:55:10.720093 carbon_python_sdk-0.2.1/carbon/pydantic/http_validation_error.py
+-rw-r--r--   0        0        0      665 2024-05-30 19:55:10.720182 carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0      673 2024-05-30 19:55:10.720274 carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0     1282 2024-05-30 19:55:10.720366 carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_request.py
+-rw-r--r--   0        0        0      710 2024-05-30 19:55:10.720455 carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_response.py
+-rw-r--r--   0        0        0     1035 2024-05-30 19:55:10.720546 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters.py
+-rw-r--r--   0        0        0      447 2024-05-30 19:55:10.720642 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_external_ids.py
+-rw-r--r--   0        0        0      439 2024-05-30 19:55:10.720853 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_ids.py
+-rw-r--r--   0        0        0     1093 2024-05-30 19:55:10.720946 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable.py
+-rw-r--r--   0        0        0      455 2024-05-30 19:55:10.721039 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable_external_ids.py
+-rw-r--r--   0        0        0      447 2024-05-30 19:55:10.721135 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable_ids.py
+-rw-r--r--   0        0        0      664 2024-05-30 19:55:10.721222 carbon_python_sdk-0.2.1/carbon/pydantic/list_request.py
+-rw-r--r--   0        0        0      638 2024-05-30 19:55:10.721314 carbon_python_sdk-0.2.1/carbon/pydantic/list_response.py
+-rw-r--r--   0        0        0      733 2024-05-30 19:55:10.721402 carbon_python_sdk-0.2.1/carbon/pydantic/modify_user_configuration_input.py
+-rw-r--r--   0        0        0      430 2024-05-30 19:57:32.279498 carbon_python_sdk-0.2.1/carbon/pydantic/multi_modal_embedding_generators.py
+-rw-r--r--   0        0        0      742 2024-05-30 19:55:10.721590 carbon_python_sdk-0.2.1/carbon/pydantic/notion_authentication.py
+-rw-r--r--   0        0        0      814 2024-05-30 19:55:10.721686 carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_authentication.py
+-rw-r--r--   0        0        0     4718 2024-05-30 19:57:32.279709 carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_url_request.py
+-rw-r--r--   0        0        0      417 2024-05-30 19:55:10.721891 carbon_python_sdk-0.2.1/carbon/pydantic/order_dir.py
+-rw-r--r--   0        0        0      419 2024-05-30 19:55:10.721984 carbon_python_sdk-0.2.1/carbon/pydantic/order_dir_v2.py
+-rw-r--r--   0        0        0     2547 2024-05-30 19:55:10.722071 carbon_python_sdk-0.2.1/carbon/pydantic/organization_response.py
+-rw-r--r--   0        0        0     2100 2024-05-30 19:55:10.722164 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_api.py
+-rw-r--r--   0        0        0      998 2024-05-30 19:55:10.722254 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0      456 2024-05-30 19:55:10.722352 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0      462 2024-05-30 19:55:10.722448 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0     1213 2024-05-30 19:55:10.722540 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0      756 2024-05-30 19:55:10.722627 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_response.py
+-rw-r--r--   0        0        0      785 2024-05-30 19:55:10.722706 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0      424 2024-05-30 19:55:10.722787 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0      789 2024-05-30 19:55:10.722867 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0      437 2024-05-30 19:55:10.722947 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     5786 2024-05-30 19:55:10.723038 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0      469 2024-05-30 19:55:10.723118 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0      457 2024-05-30 19:55:10.723199 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0      482 2024-05-30 19:55:10.723283 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0      467 2024-05-30 19:55:10.723370 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0      464 2024-05-30 19:55:10.723450 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_request_ids.py
+-rw-r--r--   0        0        0      429 2024-05-30 19:55:10.723531 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0      501 2024-05-30 19:55:10.723616 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1554 2024-05-30 19:55:10.723696 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0      571 2024-05-30 19:55:10.723774 carbon_python_sdk-0.2.1/carbon/pydantic/outh_url_response.py
+-rw-r--r--   0        0        0     2156 2024-05-30 19:55:10.723851 carbon_python_sdk-0.2.1/carbon/pydantic/outlook_sync_input.py
+-rw-r--r--   0        0        0      645 2024-05-30 19:55:10.723930 carbon_python_sdk-0.2.1/carbon/pydantic/pagination.py
+-rw-r--r--   0        0        0      584 2024-05-30 19:55:10.724030 carbon_python_sdk-0.2.1/carbon/pydantic/presigned_url_response.py
+-rw-r--r--   0        0        0     1341 2024-05-30 19:55:10.724130 carbon_python_sdk-0.2.1/carbon/pydantic/raw_text_input.py
+-rw-r--r--   0        0        0      861 2024-05-30 19:55:10.724214 carbon_python_sdk-0.2.1/carbon/pydantic/resync_file_query_input.py
+-rw-r--r--   0        0        0      588 2024-05-30 19:55:10.724316 carbon_python_sdk-0.2.1/carbon/pydantic/revoke_access_token_input.py
+-rw-r--r--   0        0        0     1515 2024-05-30 19:55:10.724393 carbon_python_sdk-0.2.1/carbon/pydantic/rss_feed_input.py
+-rw-r--r--   0        0        0      832 2024-05-30 19:55:10.724477 carbon_python_sdk-0.2.1/carbon/pydantic/s3_auth_request.py
+-rw-r--r--   0        0        0      744 2024-05-30 19:55:10.724556 carbon_python_sdk-0.2.1/carbon/pydantic/s3_authentication.py
+-rw-r--r--   0        0        0     2360 2024-05-30 19:55:10.724641 carbon_python_sdk-0.2.1/carbon/pydantic/s3_file_sync_input.py
+-rw-r--r--   0        0        0      677 2024-05-30 19:55:10.724720 carbon_python_sdk-0.2.1/carbon/pydantic/s3_get_file_input.py
+-rw-r--r--   0        0        0      829 2024-05-30 19:55:10.724800 carbon_python_sdk-0.2.1/carbon/pydantic/salesforce_authentication.py
+-rw-r--r--   0        0        0      886 2024-05-30 19:55:10.724883 carbon_python_sdk-0.2.1/carbon/pydantic/sharepoint_authentication.py
+-rw-r--r--   0        0        0      494 2024-05-30 19:55:10.724969 carbon_python_sdk-0.2.1/carbon/pydantic/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0      942 2024-05-30 19:55:10.725053 carbon_python_sdk-0.2.1/carbon/pydantic/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     2337 2024-05-30 19:55:10.725190 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request.py
+-rw-r--r--   0        0        0      456 2024-05-30 19:55:10.725288 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      458 2024-05-30 19:55:10.725376 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      454 2024-05-30 19:55:10.725462 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      415 2024-05-30 19:55:10.725543 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0      586 2024-05-30 19:55:10.725625 carbon_python_sdk-0.2.1/carbon/pydantic/sync_directory_request.py
+-rw-r--r--   0        0        0      597 2024-05-30 19:55:10.725704 carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_ids.py
+-rw-r--r--   0        0        0     2668 2024-05-30 19:55:10.725786 carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_request.py
+-rw-r--r--   0        0        0     2932 2024-05-30 19:55:10.726185 carbon_python_sdk-0.2.1/carbon/pydantic/sync_options.py
+-rw-r--r--   0        0        0      726 2024-05-30 19:55:10.726271 carbon_python_sdk-0.2.1/carbon/pydantic/text_embedding_generators.py
+-rw-r--r--   0        0        0      630 2024-05-30 19:55:10.726349 carbon_python_sdk-0.2.1/carbon/pydantic/token_response.py
+-rw-r--r--   0        0        0      724 2024-05-30 19:55:10.726432 carbon_python_sdk-0.2.1/carbon/pydantic/update_organization_input.py
+-rw-r--r--   0        0        0     1746 2024-05-30 19:55:10.726521 carbon_python_sdk-0.2.1/carbon/pydantic/update_users_input.py
+-rw-r--r--   0        0        0      430 2024-05-30 19:55:10.726606 carbon_python_sdk-0.2.1/carbon/pydantic/update_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1862 2024-05-30 19:55:10.726693 carbon_python_sdk-0.2.1/carbon/pydantic/upload_file_from_url_input.py
+-rw-r--r--   0        0        0     1582 2024-05-30 19:55:10.726783 carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration.py
+-rw-r--r--   0        0        0     1590 2024-05-30 19:55:10.726878 carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration_nullable.py
+-rw-r--r--   0        0        0     3606 2024-05-30 19:55:10.726971 carbon_python_sdk-0.2.1/carbon/pydantic/user_file.py
+-rw-r--r--   0        0        0      487 2024-05-30 19:55:10.727065 carbon_python_sdk-0.2.1/carbon/pydantic/user_file_embedding_properties.py
+-rw-r--r--   0        0        0      667 2024-05-30 19:55:10.727159 carbon_python_sdk-0.2.1/carbon/pydantic/user_files_v2.py
+-rw-r--r--   0        0        0      578 2024-05-30 19:55:10.727247 carbon_python_sdk-0.2.1/carbon/pydantic/user_request_content.py
+-rw-r--r--   0        0        0     2736 2024-05-30 19:55:10.727330 carbon_python_sdk-0.2.1/carbon/pydantic/user_response.py
+-rw-r--r--   0        0        0      503 2024-05-30 19:55:10.727417 carbon_python_sdk-0.2.1/carbon/pydantic/user_response_auto_sync_enabled_sources.py
+-rw-r--r--   0        0        0      432 2024-05-30 19:55:10.727511 carbon_python_sdk-0.2.1/carbon/pydantic/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0      504 2024-05-30 19:55:10.727602 carbon_python_sdk-0.2.1/carbon/pydantic/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0      714 2024-05-30 19:55:10.727696 carbon_python_sdk-0.2.1/carbon/pydantic/validation_error.py
+-rw-r--r--   0        0        0      440 2024-05-30 19:55:10.727793 carbon_python_sdk-0.2.1/carbon/pydantic/validation_error_loc.py
+-rw-r--r--   0        0        0      982 2024-05-30 19:55:10.727889 carbon_python_sdk-0.2.1/carbon/pydantic/webhook.py
+-rw-r--r--   0        0        0      661 2024-05-30 19:55:10.727985 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_filters.py
+-rw-r--r--   0        0        0      437 2024-05-30 19:55:10.728078 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_filters_ids.py
+-rw-r--r--   0        0        0      936 2024-05-30 19:55:10.728170 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_no_key.py
+-rw-r--r--   0        0        0      443 2024-05-30 19:55:10.728265 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_order_by_columns.py
+-rw-r--r--   0        0        0     1074 2024-05-30 19:55:10.728359 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_input.py
+-rw-r--r--   0        0        0      689 2024-05-30 19:55:10.728453 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_response.py
+-rw-r--r--   0        0        0      428 2024-05-30 19:55:10.728550 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_status.py
+-rw-r--r--   0        0        0     2380 2024-05-30 19:55:10.728643 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request.py
+-rw-r--r--   0        0        0      452 2024-05-30 19:55:10.728737 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      454 2024-05-30 19:55:10.728833 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      450 2024-05-30 19:55:10.728928 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      411 2024-05-30 19:55:10.729023 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_tags.py
+-rw-r--r--   0        0        0      727 2024-05-30 19:55:10.729116 carbon_python_sdk-0.2.1/carbon/pydantic/white_labeling_response.py
+-rw-r--r--   0        0        0      887 2024-05-30 19:55:10.729208 carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response.py
+-rw-r--r--   0        0        0      616 2024-05-30 19:55:10.729307 carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0      433 2024-05-30 19:55:10.729409 carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0      737 2024-05-30 19:55:10.729501 carbon_python_sdk-0.2.1/carbon/pydantic/zendesk_authentication.py
+-rw-r--r--   0        0        0      848 2024-05-30 19:55:10.729591 carbon_python_sdk-0.2.1/carbon/pydantic/zotero_authentication.py
+-rw-r--r--   0        0        0      654 2024-05-30 19:55:10.729683 carbon_python_sdk-0.2.1/carbon/request_after_hook.py
+-rw-r--r--   0        0        0      712 2024-05-30 19:55:10.729783 carbon_python_sdk-0.2.1/carbon/request_before_hook.py
+-rw-r--r--   0        0        0      677 2024-05-30 19:55:10.729877 carbon_python_sdk-0.2.1/carbon/request_before_url_hook.py
+-rw-r--r--   0        0        0    10974 2024-05-30 19:55:10.729974 carbon_python_sdk-0.2.1/carbon/rest.py
+-rw-r--r--   0        0        0    96042 2024-05-30 19:55:10.730197 carbon_python_sdk-0.2.1/carbon/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-30 19:55:10.730326 carbon_python_sdk-0.2.1/carbon/type/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-30 19:55:10.730426 carbon_python_sdk-0.2.1/carbon/type/add_webhook_props.py
+-rw-r--r--   0        0        0      627 2024-05-30 19:55:10.730520 carbon_python_sdk-0.2.1/carbon/type/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0      628 2024-05-30 19:55:10.730606 carbon_python_sdk-0.2.1/carbon/type/chunk_properties.py
+-rw-r--r--   0        0        0      668 2024-05-30 19:55:10.730720 carbon_python_sdk-0.2.1/carbon/type/chunk_properties_nullable.py
+-rw-r--r--   0        0        0      725 2024-05-30 19:55:10.730806 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings.py
+-rw-r--r--   0        0        0      408 2024-05-30 19:55:10.730895 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1117 2024-05-30 19:55:10.730980 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0      377 2024-05-30 19:55:10.731081 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_upload_input_custom_credentials.py
+-rw-r--r--   0        0        0      346 2024-05-30 19:55:10.731168 carbon_python_sdk-0.2.1/carbon/type/configuration_keys.py
+-rw-r--r--   0        0        0      714 2024-05-30 19:55:10.731257 carbon_python_sdk-0.2.1/carbon/type/confluence_authentication.py
+-rw-r--r--   0        0        0     1664 2024-05-30 19:55:10.731345 carbon_python_sdk-0.2.1/carbon/type/connect_data_source_input.py
+-rw-r--r--   0        0        0      733 2024-05-30 19:55:10.731432 carbon_python_sdk-0.2.1/carbon/type/connect_data_source_response.py
+-rw-r--r--   0        0        0      420 2024-05-30 19:55:10.731697 carbon_python_sdk-0.2.1/carbon/type/custom_credentials_type.py
+-rw-r--r--   0        0        0      352 2024-05-30 19:55:10.731816 carbon_python_sdk-0.2.1/carbon/type/data_source_extended_input.py
+-rw-r--r--   0        0        0      395 2024-05-30 19:55:10.731917 carbon_python_sdk-0.2.1/carbon/type/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      411 2024-05-30 19:55:10.732012 carbon_python_sdk-0.2.1/carbon/type/data_source_sync_statuses.py
+-rw-r--r--   0        0        0      829 2024-05-30 19:55:10.732107 carbon_python_sdk-0.2.1/carbon/type/data_source_type.py
+-rw-r--r--   0        0        0      837 2024-05-30 19:55:10.732203 carbon_python_sdk-0.2.1/carbon/type/data_source_type_nullable.py
+-rw-r--r--   0        0        0      929 2024-05-30 19:55:10.732307 carbon_python_sdk-0.2.1/carbon/type/delete_files_query_input.py
+-rw-r--r--   0        0        0      387 2024-05-30 19:55:10.732403 carbon_python_sdk-0.2.1/carbon/type/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0      723 2024-05-30 19:55:10.732493 carbon_python_sdk-0.2.1/carbon/type/delete_files_v2_query_input.py
+-rw-r--r--   0        0        0      647 2024-05-30 19:55:10.732592 carbon_python_sdk-0.2.1/carbon/type/delete_users_input.py
+-rw-r--r--   0        0        0      369 2024-05-30 19:55:10.732688 carbon_python_sdk-0.2.1/carbon/type/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0      574 2024-05-30 19:55:10.732783 carbon_python_sdk-0.2.1/carbon/type/directory_item.py
+-rw-r--r--   0        0        0     1356 2024-05-30 19:55:10.733004 carbon_python_sdk-0.2.1/carbon/type/document_response.py
+-rw-r--r--   0        0        0      641 2024-05-30 19:55:10.733153 carbon_python_sdk-0.2.1/carbon/type/document_response_list.py
+-rw-r--r--   0        0        0      350 2024-05-30 19:55:10.733253 carbon_python_sdk-0.2.1/carbon/type/document_response_tags.py
+-rw-r--r--   0        0        0      402 2024-05-30 19:55:10.733344 carbon_python_sdk-0.2.1/carbon/type/document_response_vector.py
+-rw-r--r--   0        0        0      877 2024-05-30 19:55:10.733437 carbon_python_sdk-0.2.1/carbon/type/embedding_and_chunk.py
+-rw-r--r--   0        0        0      406 2024-05-30 19:55:10.733523 carbon_python_sdk-0.2.1/carbon/type/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0      682 2024-05-30 19:55:10.733607 carbon_python_sdk-0.2.1/carbon/type/embedding_generators.py
+-rw-r--r--   0        0        0      690 2024-05-30 19:55:10.733694 carbon_python_sdk-0.2.1/carbon/type/embedding_generators_nullable.py
+-rw-r--r--   0        0        0      610 2024-05-30 19:55:10.733772 carbon_python_sdk-0.2.1/carbon/type/embedding_properties.py
+-rw-r--r--   0        0        0      729 2024-05-30 19:55:10.733857 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0      409 2024-05-30 19:55:10.733941 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0     1009 2024-05-30 19:55:10.734037 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0      694 2024-05-30 19:55:10.734136 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0      492 2024-05-30 19:55:10.734219 carbon_python_sdk-0.2.1/carbon/type/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1189 2024-05-30 19:55:10.734300 carbon_python_sdk-0.2.1/carbon/type/external_source_item.py
+-rw-r--r--   0        0        0      394 2024-05-30 19:55:10.734383 carbon_python_sdk-0.2.1/carbon/type/external_source_items_order_by.py
+-rw-r--r--   0        0        0      689 2024-05-30 19:55:10.734467 carbon_python_sdk-0.2.1/carbon/type/fetch_urls_response.py
+-rw-r--r--   0        0        0      363 2024-05-30 19:55:10.734553 carbon_python_sdk-0.2.1/carbon/type/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0      384 2024-05-30 19:55:10.734636 carbon_python_sdk-0.2.1/carbon/type/file_content_types.py
+-rw-r--r--   0        0        0      392 2024-05-30 19:55:10.734727 carbon_python_sdk-0.2.1/carbon/type/file_content_types_nullable.py
+-rw-r--r--   0        0        0      759 2024-05-30 19:55:10.734812 carbon_python_sdk-0.2.1/carbon/type/file_formats.py
+-rw-r--r--   0        0        0      767 2024-05-30 19:55:10.734899 carbon_python_sdk-0.2.1/carbon/type/file_formats_nullable.py
+-rw-r--r--   0        0        0      823 2024-05-30 19:55:10.734986 carbon_python_sdk-0.2.1/carbon/type/file_statistics.py
+-rw-r--r--   0        0        0      863 2024-05-30 19:55:10.735071 carbon_python_sdk-0.2.1/carbon/type/file_statistics_nullable.py
+-rw-r--r--   0        0        0     1035 2024-05-30 19:55:10.735149 carbon_python_sdk-0.2.1/carbon/type/file_sync_config.py
+-rw-r--r--   0        0        0     1075 2024-05-30 19:55:10.735231 carbon_python_sdk-0.2.1/carbon/type/file_sync_config_nullable.py
+-rw-r--r--   0        0        0      427 2024-05-30 19:55:10.735319 carbon_python_sdk-0.2.1/carbon/type/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     1449 2024-05-30 19:55:10.735395 carbon_python_sdk-0.2.1/carbon/type/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0      669 2024-05-30 19:55:10.735480 carbon_python_sdk-0.2.1/carbon/type/freskdesk_authentication.py
+-rw-r--r--   0        0        0      565 2024-05-30 19:55:10.735567 carbon_python_sdk-0.2.1/carbon/type/generic_success_response.py
+-rw-r--r--   0        0        0     2735 2024-05-30 19:55:10.735646 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body.py
+-rw-r--r--   0        0        0      391 2024-05-30 19:55:10.735727 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0      397 2024-05-30 19:55:10.735811 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0      416 2024-05-30 19:55:10.735893 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0      359 2024-05-30 19:55:10.735977 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0      670 2024-05-30 19:55:10.736057 carbon_python_sdk-0.2.1/carbon/type/gitbook_authetication.py
+-rw-r--r--   0        0        0     1272 2024-05-30 19:55:10.736135 carbon_python_sdk-0.2.1/carbon/type/gitbook_connect_request.py
+-rw-r--r--   0        0        0     1168 2024-05-30 19:55:10.736210 carbon_python_sdk-0.2.1/carbon/type/gitbook_sync_request.py
+-rw-r--r--   0        0        0      368 2024-05-30 19:55:10.736413 carbon_python_sdk-0.2.1/carbon/type/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0      661 2024-05-30 19:55:10.736499 carbon_python_sdk-0.2.1/carbon/type/github_authentication.py
+-rw-r--r--   0        0        0      709 2024-05-30 19:55:10.736584 carbon_python_sdk-0.2.1/carbon/type/github_connect_request.py
+-rw-r--r--   0        0        0      711 2024-05-30 19:55:10.736666 carbon_python_sdk-0.2.1/carbon/type/github_fetch_repos_request.py
+-rw-r--r--   0        0        0      370 2024-05-30 19:55:10.736748 carbon_python_sdk-0.2.1/carbon/type/github_fetch_repos_request_repos.py
+-rw-r--r--   0        0        0     1351 2024-05-30 19:55:10.736838 carbon_python_sdk-0.2.1/carbon/type/gmail_sync_input.py
+-rw-r--r--   0        0        0      371 2024-05-30 19:55:10.736920 carbon_python_sdk-0.2.1/carbon/type/helpdesk_file_types.py
+-rw-r--r--   0        0        0      630 2024-05-30 19:55:10.736998 carbon_python_sdk-0.2.1/carbon/type/http_validation_error.py
+-rw-r--r--   0        0        0      636 2024-05-30 19:55:10.737075 carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0      676 2024-05-30 19:55:10.737161 carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0     1025 2024-05-30 19:55:10.737267 carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_request.py
+-rw-r--r--   0        0        0      695 2024-05-30 19:55:10.737365 carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_response.py
+-rw-r--r--   0        0        0      854 2024-05-30 19:55:10.737453 carbon_python_sdk-0.2.1/carbon/type/list_items_filters.py
+-rw-r--r--   0        0        0      386 2024-05-30 19:55:10.737544 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_external_ids.py
+-rw-r--r--   0        0        0      378 2024-05-30 19:55:10.737629 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_ids.py
+-rw-r--r--   0        0        0      944 2024-05-30 19:55:10.737725 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable.py
+-rw-r--r--   0        0        0      394 2024-05-30 19:55:10.737810 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable_external_ids.py
+-rw-r--r--   0        0        0      386 2024-05-30 19:55:10.737892 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable_ids.py
+-rw-r--r--   0        0        0      544 2024-05-30 19:55:10.737971 carbon_python_sdk-0.2.1/carbon/type/list_request.py
+-rw-r--r--   0        0        0      587 2024-05-30 19:55:10.738049 carbon_python_sdk-0.2.1/carbon/type/list_response.py
+-rw-r--r--   0        0        0      709 2024-05-30 19:55:10.738140 carbon_python_sdk-0.2.1/carbon/type/modify_user_configuration_input.py
+-rw-r--r--   0        0        0      358 2024-05-30 19:57:32.279999 carbon_python_sdk-0.2.1/carbon/type/multi_modal_embedding_generators.py
+-rw-r--r--   0        0        0      665 2024-05-30 19:55:10.738325 carbon_python_sdk-0.2.1/carbon/type/notion_authentication.py
+-rw-r--r--   0        0        0      696 2024-05-30 19:55:10.738415 carbon_python_sdk-0.2.1/carbon/type/o_auth_authentication.py
+-rw-r--r--   0        0        0     3249 2024-05-30 19:57:32.280188 carbon_python_sdk-0.2.1/carbon/type/o_auth_url_request.py
+-rw-r--r--   0        0        0      356 2024-05-30 19:55:10.738598 carbon_python_sdk-0.2.1/carbon/type/order_dir.py
+-rw-r--r--   0        0        0      358 2024-05-30 19:55:10.738686 carbon_python_sdk-0.2.1/carbon/type/order_dir_v2.py
+-rw-r--r--   0        0        0     1922 2024-05-30 19:55:10.738771 carbon_python_sdk-0.2.1/carbon/type/organization_response.py
+-rw-r--r--   0        0        0     1567 2024-05-30 19:55:10.738863 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_api.py
+-rw-r--r--   0        0        0      937 2024-05-30 19:55:10.738956 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0      395 2024-05-30 19:55:10.739056 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0      401 2024-05-30 19:55:10.739155 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0     1070 2024-05-30 19:55:10.739251 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0      767 2024-05-30 19:55:10.739344 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_response.py
+-rw-r--r--   0        0        0      759 2024-05-30 19:55:10.739432 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0      363 2024-05-30 19:55:10.739524 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0      767 2024-05-30 19:55:10.739615 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0      376 2024-05-30 19:55:10.739708 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     5041 2024-05-30 19:55:10.739821 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0      408 2024-05-30 19:55:10.739921 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0      396 2024-05-30 19:55:10.740140 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0      421 2024-05-30 19:55:10.740237 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0      406 2024-05-30 19:55:10.740331 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0      403 2024-05-30 19:55:10.740422 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_request_ids.py
+-rw-r--r--   0        0        0      368 2024-05-30 19:55:10.740513 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0      440 2024-05-30 19:55:10.740610 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1228 2024-05-30 19:55:10.740699 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0      531 2024-05-30 19:55:10.740789 carbon_python_sdk-0.2.1/carbon/type/outh_url_response.py
+-rw-r--r--   0        0        0     1395 2024-05-30 19:55:10.740877 carbon_python_sdk-0.2.1/carbon/type/outlook_sync_input.py
+-rw-r--r--   0        0        0      519 2024-05-30 19:55:10.740972 carbon_python_sdk-0.2.1/carbon/type/pagination.py
+-rw-r--r--   0        0        0      560 2024-05-30 19:55:10.741065 carbon_python_sdk-0.2.1/carbon/type/presigned_url_response.py
+-rw-r--r--   0        0        0      900 2024-05-30 19:55:10.741147 carbon_python_sdk-0.2.1/carbon/type/raw_text_input.py
+-rw-r--r--   0        0        0      662 2024-05-30 19:55:10.741236 carbon_python_sdk-0.2.1/carbon/type/resync_file_query_input.py
+-rw-r--r--   0        0        0      571 2024-05-30 19:55:10.741327 carbon_python_sdk-0.2.1/carbon/type/revoke_access_token_input.py
+-rw-r--r--   0        0        0     1002 2024-05-30 19:55:10.741416 carbon_python_sdk-0.2.1/carbon/type/rss_feed_input.py
+-rw-r--r--   0        0        0      681 2024-05-30 19:55:10.741501 carbon_python_sdk-0.2.1/carbon/type/s3_auth_request.py
+-rw-r--r--   0        0        0      648 2024-05-30 19:55:10.741589 carbon_python_sdk-0.2.1/carbon/type/s3_authentication.py
+-rw-r--r--   0        0        0     1521 2024-05-30 19:55:10.741681 carbon_python_sdk-0.2.1/carbon/type/s3_file_sync_input.py
+-rw-r--r--   0        0        0      570 2024-05-30 19:55:10.741770 carbon_python_sdk-0.2.1/carbon/type/s3_get_file_input.py
+-rw-r--r--   0        0        0      711 2024-05-30 19:55:10.741852 carbon_python_sdk-0.2.1/carbon/type/salesforce_authentication.py
+-rw-r--r--   0        0        0      736 2024-05-30 19:55:10.741936 carbon_python_sdk-0.2.1/carbon/type/sharepoint_authentication.py
+-rw-r--r--   0        0        0      433 2024-05-30 19:55:10.742150 carbon_python_sdk-0.2.1/carbon/type/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0      831 2024-05-30 19:55:10.742234 carbon_python_sdk-0.2.1/carbon/type/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     1662 2024-05-30 19:55:10.742320 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request.py
+-rw-r--r--   0        0        0      395 2024-05-30 19:55:10.742413 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      397 2024-05-30 19:55:10.742506 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      393 2024-05-30 19:55:10.742599 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      354 2024-05-30 19:55:10.742688 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0      561 2024-05-30 19:55:10.742772 carbon_python_sdk-0.2.1/carbon/type/sync_directory_request.py
+-rw-r--r--   0        0        0      527 2024-05-30 19:55:10.742851 carbon_python_sdk-0.2.1/carbon/type/sync_files_ids.py
+-rw-r--r--   0        0        0     1816 2024-05-30 19:55:10.742928 carbon_python_sdk-0.2.1/carbon/type/sync_files_request.py
+-rw-r--r--   0        0        0     2058 2024-05-30 19:55:10.743003 carbon_python_sdk-0.2.1/carbon/type/sync_options.py
+-rw-r--r--   0        0        0      665 2024-05-30 19:55:10.743083 carbon_python_sdk-0.2.1/carbon/type/text_embedding_generators.py
+-rw-r--r--   0        0        0      548 2024-05-30 19:55:10.743156 carbon_python_sdk-0.2.1/carbon/type/token_response.py
+-rw-r--r--   0        0        0      697 2024-05-30 19:55:10.743235 carbon_python_sdk-0.2.1/carbon/type/update_organization_input.py
+-rw-r--r--   0        0        0     1513 2024-05-30 19:55:10.743311 carbon_python_sdk-0.2.1/carbon/type/update_users_input.py
+-rw-r--r--   0        0        0      369 2024-05-30 19:55:10.743392 carbon_python_sdk-0.2.1/carbon/type/update_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1133 2024-05-30 19:55:10.743472 carbon_python_sdk-0.2.1/carbon/type/upload_file_from_url_input.py
+-rw-r--r--   0        0        0     1396 2024-05-30 19:55:10.743550 carbon_python_sdk-0.2.1/carbon/type/user_configuration.py
+-rw-r--r--   0        0        0     1436 2024-05-30 19:55:10.743633 carbon_python_sdk-0.2.1/carbon/type/user_configuration_nullable.py
+-rw-r--r--   0        0        0     2555 2024-05-30 19:55:10.743721 carbon_python_sdk-0.2.1/carbon/type/user_file.py
+-rw-r--r--   0        0        0      422 2024-05-30 19:55:10.743804 carbon_python_sdk-0.2.1/carbon/type/user_file_embedding_properties.py
+-rw-r--r--   0        0        0      586 2024-05-30 19:55:10.743882 carbon_python_sdk-0.2.1/carbon/type/user_files_v2.py
+-rw-r--r--   0        0        0      548 2024-05-30 19:55:10.743961 carbon_python_sdk-0.2.1/carbon/type/user_request_content.py
+-rw-r--r--   0        0        0     2011 2024-05-30 19:55:10.744037 carbon_python_sdk-0.2.1/carbon/type/user_response.py
+-rw-r--r--   0        0        0      442 2024-05-30 19:55:10.744210 carbon_python_sdk-0.2.1/carbon/type/user_response_auto_sync_enabled_sources.py
+-rw-r--r--   0        0        0      371 2024-05-30 19:55:10.744288 carbon_python_sdk-0.2.1/carbon/type/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0      439 2024-05-30 19:55:10.744368 carbon_python_sdk-0.2.1/carbon/type/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0      633 2024-05-30 19:55:10.744444 carbon_python_sdk-0.2.1/carbon/type/validation_error.py
+-rw-r--r--   0        0        0      379 2024-05-30 19:55:10.744521 carbon_python_sdk-0.2.1/carbon/type/validation_error_loc.py
+-rw-r--r--   0        0        0      719 2024-05-30 19:55:10.744607 carbon_python_sdk-0.2.1/carbon/type/webhook.py
+-rw-r--r--   0        0        0      613 2024-05-30 19:55:10.744686 carbon_python_sdk-0.2.1/carbon/type/webhook_filters.py
+-rw-r--r--   0        0        0      376 2024-05-30 19:55:10.744761 carbon_python_sdk-0.2.1/carbon/type/webhook_filters_ids.py
+-rw-r--r--   0        0        0      722 2024-05-30 19:55:10.744835 carbon_python_sdk-0.2.1/carbon/type/webhook_no_key.py
+-rw-r--r--   0        0        0      382 2024-05-30 19:55:10.744922 carbon_python_sdk-0.2.1/carbon/type/webhook_order_by_columns.py
+-rw-r--r--   0        0        0      855 2024-05-30 19:55:10.745007 carbon_python_sdk-0.2.1/carbon/type/webhook_query_input.py
+-rw-r--r--   0        0        0      644 2024-05-30 19:55:10.745092 carbon_python_sdk-0.2.1/carbon/type/webhook_query_response.py
+-rw-r--r--   0        0        0      367 2024-05-30 19:55:10.745172 carbon_python_sdk-0.2.1/carbon/type/webhook_status.py
+-rw-r--r--   0        0        0     1633 2024-05-30 19:55:10.745252 carbon_python_sdk-0.2.1/carbon/type/webscrape_request.py
+-rw-r--r--   0        0        0      391 2024-05-30 19:55:10.745335 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      393 2024-05-30 19:55:10.745418 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      389 2024-05-30 19:55:10.745498 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      350 2024-05-30 19:55:10.745575 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_tags.py
+-rw-r--r--   0        0        0      675 2024-05-30 19:55:10.745769 carbon_python_sdk-0.2.1/carbon/type/white_labeling_response.py
+-rw-r--r--   0        0        0      826 2024-05-30 19:55:10.745849 carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response.py
+-rw-r--r--   0        0        0      551 2024-05-30 19:55:10.745926 carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0      372 2024-05-30 19:55:10.746010 carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0      667 2024-05-30 19:55:10.746088 carbon_python_sdk-0.2.1/carbon/type/zendesk_authentication.py
+-rw-r--r--   0        0        0      711 2024-05-30 19:55:10.746171 carbon_python_sdk-0.2.1/carbon/type/zotero_authentication.py
+-rw-r--r--   0        0        0      514 2024-05-30 19:55:10.746253 carbon_python_sdk-0.2.1/carbon/type_util.py
+-rw-r--r--   0        0        0     3162 2024-05-30 19:55:10.746335 carbon_python_sdk-0.2.1/carbon/validation_metadata.py
+-rw-r--r--   0        0        0      746 2024-05-30 19:57:32.280490 carbon_python_sdk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0   113755 1970-01-01 00:00:00.000000 carbon_python_sdk-0.2.1/PKG-INFO
```

### Comparing `carbon_python_sdk-0.2.0/LICENSE` & `carbon_python_sdk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/README.md` & `carbon_python_sdk-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Visit Carbon](https://raw.githubusercontent.com/Carbon-for-Developers/carbon-sdks/HEAD/python/header.png)](https://carbon.ai)
 
 # Carbon<a id="carbon"></a>
 
 Connect external data to LLMs, no matter the source.
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v0.2.0-blue)](https://pypi.org/project/carbon-python-sdk/0.2.0)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.2.1-blue)](https://pypi.org/project/carbon-python-sdk/0.2.1)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/Carbon-for-Developers/carbon-sdks/tree/main/python#readme)
 
 </div>
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
@@ -87,15 +87,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install carbon-python-sdk==0.2.0
+pip install carbon-python-sdk==0.2.1
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from carbon import Carbon
 
@@ -1092,15 +1092,15 @@
 ```python
 upload_response = carbon.files.upload(
     file=open("/path/to/file", "rb"),
     chunk_size=1,
     chunk_overlap=1,
     skip_embedding_generation=False,
     set_page_as_boundary=False,
-    embedding_model="OPENAI",
+    embedding_model="string_example",
     use_ocr=False,
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     parse_pdf_tables_with_ocr=False,
     detect_audio_language=False,
     media_type="TEXT",
@@ -1123,15 +1123,16 @@
 
 Flag to control whether or not embeddings should be generated and stored             when processing file.
 
 ##### set_page_as_boundary: `bool`<a id="set_page_as_boundary-bool"></a>
 
 Flag to control whether or not to set the a page's worth of content as the maximum             amount of content that can appear in a chunk. Only valid for PDFs. See description route description for             more information.
 
-##### embedding_model: [`TextEmbeddingGenerators`](./carbon/type/.py)<a id="embedding_model-textembeddinggeneratorscarbontypepy"></a>
+##### embedding_model: Union[[`TextEmbeddingGenerators`](./carbon/type/text_embedding_generators.py), `str`]<a id="embedding_model-uniontextembeddinggeneratorscarbontypetext_embedding_generatorspy-str"></a>
+
 
 Embedding model that will be used to embed file chunks.
 
 ##### use_ocr: `bool`<a id="use_ocr-bool"></a>
 
 Whether or not to use OCR when processing files. Only valid for PDFs. Useful for documents with             tables, images, and/or scanned text.
 
@@ -1339,15 +1340,15 @@
         "chunk_overlap": 20,
         "skip_embedding_generation": False,
         "embedding_model": "OPENAI",
         "generate_sparse_vectors": False,
         "prepend_filename_to_chunks": False,
         "sync_files_on_connection": True,
         "set_page_as_boundary": False,
-        "request_id": "f5552316-5da3-46e6-ad9f-2f94e30d02cd",
+        "request_id": "fceb0182-329c-4e45-953b-885c747cf4a3",
         "enable_file_picker": True,
         "sync_source_items": True,
         "incremental_sync": False,
     },
 )
 ```
 
@@ -1592,15 +1593,15 @@
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     salesforce_domain="string_example",
     sync_files_on_connection=True,
     set_page_as_boundary=False,
     data_source_id=1,
     connecting_new_account=False,
-    request_id="273420dd-e05c-463f-a3cf-0ff28029639e",
+    request_id="ce1b1ec8-be64-491c-9159-c40f85fa0073",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     enable_file_picker=True,
     sync_source_items=True,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
@@ -1666,15 +1667,15 @@
 
 Enable OCR for files that support it. Supported formats: pdf
 
 ##### parse_pdf_tables_with_ocr: `Optional[bool]`<a id="parse_pdf_tables_with_ocr-optionalbool"></a>
 
 ##### enable_file_picker: `bool`<a id="enable_file_picker-bool"></a>
 
-Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, DROPBOX, GOOGLE_DRIVE, BOX, ONEDRIVE
+Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
 
 ##### sync_source_items: `bool`<a id="sync_source_items-bool"></a>
 
 Enabling this flag will fetch all available content from the source to be listed via list items endpoint
 
 ##### incremental_sync: `bool`<a id="incremental_sync-bool"></a>
 
@@ -1937,15 +1938,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="2782cb96-1bf6-452c-a8d9-60c2378fd079",
+    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
@@ -2057,15 +2058,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="2782cb96-1bf6-452c-a8d9-60c2378fd079",
+    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
```

### Comparing `carbon_python_sdk-0.2.0/carbon/__init__.py` & `carbon_python_sdk-0.2.1/carbon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Connect external data to LLMs, no matter the source.
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 # import ApiClient
 from carbon.api_client import ApiClient
 
 # import Configuration
 from carbon.configuration import Configuration
```

### Comparing `carbon_python_sdk-0.2.0/carbon/api_client.py` & `carbon_python_sdk-0.2.1/carbon/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2961,15 +2961,15 @@
 0000b900: 5f6e 616d 655d 203d 2068 6561 6465 725f  _name] = header_
 0000b910: 7661 6c75 650a 2020 2020 2020 2020 7365  value.        se
 0000b920: 6c66 2e63 6f6f 6b69 6520 3d20 636f 6f6b  lf.cookie = cook
 0000b930: 6965 0a20 2020 2020 2020 2023 2053 6574  ie.        # Set
 0000b940: 2064 6566 6175 6c74 2055 7365 722d 4167   default User-Ag
 0000b950: 656e 742e 0a20 2020 2020 2020 2073 656c  ent..        sel
 0000b960: 662e 7573 6572 5f61 6765 6e74 203d 2027  f.user_agent = '
-0000b970: 4b6f 6e66 6967 2f30 2e32 2e30 2f70 7974  Konfig/0.2.0/pyt
+0000b970: 4b6f 6e66 6967 2f30 2e32 2e31 2f70 7974  Konfig/0.2.1/pyt
 0000b980: 686f 6e27 0a0a 2020 2020 6465 6620 5f5f  hon'..    def __
 0000b990: 656e 7465 725f 5f28 7365 6c66 293a 0a20  enter__(self):. 
 0000b9a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
 0000b9b0: 6c66 0a0a 2020 2020 6465 6620 5f5f 6578  lf..    def __ex
 0000b9c0: 6974 5f5f 2873 656c 662c 2065 7863 5f74  it__(self, exc_t
 0000b9d0: 7970 652c 2065 7863 5f76 616c 7565 2c20  ype, exc_value, 
 0000b9e0: 7472 6163 6562 6163 6b29 3a0a 2020 2020  traceback):.
```

### Comparing `carbon_python_sdk-0.2.0/carbon/api_response.py` & `carbon_python_sdk-0.2.1/carbon/api_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/path_to_api.py` & `carbon_python_sdk-0.2.1/carbon/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tag_to_api.py` & `carbon_python_sdk-0.2.1/carbon/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/__init__.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/auth_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/data_sources_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/embeddings_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/embeddings_api_raw.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/files_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/files_api_raw.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/health_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/health_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/integrations_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/integrations_api_raw.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/organizations_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/organizations_api_raw.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/users_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/users_api_raw.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/utilities_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/utilities_api_raw.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/webhooks_api_generated.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/apis/tags/webhooks_api_raw.py` & `carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/client.py` & `carbon_python_sdk-0.2.1/carbon/client.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/client.pyi` & `carbon_python_sdk-0.2.1/carbon/client.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/client_custom.py` & `carbon_python_sdk-0.2.1/carbon/client_custom.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/configuration.py` & `carbon_python_sdk-0.2.1/carbon/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.2.0".\
+               "SDK Package Version: 0.2.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `carbon_python_sdk-0.2.0/carbon/exceptions.py` & `carbon_python_sdk-0.2.1/carbon/exceptions.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/exceptions_base.py` & `carbon_python_sdk-0.2.1/carbon/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/add_webhook_props.py` & `carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/add_webhook_props.pyi` & `carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/body_create_upload_file_uploadfile_post.pyi` & `carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunk_properties.py` & `carbon_python_sdk-0.2.1/carbon/model/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunk_properties.pyi` & `carbon_python_sdk-0.2.1/carbon/model/chunk_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunk_properties_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunk_properties_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings.py` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings.pyi` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_embedding.py` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_embedding.pyi` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi` & `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/configuration_keys.py` & `carbon_python_sdk-0.2.1/carbon/model/configuration_keys.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/configuration_keys.pyi` & `carbon_python_sdk-0.2.1/carbon/model/configuration_keys.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/confluence_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/confluence_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/connect_data_source_input.py` & `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/connect_data_source_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/connect_data_source_response.py` & `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/connect_data_source_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/custom_credentials_type.py` & `carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/custom_credentials_type.pyi` & `carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_extended_input.py` & `carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_extended_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_last_sync_actions.py` & `carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_last_sync_actions.pyi` & `carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_sync_statuses.py` & `carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_sync_statuses.pyi` & `carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_type.py` & `carbon_python_sdk-0.2.1/carbon/model/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_type.pyi` & `carbon_python_sdk-0.2.1/carbon/model/data_source_type.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_type_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/data_source_type_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input.py` & `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input_file_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_files_query_input_file_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_files_v2_query_input.py` & `carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_files_v2_query_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_users_input.py` & `carbon_python_sdk-0.2.1/carbon/model/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_users_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/delete_users_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_users_input_customer_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/delete_users_input_customer_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/directory_item.py` & `carbon_python_sdk-0.2.1/carbon/model/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/directory_item.pyi` & `carbon_python_sdk-0.2.1/carbon/model/directory_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response.py` & `carbon_python_sdk-0.2.1/carbon/model/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/document_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response_list.py` & `carbon_python_sdk-0.2.1/carbon/model/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response_list.pyi` & `carbon_python_sdk-0.2.1/carbon/model/document_response_list.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/document_response_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/document_response_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response_vector.py` & `carbon_python_sdk-0.2.1/carbon/model/document_response_vector.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/document_response_vector.pyi` & `carbon_python_sdk-0.2.1/carbon/model/document_response_vector.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk.py` & `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk_embedding.py` & `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_and_chunk_embedding.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_generators.py` & `carbon_python_sdk-0.2.1/carbon/model/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_generators.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embedding_generators.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_generators_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_generators_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_properties.py` & `carbon_python_sdk-0.2.1/carbon/model/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embedding_properties.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embedding_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_filters.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_order_by_columns.py` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_order_by_columns.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_query_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/embeddings_and_chunks_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/external_file_sync_statuses.py` & `carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/external_file_sync_statuses.pyi` & `carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/external_source_item.py` & `carbon_python_sdk-0.2.1/carbon/model/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/external_source_item.pyi` & `carbon_python_sdk-0.2.1/carbon/model/external_source_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/external_source_items_order_by.py` & `carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/external_source_items_order_by.pyi` & `carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response.py` & `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response_urls.py` & `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/fetch_urls_response_urls.pyi` & `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_content_types.py` & `carbon_python_sdk-0.2.1/carbon/model/file_content_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_content_types.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_content_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_content_types_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_content_types_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_formats.py` & `carbon_python_sdk-0.2.1/carbon/model/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_formats.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_formats.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_formats_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_formats_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_statistics.py` & `carbon_python_sdk-0.2.1/carbon/model/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_statistics.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_statistics.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_statistics_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_statistics_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_sync_config.py` & `carbon_python_sdk-0.2.1/carbon/model/file_sync_config.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_sync_config.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_sync_config.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_sync_config_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/file_sync_config_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/files_query_user_files_deprecated_response.py` & `carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/files_query_user_files_deprecated_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/fresh_desk_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/fresh_desk_connect_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/freskdesk_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/freskdesk_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/generic_success_response.py` & `carbon_python_sdk-0.2.1/carbon/model/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/generic_success_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/generic_success_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body.py` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body.pyi` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_file_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_file_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_parent_file_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_parent_file_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_query_vector.py` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_query_vector.pyi` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/get_embedding_documents_body_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_authetication.py` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_authetication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_connect_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request.py` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request_space_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gitbook_sync_request_space_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/github_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/github_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/model/github_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_connect_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/github_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request.py` & `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request_repos.py` & `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/github_fetch_repos_request_repos.pyi` & `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gmail_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/gmail_sync_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/helpdesk_file_types.py` & `carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/helpdesk_file_types.pyi` & `carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/http_validation_error.py` & `carbon_python_sdk-0.2.1/carbon/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/http_validation_error.pyi` & `carbon_python_sdk-0.2.1/carbon/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params.pyi` & `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/hybrid_search_tuning_params_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_request.py` & `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_response.py` & `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_data_source_items_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters.py` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_external_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_external_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_external_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_external_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_items_filters_nullable_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_request.py` & `carbon_python_sdk-0.2.1/carbon/model/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_response.py` & `carbon_python_sdk-0.2.1/carbon/model/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/list_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/list_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/modify_user_configuration_input.py` & `carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/modify_user_configuration_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/notion_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/notion_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/notion_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/notion_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/o_auth_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/o_auth_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/o_auth_url_request.py` & `carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/o_auth_url_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/order_dir.py` & `carbon_python_sdk-0.2.1/carbon/model/order_dir.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/order_dir.pyi` & `carbon_python_sdk-0.2.1/carbon/model/order_dir.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/order_dir_v2.py` & `carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/order_dir_v2.pyi` & `carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_response.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_api.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_api.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_filters_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_order_by_columns.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_order_by_columns.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_query_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_response.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_data_source_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tag_create_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_file_tags_remove_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_request_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_filters_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_order_by_types.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_order_by_types.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/organization_user_files_to_sync_query_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/outh_url_response.py` & `carbon_python_sdk-0.2.1/carbon/model/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/outh_url_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/outh_url_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/outlook_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/outlook_sync_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/pagination.py` & `carbon_python_sdk-0.2.1/carbon/model/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/pagination.pyi` & `carbon_python_sdk-0.2.1/carbon/model/pagination.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/presigned_url_response.py` & `carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/presigned_url_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/raw_text_input.py` & `carbon_python_sdk-0.2.1/carbon/model/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/raw_text_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/raw_text_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/resync_file_query_input.py` & `carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/resync_file_query_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/revoke_access_token_input.py` & `carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/revoke_access_token_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/rss_feed_input.py` & `carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/rss_feed_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_auth_request.py` & `carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_auth_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/s3_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/s3_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_file_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_file_sync_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_get_file_input.py` & `carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/s3_get_file_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/salesforce_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/salesforce_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sharepoint_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sharepoint_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/simple_o_auth_data_sources.py` & `carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/simple_o_auth_data_sources.pyi` & `carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/single_chunks_and_embeddings_upload_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request.py` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_classes_to_skip.py` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_html_tags_to_skip.py` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sitemap_scrape_request_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_directory_request.py` & `carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_directory_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_files_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_files_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_files_request.py` & `carbon_python_sdk-0.2.1/carbon/model/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_files_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sync_files_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_options.py` & `carbon_python_sdk-0.2.1/carbon/model/sync_options.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/sync_options.pyi` & `carbon_python_sdk-0.2.1/carbon/model/sync_options.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/text_embedding_generators.py` & `carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/text_embedding_generators.pyi` & `carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/token_response.py` & `carbon_python_sdk-0.2.1/carbon/model/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/token_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/token_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/update_organization_input.py` & `carbon_python_sdk-0.2.1/carbon/model/update_organization_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/update_organization_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/update_organization_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/update_users_input.py` & `carbon_python_sdk-0.2.1/carbon/model/update_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/update_users_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/update_users_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/update_users_input_customer_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/update_users_input_customer_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/upload_file_from_url_input.py` & `carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/upload_file_from_url_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_configuration.py` & `carbon_python_sdk-0.2.1/carbon/model/user_configuration.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_configuration.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_configuration.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_configuration_nullable.py` & `carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_configuration_nullable.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_file.py` & `carbon_python_sdk-0.2.1/carbon/model/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_file.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_file.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_file_embedding_properties.py` & `carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_file_embedding_properties.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_files_v2.py` & `carbon_python_sdk-0.2.1/carbon/model/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_files_v2.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_files_v2.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_request_content.py` & `carbon_python_sdk-0.2.1/carbon/model/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_request_content.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_request_content.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_response.py` & `carbon_python_sdk-0.2.1/carbon/model/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_response_auto_sync_enabled_sources.py` & `carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_response_auto_sync_enabled_sources.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_response_unique_file_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/user_response_unique_file_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/utilities_scrape_web_request.py` & `carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/utilities_scrape_web_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/validation_error.py` & `carbon_python_sdk-0.2.1/carbon/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/validation_error.pyi` & `carbon_python_sdk-0.2.1/carbon/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/validation_error_loc.py` & `carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/validation_error_loc.pyi` & `carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_filters.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_filters.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_filters_ids.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_filters_ids.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_no_key.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_no_key.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_order_by_columns.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_order_by_columns.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_query_input.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_query_input.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_query_response.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_query_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_status.py` & `carbon_python_sdk-0.2.1/carbon/model/webhook_status.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webhook_status.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webhook_status.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request.py` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_classes_to_skip.py` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_classes_to_skip.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_selectors_to_skip.py` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_css_selectors_to_skip.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_html_tags_to_skip.py` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_html_tags_to_skip.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_tags.py` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/webscrape_request_tags.pyi` & `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/white_labeling_response.py` & `carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/white_labeling_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response.py` & `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response.pyi` & `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript.pyi` & `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript_item.py` & `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/youtube_transcript_response_raw_transcript_item.pyi` & `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/zendesk_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/zendesk_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/zotero_authentication.py` & `carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/model/zotero_authentication.pyi` & `carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/models/__init__.py` & `carbon_python_sdk-0.2.1/carbon/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 from carbon.model.list_items_filters_ids import ListItemsFiltersIds
 from carbon.model.list_items_filters_nullable import ListItemsFiltersNullable
 from carbon.model.list_items_filters_nullable_external_ids import ListItemsFiltersNullableExternalIds
 from carbon.model.list_items_filters_nullable_ids import ListItemsFiltersNullableIds
 from carbon.model.list_request import ListRequest
 from carbon.model.list_response import ListResponse
 from carbon.model.modify_user_configuration_input import ModifyUserConfigurationInput
+from carbon.model.multi_modal_embedding_generators import MultiModalEmbeddingGenerators
 from carbon.model.notion_authentication import NotionAuthentication
 from carbon.model.o_auth_authentication import OAuthAuthentication
 from carbon.model.o_auth_url_request import OAuthURLRequest
 from carbon.model.order_dir import OrderDir
 from carbon.model.order_dir_v2 import OrderDirV2
 from carbon.model.organization_response import OrganizationResponse
 from carbon.model.organization_user_data_source_api import OrganizationUserDataSourceAPI
```

### Comparing `carbon_python_sdk-0.2.0/carbon/operation_parameter_map.py` & `carbon_python_sdk-0.2.1/carbon/operation_parameter_map.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/__init__.py` & `carbon_python_sdk-0.2.1/carbon/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/add_webhook/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/add_webhook/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/auth_v1_access_token/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/auth_v1_access_token/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/auth_v1_white_labeling/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/auth_v1_white_labeling/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/create_user_file_tags/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/create_user_file_tags/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_files/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_files/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_files_v2/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_files_v2/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_user_file_tags/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_user_file_tags/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_users/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_users/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_webhook_webhook_id/delete.py` & `carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/delete_webhook_webhook_id/delete.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/deletefile_file_id/delete.py` & `carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/deletefile_file_id/delete.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/embeddings/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/embeddings/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/fetch_urls/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/fetch_urls/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/fetch_youtube_transcript/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/fetch_youtube_transcript/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/health/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/health/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/health/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/health/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_list/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_list/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_sync/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_confluence_sync/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_connect/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_connect/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_files_sync/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_files_sync/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_freshdesk/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_freshdesk/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_spaces/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_spaces/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_sync/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gitbook_sync/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_github/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_github/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_github_repos/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_github_repos/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_github_sync_repos/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_github_sync_repos/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_sync/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_sync/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_user_labels/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_gmail_user_labels/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_items_list/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_items_list/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_items_sync/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_items_sync/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_oauth_url/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_oauth_url/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_sync/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_sync/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_categories/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_categories/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_folders/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_outlook_user_folders/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_rss_feed/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_rss_feed/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_s3/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_s3/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_s3_files/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/integrations_s3_files/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/modify_user_configuration/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/modify_user_configuration/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/organization/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/organization/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/organization/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/organization/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/organization_statistics/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/organization_statistics/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/organization_update/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/organization_update/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/parsed_file_file_id/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/parsed_file_file_id/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/process_sitemap/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/process_sitemap/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/raw_file_file_id/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/raw_file_file_id/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/resync_file/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/resync_file/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/revoke_access_token/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/revoke_access_token/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/scrape_sitemap/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/scrape_sitemap/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/search_urls/get.py` & `carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/search_urls/get.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/text_chunks/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/text_chunks/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/update_users/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/update_users/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/update_users/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/update_users/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/upload_chunks_and_embeddings/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/upload_chunks_and_embeddings/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/upload_file_from_url/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/upload_file_from_url/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/upload_text/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/upload_text/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/uploadfile/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,52 @@
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
         )
 SkipEmbeddingGenerationSchema = schemas.BoolSchema
 SetPageAsBoundarySchema = schemas.BoolSchema
-EmbeddingModelSchema = TextEmbeddingGeneratorsSchema
+
+
+class EmbeddingModelSchema(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        any_of_1 = schemas.StrSchema
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                TextEmbeddingGeneratorsSchema,
+                cls.any_of_1,
+            ]
+
+
+    def __new__(
+        cls,
+        *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'EmbeddingModelSchema':
+        return super().__new__(
+            cls,
+            *args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 UseOcrSchema = schemas.BoolSchema
 GenerateSparseVectorsSchema = schemas.BoolSchema
 PrependFilenameToChunksSchema = schemas.BoolSchema
 
 
 class MaxItemsPerChunkSchema(
     schemas.IntBase,
@@ -131,15 +168,15 @@
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
         'chunk_size': typing.Union[ChunkSizeSchema, None, decimal.Decimal, int, ],
         'chunk_overlap': typing.Union[ChunkOverlapSchema, None, decimal.Decimal, int, ],
         'skip_embedding_generation': typing.Union[SkipEmbeddingGenerationSchema, bool, ],
         'set_page_as_boundary': typing.Union[SetPageAsBoundarySchema, bool, ],
-        'embedding_model': typing.Union[EmbeddingModelSchema, ],
+        'embedding_model': typing.Union[EmbeddingModelSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'use_ocr': typing.Union[UseOcrSchema, bool, ],
         'generate_sparse_vectors': typing.Union[GenerateSparseVectorsSchema, bool, ],
         'prepend_filename_to_chunks': typing.Union[PrependFilenameToChunksSchema, bool, ],
         'max_items_per_chunk': typing.Union[MaxItemsPerChunkSchema, None, decimal.Decimal, int, ],
         'parse_pdf_tables_with_ocr': typing.Union[ParsePdfTablesWithOcrSchema, bool, ],
         'detect_audio_language': typing.Union[DetectAudioLanguageSchema, bool, ],
         'media_type': typing.Union[MediaTypeSchema, ],
@@ -175,15 +212,15 @@
     style=api_client.ParameterStyle.FORM,
     schema=SetPageAsBoundarySchema,
     explode=True,
 )
 request_query_embedding_model = api_client.QueryParameter(
     name="embedding_model",
     style=api_client.ParameterStyle.FORM,
-    schema=TextEmbeddingGeneratorsSchema,
+    schema=EmbeddingModelSchema,
     explode=True,
 )
 request_query_use_ocr = api_client.QueryParameter(
     name="use_ocr",
     style=api_client.ParameterStyle.FORM,
     schema=UseOcrSchema,
     explode=True,
@@ -296,15 +333,15 @@
     def _upload_mapped_args(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -601,15 +638,15 @@
     async def aupload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -643,15 +680,15 @@
     def upload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -684,15 +721,15 @@
     async def aupload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -723,15 +760,15 @@
     def upload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -763,15 +800,15 @@
     async def apost(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -805,15 +842,15 @@
     def post(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
```

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/uploadfile/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,52 @@
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
         )
 SkipEmbeddingGenerationSchema = schemas.BoolSchema
 SetPageAsBoundarySchema = schemas.BoolSchema
-EmbeddingModelSchema = TextEmbeddingGeneratorsSchema
+
+
+class EmbeddingModelSchema(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        any_of_1 = schemas.StrSchema
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                TextEmbeddingGeneratorsSchema,
+                cls.any_of_1,
+            ]
+
+
+    def __new__(
+        cls,
+        *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'EmbeddingModelSchema':
+        return super().__new__(
+            cls,
+            *args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 UseOcrSchema = schemas.BoolSchema
 GenerateSparseVectorsSchema = schemas.BoolSchema
 PrependFilenameToChunksSchema = schemas.BoolSchema
 
 
 class MaxItemsPerChunkSchema(
     schemas.IntBase,
@@ -129,15 +166,15 @@
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
         'chunk_size': typing.Union[ChunkSizeSchema, None, decimal.Decimal, int, ],
         'chunk_overlap': typing.Union[ChunkOverlapSchema, None, decimal.Decimal, int, ],
         'skip_embedding_generation': typing.Union[SkipEmbeddingGenerationSchema, bool, ],
         'set_page_as_boundary': typing.Union[SetPageAsBoundarySchema, bool, ],
-        'embedding_model': typing.Union[EmbeddingModelSchema, ],
+        'embedding_model': typing.Union[EmbeddingModelSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'use_ocr': typing.Union[UseOcrSchema, bool, ],
         'generate_sparse_vectors': typing.Union[GenerateSparseVectorsSchema, bool, ],
         'prepend_filename_to_chunks': typing.Union[PrependFilenameToChunksSchema, bool, ],
         'max_items_per_chunk': typing.Union[MaxItemsPerChunkSchema, None, decimal.Decimal, int, ],
         'parse_pdf_tables_with_ocr': typing.Union[ParsePdfTablesWithOcrSchema, bool, ],
         'detect_audio_language': typing.Union[DetectAudioLanguageSchema, bool, ],
         'media_type': typing.Union[MediaTypeSchema, ],
@@ -173,15 +210,15 @@
     style=api_client.ParameterStyle.FORM,
     schema=SetPageAsBoundarySchema,
     explode=True,
 )
 request_query_embedding_model = api_client.QueryParameter(
     name="embedding_model",
     style=api_client.ParameterStyle.FORM,
-    schema=TextEmbeddingGeneratorsSchema,
+    schema=EmbeddingModelSchema,
     explode=True,
 )
 request_query_use_ocr = api_client.QueryParameter(
     name="use_ocr",
     style=api_client.ParameterStyle.FORM,
     schema=UseOcrSchema,
     explode=True,
@@ -285,15 +322,15 @@
     def _upload_mapped_args(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -590,15 +627,15 @@
     async def aupload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -632,15 +669,15 @@
     def upload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -673,15 +710,15 @@
     async def aupload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -712,15 +749,15 @@
     def upload(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -752,15 +789,15 @@
     async def apost(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
@@ -794,15 +831,15 @@
     def post(
         self,
         file: typing.IO,
         chunk_size: typing.Optional[typing.Optional[int]] = None,
         chunk_overlap: typing.Optional[typing.Optional[int]] = None,
         skip_embedding_generation: typing.Optional[bool] = None,
         set_page_as_boundary: typing.Optional[bool] = None,
-        embedding_model: typing.Optional[TextEmbeddingGenerators] = None,
+        embedding_model: typing.Optional[typing.Union[TextEmbeddingGenerators, str]] = None,
         use_ocr: typing.Optional[bool] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
         media_type: typing.Optional[FileContentTypesNullable] = None,
```

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/user/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/user/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user_data_sources/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user_data_sources/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user_files/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/user_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user_files/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/user_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user_files_v2/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/user_files_v2/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/web_scrape/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/web_scrape/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/webhooks/post.py` & `carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/paths/webhooks/post.pyi` & `carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/add_webhook_props.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/chunk_properties.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/chunk_properties_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/chunks_and_embeddings.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/confluence_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/confluence_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/connect_data_source_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/connect_data_source_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/data_source_type.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/data_source_type_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/delete_files_query_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/delete_files_v2_query_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_v2_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/delete_users_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/directory_item.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/document_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/document_response_list.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/embedding_and_chunk.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/embedding_generators.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/embedding_generators_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/embedding_properties.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/external_file_sync_statuses.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/external_file_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/external_source_item.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/fetch_urls_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/file_formats.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/file_formats_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/file_statistics.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/file_statistics_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/file_sync_config.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/file_sync_config_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/fresh_desk_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/freskdesk_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/freskdesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/generic_success_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/get_embedding_documents_body.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/gitbook_authetication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_authetication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/gitbook_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/gitbook_sync_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/github_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/github_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/github_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/github_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/github_fetch_repos_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/github_fetch_repos_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/gmail_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/http_validation_error.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/list_data_source_items_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/list_data_source_items_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/list_items_filters_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/list_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/list_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/modify_user_configuration_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/notion_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/notion_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/o_auth_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/o_auth_url_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_url_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     request_id: typing.Optional[str] = Field(None, alias='request_id')
 
     # Enable OCR for files that support it. Supported formats: pdf
     use_ocr: typing.Optional[typing.Optional[bool]] = Field(None, alias='use_ocr')
 
     parse_pdf_tables_with_ocr: typing.Optional[typing.Optional[bool]] = Field(None, alias='parse_pdf_tables_with_ocr')
 
-    # Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, DROPBOX, GOOGLE_DRIVE, BOX, ONEDRIVE
+    # Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
     enable_file_picker: typing.Optional[bool] = Field(None, alias='enable_file_picker')
 
     # Enabling this flag will fetch all available content from the source to be listed via list items endpoint
     sync_source_items: typing.Optional[bool] = Field(None, alias='sync_source_items')
 
     # Only sync files if they have not already been synced or if the embedding properties have changed.         This flag is currently supported by ONEDRIVE, GOOGLE_DRIVE, BOX, DROPBOX. It will be ignored for other data sources.
     incremental_sync: typing.Optional[bool] = Field(None, alias='incremental_sync')
```

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_api.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_filters.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_data_source_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_file_tag_create.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/outh_url_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/outlook_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/pagination.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/presigned_url_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/raw_text_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/resync_file_query_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/revoke_access_token_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/rss_feed_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/s3_auth_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/s3_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/s3_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/s3_file_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/s3_get_file_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/salesforce_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/salesforce_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/sharepoint_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/sharepoint_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/sitemap_scrape_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/sync_directory_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/sync_files_ids.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/sync_files_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/sync_options.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/sync_options.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/text_embedding_generators.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/token_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/update_organization_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/update_organization_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/update_users_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/update_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/upload_file_from_url_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/upload_file_from_url_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/user_configuration.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/user_configuration_nullable.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/user_file.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/user_files_v2.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/user_request_content.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/user_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/validation_error.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/webhook.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/webhook_filters.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/webhook_no_key.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/webhook_query_input.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/webhook_query_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/webscrape_request.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/white_labeling_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/youtube_transcript_response.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/zendesk_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/zendesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/pydantic/zotero_authentication.py` & `carbon_python_sdk-0.2.1/carbon/pydantic/zotero_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/request_after_hook.py` & `carbon_python_sdk-0.2.1/carbon/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/request_before_hook.py` & `carbon_python_sdk-0.2.1/carbon/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/request_before_url_hook.py` & `carbon_python_sdk-0.2.1/carbon/request_before_url_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/rest.py` & `carbon_python_sdk-0.2.1/carbon/rest.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/schemas.py` & `carbon_python_sdk-0.2.1/carbon/schemas.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/add_webhook_props.py` & `carbon_python_sdk-0.2.1/carbon/type/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.2.1/carbon/type/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/chunk_properties.py` & `carbon_python_sdk-0.2.1/carbon/type/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/chunk_properties_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/chunks_and_embeddings.py` & `carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/confluence_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/confluence_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/connect_data_source_input.py` & `carbon_python_sdk-0.2.1/carbon/type/connect_data_source_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/connect_data_source_response.py` & `carbon_python_sdk-0.2.1/carbon/type/connect_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/data_source_type.py` & `carbon_python_sdk-0.2.1/carbon/type/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/data_source_type_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/delete_files_query_input.py` & `carbon_python_sdk-0.2.1/carbon/type/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/delete_files_v2_query_input.py` & `carbon_python_sdk-0.2.1/carbon/type/delete_files_v2_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/delete_users_input.py` & `carbon_python_sdk-0.2.1/carbon/type/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/directory_item.py` & `carbon_python_sdk-0.2.1/carbon/type/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/document_response.py` & `carbon_python_sdk-0.2.1/carbon/type/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/document_response_list.py` & `carbon_python_sdk-0.2.1/carbon/type/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/embedding_and_chunk.py` & `carbon_python_sdk-0.2.1/carbon/type/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/embedding_generators.py` & `carbon_python_sdk-0.2.1/carbon/type/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/embedding_generators_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/embedding_properties.py` & `carbon_python_sdk-0.2.1/carbon/type/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/external_source_item.py` & `carbon_python_sdk-0.2.1/carbon/type/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/fetch_urls_response.py` & `carbon_python_sdk-0.2.1/carbon/type/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/file_formats.py` & `carbon_python_sdk-0.2.1/carbon/type/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/file_formats_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/file_statistics.py` & `carbon_python_sdk-0.2.1/carbon/type/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/file_statistics_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/file_sync_config.py` & `carbon_python_sdk-0.2.1/carbon/type/file_sync_config.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/file_sync_config_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/file_sync_config_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/fresh_desk_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/type/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/freskdesk_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/freskdesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/generic_success_response.py` & `carbon_python_sdk-0.2.1/carbon/type/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/get_embedding_documents_body.py` & `carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/gitbook_authetication.py` & `carbon_python_sdk-0.2.1/carbon/type/gitbook_authetication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/gitbook_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/type/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/gitbook_sync_request.py` & `carbon_python_sdk-0.2.1/carbon/type/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/github_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/github_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/github_connect_request.py` & `carbon_python_sdk-0.2.1/carbon/type/github_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/github_fetch_repos_request.py` & `carbon_python_sdk-0.2.1/carbon/type/github_fetch_repos_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/gmail_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/type/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/http_validation_error.py` & `carbon_python_sdk-0.2.1/carbon/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/list_data_source_items_request.py` & `carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/list_data_source_items_response.py` & `carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/list_items_filters.py` & `carbon_python_sdk-0.2.1/carbon/type/list_items_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/list_items_filters_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/list_request.py` & `carbon_python_sdk-0.2.1/carbon/type/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/list_response.py` & `carbon_python_sdk-0.2.1/carbon/type/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/modify_user_configuration_input.py` & `carbon_python_sdk-0.2.1/carbon/type/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/notion_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/notion_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/o_auth_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/o_auth_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/o_auth_url_request.py` & `carbon_python_sdk-0.2.1/carbon/type/o_auth_url_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     request_id: str
 
     # Enable OCR for files that support it. Supported formats: pdf
     use_ocr: typing.Optional[bool]
 
     parse_pdf_tables_with_ocr: typing.Optional[bool]
 
-    # Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, DROPBOX, GOOGLE_DRIVE, BOX, ONEDRIVE
+    # Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
     enable_file_picker: bool
 
     # Enabling this flag will fetch all available content from the source to be listed via list items endpoint
     sync_source_items: bool
 
     # Only sync files if they have not already been synced or if the embedding properties have changed.         This flag is currently supported by ONEDRIVE, GOOGLE_DRIVE, BOX, DROPBOX. It will be ignored for other data sources.
     incremental_sync: bool
```

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_response.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_api.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_filters.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_data_source_response.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_file_tag_create.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/outh_url_response.py` & `carbon_python_sdk-0.2.1/carbon/type/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/outlook_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/type/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/pagination.py` & `carbon_python_sdk-0.2.1/carbon/type/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/presigned_url_response.py` & `carbon_python_sdk-0.2.1/carbon/type/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/raw_text_input.py` & `carbon_python_sdk-0.2.1/carbon/type/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/resync_file_query_input.py` & `carbon_python_sdk-0.2.1/carbon/type/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/revoke_access_token_input.py` & `carbon_python_sdk-0.2.1/carbon/type/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/rss_feed_input.py` & `carbon_python_sdk-0.2.1/carbon/type/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/s3_auth_request.py` & `carbon_python_sdk-0.2.1/carbon/type/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/s3_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/s3_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/s3_file_sync_input.py` & `carbon_python_sdk-0.2.1/carbon/type/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/s3_get_file_input.py` & `carbon_python_sdk-0.2.1/carbon/type/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/salesforce_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/salesforce_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/sharepoint_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/sharepoint_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.1/carbon/type/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/sitemap_scrape_request.py` & `carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/sync_directory_request.py` & `carbon_python_sdk-0.2.1/carbon/type/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/sync_files_ids.py` & `carbon_python_sdk-0.2.1/carbon/type/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/sync_files_request.py` & `carbon_python_sdk-0.2.1/carbon/type/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/sync_options.py` & `carbon_python_sdk-0.2.1/carbon/type/sync_options.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/text_embedding_generators.py` & `carbon_python_sdk-0.2.1/carbon/type/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/token_response.py` & `carbon_python_sdk-0.2.1/carbon/type/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/update_organization_input.py` & `carbon_python_sdk-0.2.1/carbon/type/update_organization_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/update_users_input.py` & `carbon_python_sdk-0.2.1/carbon/type/update_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/upload_file_from_url_input.py` & `carbon_python_sdk-0.2.1/carbon/type/upload_file_from_url_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/user_configuration.py` & `carbon_python_sdk-0.2.1/carbon/type/user_configuration.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/user_configuration_nullable.py` & `carbon_python_sdk-0.2.1/carbon/type/user_configuration_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/user_file.py` & `carbon_python_sdk-0.2.1/carbon/type/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/user_files_v2.py` & `carbon_python_sdk-0.2.1/carbon/type/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/user_request_content.py` & `carbon_python_sdk-0.2.1/carbon/type/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/user_response.py` & `carbon_python_sdk-0.2.1/carbon/type/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/validation_error.py` & `carbon_python_sdk-0.2.1/carbon/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/webhook.py` & `carbon_python_sdk-0.2.1/carbon/type/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/webhook_filters.py` & `carbon_python_sdk-0.2.1/carbon/type/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/webhook_no_key.py` & `carbon_python_sdk-0.2.1/carbon/type/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/webhook_query_input.py` & `carbon_python_sdk-0.2.1/carbon/type/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/webhook_query_response.py` & `carbon_python_sdk-0.2.1/carbon/type/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/webscrape_request.py` & `carbon_python_sdk-0.2.1/carbon/type/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/white_labeling_response.py` & `carbon_python_sdk-0.2.1/carbon/type/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/youtube_transcript_response.py` & `carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/zendesk_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/zendesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type/zotero_authentication.py` & `carbon_python_sdk-0.2.1/carbon/type/zotero_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/type_util.py` & `carbon_python_sdk-0.2.1/carbon/type_util.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/carbon/validation_metadata.py` & `carbon_python_sdk-0.2.1/carbon/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.0/pyproject.toml` & `carbon_python_sdk-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "carbon-python-sdk"
-version = "0.2.0"
+version = "0.2.1"
 description = "Client for Carbon"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "carbon"}]
 
 [tool.poetry.dependencies]
```

### Comparing `carbon_python_sdk-0.2.0/PKG-INFO` & `carbon_python_sdk-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-python-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Client for Carbon
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 [![Visit Carbon](https://raw.githubusercontent.com/Carbon-for-Developers/carbon-sdks/HEAD/python/header.png)](https://carbon.ai)
 
 # Carbon<a id="carbon"></a>
 
 Connect external data to LLMs, no matter the source.
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v0.2.0-blue)](https://pypi.org/project/carbon-python-sdk/0.2.0)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.2.1-blue)](https://pypi.org/project/carbon-python-sdk/0.2.1)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/Carbon-for-Developers/carbon-sdks/tree/main/python#readme)
 
 </div>
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
@@ -112,15 +112,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install carbon-python-sdk==0.2.0
+pip install carbon-python-sdk==0.2.1
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from carbon import Carbon
 
@@ -1117,15 +1117,15 @@
 ```python
 upload_response = carbon.files.upload(
     file=open("/path/to/file", "rb"),
     chunk_size=1,
     chunk_overlap=1,
     skip_embedding_generation=False,
     set_page_as_boundary=False,
-    embedding_model="OPENAI",
+    embedding_model="string_example",
     use_ocr=False,
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     parse_pdf_tables_with_ocr=False,
     detect_audio_language=False,
     media_type="TEXT",
@@ -1148,15 +1148,16 @@
 
 Flag to control whether or not embeddings should be generated and stored             when processing file.
 
 ##### set_page_as_boundary: `bool`<a id="set_page_as_boundary-bool"></a>
 
 Flag to control whether or not to set the a page's worth of content as the maximum             amount of content that can appear in a chunk. Only valid for PDFs. See description route description for             more information.
 
-##### embedding_model: [`TextEmbeddingGenerators`](./carbon/type/.py)<a id="embedding_model-textembeddinggeneratorscarbontypepy"></a>
+##### embedding_model: Union[[`TextEmbeddingGenerators`](./carbon/type/text_embedding_generators.py), `str`]<a id="embedding_model-uniontextembeddinggeneratorscarbontypetext_embedding_generatorspy-str"></a>
+
 
 Embedding model that will be used to embed file chunks.
 
 ##### use_ocr: `bool`<a id="use_ocr-bool"></a>
 
 Whether or not to use OCR when processing files. Only valid for PDFs. Useful for documents with             tables, images, and/or scanned text.
 
@@ -1364,15 +1365,15 @@
         "chunk_overlap": 20,
         "skip_embedding_generation": False,
         "embedding_model": "OPENAI",
         "generate_sparse_vectors": False,
         "prepend_filename_to_chunks": False,
         "sync_files_on_connection": True,
         "set_page_as_boundary": False,
-        "request_id": "f5552316-5da3-46e6-ad9f-2f94e30d02cd",
+        "request_id": "fceb0182-329c-4e45-953b-885c747cf4a3",
         "enable_file_picker": True,
         "sync_source_items": True,
         "incremental_sync": False,
     },
 )
 ```
 
@@ -1617,15 +1618,15 @@
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     salesforce_domain="string_example",
     sync_files_on_connection=True,
     set_page_as_boundary=False,
     data_source_id=1,
     connecting_new_account=False,
-    request_id="273420dd-e05c-463f-a3cf-0ff28029639e",
+    request_id="ce1b1ec8-be64-491c-9159-c40f85fa0073",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     enable_file_picker=True,
     sync_source_items=True,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
@@ -1691,15 +1692,15 @@
 
 Enable OCR for files that support it. Supported formats: pdf
 
 ##### parse_pdf_tables_with_ocr: `Optional[bool]`<a id="parse_pdf_tables_with_ocr-optionalbool"></a>
 
 ##### enable_file_picker: `bool`<a id="enable_file_picker-bool"></a>
 
-Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, DROPBOX, GOOGLE_DRIVE, BOX, ONEDRIVE
+Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
 
 ##### sync_source_items: `bool`<a id="sync_source_items-bool"></a>
 
 Enabling this flag will fetch all available content from the source to be listed via list items endpoint
 
 ##### incremental_sync: `bool`<a id="incremental_sync-bool"></a>
 
@@ -1962,15 +1963,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="2782cb96-1bf6-452c-a8d9-60c2378fd079",
+    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
@@ -2082,15 +2083,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="2782cb96-1bf6-452c-a8d9-60c2378fd079",
+    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
```

